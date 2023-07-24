# Comparing `tmp/paper-qa-3.4.0.tar.gz` & `tmp/paper-qa-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.4.0.tar", last modified: Sat Jul 22 16:10:24 2023, max compression
+gzip compressed data, was "paper-qa-3.4.1.tar", last modified: Mon Jul 24 19:21:56 2023, max compression
```

## Comparing `paper-qa-3.4.0.tar` & `paper-qa-3.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.078141 paper-qa-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 16:09:47.000000 paper-qa-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-22 16:10:24.078141 paper-qa-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-22 16:09:47.000000 paper-qa-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.070141 paper-qa-3.4.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.074141 paper-qa-3.4.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.074141 paper-qa-3.4.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:10:24.078141 paper-qa-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-22 16:09:47.000000 paper-qa-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.078141 paper-qa-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-07-22 16:09:47.000000 paper-qa-3.4.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 19:21:09.000000 paper-qa-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-24 19:21:56.796503 paper-qa-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-24 19:21:09.000000 paper-qa-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.792503 paper-qa-3.4.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23961 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:21:56.796503 paper-qa-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-24 19:21:09.000000 paper-qa-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-07-24 19:21:09.000000 paper-qa-3.4.1/tests/test_paperqa.py
```

### Comparing `paper-qa-3.4.0/LICENSE` & `paper-qa-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/PKG-INFO` & `paper-qa-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.4.0
+Version: 3.4.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.4.0/README.md` & `paper-qa-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.4.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.4.0
+Version: 3.4.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.4.0/paperqa/chains.py` & `paper-qa-3.4.1/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paperqa/contrib/zotero.py` & `paper-qa-3.4.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paperqa/docs.py` & `paper-qa-3.4.1/paperqa/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
             # I also cannot know what the exception
             # type is because any model could be used
             # my best idea is see if there is a 4XX
             # http code in the exception
             try:
                 citation = match.metadata["doc"]["citation"]
                 if detailed_citations:
-                    match.metadata["name"] + ": " + citation
+                    citation = match.metadata["name"] + ": " + citation
                 context = await summary_chain.arun(
                     question=answer.question,
                     # Add name so chunk is stated
                     citation=citation,
                     summary_length=answer.summary_length,
                     text=match.page_content,
                     callbacks=callbacks,
@@ -489,15 +489,15 @@
         contexts = sorted(contexts, key=lambda x: x.score, reverse=True)
         contexts = contexts[:max_sources]
         # add to answer contexts
         answer.contexts += contexts
         context_str = "\n\n".join(
             [
                 f"{c.text.name}: {c.context}"
-                + (f". Based on {c.text.doc.citation}" if detailed_citations else "")
+                + (f" Based on {c.text.doc.citation}" if detailed_citations else "")
                 for c in answer.contexts
             ]
         )
         valid_names = [c.text.name for c in answer.contexts]
         context_str += "\n\nValid keys: " + ", ".join(valid_names)
         answer.context = context_str
         return answer
```

### Comparing `paper-qa-3.4.0/paperqa/prompts.py` & `paper-qa-3.4.1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paperqa/readers.py` & `paper-qa-3.4.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paperqa/types.py` & `paper-qa-3.4.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/paperqa/utils.py` & `paper-qa-3.4.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/setup.py` & `paper-qa-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.0/tests/test_paperqa.py` & `paper-qa-3.4.1/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,30 @@
 
 
 class TestHandler(AsyncCallbackHandler):
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         print(token)
 
 
+def test_location_awareness():
+    tests_dir = os.path.dirname(os.path.abspath(__file__))
+    doc_path = os.path.join(tests_dir, "paper.pdf")
+    with open(doc_path, "rb") as f:
+        docs = Docs()
+        docs.add_file(f, "Wellawatte et al, XAI Review, 2023")
+        answer = docs.get_evidence(
+            Answer(
+                question="Which page is the statement 'Deep learning (DL) is advancing the boundaries of computational"
+                + "chemistry because it can accurately model non-linear structure-function relationships.' on?"
+            ),
+            detailed_citations=True,
+        )
+        assert "2" in answer.context or "1" in answer.context
+
+
 def test_maybe_is_text():
     assert maybe_is_text("This is a test. The sample conc. was 1.0 mM (at 245 ^F)")
     assert not maybe_is_text("\\C0\\C0\\B1\x00")
     # get front page of wikipedia
     r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
     assert maybe_is_text(r.text)
```

