# Comparing `tmp/aihero-0.2.6.tar.gz` & `tmp/aihero-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihero-0.2.6.tar", last modified: Mon Jul 17 06:22:27 2023, max compression
+gzip compressed data, was "aihero-0.2.7.tar", last modified: Mon Jul 24 02:54:41 2023, max compression
```

## Comparing `aihero-0.2.6.tar` & `aihero-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.047639 aihero-0.2.6/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.6/LICENSE
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-17 06:22:27.047899 aihero-0.2.6/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.6/README.md
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.040615 aihero-0.2.6/aihero/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      242 2023-07-14 19:26:45.000000 aihero-0.2.6/aihero/__init__.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 14:51:50.000000 aihero-0.2.6/aihero/client.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.6/aihero/exceptions.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.6/aihero/openai_helper.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1202 2023-07-13 14:38:04.000000 aihero-0.2.6/aihero/project.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     4919 2023-07-15 17:44:18.000000 aihero-0.2.6/aihero/promptstash.py
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.046991 aihero-0.2.6/aihero.egg-info/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/SOURCES.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/dependency_links.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       13 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/requires.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/top_level.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1017 2023-07-17 06:22:27.048884 aihero-0.2.6/setup.cfg
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.6/setup.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-24 02:54:41.149296 aihero-0.2.7/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.7/LICENSE
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     4471 2023-07-24 02:54:41.149495 aihero-0.2.7/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3496 2023-07-17 19:30:18.000000 aihero-0.2.7/README.md
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-24 02:54:41.142973 aihero-0.2.7/aihero/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      242 2023-07-22 16:49:15.000000 aihero-0.2.7/aihero/__init__.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 14:51:50.000000 aihero-0.2.7/aihero/client.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     9684 2023-07-23 02:05:03.000000 aihero-0.2.7/aihero/eval.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.7/aihero/exceptions.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3596 2023-07-23 01:22:45.000000 aihero-0.2.7/aihero/openai_helper.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1202 2023-07-22 17:52:48.000000 aihero-0.2.7/aihero/project.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     7602 2023-07-24 02:05:42.000000 aihero-0.2.7/aihero/promptstash.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-24 02:54:41.148727 aihero-0.2.7/aihero.egg-info/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     4471 2023-07-24 02:54:41.000000 aihero-0.2.7/aihero.egg-info/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      321 2023-07-24 02:54:41.000000 aihero-0.2.7/aihero.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-24 02:54:41.000000 aihero-0.2.7/aihero.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       13 2023-07-24 02:54:41.000000 aihero-0.2.7/aihero.egg-info/requires.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-24 02:54:41.000000 aihero-0.2.7/aihero.egg-info/top_level.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1017 2023-07-24 02:54:41.150611 aihero-0.2.7/setup.cfg
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.7/setup.py
```

### Comparing `aihero-0.2.6/LICENSE` & `aihero-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aihero-0.2.6/aihero/client.py` & `aihero-0.2.7/aihero/client.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.6/aihero/openai_helper.py` & `aihero-0.2.7/aihero/openai_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-
 import httpx
 
 BASE_URL = "https://api.openai.com/v1/"
 COMPLETIONS = "completions"
 MODEL = "text-davinci-003"
 EMBEDDINGS = "embeddings"
+CHAT_COMPLETIONS = "chat/completions"
 EMBEDDINGS_MODEL = "text-embedding-ada-002"
 OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
 
 
 def has_key():
     return OPENAI_API_KEY is not None
 
@@ -60,7 +60,46 @@
             if "errors" in prediction_object:
                 return None, prediction_object["errors"][0]["text"].strip()
             else:
                 embedding = prediction_object["data"][0]["embedding"]
                 return embedding, None
     except httpx.HTTPError as http_error:
         return None, str(http_error)
+
+
+class ChatCompletion:
+    def __init__(self, system_message, api_key: str = OPENAI_API_KEY):
+        self.api_key = api_key
+        self.messages = [
+            {
+                "role": "system",
+                "content": system_message,
+            }
+        ]
+
+    def chat(self, message: str) -> str:
+        self.messages.append(
+            {"role": "user", "content": message},
+        )
+        try:
+            with httpx.Client(
+                base_url=BASE_URL,
+                headers={
+                    "Content-Type": "application/json",
+                    "Authorization": f"Bearer {self.api_key}",
+                },
+            ) as client:
+                resp = client.post(
+                    CHAT_COMPLETIONS,
+                    json={"model": "gpt-3.5-turbo", "messages": self.messages},
+                    timeout=30,
+                )
+                resp.raise_for_status()
+                prediction_object = resp.json()
+                if "errors" in prediction_object:
+                    return None, prediction_object["errors"][0]["text"].strip()
+                else:
+                    reply = prediction_object["choices"][0]["message"]["content"]
+                    self.messages.append({"role": "assistant", "content": reply})
+                    return reply, None
+        except httpx.HTTPError as http_error:
+            return None, str(http_error)
```

### Comparing `aihero-0.2.6/aihero/project.py` & `aihero-0.2.7/aihero/project.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.6/aihero/promptstash.py` & `aihero-0.2.7/aihero/promptstash.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from threading import Thread
 from .client import Client
+from threading import Thread
 from .exceptions import AIHeroException
 from .openai_helper import get_embedding, has_key
 from warnings import warn
+from datetime import datetime
+from .eval import PromptTestSuite
 
 
 class PromptStash:
     def __init__(
         self,
         project_id: str,
         client: Client,
@@ -75,65 +77,159 @@
             )
             return prompt_template_dict["template"]
 
     def _sync_stash_completion(
         self,
         template_id: str,
         variant: str,
-        inputs: str,
+        trace_id: str,
+        step_id: str,
+        inputs: dict,
+        rendered_inputs: str,
         prompt: str,
         output: str,
-        trace_id: str = None,
+        model: dict,
+        metrics: dict,
         other: dict = None,
+        created_at: str = datetime.now().isoformat(),
     ):
-        inputs_embedding, err = get_embedding(inputs)
+        inputs_embedding, err = get_embedding(rendered_inputs)
         if err:
-            warn("Error generating embedding for inputs in child thread.")
+            warn("Error generating embedding for rendered_inputs in child thread.")
             raise AIHeroException(err)
         prompt_embedding, err = get_embedding(prompt)
         if err:
             warn("Error generating embedding for prompt in child thread.")
             raise AIHeroException(err)
         output_embedding, err = get_embedding(output)
         if err:
             warn("Error generating embedding for output in child thread.")
             raise AIHeroException(err)
 
         stash_obj = {
+            "trace_id": trace_id,
+            "step_id": step_id,
+            "step_type": "completion",
+            "template_id": template_id,
+            "variant": variant,
             "inputs": inputs,
+            "rendered_inputs": rendered_inputs,
             "prompt": prompt,
             "output": output,
             "inputs_embedding": inputs_embedding,
             "prompt_embedding": prompt_embedding,
             "output_embedding": output_embedding,
-            "trace_id": trace_id,
+            "model": model,
+            "metrics": metrics,
+            "created_at": created_at,
         }
 
         if other is None:
             other = {}
         other.update({"embedding_model": "text-embedding-ada-002"})
         stash_obj["other"] = other
 
         self._client.post(
-            f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}/variants/{variant}/stash",
+            f"/tools/promptstash/projects/{self._project_id}/stash",
             obj=stash_obj,
             timeout=30,
         )
         print("Prompt stashed.")
 
     def stash_completion(
         self,
         template_id: str,
         variant: str,
-        inputs: str,
+        trace_id: str,
+        step_id: str,
+        inputs: dict,
+        rendered_inputs: str,
         prompt: str,
         output: str,
+        model: dict,
+        metrics: dict,
         other: dict = None,
-        trace_id: str = None,
     ):
         if has_key():
             Thread(
                 target=self._sync_stash_completion,
-                args=(template_id, variant, prompt, output, inputs, trace_id, other),
+                args=(
+                    template_id,
+                    variant,
+                    trace_id,
+                    step_id,
+                    inputs,
+                    rendered_inputs,
+                    prompt,
+                    output,
+                    model,
+                    metrics,
+                    other,
+                ),
             ).start()
         else:
             raise AIHeroException("No OPENAI_API_KEY in env variables.")
+
+    def _sync_stash_feedback(
+        self,
+        trace_id: str,
+        step_id: str,
+        thumbs_up: bool,
+        thumbs_down: bool,
+        correction: str,
+        annotations: dict,
+        other: dict = None,
+        created_at: str = datetime.now().isoformat(),
+    ):
+        stash_obj = {
+            "trace_id": trace_id,
+            "step_id": step_id,
+            "step_type": "feedback",
+            "thumbs_up": thumbs_up,
+            "thumbs_down": thumbs_down,
+            "correction": correction,
+            "annotations": annotations,
+            "created_at": created_at,
+        }
+        if other is None:
+            other = {}
+        stash_obj["other"] = other
+        self._client.post(
+            f"/tools/promptstash/projects/{self._project_id}/stash",
+            obj=stash_obj,
+            timeout=30,
+        )
+        print("Feedback stashed.")
+
+    def stash_feedback(
+        self,
+        trace_id: str,
+        step_id: str,
+        thumbs_up: bool,
+        thumbs_down: bool,
+        correction: str,
+        annotations: dict,
+        other: dict = None,
+    ):
+        if has_key():
+            Thread(
+                target=self._sync_stash_feedback,
+                args=(
+                    trace_id,
+                    step_id,
+                    thumbs_up,
+                    thumbs_down,
+                    correction,
+                    annotations,
+                    other,
+                ),
+            ).start()
+        else:
+            raise AIHeroException("No OPENAI_API_KEY in env variables.")
+
+    def build_test_suite(
+        self, test_suite_id: str, test_suite_cls: type
+    ) -> PromptTestSuite:
+        assert issubclass(test_suite_cls, PromptTestSuite)
+        return test_suite_cls(
+            self._project_id, self._client, test_suite_id=test_suite_id
+        )
```

### Comparing `aihero-0.2.6/setup.cfg` & `aihero-0.2.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aihero
-version = 0.2.6
+version = 0.2.7
 description = AI Hero Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ai-hero/python-client-sdk
 author = AI Hero Team
 author_email = team@aihero.studio
 license = MIT
```

