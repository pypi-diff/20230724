# Comparing `tmp/ai_transform-0.32.5.tar.gz` & `tmp/ai_transform-0.32.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.32.5.tar", last modified: Thu Jul 20 02:38:25 2023, max compression
+gzip compressed data, was "ai_transform-0.32.6.tar", last modified: Mon Jul 24 01:09:54 2023, max compression
```

## Comparing `ai_transform-0.32.5.tar` & `ai_transform-0.32.6.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.276133 ai_transform-0.32.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-20 02:38:03.000000 ai_transform-0.32.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-20 02:38:25.276133 ai_transform-0.32.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-20 02:38:03.000000 ai_transform-0.32.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.256133 ai_transform-0.32.5/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.260133 ai_transform-0.32.5/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.260133 ai_transform-0.32.5/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.260133 ai_transform-0.32.5/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.264133 ai_transform-0.32.5/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.268133 ai_transform-0.32.5/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.268133 ai_transform-0.32.5/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.268133 ai_transform-0.32.5/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-20 02:38:03.000000 ai_transform-0.32.5/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.260133 ai_transform-0.32.5/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-20 02:38:25.000000 ai_transform-0.32.5/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-20 02:38:25.000000 ai_transform-0.32.5/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 02:38:25.000000 ai_transform-0.32.5/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 02:38:25.000000 ai_transform-0.32.5/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 02:38:25.000000 ai_transform-0.32.5/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 02:38:03.000000 ai_transform-0.32.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 02:38:25.276133 ai_transform-0.32.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-20 02:38:03.000000 ai_transform-0.32.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.272133 ai_transform-0.32.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.272133 ai_transform-0.32.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.272133 ai_transform-0.32.5/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.272133 ai_transform-0.32.5/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.272133 ai_transform-0.32.5/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.276133 ai_transform-0.32.5/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:25.276133 ai_transform-0.32.5/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-20 02:38:03.000000 ai_transform-0.32.5/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.334673 ai_transform-0.32.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-24 01:09:33.000000 ai_transform-0.32.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 01:09:54.334673 ai_transform-0.32.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-24 01:09:33.000000 ai_transform-0.32.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.314672 ai_transform-0.32.6/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.318672 ai_transform-0.32.6/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.318672 ai_transform-0.32.6/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.318672 ai_transform-0.32.6/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.322673 ai_transform-0.32.6/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.322673 ai_transform-0.32.6/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.326673 ai_transform-0.32.6/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.326673 ai_transform-0.32.6/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-24 01:09:33.000000 ai_transform-0.32.6/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.314672 ai_transform-0.32.6/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 01:09:54.000000 ai_transform-0.32.6/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-24 01:09:54.000000 ai_transform-0.32.6/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 01:09:54.000000 ai_transform-0.32.6/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 01:09:54.000000 ai_transform-0.32.6/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 01:09:54.000000 ai_transform-0.32.6/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 01:09:33.000000 ai_transform-0.32.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 01:09:54.334673 ai_transform-0.32.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 01:09:33.000000 ai_transform-0.32.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.326673 ai_transform-0.32.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.326673 ai_transform-0.32.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.330673 ai_transform-0.32.6/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.330673 ai_transform-0.32.6/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.330673 ai_transform-0.32.6/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.334673 ai_transform-0.32.6/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:54.334673 ai_transform-0.32.6/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 01:09:33.000000 ai_transform-0.32.6/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.32.5/LICENSE` & `ai_transform-0.32.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/README.md` & `ai_transform-0.32.6/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/__init__.py` & `ai_transform-0.32.6/ai_transform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.32.5"
+__version__ = "0.32.6"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.32.5/ai_transform/api/api.py` & `ai_transform-0.32.6/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/api/client.py` & `ai_transform-0.32.6/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/api/helpers.py` & `ai_transform-0.32.6/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/api/wrappers.py` & `ai_transform-0.32.6/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/components/components.py` & `ai_transform-0.32.6/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/config.py` & `ai_transform-0.32.6/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/dataset/dataset.py` & `ai_transform-0.32.6/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/dataset/field.py` & `ai_transform-0.32.6/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/abstract_engine.py` & `ai_transform-0.32.6/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.32.6/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.32.6/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.6/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.32.6/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.6/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/errors.py` & `ai_transform-0.32.6/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/logger.py` & `ai_transform-0.32.6/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/operator/abstract_operator.py` & `ai_transform-0.32.6/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.6/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/timer.py` & `ai_transform-0.32.6/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/types.py` & `ai_transform-0.32.6/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/utils/document.py` & `ai_transform-0.32.6/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/utils/document_list.py` & `ai_transform-0.32.6/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/utils/example_documents.py` & `ai_transform-0.32.6/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.6/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.6/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.6/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/workflow/context_manager.py` & `ai_transform-0.32.6/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform/workflow/helpers.py` & `ai_transform-0.32.6/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.6/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/setup.py` & `ai_transform-0.32.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from setuptools import find_packages, setup
 
 from ai_transform import __version__
 
-requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic==1.10.2", "icecream==2.1.3"]
+requirements = [
+    "tqdm>=4.49.0",
+    "requests>=2.0.0",
+    "pandas>=1.5.0",
+    "pydantic==1.10.2",
+    "icecream==2.1.3",
+    "typing_extensions<4.6.0",
+]
 
 ray_requirements = ["numpy>=1.19.0", "pyarrow==9.0.0", "ray==2.0.0"]
 
 core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov", "sentence-splitter"]
 
 example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
```

### Comparing `ai_transform-0.32.5/tests/conftest.py` & `ai_transform-0.32.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_api/test_client.py` & `ai_transform-0.32.6/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.6/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.6/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_api/test_wrappers.py` & `ai_transform-0.32.6/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.6/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_dataset/test_field.py` & `ai_transform-0.32.6/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.6/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.32.6/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.6/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.32.6/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.32.6/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.32.6/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.32.6/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.6/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.6/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.5/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.6/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

