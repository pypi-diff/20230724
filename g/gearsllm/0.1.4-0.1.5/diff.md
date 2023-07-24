# Comparing `tmp/gearsllm-0.1.4.tar.gz` & `tmp/gearsllm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.4.tar", max compression
+gzip compressed data, was "gearsllm-0.1.5.tar", max compression
```

## Comparing `gearsllm-0.1.4.tar` & `gearsllm-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.4/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.4/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.4/gears/__init__.py
--rw-r--r--   0        0        0     2120 2023-07-24 03:01:58.378599 gearsllm-0.1.4/gears/gear.py
--rw-r--r--   0        0        0     2635 2023-07-24 00:59:40.750920 gearsllm-0.1.4/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.4/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.4/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.4/gears/llms/echo.py
--rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.4/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.4/gears/utils.py
--rw-r--r--   0        0        0      554 2023-07-24 03:02:32.465474 gearsllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.5/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.5/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.5/gears/__init__.py
+-rw-r--r--   0        0        0     2120 2023-07-24 03:01:58.378599 gearsllm-0.1.5/gears/gear.py
+-rw-r--r--   0        0        0     2592 2023-07-24 03:07:29.911750 gearsllm-0.1.5/gears/history.py
+-rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.5/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.5/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.5/gears/llms/echo.py
+-rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.5/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.5/gears/utils.py
+-rw-r--r--   0        0        0      554 2023-07-24 03:08:12.394230 gearsllm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.5/PKG-INFO
```

### Comparing `gearsllm-0.1.4/LICENSE` & `gearsllm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.4/gears/gear.py` & `gearsllm-0.1.5/gears/gear.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.4/gears/history.py` & `gearsllm-0.1.5/gears/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from typing import List
-from pydantic import BaseModel, Field, ConfigDict
+from pydantic import BaseModel, Field
 
 
-class Message(BaseModel):
+class Message(BaseModel, extra="allow"):
     """This class is a wrapper around a message. It is a building block of a history.
 
     Attributes:
         role (str): The role of the message. Something like "user" or "system".
         content (str): The content of the message. A string.
     """
 
-    model_config = ConfigDict(extra="allow")
-
     role: str = Field(
         ...,
         description="The role of the message. Something like 'user' or 'system'.",
     )
     content: str = Field(
         ..., description="The content of the message. A string."
     )
```

### Comparing `gearsllm-0.1.4/gears/llms/echo.py` & `gearsllm-0.1.5/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.4/gears/llms/oai.py` & `gearsllm-0.1.5/gears/llms/oai.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.4/gears/utils.py` & `gearsllm-0.1.5/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.4/pyproject.toml` & `gearsllm-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.4"
+version = "0.1.5"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gearsllm-0.1.4/PKG-INFO` & `gearsllm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

