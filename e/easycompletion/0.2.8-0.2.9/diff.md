# Comparing `tmp/easycompletion-0.2.8.tar.gz` & `tmp/easycompletion-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.8.tar", last modified: Sat Jul 22 00:32:39 2023, max compression
+gzip compressed data, was "easycompletion-0.2.9.tar", last modified: Mon Jul 24 08:03:41 2023, max compression
```

## Comparing `easycompletion-0.2.8.tar` & `easycompletion-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:32:39.687773 easycompletion-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-22 00:32:30.000000 easycompletion-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-22 00:32:39.687773 easycompletion-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-22 00:32:30.000000 easycompletion-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:32:39.687773 easycompletion-0.2.8/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-22 00:32:30.000000 easycompletion-0.2.8/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-22 00:32:30.000000 easycompletion-0.2.8/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-22 00:32:30.000000 easycompletion-0.2.8/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-07-22 00:32:30.000000 easycompletion-0.2.8/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-22 00:32:30.000000 easycompletion-0.2.8/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:32:39.687773 easycompletion-0.2.8/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-22 00:32:39.000000 easycompletion-0.2.8/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-22 00:32:39.000000 easycompletion-0.2.8/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 00:32:39.000000 easycompletion-0.2.8/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-22 00:32:39.000000 easycompletion-0.2.8/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 00:32:39.000000 easycompletion-0.2.8/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 00:32:39.687773 easycompletion-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-22 00:32:30.000000 easycompletion-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 08:03:26.000000 easycompletion-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-24 08:03:41.056806 easycompletion-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-24 08:03:26.000000 easycompletion-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:03:41.056806 easycompletion-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-24 08:03:26.000000 easycompletion-0.2.9/setup.py
```

### Comparing `easycompletion-0.2.8/LICENSE` & `easycompletion-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/PKG-INFO` & `easycompletion-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.8/README.md` & `easycompletion-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/easycompletion/__init__.py` & `easycompletion-0.2.9/easycompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/easycompletion/constants.py` & `easycompletion-0.2.9/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/easycompletion/logger.py` & `easycompletion-0.2.9/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/easycompletion/model.py` & `easycompletion-0.2.9/easycompletion/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     Usage:
         isValid = validate_functions(response, functions, function_call)
     """
     response_function_call = response["choices"][0]["message"].get(
         "function_call", None
     )
     if response_function_call is None:
-        log("No function call in response", type="error", log=debug)
+        log(f"No function call in response\n{response}", type="error", log=debug)
         return False
 
     # If function_call is not "auto" and the name does not match with the response, return False
     if (
         function_call != "auto"
         and response_function_call["name"] != function_call["name"]
     ):
@@ -99,33 +99,50 @@
         function_call["name"]
         if function_call != "auto"
         else response_function_call["name"]
     )
 
     # Parse the arguments from the response
     arguments = parse_arguments(response_function_call["arguments"])
-
-    # If arguments are None, return False
-    if arguments is None:
-        log("Arguments are None", type="error", log=debug)
-        return False
-
+    
     # Get the function that matches the function name from the list of functions
     function = next(
         (item for item in functions if item["name"] == function_call_name), None
     )
 
     # If no matching function is found, return False
     if function is None:
-        log("No matching function found", type="error", log=debug)
+        log(
+            "No matching function found"
+            + f"\nExpected function name:\n{str(function_call_name)}"
+            + f"\n\nResponse:\n{str(response)}"
+            , type="error", log=debug)
+        return False
+
+    # If arguments are None, return False
+    if arguments is None:
+        log(
+            "Arguments are None"
+            + f"\nExpected arguments:\n{str(function['parameters']['properties'].keys())}"
+            + f"\n\nResponse function call:\n{str(response_function_call)}"
+            , type="error", log=debug)
+        #
         return False
 
-    # Check if the function's argument keys match with the response's argument keys
-    if set(function["parameters"]["properties"].keys()) != set(arguments.keys()):
-        log("Argument keys do not match", type="error", log=debug)
+    
+    required_properties = function["parameters"].get("required", [])
+
+    # Check that arguments.keys() contains all of the required properties
+    if not all(required_property in arguments.keys() for required_property in required_properties):
+        log(
+            "ERROR: Response did not contain all required properties.\n"
+            + f"\nExpected keys:\n{str(function['parameters']['properties'].keys())}"
+            +f"\n\nActual keys:\n{str(arguments.keys())}",
+            type="error", log=debug)
+
         return False
 
     log("Function call is valid", type="success", log=debug)
     return True
 
 
 def compose_function(name, description, properties, required_properties, debug=DEBUG):
@@ -430,15 +447,15 @@
     usage = response["usage"]
 
     text = response_data["content"]
     function_call_response = response_data.get("function_call", None)
 
     # If no function call in response, return an error
     if function_call_response is None:
-        log("No function call in response", type="error", log=debug)
+        log(f"No function call in response\n{response}", type="error", log=debug)
         return {"error": "No function call in response"}
     function_name = function_call_response["name"]
     arguments = parse_arguments(function_call_response["arguments"])
     log(
         f"Response\n\nFunction Name: {function_name}\n\nArguments:\n{arguments}\n\nText:\n{text}\n\nFinish Reason: {finish_reason}\n\nUsage:\n{usage}",
         type="response",
         log=debug,
```

### Comparing `easycompletion-0.2.8/easycompletion/prompt.py` & `easycompletion-0.2.9/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.8/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.2.9/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.8/setup.py` & `easycompletion-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.8',
+    version='0.2.9',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

