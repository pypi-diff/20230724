# Comparing `tmp/parea_ai-0.1.1a1.tar.gz` & `tmp/parea_ai-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parea_ai-0.1.1a1.tar", max compression
+gzip compressed data, was "parea_ai-0.1.1a2.tar", max compression
```

## Comparing `parea_ai-0.1.1a1.tar` & `parea_ai-0.1.1a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a1/LICENSE
--rw-r--r--   0        0        0     3958 2023-07-24 19:38:17.202699 parea_ai-0.1.1a1/README.md
--rw-r--r--   0        0        0      595 2023-07-24 19:38:17.209741 parea_ai-0.1.1a1/parea/__init__.py
--rw-r--r--   0        0        0     2205 2023-07-24 17:50:56.645582 parea_ai-0.1.1a1/parea/api_client.py
--rw-r--r--   0        0        0     1625 2023-07-24 19:38:17.216822 parea_ai-0.1.1a1/parea/client.py
--rw-r--r--   0        0        0     1722 2023-07-24 19:39:30.823388 parea_ai-0.1.1a1/parea/example.py
--rw-r--r--   0        0        0     2307 2023-07-24 17:50:56.646234 parea_ai-0.1.1a1/parea/schemas/models.py
--rw-r--r--   0        0        0     3525 2023-07-24 19:40:12.065754 parea_ai-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 parea_ai-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     3847 2023-07-24 19:52:00.224089 parea_ai-0.1.1a2/README.md
+-rw-r--r--   0        0        0      595 2023-07-24 19:44:01.025559 parea_ai-0.1.1a2/parea/__init__.py
+-rw-r--r--   0        0        0     2205 2023-07-24 19:44:01.025685 parea_ai-0.1.1a2/parea/api_client.py
+-rw-r--r--   0        0        0     1625 2023-07-24 19:44:01.025796 parea_ai-0.1.1a2/parea/client.py
+-rw-r--r--   0        0        0     1722 2023-07-24 19:44:01.025915 parea_ai-0.1.1a2/parea/example.py
+-rw-r--r--   0        0        0     2082 2023-07-24 20:01:40.458007 parea_ai-0.1.1a2/parea/schemas/models.py
+-rw-r--r--   0        0        0     3525 2023-07-24 20:03:08.359942 parea_ai-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     4897 1970-01-01 00:00:00.000000 parea_ai-0.1.1a2/PKG-INFO
```

### Comparing `parea_ai-0.1.1a1/LICENSE` & `parea_ai-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a1/README.md` & `parea_ai-0.1.1a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # parea-sdk
 
 <div align="center">
 
 [![Build status](https://github.com/parea-ai/parea-sdk/workflows/build/badge.svg?branch=master&event=push)](https://github.com/parea-ai/parea-sdk/actions?query=workflow%3Abuild)
-[![Python Version](https://img.shields.io/pypi/pyversions/parea-sdk.svg)](https://pypi.org/project/parea-sdk/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/parea-ai/parea-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/parea-ai/parea-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/parea-ai/parea-sdk/releases)
 [![License](https://img.shields.io/github/license/parea-ai/parea-sdk)](https://github.com/parea-ai/parea-sdk/blob/master/LICENSE)
 
 Parea python sdk
 
 </div>
```

### Comparing `parea_ai-0.1.1a1/parea/__init__.py` & `parea_ai-0.1.1a2/parea/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a1/parea/api_client.py` & `parea_ai-0.1.1a2/parea/api_client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a1/parea/client.py` & `parea_ai-0.1.1a2/parea/client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a1/parea/example.py` & `parea_ai-0.1.1a2/parea/example.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a1/parea/schemas/models.py` & `parea_ai-0.1.1a2/parea/schemas/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from enum import Enum
 
 from attrs import define
 
 
 class Role(str, Enum):
@@ -30,34 +30,28 @@
 
 
 @define
 class LLMInputs:
     inputs: Optional[dict[str, Any]] = None
     model: Optional[str] = None
     provider: Optional[str] = None
-    is_azure: bool = False
     model_params: Optional[ModelParams] = None
     messages: Optional[list[Message]] = None
     functions: Optional[list[Any]] = None
     function_call: Optional[Union[str, dict[str, str]]] = None
 
 
 @define
 class Completion:
     llm_inputs: LLMInputs
     end_user_identifier: Optional[str] = None
     deployment_id: Optional[str] = None
     name: Optional[str] = None
-    eval_metric_id: Optional[int] = None
     metadata: Optional[dict] = None
-    provider_api_key: Optional[str] = None
-    stream: bool = False
     cache: bool = True
-    retry: bool = False
-    fallback_strategy: Optional[list[str]] = None
     log_omit_inputs: bool = False
     log_omit_outputs: bool = False
     log_omit: bool = False
 
 
 @define
 class CompletionResponse:
@@ -94,9 +88,8 @@
     deployment_id: str
     name: Optional[str] = None
     functions: Optional[dict[str, Any]] = None
     function_call: Optional[str] = None
     prompt: Optional[Prompt] = None
     model: Optional[str] = None
     provider: Optional[str] = None
-    is_azure: bool = False
     model_params: Optional[dict[str, Any]] = None
```

### Comparing `parea_ai-0.1.1a1/pyproject.toml` & `parea_ai-0.1.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parea-ai"
 packages = [{ include = "parea" }]
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "Parea python sdk"
 readme = "README.md"
 authors = ["joel-parea-ai <joel@parea.ai>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/parea-ai/parea-sdk"
 homepage = "https://github.com/parea-ai/parea-sdk"
```

### Comparing `parea_ai-0.1.1a1/PKG-INFO` & `parea_ai-0.1.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parea-ai
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Parea python sdk
 Home-page: https://github.com/parea-ai/parea-sdk
 License: Apache Software License 2.0
 Author: joel-parea-ai
 Author-email: joel@parea.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -25,18 +25,17 @@
 Description-Content-Type: text/markdown
 
 # parea-sdk
 
 <div align="center">
 
 [![Build status](https://github.com/parea-ai/parea-sdk/workflows/build/badge.svg?branch=master&event=push)](https://github.com/parea-ai/parea-sdk/actions?query=workflow%3Abuild)
-[![Python Version](https://img.shields.io/pypi/pyversions/parea-sdk.svg)](https://pypi.org/project/parea-sdk/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/parea-ai/parea-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/parea-ai/parea-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/parea-ai/parea-sdk/releases)
 [![License](https://img.shields.io/github/license/parea-ai/parea-sdk)](https://github.com/parea-ai/parea-sdk/blob/master/LICENSE)
 
 Parea python sdk
 
 </div>
```

