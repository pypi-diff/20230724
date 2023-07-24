# Comparing `tmp/chatlab-1.0.0a3.tar.gz` & `tmp/chatlab-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-1.0.0a3.tar", max compression
+gzip compressed data, was "chatlab-1.0.0a4.tar", max compression
```

## Comparing `chatlab-1.0.0a3.tar` & `chatlab-1.0.0a4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1504 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     6865 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/README.md
--rw-r--r--   0        0        0     2324 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/__init__.py
--rw-r--r--   0        0        0       30 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/_version.py
--rw-r--r--   0        0        0      588 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/builtins.py
--rw-r--r--   0        0        0    14242 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/conversation.py
--rw-r--r--   0        0        0     2358 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/decorators.py
--rw-r--r--   0        0        0     8006 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/models.py
--rw-r--r--   0        0        0      174 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/prompts.py
--rw-r--r--   0        0        0     8158 2023-07-23 15:36:54.870663 chatlab-1.0.0a3/chatlab/registry.py
--rw-r--r--   0        0        0     7177 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/chatlab/shells/python.py
--rw-r--r--   0        0        0     2653 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/tests/test_messaging.py
--rw-r--r--   0        0        0     6052 2023-07-23 15:36:54.874663 chatlab-1.0.0a3/tests/test_registry.py
--rw-r--r--   0        0        0     8402 1970-01-01 00:00:00.000000 chatlab-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0     6009 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/README.md
+-rw-r--r--   0        0        0     2324 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/_version.py
+-rw-r--r--   0        0        0      407 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/__init__.py
+-rw-r--r--   0        0        0     4956 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/noteable.py
+-rw-r--r--   0        0        0     8330 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/python.py
+-rw-r--r--   0        0        0    14242 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/conversation.py
+-rw-r--r--   0        0        0     2358 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/decorators.py
+-rw-r--r--   0        0        0     8006 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/models.py
+-rw-r--r--   0        0        0      174 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/prompts.py
+-rw-r--r--   0        0        0     8158 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/registry.py
+-rw-r--r--   0        0        0     2653 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_messaging.py
+-rw-r--r--   0        0        0     6052 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_registry.py
+-rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 chatlab-1.0.0a4/PKG-INFO
```

### Comparing `chatlab-1.0.0a3/LICENSE` & `chatlab-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/README.md` & `chatlab-1.0.0a4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,56 @@
+Metadata-Version: 2.1
+Name: chatlab
+Version: 1.0.0a4
+Summary: Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks.
+Home-page: https://github.com/rgbkrk/chatlab
+License: BSD-3-Clause
+Author: Kyle Kelley
+Author-email: rgbkrk@gmail.com
+Requires-Python: >=3.9.0,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Artificial Life
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Provides-Extra: dev
+Provides-Extra: test
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: ipython (>=7.0.0,<9.0.0)
+Requires-Dist: openai (>=0.27.4,<0.28.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: repr-llm (>=0.2.0,<0.3.0)
+Requires-Dist: vdom (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # ChatLab
 
 **Chat Experiments, Simplified**
 
 💬🔬
 
 ChatLab is a Python package that makes it easy to experiment with OpenAI's chat models. It provides a simple interface for chatting with the models and a way to register functions that can be called from the chat model.
 
 Best yet, it's interactive in the notebook!
 
+⚠️ NOTE: The following docs are for the `1.0.0-alpha` release and `main`. They will not work with the `0.16.0` release. Check out [chatlab.dev](https://chatlab.dev) for the latest docs. For the pre-release, check out [pre.chatlab.dev](https://pre.chatlab.dev).
+
 ## Introduction
 
 ```python
 import chatlab
 import random
 
 def flip_a_coin():
@@ -45,32 +84,20 @@
 
 ```markdown
 It landed on tails!
 ```
 
 In the notebook, text will stream into a Markdown output and function inputs and outputs are a nice collapsible display, like with ChatGPT Plugins.
 
-<details class="details-reset border rounded-2" open="">
-  <summary class="px-3 py-2">
-    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-device-camera-video">
-    <path d="M16 3.75v8.5a.75.75 0 0 1-1.136.643L11 10.575v.675A1.75 1.75 0 0 1 9.25 13h-7.5A1.75 1.75 0 0 1 0 11.25v-6.5C0 3.784.784 3 1.75 3h7.5c.966 0 1.75.784 1.75 1.75v.675l3.864-2.318A.75.75 0 0 1 16 3.75Zm-6.5 1a.25.25 0 0 0-.25-.25h-7.5a.25.25 0 0 0-.25.25v6.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-6.5ZM11 8.825l3.5 2.1v-5.85l-3.5 2.1Z"></path>
-</svg>
-    <span aria-label="Video description flip-a-coin-chatlab.mp4" class="m-1">flip-a-coin-chatlab.mp4</span>
-    <span class="dropdown-caret"></span>
-  </summary>
-
-  <video src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" data-canonical-src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" controls="controls" muted="muted" class="d-block rounded-bottom-2 border-top width-fit" style="max-height:640px; min-height: 200px">
-
-  </video>
-</details>
+TODO: Include GIF/mp4 of this in action
 
 ### Installation
 
 ```bash
-pip install chatlab
+pip install chatlab --pre
 ```
 
 ### Configuration
 
 You'll need to set your `OPENAI_API_KEY` environment variable. You can find your API key on your [OpenAI account page](https://platform.openai.com/account/api-keys). I recommend setting it in an `.env` file when working locally.
 
 On hosted environments like Noteable, set it in your Secrets to keep it safe from prying LLM eyes.
@@ -248,7 +275,8 @@
 ```
 
 We use `black`, `isort`, and `mypy`.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
```

### Comparing `chatlab-1.0.0a3/chatlab/__init__.py` & `chatlab-1.0.0a4/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/conversation.py` & `chatlab-1.0.0a4/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/decorators.py` & `chatlab-1.0.0a4/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/display.py` & `chatlab-1.0.0a4/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/markdown.py` & `chatlab-1.0.0a4/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/messaging.py` & `chatlab-1.0.0a4/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/models.py` & `chatlab-1.0.0a4/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/registry.py` & `chatlab-1.0.0a4/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/chatlab/shells/python.py` & `chatlab-1.0.0a4/chatlab/builtins/python.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-"""Builtins for ChatLab."""
+"""The in-IPython python code runner for ChatLab."""
 import json
 from traceback import TracebackException
 from typing import Optional
 
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.display import display
 from IPython.utils.capture import RichOutput, capture_output
 from repr_llm import register_llm_formatter
 from repr_llm.pandas import format_dataframe_for_llm, format_series_for_llm
 
-# Formats to show to large language models
+from chatlab.decorators import expose_exception_to_llm
+
+# Prioritized formats to show to large language models
 formats_for_llm = [
     # Repr LLM is the richest text
     'text/llm+plain',
+    # Assume that if we get markdown we know it's rich for an LLM
+    'text/markdown',
+    # Same with LaTeX
+    'text/latex',
     # All the normal ones
     'application/vnd.jupyter.error+json',
     'application/vdom.v1+json',
     'application/json',
-    'text/latex',
-    'text/html',
-    'text/markdown',
-    'image/svg+xml',
+    # Since every object has a text/plain repr, even though the LLM would understand `text/plain` well,
+    # bumping this priority up would override more rich media types we definitely want to show.
     'text/plain',
+    # Both HTML and SVG should be conditional on size, considering many libraries
+    # Will emit giant JavaScript blobs for interactivity
+    # For now, we'll assume not to show these
+    # 'text/html',
+    # 'image/svg+xml',
 ]
 
-# Formats to redisplay for the user, since we capture the output during execution
+# Prioritized formats to redisplay for the user, since we capture the output during execution
 formats_to_redisplay = [
     'application/vnd.jupyter.widget-view+json',
     'application/vnd.dex.v1+json',
     'application/vnd.dataresource+json',
     'application/vnd.plotly.v1+json',
     'text/vnd.plotly.v1+html',
     'application/vdom.v1+json',
     'application/json',
     'application/javascript',
     'image/svg+xml',
     'image/png',
     'image/jpeg',
     'image/gif',
+    'text/html',
+    'image/svg+xml',
 ]
 
 
 def redisplay_superrich(output: RichOutput):
     """Redisplay an image."""
     data = output.data
     metadata = output.metadata
@@ -206,7 +217,32 @@
             # Now for text for the llm
             text, _ = pluck_richest_text(result.result)
 
             if text is not None:
                 outputs += f"RESULT:\n{text}\n\n"
 
         return outputs
+
+
+__shell: Optional[ChatLabShell] = None
+
+
+@expose_exception_to_llm
+def run_python(code: str):
+    """Execute code in python and return the result."""
+    global __shell
+
+    if __shell is None:
+        # Since ChatLabShell has imports that are "costly" (e.g. IPython, numpy, pandas),
+        # we only import it on the first call to run_cell.
+        from .python import ChatLabShell
+
+        __shell = ChatLabShell()
+
+    return __shell.run_cell(code)
+
+
+__all__ = ["run_python", "ChatLabShell"]
+
+
+def __dir__():
+    return __all__
```

### Comparing `chatlab-1.0.0a3/pyproject.toml` & `chatlab-1.0.0a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "1.0.0-alpha.3"
+version = "1.0.0-alpha.4"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `chatlab-1.0.0a3/tests/test_decorators.py` & `chatlab-1.0.0a4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/tests/test_messaging.py` & `chatlab-1.0.0a4/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a3/tests/test_registry.py` & `chatlab-1.0.0a4/tests/test_registry.py`

 * *Files identical despite different names*

