# Comparing `tmp/open_interpreter-0.0.237.tar.gz` & `tmp/open_interpreter-0.0.238.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.237.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.238.tar", max compression
```

## Comparing `open_interpreter-0.0.237.tar` & `open_interpreter-0.0.238.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.237/LICENSE
--rw-r--r--   0        0        0     6106 2023-07-24 03:07:00.576388 open_interpreter-0.0.237/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.237/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.237/interpreter/exec.py
--rw-r--r--   0        0        0     8485 2023-07-24 02:59:59.898762 open_interpreter-0.0.237/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.237/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.237/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.237/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.237/interpreter/view.py
--rw-r--r--   0        0        0      564 2023-07-24 05:09:56.528940 open_interpreter-0.0.237/pyproject.toml
--rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 open_interpreter-0.0.237/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.238/LICENSE
+-rw-r--r--   0        0        0     6106 2023-07-24 03:07:00.576388 open_interpreter-0.0.238/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.238/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.238/interpreter/exec.py
+-rw-r--r--   0        0        0     8636 2023-07-24 05:18:21.839348 open_interpreter-0.0.238/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.238/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.238/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.238/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.238/interpreter/view.py
+-rw-r--r--   0        0        0      564 2023-07-24 05:19:34.636882 open_interpreter-0.0.238/pyproject.toml
+-rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 open_interpreter-0.0.238/PKG-INFO
```

### Comparing `open_interpreter-0.0.237/LICENSE` & `open_interpreter-0.0.238/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/README.md` & `open_interpreter-0.0.238/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/interpreter/exec.py` & `open_interpreter-0.0.238/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/interpreter/interpreter.py` & `open_interpreter-0.0.238/interpreter/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from .exec import exec_and_capture_output
 from .view import View
 from .json_utils import JsonDeltaCalculator
 from .openai_utils import openai_streaming_response
 import os
+import readline
+
 
 functions = [{
   "name": "run_code",
   "description":
   "Executes code in a stateful IPython shell, capturing prints, return values, terminal outputs, and tracebacks.",
   "parameters": {
     "type": "object",
@@ -107,19 +109,23 @@
       self.messages.append({"role": "user", "content": message})
       self.respond()
 
     else:
       print("Type 'exit' to leave the chat.\n")
 
       while True:
-        user_input = input("> ").strip()
+        try:
+          user_input = input("> ").strip()
+        except EOFError:
+          break
 
         if user_input == 'exit' or user_input == 'exit()':
           break
 
+        readline.add_history(user_input)  # add input to the readline history
         self.messages.append({"role": "user", "content": user_input})
         self.respond()
 
     if return_messages:
       return self.messages
 
   def display(self, delta):
```

### Comparing `open_interpreter-0.0.237/interpreter/json_utils.py` & `open_interpreter-0.0.238/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/interpreter/openai_utils.py` & `open_interpreter-0.0.238/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/interpreter/system_message.txt` & `open_interpreter-0.0.238/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/interpreter/view.py` & `open_interpreter-0.0.238/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.237/pyproject.toml` & `open_interpreter-0.0.238/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.237"
+version = "0.0.238"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.237/PKG-INFO` & `open_interpreter-0.0.238/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.237
+Version: 0.0.238
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

