# Comparing `tmp/parea_ai-0.1.1a0.tar.gz` & `tmp/parea_ai-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parea_ai-0.1.1a0.tar", max compression
+gzip compressed data, was "parea_ai-0.1.1a1.tar", max compression
```

## Comparing `parea_ai-0.1.1a0.tar` & `parea_ai-0.1.1a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-24 19:26:39.839029 parea_ai-0.1.1a0/README.md
--rw-r--r--   0        0        0      598 2023-07-24 19:26:39.845895 parea_ai-0.1.1a0/parea_ai/__init__.py
--rw-r--r--   0        0        0     2205 2023-07-24 17:50:56.645582 parea_ai-0.1.1a0/parea_ai/api_client.py
--rw-r--r--   0        0        0     1631 2023-07-24 19:26:39.855219 parea_ai-0.1.1a0/parea_ai/client.py
--rw-r--r--   0        0        0     1728 2023-07-24 19:26:44.319965 parea_ai-0.1.1a0/parea_ai/example.py
--rw-r--r--   0        0        0     2307 2023-07-24 17:50:56.646234 parea_ai-0.1.1a0/parea_ai/schemas/models.py
--rw-r--r--   0        0        0     3493 2023-07-24 19:27:20.166741 parea_ai-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 parea_ai-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     3958 2023-07-24 19:38:17.202699 parea_ai-0.1.1a1/README.md
+-rw-r--r--   0        0        0      595 2023-07-24 19:38:17.209741 parea_ai-0.1.1a1/parea/__init__.py
+-rw-r--r--   0        0        0     2205 2023-07-24 17:50:56.645582 parea_ai-0.1.1a1/parea/api_client.py
+-rw-r--r--   0        0        0     1625 2023-07-24 19:38:17.216822 parea_ai-0.1.1a1/parea/client.py
+-rw-r--r--   0        0        0     1722 2023-07-24 19:39:30.823388 parea_ai-0.1.1a1/parea/example.py
+-rw-r--r--   0        0        0     2307 2023-07-24 17:50:56.646234 parea_ai-0.1.1a1/parea/schemas/models.py
+-rw-r--r--   0        0        0     3525 2023-07-24 19:40:12.065754 parea_ai-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 parea_ai-0.1.1a1/PKG-INFO
```

### Comparing `parea_ai-0.1.1a0/LICENSE` & `parea_ai-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a0/README.md` & `parea_ai-0.1.1a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 ## Getting Started
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from parea_ai.client import Parea
-from parea_ai.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
+from parea.client import Parea
+from parea.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
 
 load_dotenv()
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = '<DEPLOYMENT_ID>'
```

### Comparing `parea_ai-0.1.1a0/parea_ai/__init__.py` & `parea_ai-0.1.1a1/parea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     The Parea SDK allows you to interact with Parea from your product or service.
     To install the official [Python SDK](https://pypi.org/project/parea/),
     run the following command:  ```bash pip install parea ```.
 """
 
 from importlib import metadata as importlib_metadata
 
-from parea_ai.client import Parea
+from parea.client import Parea
 
 
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
         return "unknown"
```

### Comparing `parea_ai-0.1.1a0/parea_ai/api_client.py` & `parea_ai-0.1.1a1/parea/api_client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a0/parea_ai/client.py` & `parea_ai-0.1.1a1/parea/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from attrs import asdict, define, field
 
-from parea_ai.api_client import HTTPClient
-from parea_ai.schemas.models import Completion, CompletionResponse, UseDeployedPrompt, UseDeployedPromptResponse
+from parea.api_client import HTTPClient
+from parea.schemas.models import Completion, CompletionResponse, UseDeployedPrompt, UseDeployedPromptResponse
 
 COMPLETION_ENDPOINT = "/completion"
 DEPLOYED_PROMPT_ENDPOINT = "/deployed-prompt"
 
 
 @define
 class Parea:
```

### Comparing `parea_ai-0.1.1a0/parea_ai/example.py` & `parea_ai-0.1.1a1/parea/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import os
 
 from dotenv import load_dotenv
 
-from parea_ai.client import Parea
-from parea_ai.schemas.models import Completion, CompletionResponse, UseDeployedPrompt, UseDeployedPromptResponse
+from parea.client import Parea
+from parea.schemas.models import Completion, CompletionResponse, UseDeployedPrompt, UseDeployedPromptResponse
 
 load_dotenv()
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = os.getenv("DEPLOYMENT_ID")
```

### Comparing `parea_ai-0.1.1a0/parea_ai/schemas/models.py` & `parea_ai-0.1.1a1/parea/schemas/models.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a0/pyproject.toml` & `parea_ai-0.1.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parea-ai"
-version = "0.1.1a0"
+packages = [{ include = "parea" }]
+version = "0.1.1a1"
 description = "Parea python sdk"
 readme = "README.md"
 authors = ["joel-parea-ai <joel@parea.ai>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/parea-ai/parea-sdk"
 homepage = "https://github.com/parea-ai/parea-sdk"
 
@@ -132,15 +133,15 @@
   "--doctest-continue-on-failure",
 ]
 
 [tool.coverage.run]
 source = ["tests"]
 
 [coverage.paths]
-source = "parea_ai"
+source = "parea"
 
 [coverage.run]
 branch = true
 
 [coverage.report]
 fail_under = 50
 show_missing = true
```

### Comparing `parea_ai-0.1.1a0/PKG-INFO` & `parea_ai-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parea-ai
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: Parea python sdk
 Home-page: https://github.com/parea-ai/parea-sdk
 License: Apache Software License 2.0
 Author: joel-parea-ai
 Author-email: joel@parea.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -56,16 +56,16 @@
 ## Getting Started
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from parea_ai.client import Parea
-from parea_ai.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
+from parea.client import Parea
+from parea.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
 
 load_dotenv()
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = '<DEPLOYMENT_ID>'
```

