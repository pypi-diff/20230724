# Comparing `tmp/autopack_tools-0.3.2.tar.gz` & `tmp/autopack_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.3.2.tar", max compression
+gzip compressed data, was "autopack_tools-0.3.3.tar", max compression
```

## Comparing `autopack_tools-0.3.2.tar` & `autopack_tools-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.3.2/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.3.2/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.3.2/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.3.2/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.3.2/autopack/__main__.py
--rw-r--r--   0        0        0     2869 2023-07-23 21:13:30.082198 autopack_tools-0.3.2/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.3.2/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.3.2/autopack/errors.py
--rw-r--r--   0        0        0     2568 2023-07-23 01:25:16.569309 autopack_tools-0.3.2/autopack/get_pack.py
--rw-r--r--   0        0        0     3935 2023-07-23 04:34:40.466812 autopack_tools-0.3.2/autopack/installation.py
--rw-r--r--   0        0        0     5029 2023-07-23 20:21:14.829622 autopack_tools-0.3.2/autopack/pack.py
--rw-r--r--   0        0        0      276 2023-07-23 21:19:00.939247 autopack_tools-0.3.2/autopack/pack_response.py
--rw-r--r--   0        0        0      393 2023-07-22 23:02:14.133585 autopack_tools-0.3.2/autopack/pack_search_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.3.2/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.3.2/autopack/search.py
--rw-r--r--   0        0        0     3604 2023-07-23 21:07:17.383625 autopack_tools-0.3.2/autopack/selection.py
--rw-r--r--   0        0        0     7904 2023-07-23 05:25:55.315020 autopack_tools-0.3.2/autopack/utils.py
--rw-r--r--   0        0        0     1080 2023-07-23 21:21:04.533722 autopack_tools-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 autopack_tools-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.3.3/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.3.3/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.3.3/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.3.3/autopack/__main__.py
+-rw-r--r--   0        0        0     2869 2023-07-23 21:13:30.082198 autopack_tools-0.3.3/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.3.3/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.3.3/autopack/errors.py
+-rw-r--r--   0        0        0     2464 2023-07-23 22:09:39.852735 autopack_tools-0.3.3/autopack/get_pack.py
+-rw-r--r--   0        0        0     3935 2023-07-23 04:34:40.466812 autopack_tools-0.3.3/autopack/installation.py
+-rw-r--r--   0        0        0     5029 2023-07-23 20:21:14.829622 autopack_tools-0.3.3/autopack/pack.py
+-rw-r--r--   0        0        0      276 2023-07-23 21:19:00.939247 autopack_tools-0.3.3/autopack/pack_response.py
+-rw-r--r--   0        0        0      393 2023-07-22 23:02:14.133585 autopack_tools-0.3.3/autopack/pack_search_response.py
+-rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.3.3/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.3.3/autopack/search.py
+-rw-r--r--   0        0        0     3335 2023-07-23 22:12:19.940610 autopack_tools-0.3.3/autopack/selection.py
+-rw-r--r--   0        0        0     7904 2023-07-23 05:25:55.315020 autopack_tools-0.3.3/autopack/utils.py
+-rw-r--r--   0        0        0     1080 2023-07-23 22:15:33.944829 autopack_tools-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 autopack_tools-0.3.3/PKG-INFO
```

### Comparing `autopack_tools-0.3.2/LICENSE` & `autopack_tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/README.md` & `autopack_tools-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # AutoPack
 
-AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai), a
-collection of tools for AI
-Agents, currently tailored for LangChain implementations.
+AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai)
+repository, a collection of tools for AI. It is designed to be agent-neutral with a simple interface.
 
 ## Installation
 
 You can install AutoPack using pip:
 
 ```bash
 pip install autopack-tools
@@ -30,34 +29,20 @@
 - Get all installed Packs: `get_all_installed_packs()`
 - Install a Pack: `install_pack(pack_id)`
 - Select packs using an LLM: `select_packs(task_description, llm)`
 
 For detailed examples and more information, refer to
 the [AutoPack documentation](https://github.com/AutoPackAI/autopack/wiki).
 
-## Safety and Security Notice
-
-Please exercise caution when using the AutoPack repository and library. The repository and library are currently in the
-early stages and intended for research purposes only. Ensure you review the Packs you install as they are directly
-cloned from GitHub. AutoPack and its maintainers are not liable for any misuse or negligence regarding the repository
-and library.
-
-For more details, please refer to
-the [Safety and Security section](https://github.com/AutoPackAI/autopack/wiki#safety-and-security-notice) in the
-documentation.
-
 ## Contributing
 
 We welcome contributions to the AutoPack ecosystem. Here are some ways you can help:
 
 - **Create new tools!** Expand the AutoPack repository by developing and submitting your own tools. Share your ideas and
   solutions with the AutoPack community.
-- **Submit GitHub repos**: If you come across GitHub repositories containing useful tools, submit them to
-  the [AutoPack repository](https://autopack.ai/submissions). We'll create Packs out of the tools in those repositories
-  by providing the necessary metadata.
 - **Try it out for yourself**: Test AutoPack in your projects and provide feedback. Share your experiences, report bugs,
   and suggest improvements by opening issues on GitHub.
 - **Contribute code**: Help improve AutoPack by opening pull requests. You can choose to work on unresolved issues or
   implement new features that you believe would enhance the functionality of the library. Please note that the AutoPack
   library is intentionally designed to be compact and straightforward.
 
 We appreciate your contributions and look forward to your involvement in making AutoPack a vibrant and valuable resource
```

### Comparing `autopack_tools-0.3.2/autopack/api.py` & `autopack_tools-0.3.3/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/autopack/cli.py` & `autopack_tools-0.3.3/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/autopack/get_pack.py` & `autopack_tools-0.3.3/autopack/get_pack.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,19 +52,18 @@
             packs.append(pack)
 
     return packs
 
 
 def get_pack(pack_id: str, remote=False) -> type[Pack]:
     """
-    Get a pack based on its ID, in `author/repo_name/pack_name` format.
+    Get a pack based on its ID.
 
     Args:
         pack_id (str): The ID of the pack to fetch.
-        quiet (bool, Optional): If True, won't print any output
         remote (bool, Optional): If True, will make network requests to fetch pack metadata
 
     Returns:
         Pack: The fetched pack
 
     Raises:
         AutoPackFetchError: If there was an error during the data fetch.
```

### Comparing `autopack_tools-0.3.2/autopack/installation.py` & `autopack_tools-0.3.3/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/autopack/pack.py` & `autopack_tools-0.3.3/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/autopack/prompts.py` & `autopack_tools-0.3.3/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/autopack/selection.py` & `autopack_tools-0.3.3/autopack/selection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 import re
 from typing import Callable, Union, Optional
 
 from langchain.chat_models.base import BaseChatModel
 
-from autopack.api import pack_search
-from autopack.get_pack import try_get_pack
-from autopack.installation import install_pack
+from autopack import Pack
+from autopack.get_pack import get_all_installed_packs
 from autopack.prompts import GET_MORE_TOOLS_TEMPLATE, TOOL_SELECTION_TEMPLATE
 from autopack.utils import functions_bulleted_list, call_llm
 
 
-def select_packs_prompt(task_description: str, function_request: Optional[str] = None, installed_only=False) -> str:
+def select_packs_prompt(task_description: str, function_request: Optional[str] = None) -> str:
     """
     Generate a prompt for the pack selection process based on the task description and an optional function request.
 
     Args:
         task_description (str): A description of the task to be used when selecting tools.
         function_request (Optional[str]): A specific type of function asked for (e.g. a `get_more_tools` function).
-        installed_only (Optional[bool]): If True will only use already-installed pack. If False will install the packs.
 
     Returns:
         str: A prompt that can be fed to the LLM for pack selection.
     """
 
-    pack_ids = [pack.pack_id for pack in pack_search("")]
-    if installed_only:
-        fetched_packs = [try_get_pack(pack_id) for pack_id in pack_ids]
-        installed_packs = [pack for pack in fetched_packs if pack is not None]
-    else:
-        fetched_packs = [install_pack(pack_id, force_dependencies=True) for pack_id in pack_ids]
-        installed_packs = [pack for pack in fetched_packs if pack is not None]
+    installed_packs = get_all_installed_packs()
 
     if function_request:
         return TOOL_SELECTION_TEMPLATE.format(task=task_description, functions=functions_bulleted_list(installed_packs))
 
     return GET_MORE_TOOLS_TEMPLATE.format(
         task=task_description,
         functions=functions_bulleted_list(installed_packs),
@@ -41,48 +33,57 @@
     )
 
 
 def select_packs(
     task_description: str,
     llm: Union[BaseChatModel, Callable],
     function_request: Optional[str] = None,
-    installed_only=False,
-) -> list[str]:
+) -> list[type[Pack]]:
     """Given a user input describing the task they wish to accomplish, return a list of Pack IDs that the given LLM
     thinks will be suitable for this task.
 
     This is good for a "pre-processing" step after receiving the task but before trying to solve it. This allows you
     to benefit from the wide tool selection while keeping your token usage low.
 
     You can then further filter, install the packs if desired, and then fetch them using get_pack().
 
     # TODO: Include user-provided packs into selection
 
     Args:
         task_description (str): A description of the task to be used when selecting tools
         llm (BaseChatModel): An LLM which will be used to evaluate the selection
         function_request (Optional[str]): A specific type of function asked for (e.g. a `get_more_tools` function)
-        installed_only (Optional[bool]): If True will only use already-installed pack. If False will install the packs.
 
     Returns:
         list[str]: A list of selected Pack IDs
     """
-    prompt = select_packs_prompt(task_description, function_request, installed_only=installed_only)
+    prompt = select_packs_prompt(task_description, function_request)
 
     response = call_llm(prompt, llm)
 
     return parse_selection_response(response)
 
 
-def parse_selection_response(response: str) -> list[str]:
+def parse_selection_response(response: str) -> list[type[Pack]]:
     """
     Parse the response from the LLM and extract pack IDs.
 
     The response is split by commas and newlines, and any arguments provided in the response are removed.
 
     Args:
         response (str): The response from the LLM.
 
     Returns:
         list[str]: A list of parsed pack IDs.
     """
-    return [r.split("(")[0].strip() for r in re.split(r"(?<=\w),|\n", response)]
+    pack_names = [r.split("(")[0].strip() for r in re.split(r"(?<=\w),|\n", response)]
+    installed_packs = get_all_installed_packs()
+    selected_packs = []
+    for pack_name in pack_names:
+        try:
+            selected_pack = next(pack for pack in installed_packs if pack.name == pack_name)
+            selected_packs.append(selected_pack)
+        except StopIteration:
+            # This means that the pack selected is not installed. This error should've been caught elsewhere
+            continue
+
+    return selected_packs
```

### Comparing `autopack_tools-0.3.2/autopack/utils.py` & `autopack_tools-0.3.3/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.2/pyproject.toml` & `autopack_tools-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.3.2"
+version = "0.3.3"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.3.2/PKG-INFO` & `autopack_tools-0.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,17 +19,16 @@
 Requires-Dist: types-requests (>=2.31.0.2,<3.0.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/AutoPackAI/autopack
 Description-Content-Type: text/markdown
 
 # AutoPack
 
-AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai), a
-collection of tools for AI
-Agents, currently tailored for LangChain implementations.
+AutoPack is a Python library and CLI designed to interact with the [AutoPack repository](https://autopack.ai)
+repository, a collection of tools for AI. It is designed to be agent-neutral with a simple interface.
 
 ## Installation
 
 You can install AutoPack using pip:
 
 ```bash
 pip install autopack-tools
@@ -53,34 +52,20 @@
 - Get all installed Packs: `get_all_installed_packs()`
 - Install a Pack: `install_pack(pack_id)`
 - Select packs using an LLM: `select_packs(task_description, llm)`
 
 For detailed examples and more information, refer to
 the [AutoPack documentation](https://github.com/AutoPackAI/autopack/wiki).
 
-## Safety and Security Notice
-
-Please exercise caution when using the AutoPack repository and library. The repository and library are currently in the
-early stages and intended for research purposes only. Ensure you review the Packs you install as they are directly
-cloned from GitHub. AutoPack and its maintainers are not liable for any misuse or negligence regarding the repository
-and library.
-
-For more details, please refer to
-the [Safety and Security section](https://github.com/AutoPackAI/autopack/wiki#safety-and-security-notice) in the
-documentation.
-
 ## Contributing
 
 We welcome contributions to the AutoPack ecosystem. Here are some ways you can help:
 
 - **Create new tools!** Expand the AutoPack repository by developing and submitting your own tools. Share your ideas and
   solutions with the AutoPack community.
-- **Submit GitHub repos**: If you come across GitHub repositories containing useful tools, submit them to
-  the [AutoPack repository](https://autopack.ai/submissions). We'll create Packs out of the tools in those repositories
-  by providing the necessary metadata.
 - **Try it out for yourself**: Test AutoPack in your projects and provide feedback. Share your experiences, report bugs,
   and suggest improvements by opening issues on GitHub.
 - **Contribute code**: Help improve AutoPack by opening pull requests. You can choose to work on unresolved issues or
   implement new features that you believe would enhance the functionality of the library. Please note that the AutoPack
   library is intentionally designed to be compact and straightforward.
 
 We appreciate your contributions and look forward to your involvement in making AutoPack a vibrant and valuable resource
```

