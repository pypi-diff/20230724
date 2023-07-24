# Comparing `tmp/modelz-llm-23.7.1.tar.gz` & `tmp/modelz-llm-23.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.7.1.tar", last modified: Fri Jul 21 04:35:20 2023, max compression
+gzip compressed data, was "modelz-llm-23.7.2.tar", last modified: Mon Jul 24 04:00:20 2023, max compression
```

## Comparing `modelz-llm-23.7.1.tar` & `modelz-llm-23.7.2.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/docs/images/deploy.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.114982 modelz-llm-23.7.1/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/bloomz-560m/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/bloomz-560m/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/chatglm-6b-int4/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/chatglm-6b-int4/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.118982 modelz-llm-23.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 04:35:19.000000 modelz-llm-23.7.1/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/uds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-21 04:35:05.000000 modelz-llm-23.7.1/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:35:20.122982 modelz-llm-23.7.1/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 04:35:20.000000 modelz-llm-23.7.1/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.704725 modelz-llm-23.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.704725 modelz-llm-23.7.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/docs/images/deploy.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/bloomz-560m/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/bloomz-560m/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/chatglm-6b-int4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/chatglm-6b-int4/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/llama-2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-2-7b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/uds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.7.1/.github/workflows/docker-publish.yml` & `modelz-llm-23.7.2/.github/workflows/docker-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
           - name: modelzai/llm-fastchat-t5-3b
             dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
             dockerfile: ./images/vicuna-7b/Dockerfile
+          - name: meta-llama/Llama-2-7b-hf
+            dockerfile: ./images/llama-2-7b/Dockerfile
     runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
```

### Comparing `modelz-llm-23.7.1/.github/workflows/gcr.yml` & `modelz-llm-23.7.2/.github/workflows/gcr.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
           - name: modelzai/llm-fastchat-t5-3b
             dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
             dockerfile: ./images/vicuna-7b/Dockerfile
+          - name: meta-llama/Llama-2-7b-hf
+            dockerfile: ./images/llama-2-7b/Dockerfile
     runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
```

### Comparing `modelz-llm-23.7.1/.github/workflows/python-check.yml` & `modelz-llm-23.7.2/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/.github/workflows/python-publish.yml` & `modelz-llm-23.7.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/.gitignore` & `modelz-llm-23.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/PKG-INFO` & `modelz-llm-23.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.7.1
+Version: 23.7.2
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.1 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.2 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.7.1/README.md` & `modelz-llm-23.7.2/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/build.envd` & `modelz-llm-23.7.2/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/client.py` & `modelz-llm-23.7.2/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/docs/images/deploy.svg` & `modelz-llm-23.7.2/docs/images/deploy.svg`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/images/bloomz-560m/Dockerfile` & `modelz-llm-23.7.2/images/bloomz-560m/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,18 @@
 ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
-COPY requirements.txt /
+COPY requirements-cpu.txt /
 
-RUN pip install -r requirements.txt
+RUN pip install torch --extra-index-url https://download.pytorch.org/whl/cpu
+RUN pip install -r requirements-cpu.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .
```

### Comparing `modelz-llm-23.7.1/images/chatglm-6b/Dockerfile` & `modelz-llm-23.7.2/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/images/chatglm-6b-int4/Dockerfile` & `modelz-llm-23.7.2/images/chatglm-6b-int4/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.7.2/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/images/llama-7b/Dockerfile` & `modelz-llm-23.7.2/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/images/vicuna-7b/Dockerfile` & `modelz-llm-23.7.2/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/pyproject.toml` & `modelz-llm-23.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/cli.py` & `modelz-llm-23.7.2/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/emb.py` & `modelz-llm-23.7.2/src/modelz_llm/emb.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/falcon_service.py` & `modelz-llm-23.7.2/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/model.py` & `modelz-llm-23.7.2/src/modelz_llm/model.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/mosec_service.py` & `modelz-llm-23.7.2/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/uds.py` & `modelz-llm-23.7.2/src/modelz_llm/uds.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm/utils.py` & `modelz-llm-23.7.2/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.1/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.7.2/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.7.1
+Version: 23.7.2
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.1 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.2 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.7.1/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.7.2/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/workflows/python-check.yml
 .github/workflows/python-publish.yml
 docs/images/deploy.svg
 images/bloomz-560m/Dockerfile
 images/chatglm-6b/Dockerfile
 images/chatglm-6b-int4/Dockerfile
 images/fastchat-t5-3b/Dockerfile
+images/llama-2-7b/Dockerfile
 images/llama-7b/Dockerfile
 images/llama-7b/requirements.txt
 images/vicuna-7b/Dockerfile
 src/modelz_llm/__init__.py
 src/modelz_llm/_version.py
 src/modelz_llm/cli.py
 src/modelz_llm/emb.py
```

