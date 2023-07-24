# Comparing `tmp/sparsify-nightly-1.6.0.20230721.tar.gz` & `tmp/sparsify-nightly-1.6.0.20230723.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230721.tar", last modified: Thu Jul 20 20:11:15 2023, max compression
+gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230723.tar", last modified: Sun Jul 23 20:07:38 2023, max compression
```

## Comparing `sparsify-nightly-1.6.0.20230721.tar` & `sparsify-nightly-1.6.0.20230723.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/NOTICE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/create/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4248 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/create/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/create/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/create/schemas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5235 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/login.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/cli/opts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5045 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/cli/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-07-20 20:10:43.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/nm_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/hardware_analyzer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6855 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/error_handler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/scripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2385 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/scripts/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/scripts/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26268 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13031 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/deployment_instructions.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18157 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6896 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8349 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6146 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8345 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/pathway_checks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/ort_health.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/gpu_device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3681 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/task_name.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/nm_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4393 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5067 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      758 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/utils/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/one_shot/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/one_shot/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/one_shot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3758 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/tuning_hyperparameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11587 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/auto_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      316 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23875 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-07-20 20:05:04.000000 sparsify-nightly-1.6.0.20230721/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-20 20:11:15.000000 sparsify-nightly-1.6.0.20230721/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/NOTICE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4248 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5235 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/login.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/opts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5045 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/hardware_analyzer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6855 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/error_handler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2385 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26268 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13031 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/deployment_instructions.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18157 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6896 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8349 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6146 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8088 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/pathway_checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/ort_health.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/gpu_device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/system.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3681 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/task_name.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4393 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5067 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      758 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3758 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/tuning_hyperparameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11587 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/auto_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      316 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23875 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/setup.cfg
```

### Comparing `sparsify-nightly-1.6.0.20230721/NOTICE` & `sparsify-nightly-1.6.0.20230723/NOTICE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/create/api.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/create/api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/create/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/create/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/create/schemas.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/create/schemas.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/login.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/login.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/cli/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/cli/opts.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/opts.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/cli/run.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/run.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/version.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 is_release = False  # change to True to set the generated version as a release version
 
 
 def _generate_version():
     return (
         version_base
         if is_release
-        #else f"{version_base}.{date.today().strftime('%Y%m%d')}"
-        else f"{version_base}.20230721"
+        else f"{version_base}.{date.today().strftime('%Y%m%d')}"
     )
 
 
 __all__ = [
     "__version__",
     "version_base",
     "is_release",
```

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/nm_api.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/nm_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/hardware_analyzer.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/hardware_analyzer.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/helpers.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/utils/error_handler.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/error_handler.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/scripts/main.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/main.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/scripts/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/args.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/transformers/runner.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/deployment_instructions.md` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/deployment_instructions.md`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/args.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/runner.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/args.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/yolov5/runner.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/object_detection/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/args.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/auto/tasks/image_classification/runner.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,19 +73,14 @@
         :return: tuple of training and export arguments
         """
 
         # create train args
         if "dataset" not in config.kwargs:
             # custom datasets are set to imagefolder
             config.kwargs["dataset"] = "imagefolder"
-            if not os.path.exists(config.dataset):
-                raise FileNotFoundError(
-                    f"The custom dataset {config.dataset} "
-                    "does not exist. Please ensure that the path provided is correct."
-                )
 
         if "model_tag" not in config.kwargs:
             config.kwargs["model_tag"] = "sparsify_auto_image_classification"
         train_args = ImageClassificationTrainArgs(
             dataset_path=config.dataset,
             checkpoint_path=config.base_model,
             recipe_path=config.recipe,
```

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/main.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/main.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/pathway_checks.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/pathway_checks.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/ort_health.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/ort_health.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/check_environment/gpu_device.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/gpu_device.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/system.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/system.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/task_name.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/task_name.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/nm_api.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/nm_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/helpers.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/constants.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/utils/exceptions.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/one_shot/api.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/one_shot/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/tuning_hyperparameters.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/tuning_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/auto_api.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/auto_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify/schemas/__init__.py` & `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/PKG-INFO` & `sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsify-nightly
-Version: 1.6.0.20230721
+Version: 1.6.0.20230723
 Summary: Easy-to-use UI for automatically sparsifying neural networks and creating sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Description: 
         <!--
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230721 Summary:
+Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230723 Summary:
 Easy-to-use UI for automatically sparsifying neural networks and creating
 sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com License: Apache Description:
 ****** [Sparsify tool icon]  Sparsify [Alpha] ******
 **** ML model optimization product to accelerate inference ****
 [Documentation] [https://img.shields.io/badge/slack-purple?style=for-the-
```

### Comparing `sparsify-nightly-1.6.0.20230721/src/sparsify_nightly.egg-info/SOURCES.txt` & `sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/README.md` & `sparsify-nightly-1.6.0.20230723/README.md`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/LICENSE` & `sparsify-nightly-1.6.0.20230723/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/setup.py` & `sparsify-nightly-1.6.0.20230723/setup.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230721/PKG-INFO` & `sparsify-nightly-1.6.0.20230723/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsify-nightly
-Version: 1.6.0.20230721
+Version: 1.6.0.20230723
 Summary: Easy-to-use UI for automatically sparsifying neural networks and creating sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Description: 
         <!--
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230721 Summary:
+Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230723 Summary:
 Easy-to-use UI for automatically sparsifying neural networks and creating
 sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com License: Apache Description:
 ****** [Sparsify tool icon]  Sparsify [Alpha] ******
 **** ML model optimization product to accelerate inference ****
 [Documentation] [https://img.shields.io/badge/slack-purple?style=for-the-
```

### Comparing `sparsify-nightly-1.6.0.20230721/setup.cfg` & `sparsify-nightly-1.6.0.20230723/setup.cfg`

 * *Files identical despite different names*

