# Comparing `tmp/modelz-llm-23.7.2.tar.gz` & `tmp/modelz-llm-23.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.7.2.tar", last modified: Mon Jul 24 04:00:20 2023, max compression
+gzip compressed data, was "modelz-llm-23.7.3.tar", last modified: Mon Jul 24 08:42:24 2023, max compression
```

## Comparing `modelz-llm-23.7.2.tar` & `modelz-llm-23.7.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.704725 modelz-llm-23.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.704725 modelz-llm-23.7.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/docs/images/deploy.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/bloomz-560m/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/bloomz-560m/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/chatglm-6b-int4/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/chatglm-6b-int4/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/llama-2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-2-7b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.708725 modelz-llm-23.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/uds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 04:00:07.000000 modelz-llm-23.7.2/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 04:00:20.712725 modelz-llm-23.7.2/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 04:00:20.000000 modelz-llm-23.7.2/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.216551 modelz-llm-23.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.208551 modelz-llm-23.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 08:42:24.216551 modelz-llm-23.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.208551 modelz-llm-23.7.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/docs/images/deploy.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.208551 modelz-llm-23.7.3/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/bloomz-560m/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/bloomz-560m/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/chatglm-6b-int4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/chatglm-6b-int4/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/llama-2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/llama-2-7b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:42:24.216551 modelz-llm-23.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.208551 modelz-llm-23.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.212551 modelz-llm-23.7.3/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/uds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 08:42:12.000000 modelz-llm-23.7.3/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:42:24.216551 modelz-llm-23.7.3/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 08:42:24.000000 modelz-llm-23.7.3/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.7.2/.github/workflows/docker-publish.yml` & `modelz-llm-23.7.3/.github/workflows/docker-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   release:
     types: [created]
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.ref }}-${{ github.workflow }}
-  cancel-in-progress: true
+  cancel-in-progress: false
 
 env:
   REGISTRY: docker.io
 
 jobs:
   build:
     strategy:
```

### Comparing `modelz-llm-23.7.2/.github/workflows/gcr.yml` & `modelz-llm-23.7.3/.github/workflows/gcr.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   release:
     types: [created]
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.ref }}-${{ github.workflow }}
-  cancel-in-progress: true
+  cancel-in-progress: false
 
 env:
   REGISTRY: us-central1-docker.pkg.dev/nth-guide-378813
 
 jobs:
   build:
     strategy:
```

### Comparing `modelz-llm-23.7.2/.github/workflows/python-check.yml` & `modelz-llm-23.7.3/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/.github/workflows/python-publish.yml` & `modelz-llm-23.7.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/.gitignore` & `modelz-llm-23.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/PKG-INFO` & `modelz-llm-23.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.7.2
+Version: 23.7.3
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.2 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.3 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.7.2/README.md` & `modelz-llm-23.7.3/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/build.envd` & `modelz-llm-23.7.3/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/client.py` & `modelz-llm-23.7.3/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/docs/images/deploy.svg` & `modelz-llm-23.7.3/docs/images/deploy.svg`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/images/bloomz-560m/Dockerfile` & `modelz-llm-23.7.3/images/bloomz-560m/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/images/chatglm-6b/Dockerfile` & `modelz-llm-23.7.3/images/chatglm-6b-int4/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,15 @@
     ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
     echo "conda activate base" >> ~/.bashrc && \
     find /opt/conda/ -follow -type f -name '*.a' -delete && \
     find /opt/conda/ -follow -type f -name '*.js.map' -delete && \
     /opt/conda/bin/conda clean -afy
 
-RUN conda create -n envd python=3.9
-
-ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
+ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
 COPY requirements.txt /
@@ -61,14 +59,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model THUDM/chatglm-6b
+# RUN modelz-llm --dry-run --model THUDM/chatglm-6b-int4
 
-# # disable huggingface update check (could be very slow)
+# disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
-CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b" ]
+CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b-int4" ]
```

### Comparing `modelz-llm-23.7.2/images/chatglm-6b-int4/Dockerfile` & `modelz-llm-23.7.3/images/vicuna-7b/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -51,24 +51,24 @@
 ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
-COPY requirements.txt /
+COPY ./images/llama-7b/requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run --model THUDM/chatglm-6b-int4
+# RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
 
-# disable huggingface update check (could be very slow)
-ENV HF_HUB_OFFLINE=true
+# # disable huggingface update check (could be very slow)
+# ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
-CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b-int4" ]
+CMD [ "--port", "8080", "--model", "lmsys/vicuna-7b-delta-v1.1" ]
```

### Comparing `modelz-llm-23.7.2/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.7.3/images/fastchat-t5-3b/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,15 @@
     ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
     echo "conda activate base" >> ~/.bashrc && \
     find /opt/conda/ -follow -type f -name '*.a' -delete && \
     find /opt/conda/ -follow -type f -name '*.js.map' -delete && \
     /opt/conda/bin/conda clean -afy
 
-RUN conda create -n envd python=3.9
-
-ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
+ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
 COPY requirements.txt /
```

### Comparing `modelz-llm-23.7.2/images/llama-2-7b/Dockerfile` & `modelz-llm-23.7.3/images/llama-2-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
+# RUN modelz-llm --dry-run --model meta-llama/Llama-2-7b-hf
 
 # # disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "meta-llama/Llama-2-7b-hf" ]
```

### Comparing `modelz-llm-23.7.2/images/llama-7b/Dockerfile` & `modelz-llm-23.7.3/images/llama-7b/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,15 @@
     ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
     echo "conda activate base" >> ~/.bashrc && \
     find /opt/conda/ -follow -type f -name '*.a' -delete && \
     find /opt/conda/ -follow -type f -name '*.js.map' -delete && \
     /opt/conda/bin/conda clean -afy
 
-RUN conda create -n envd python=3.9
-
-ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
+ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
 COPY ./images/llama-7b/requirements.txt /
```

### Comparing `modelz-llm-23.7.2/images/vicuna-7b/Dockerfile` & `modelz-llm-23.7.3/images/chatglm-6b/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -42,33 +42,31 @@
     ln -s /opt/conda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     echo ". /opt/conda/etc/profile.d/conda.sh" >> ~/.bashrc && \
     echo "conda activate base" >> ~/.bashrc && \
     find /opt/conda/ -follow -type f -name '*.a' -delete && \
     find /opt/conda/ -follow -type f -name '*.js.map' -delete && \
     /opt/conda/bin/conda clean -afy
 
-RUN conda create -n envd python=3.9
-
-ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
+ENV ENVD_PREFIX=/opt/conda/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
-COPY ./images/llama-7b/requirements.txt /
+COPY requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
+# RUN modelz-llm --dry-run --model THUDM/chatglm-6b
 
 # # disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
-CMD [ "--port", "8080", "--model", "lmsys/vicuna-7b-delta-v1.1" ]
+CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b" ]
```

### Comparing `modelz-llm-23.7.2/pyproject.toml` & `modelz-llm-23.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/cli.py` & `modelz-llm-23.7.3/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/emb.py` & `modelz-llm-23.7.3/src/modelz_llm/emb.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/falcon_service.py` & `modelz-llm-23.7.3/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/model.py` & `modelz-llm-23.7.3/src/modelz_llm/model.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/mosec_service.py` & `modelz-llm-23.7.3/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/uds.py` & `modelz-llm-23.7.3/src/modelz_llm/uds.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm/utils.py` & `modelz-llm-23.7.3/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.7.2/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.7.3/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.7.2
+Version: 23.7.3
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.2 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.7.3 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.7.2/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.7.3/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

