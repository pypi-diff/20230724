# Comparing `tmp/airoboros-2.0.7.tar.gz` & `tmp/airoboros-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.7.tar", last modified: Sat Jul 22 17:57:11 2023, max compression
+gzip compressed data, was "airoboros-2.0.8.tar", last modified: Mon Jul 24 12:06:29 2023, max compression
```

## Comparing `airoboros-2.0.7.tar` & `airoboros-2.0.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:11.606972 airoboros-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 17:57:00.000000 airoboros-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:57:11.606972 airoboros-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 17:57:00.000000 airoboros-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:11.602972 airoboros-2.0.7/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:11.606972 airoboros-2.0.7/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:11.606972 airoboros-2.0.7/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/card.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/writing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/prompts/writing_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/riddle.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/wordgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/instructors/writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-22 17:57:00.000000 airoboros-2.0.7/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:57:11.602972 airoboros-2.0.7/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 17:57:11.000000 airoboros-2.0.7/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:57:11.606972 airoboros-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 17:57:00.000000 airoboros-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.371126 airoboros-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 12:06:16.000000 airoboros-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 12:06:29.371126 airoboros-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-24 12:06:16.000000 airoboros-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.363126 airoboros-2.0.8/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.367126 airoboros-2.0.8/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.371126 airoboros-2.0.8/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/card.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/writing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/writing_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/riddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/wordgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21035 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.367126 airoboros-2.0.8/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:06:29.371126 airoboros-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-24 12:06:16.000000 airoboros-2.0.8/setup.py
```

### Comparing `airoboros-2.0.7/LICENSE` & `airoboros-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/PKG-INFO` & `airoboros-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.7
+Version: 2.0.8
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.7/README.md` & `airoboros-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/entrypoint.py` & `airoboros-2.0.8/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/coding.py` & `airoboros-2.0.8/airoboros/instructors/coding.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,19 @@
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
-    count = instructor.instructor_counts.get("coding", 0)
+    if "coding" not in instructor.instructor_counts:
+        instructor.instructor_counts["coding"] = 0
     language_index = 0
     language = config.get("language") or instructor.language
-    while count < target_count:
+    while instructor.instructor_counts["coding"] < target_count:
         # Inject languages to use for this batch.
         current_languages = []
         for _ in range(batch_size):
             current_languages.append(coding_languages[language_index])
             language_index += 1
             if language_index >= len(coding_languages):
                 language_index = 0
@@ -107,15 +108,19 @@
                         ),
                     ]
                 )
             )
             instructions.append(
                 instruction if not plain else instruction + " PLAINFORMAT"
             )
-            futures.append(instructor.generate_response(full_instruction, **api_params))
+            futures.append(
+                instructor.generate_response(
+                    full_instruction, filter_response=False, **api_params
+                )
+            )
         if not futures:
             continue
         responses = await asyncio.gather(*futures)
         for idx in range(len(futures)):
             response = responses[idx]
             if not response:
                 continue
@@ -124,10 +129,9 @@
                 if not response:
                     continue
             yield {
                 "instruction": instructions[idx].strip(),
                 "response": response.strip(),
                 "category": "coding",
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts["coding"] >= target_count:
                 break
```

### Comparing `airoboros-2.0.7/airoboros/instructors/contextual.py` & `airoboros-2.0.8/airoboros/instructors/contextual.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,21 +176,22 @@
     # Min similarity score.
     min_score = config.get("min_docsearch_score")
     if min_score is None:
         min_score = instructor.min_docsearch_score
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    count = instructor.instructor_counts.get("contextual", 0)
+    if "contextual" not in instructor.instructor_counts:
+        instructor.instructor_counts["contextual"] = 0
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     futures = []
-    while count < target_count:
+    while instructor.instructor_counts["contextual"] < target_count:
         prompt = generate_prompt(instructor, config, template, topic_iter)
         futures.append(instructor.generate_response(prompt, **api_params))
         if len(futures) < batch_size:
             continue
         instructions = []
         for instruction in await asyncio.gather(*futures):
             if not instruction or not instruction.strip():
@@ -219,11 +220,10 @@
             if not response or not response.strip():
                 continue
             yield {
                 "instruction": instructions[idx].strip(),
                 "response": response.strip(),
                 "category": "contextual",
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts["contextual"] >= target_count:
                 break
         futures = []
```

### Comparing `airoboros-2.0.7/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.8/airoboros/instructors/counterfactual_contextual.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,21 +51,22 @@
     # Min similarity score.
     min_score = config.get("min_docsearch_score")
     if min_score is None:
         min_score = instructor.min_docsearch_score
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    count = instructor.instructor_counts.get("counterfactual_contextual", 0)
+    if "counterfactual_contextual" not in instructor.instructor_counts:
+        instructor.instructor_counts["counterfactual_contextual"] = 0
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     language = config.get("language") or instructor.language
-    while count < target_count:
+    while instructor.instructor_counts["counterfactual_contextual"] < target_count:
         response = await instructor.generate_response(
             template.format(batch_size=batch_size, language=language), **api_params
         )
         if not response or not response.strip():
             continue
         match = re.search("FACTS(.*)COUNTER(.*)QUESTIONS(.*)", response, re.DOTALL)
         if not match:
@@ -160,11 +161,13 @@
             if not response or not response.strip():
                 continue
             yield {
                 "instruction": instructions[idx].strip(),
                 "response": response.strip(),
                 "category": "counterfactual_contextual",
             }
-            count += 1
-            if count >= target_count:
+            if (
+                instructor.instructor_counts["counterfactual_contextual"]
+                >= target_count
+            ):
                 break
         futures = []
```

### Comparing `airoboros-2.0.7/airoboros/instructors/experience.py` & `airoboros-2.0.8/airoboros/instructors/experience.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,24 +26,27 @@
     # Min similarity score.
     min_score = config.get("min_docsearch_score")
     if min_score is None:
         min_score = instructor.min_docsearch_score
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    count = instructor.instructor_counts.get("experience", 0)
+    if "experience" not in instructor.instructor_counts:
+        instructor.instructor_counts["experience"] = 0
     language = config.get("language") or instructor.language
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     futures = []
-    while count < target_count:
+    while instructor.instructor_counts["experience"] < target_count:
         futures.append(
-            instructor.generate_response(prompt.format(language=language), **api_params)
+            instructor.generate_response(
+                prompt.format(language=language), filter_response=False, **api_params
+            )
         )
         if len(futures) < batch_size:
             continue
         for response in await asyncio.gather(*futures):
             if not response or not response.strip():
                 continue
 
@@ -63,11 +66,10 @@
             ):
                 continue
             yield {
                 "instruction": instruction,
                 "response": response,
                 "category": "experience",
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts["experience"] >= target_count:
                 break
         futures = []
```

### Comparing `airoboros-2.0.7/airoboros/instructors/general.py` & `airoboros-2.0.8/airoboros/instructors/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,18 @@
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
-    count = instructor.instructor_counts.get("general", 0)
+    if "general" not in instructor.instructor_counts:
+        instructor.instructor_counts["general"] = 0
     language = config.get("language") or instructor.language
-    while count < target_count:
+    while instructor.instructor_counts["general"] < target_count:
         # Inject the topics to use for this batch.
         current_topics = []
         for _ in range(batch_size):
             current_topics.append(topics[topic_index])
             topic_index += 1
             if topic_index >= len(topics):
                 topic_index = 0
@@ -89,10 +90,9 @@
             if not response or not response.strip():
                 continue
             yield {
                 "instruction": instructions[idx].strip(),
                 "response": response.strip(),
                 "category": "general",
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts["general"] >= target_count:
                 break
```

### Comparing `airoboros-2.0.7/airoboros/instructors/inline_qa.py` & `airoboros-2.0.8/airoboros/instructors/inline_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,18 @@
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
-    count = instructor.instructor_counts.get(category, 0)
+    if category not in instructor.instructor_counts:
+        instructor.instructor_counts[category] = 0
     language = config.get("language") or instructor.language
-    while count < target_count:
+    while instructor.instructor_counts[category] < target_count:
         # Get a batch of instructions.
         prompt_args = {"language": language}
         if "{batch_size}" in template:
             prompt_args["batch_size"] = batch_size
         if "{topic_avoidance}" in template:
             prompt_args["topic_avoidance"] = instructor.topic_avoidance
         prompt = template.format(**prompt_args)
@@ -62,10 +63,9 @@
             ):
                 continue
             yield {
                 "instruction": instruction.strip(),
                 "response": response.strip(),
                 "category": category,
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts[category] >= target_count:
                 break
```

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/agent.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/card.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/card.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/cot.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/plan.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/plan.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/riddle.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/writing.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/writing.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/prompts/writing_response.txt` & `airoboros-2.0.8/airoboros/instructors/prompts/writing_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/instructors/simple_task.py` & `airoboros-2.0.8/airoboros/instructors/simple_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,18 @@
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
-    count = instructor.instructor_counts.get(category, 0)
+    if category not in instructor.instructor_counts:
+        instructor.instructor_counts[category] = 0
     language = config.get("language") or instructor.language
-    while count < target_count:
+    while instructor.instructor_counts[category] < target_count:
         # Get a batch of instructions.
         prompt = (
             template.format(batch_size=batch_size, language=language)
             if "{topic_avoidance}" not in template
             else template.format(
                 batch_size=batch_size,
                 language=language,
@@ -85,10 +86,9 @@
             if not response or not response.strip():
                 continue
             yield {
                 "instruction": instructions[idx].strip(),
                 "response": response.strip(),
                 "category": category,
             }
-            count += 1
-            if count >= target_count:
+            if instructor.instructor_counts[category] >= target_count:
                 break
```

### Comparing `airoboros-2.0.7/airoboros/instructors/trivia.py` & `airoboros-2.0.8/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/airoboros/self_instruct.py` & `airoboros-2.0.8/airoboros/self_instruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,15 @@
 
     def persist(self, item):
         """Persist a single item to the output file and docstore."""
         self.outfile.write(json.dumps(item) + "\n")
         self.outfile.flush()
         self.docstores[-1].add_texts([item["instruction"]])
         self.docstore_size += 1
+        self.instructor_counts[item["category"]] += 1
         if self.docstore_size >= MAX_DOCSTORE_SIZE:
             logger.info("Initializing new docstore...")
             self.docstores.append(
                 Chroma.from_texts(["__initialize__"], self.embeddings)
             )
             self.docstore_size = 0
```

### Comparing `airoboros-2.0.7/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.8/airoboros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.7
+Version: 2.0.8
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.7/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.8/airoboros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.7/setup.py` & `airoboros-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.7",
+    version="2.0.8",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

