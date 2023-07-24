# Comparing `tmp/BlitzChain-0.8.0.tar.gz` & `tmp/BlitzChain-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.8.0.tar", last modified: Mon Jul 24 03:32:25 2023, max compression
+gzip compressed data, was "BlitzChain-0.8.1.tar", last modified: Mon Jul 24 03:47:04 2023, max compression
```

## Comparing `BlitzChain-0.8.0.tar` & `BlitzChain-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:32:25.347622 BlitzChain-0.8.0/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:32:25.344585 BlitzChain-0.8.0/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:32:25.000000 BlitzChain-0.8.0/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-24 03:32:25.000000 BlitzChain-0.8.0/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-24 03:32:25.000000 BlitzChain-0.8.0/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-24 03:32:25.000000 BlitzChain-0.8.0/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-24 03:32:25.000000 BlitzChain-0.8.0/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.8.0/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:32:25.347435 BlitzChain-0.8.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3436 2023-07-09 13:29:34.000000 BlitzChain-0.8.0/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:32:25.345462 BlitzChain-0.8.0/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-24 03:28:20.000000 BlitzChain-0.8.0/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)    10297 2023-07-24 03:27:57.000000 BlitzChain-0.8.0/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2079 2023-07-23 13:02:56.000000 BlitzChain-0.8.0/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      794 2023-07-23 13:02:56.000000 BlitzChain-0.8.0/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:32:25.345733 BlitzChain-0.8.0/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-07-09 14:53:24.000000 BlitzChain-0.8.0/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      435 2023-07-20 07:06:24.000000 BlitzChain-0.8.0/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-24 03:32:25.347679 BlitzChain-0.8.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      481 2023-07-24 03:30:52.000000 BlitzChain-0.8.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:32:25.346805 BlitzChain-0.8.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-07-23 13:02:56.000000 BlitzChain-0.8.0/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      722 2023-07-23 13:02:56.000000 BlitzChain-0.8.0/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      615 2023-07-23 13:02:56.000000 BlitzChain-0.8.0/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.986428 BlitzChain-0.8.1/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.983977 BlitzChain-0.8.1/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.8.1/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:47:04.986291 BlitzChain-0.8.1/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3436 2023-07-09 13:29:34.000000 BlitzChain-0.8.1/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.984835 BlitzChain-0.8.1/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-24 03:46:21.000000 BlitzChain-0.8.1/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)    10275 2023-07-24 03:46:09.000000 BlitzChain-0.8.1/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2079 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      794 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.985234 BlitzChain-0.8.1/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-07-09 14:53:24.000000 BlitzChain-0.8.1/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      435 2023-07-20 07:06:24.000000 BlitzChain-0.8.1/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-24 03:47:04.986472 BlitzChain-0.8.1/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      481 2023-07-24 03:30:52.000000 BlitzChain-0.8.1/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.986045 BlitzChain-0.8.1/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      722 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      615 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_qa.py
```

### Comparing `BlitzChain-0.8.0/LICENSE` & `BlitzChain-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.0/README.md` & `BlitzChain-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.0/blitzchain/api.py` & `BlitzChain-0.8.1/blitzchain/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,29 +145,29 @@
                 "metadata": metadata,
             },
         )
         return get_json_response(response)
 
     def generative_qa(
         self,
-        user_input: str,
+        prompt: str,
         prompt_fields: list,
         conversation_id: str = None,
         limit: int = 5,
         fields: list = None,
         include_rerank: bool = False,
         minimum_rerank_score: float = 0.7,
         include_moderation: bool = False,
     ):
         """Get an answer based on a question that you ask."""
         url = self.base_url + "collection/generative-qa"
         print(url)
         data = {
             "collection": self.collection_name,
-            "userInput": user_input,
+            "prompt": prompt,
             "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
             "include_moderation": include_moderation,
         }
@@ -182,29 +182,29 @@
             },
             json=data,
         )
         return get_json_response(response)
 
     def copilot(
         self,
-        user_input: str,
+        prompt: str,
         prompt_fields: list,
         conversation_id: str = None,
         limit: int = 5,
         fields: list = None,
         include_rerank: bool = False,
         minimum_rerank_score: float = 0.7,
         include_moderation: bool = False,
     ):
         """Get an answer based on a question that you ask."""
         url = self.base_url + "collection/copilot"
         print(url)
         data = {
             "collection": self.collection_name,
-            "userInput": user_input,
+            "prompt": prompt,
             "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
             "includeModeration": include_moderation,
         }
```

### Comparing `BlitzChain-0.8.0/blitzchain/splitter.py` & `BlitzChain-0.8.1/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.0/blitzchain/utils.py` & `BlitzChain-0.8.1/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.0/tests/test_pdf.py` & `BlitzChain-0.8.1/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.0/tests/test_qa.py` & `BlitzChain-0.8.1/tests/test_qa.py`

 * *Files identical despite different names*

