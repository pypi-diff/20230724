# Comparing `tmp/microlearn_llm_factory-0.0.3.tar.gz` & `tmp/microlearn_llm_factory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_llm_factory-0.0.3.tar", last modified: Thu Jul 20 08:54:29 2023, max compression
+gzip compressed data, was "microlearn_llm_factory-0.0.4.tar", last modified: Mon Jul 24 06:59:33 2023, max compression
```

## Comparing `microlearn_llm_factory-0.0.3.tar` & `microlearn_llm_factory-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.818252 microlearn_llm_factory-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.814252 microlearn_llm_factory-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.814252 microlearn_llm_factory-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 08:54:29.818252 microlearn_llm_factory-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-20 08:54:29.818252 microlearn_llm_factory-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.814252 microlearn_llm_factory-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.814252 microlearn_llm_factory-0.0.3/src/llm_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/src/llm_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/src/llm_factory/llm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/src/llm_factory/llm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/src/llm_factory/llm_openai_chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.814252 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 08:54:29.000000 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 08:54:29.000000 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:54:29.000000 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 08:54:29.000000 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 08:54:29.000000 microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:54:29.818252 microlearn_llm_factory-0.0.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-20 08:54:17.000000 microlearn_llm_factory-0.0.3/src/tests/test_llm_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/src/llm_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_openai_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/tests/test_llm_factory.py
```

### Comparing `microlearn_llm_factory-0.0.3/.github/workflows/publish.yml` & `microlearn_llm_factory-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.3/PKG-INFO` & `microlearn_llm_factory-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn_llm_factory
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for managing microlearn LLM interaction classes
 Home-page: https://github.com/AIprojectflow/llm_factory
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/llm_factory/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/llm_factory/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_llm_factory-0.0.3/setup.cfg` & `microlearn_llm_factory-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.3/src/llm_factory/llm_factory.py` & `microlearn_llm_factory-0.0.4/src/llm_factory/llm_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,7 +18,15 @@
 
     def build_llm(self, llm_type: str, **kwargs):
         if llm_type == self.LLM_OPENAI_CHAT_NAME:
             from llm_factory.llm_openai_chat import LLMOpenAIChat
             return LLMOpenAIChat().get_llm(**kwargs)
         else:
             raise ValueError(f"Invalid llm_type: {llm_type}")
+
+    def build_llm_default(self):
+        from llm_factory.llm_openai_chat import LLMOpenAIChat
+        kwargs = LLMOpenAIChat.get_default_args()
+        return self.build_llm(
+            llm_type=self.LLM_OPENAI_CHAT_NAME,
+            **kwargs,
+        )
```

### Comparing `microlearn_llm_factory-0.0.3/src/microlearn_llm_factory.egg-info/PKG-INFO` & `microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn-llm-factory
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for managing microlearn LLM interaction classes
 Home-page: https://github.com/AIprojectflow/llm_factory
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/llm_factory/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/llm_factory/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

