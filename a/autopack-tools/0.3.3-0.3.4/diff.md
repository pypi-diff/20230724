# Comparing `tmp/autopack_tools-0.3.3.tar.gz` & `tmp/autopack_tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.3.3.tar", max compression
+gzip compressed data, was "autopack_tools-0.3.4.tar", max compression
```

## Comparing `autopack_tools-0.3.3.tar` & `autopack_tools-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.3.3/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.3.3/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.3.3/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.3.3/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.3.3/autopack/__main__.py
--rw-r--r--   0        0        0     2869 2023-07-23 21:13:30.082198 autopack_tools-0.3.3/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.3.3/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.3.3/autopack/errors.py
--rw-r--r--   0        0        0     2464 2023-07-23 22:09:39.852735 autopack_tools-0.3.3/autopack/get_pack.py
--rw-r--r--   0        0        0     3935 2023-07-23 04:34:40.466812 autopack_tools-0.3.3/autopack/installation.py
--rw-r--r--   0        0        0     5029 2023-07-23 20:21:14.829622 autopack_tools-0.3.3/autopack/pack.py
--rw-r--r--   0        0        0      276 2023-07-23 21:19:00.939247 autopack_tools-0.3.3/autopack/pack_response.py
--rw-r--r--   0        0        0      393 2023-07-22 23:02:14.133585 autopack_tools-0.3.3/autopack/pack_search_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.3.3/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.3.3/autopack/search.py
--rw-r--r--   0        0        0     3335 2023-07-23 22:12:19.940610 autopack_tools-0.3.3/autopack/selection.py
--rw-r--r--   0        0        0     7904 2023-07-23 05:25:55.315020 autopack_tools-0.3.3/autopack/utils.py
--rw-r--r--   0        0        0     1080 2023-07-23 22:15:33.944829 autopack_tools-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 autopack_tools-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.3.4/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.3.4/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.3.4/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.3.4/autopack/__main__.py
+-rw-r--r--   0        0        0     2869 2023-07-23 21:13:30.082198 autopack_tools-0.3.4/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.3.4/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.3.4/autopack/errors.py
+-rw-r--r--   0        0        0     2464 2023-07-23 22:09:39.852735 autopack_tools-0.3.4/autopack/get_pack.py
+-rw-r--r--   0        0        0     3935 2023-07-23 04:34:40.466812 autopack_tools-0.3.4/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.3.4/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5173 2023-07-23 22:31:30.673220 autopack_tools-0.3.4/autopack/pack.py
+-rw-r--r--   0        0        0      276 2023-07-23 21:19:00.939247 autopack_tools-0.3.4/autopack/pack_response.py
+-rw-r--r--   0        0        0      393 2023-07-22 23:02:14.133585 autopack_tools-0.3.4/autopack/pack_search_response.py
+-rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.3.4/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.3.4/autopack/search.py
+-rw-r--r--   0        0        0     3335 2023-07-23 22:12:19.940610 autopack_tools-0.3.4/autopack/selection.py
+-rw-r--r--   0        0        0     7904 2023-07-23 05:25:55.315020 autopack_tools-0.3.4/autopack/utils.py
+-rw-r--r--   0        0        0     1080 2023-07-23 22:31:44.689747 autopack_tools-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 autopack_tools-0.3.4/PKG-INFO
```

### Comparing `autopack_tools-0.3.3/LICENSE` & `autopack_tools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/README.md` & `autopack_tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/api.py` & `autopack_tools-0.3.4/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/cli.py` & `autopack_tools-0.3.4/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/get_pack.py` & `autopack_tools-0.3.4/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/installation.py` & `autopack_tools-0.3.4/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/pack.py` & `autopack_tools-0.3.4/autopack/pack.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,7 +127,12 @@
             True if the arguments are valid.
         Raises:
             ValidationError If any arguments are invalid.
         """
         self.args_schema(**kwargs)
 
         return True
+
+    def init_langchain_tool(self):
+        from autopack.langchain_wrapper import LangchainWrapper
+
+        return LangchainWrapper(pack=self)
```

### Comparing `autopack_tools-0.3.3/autopack/prompts.py` & `autopack_tools-0.3.4/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/selection.py` & `autopack_tools-0.3.4/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/autopack/utils.py` & `autopack_tools-0.3.4/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.3/pyproject.toml` & `autopack_tools-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.3.3"
+version = "0.3.4"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.3.3/PKG-INFO` & `autopack_tools-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

