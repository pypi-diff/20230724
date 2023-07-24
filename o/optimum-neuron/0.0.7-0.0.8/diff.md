# Comparing `tmp/optimum-neuron-0.0.7.tar.gz` & `tmp/optimum-neuron-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.7.tar", last modified: Wed Jul  5 10:24:25 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.8.tar", last modified: Mon Jul 24 15:59:54 2023, max compression
```

## Comparing `optimum-neuron-0.0.7.tar` & `optimum-neuron-0.0.8.tar`

### file list

```diff
@@ -1,93 +1,101 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.7/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.7/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.7/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5327 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/optimum/commands/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-07-04 11:50:34.000000 optimum-neuron-0.0.7/optimum/commands/neuron/cache.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.7/optimum/commands/register/register_export.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.7/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      855 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9110 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12319 2023-07-05 10:19:53.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1669 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22439 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9148 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/model_configs.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5953 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2498 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/accelerate/
--rw-rw-r--   0 michael   (1000) michael   (1000)      785 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    19501 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/accelerator.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3019 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/optimizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/scheduler.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    16801 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/state.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)      789 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7907 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/dataclasses.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/misc.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/distributed/
--rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7687 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2247 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/decoder_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2666 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/encoder_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4502 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/parallel_layers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3219 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/parallelizers_manager.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4749 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/generation/
--rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.7/optimum/neuron/generation/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/generation/utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    20362 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/modeling_base.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/pipelines/
--rw-rw-r--   0 michael   (1000) michael   (1000)      666 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/
--rw-rw-r--   0 michael   (1000) michael   (1000)      658 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9124 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13323 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    17146 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9224 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/training_args.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1297 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6397 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    33731 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/utils/compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/utils/constant.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/misc.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1994 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/optimization_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7282 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/utils/patching.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1461 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-07-05 10:21:01.000000 optimum-neuron-0.0.7/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     2513 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.7/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-07-05 10:23:48.000000 optimum-neuron-0.0.7/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    35375 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/tests/test_compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/tests/test_generate.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    49320 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/tests/test_modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.7/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.509668 optimum-neuron-0.0.8/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11357 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/LICENSE
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      651 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/MANIFEST.in
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10778 2023-07-24 15:59:54.509976 optimum-neuron-0.0.8/PKG-INFO
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9523 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/README.md
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.411312 optimum-neuron-0.0.8/optimum/
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.410793 optimum-neuron-0.0.8/optimum/commands/
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.423614 optimum-neuron-0.0.8/optimum/commands/export/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5451 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/export/neuron.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5327 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/export/neuronx.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.426373 optimum-neuron-0.0.8/optimum/commands/neuron/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1428 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/base.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     8808 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/cache.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2214 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/subcommands.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.428052 optimum-neuron-0.0.8/optimum/commands/register/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1270 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/register/register_export.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      755 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/register/register_neuron.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.411122 optimum-neuron-0.0.8/optimum/exporters/
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.436245 optimum-neuron-0.0.8/optimum/exporters/neuron/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      998 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11479 2023-07-24 15:26:45.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/__main__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    14853 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/base.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1810 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/config.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    22613 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/convert.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9979 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/model_configs.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11140 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/utils.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.447655 optimum-neuron-0.0.8/optimum/neuron/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2993 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/__init__.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.455206 optimum-neuron-0.0.8/optimum/neuron/accelerate/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      785 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    23071 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/accelerator.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4637 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/optimizer.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2212 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/scheduler.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16801 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/state.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.459670 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      789 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     7899 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/dataclasses.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1076 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/misc.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.467890 optimum-neuron-0.0.8/optimum/neuron/distributed/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      902 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16900 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/base.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4041 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/checkpointing.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5459 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/decoder_models.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2844 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/encoder_models.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11929 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/parallel_layers.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3364 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/parallelizers_manager.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    23651 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/utils.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.470228 optimum-neuron-0.0.8/optimum/neuron/generation/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      668 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/generation/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    70566 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/generation/utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2337 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/hf_argparser.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    38265 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    19850 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_base.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10917 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_decoder.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    21219 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_diffusion.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.473454 optimum-neuron-0.0.8/optimum/neuron/pipelines/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      666 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/__init__.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.474301 optimum-neuron-0.0.8/optimum/neuron/pipelines/diffusers/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    12432 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.475990 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      658 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9124 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/base.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    14102 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/trainer_callback.py
+-rwxr-xr-x   0 michaelbenayoun   (501) staff       (20)    20239 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/trainers.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9419 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/training_args.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.494068 optimum-neuron-0.0.8/optimum/neuron/utils/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1491 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/__init__.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     6793 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/argument_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    34728 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/cache_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16574 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/compilation_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      885 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/constant.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2002 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/import_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    22030 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/misc.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1994 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/optimization_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     7766 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/patching.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1734 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/require_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1644 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/testing_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10602 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/training_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3102 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/version_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      639 2023-07-24 15:27:59.000000 optimum-neuron-0.0.8/optimum/neuron/version.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.498348 optimum-neuron-0.0.8/optimum_neuron.egg-info/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10778 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/PKG-INFO
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2801 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)       39 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)       66 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/entry_points.txt
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)        1 2023-07-24 14:56:07.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/not-zip-safe
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      507 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/requires.txt
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)        8 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/top_level.txt
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1161 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/pyproject.toml
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)      430 2023-07-24 15:59:54.511131 optimum-neuron-0.0.8/setup.cfg
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3060 2023-07-24 15:59:45.000000 optimum-neuron-0.0.8/setup.py
+drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.508808 optimum-neuron-0.0.8/tests/
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    35375 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_cache_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3415 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_compilation_utils.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    27302 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_examples.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4696 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_generate.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    49320 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_modeling.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5994 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_modeling_decoder.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9277 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_trainer_callback.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)    17847 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_trainers.py
+-rw-r--r--   0 michaelbenayoun   (501) staff       (20)     8584 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.7/LICENSE` & `optimum-neuron-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/MANIFEST.in` & `optimum-neuron-0.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/PKG-INFO` & `optimum-neuron-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.7
+Version: 0.0.8
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: quality
 Provides-Extra: neuron
 Provides-Extra: neuronx
+Provides-Extra: diffusers
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
@@ -37,15 +38,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 -->
 
 # Optimum Neuron
 
-🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls). 
+🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls).
 It provides a set of tools enabling easy model loading, training and inference on single- and multi-Accelerator settings for different downstream tasks.
 The list of officially validated models and tasks is available [here](TODO:). Users can try other models and tasks with only few changes.
 
 ## Install
 To install the latest release of this package:
 
 ```bash
@@ -79,22 +80,22 @@
 
 🤗 Optimum Neuron was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers user while leveraging the complete power of AWS Accelerators**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - TrainiumArgumentParser: inherits the original [HfArgumentParser](https://huggingface.co/docs/transformers/main/en/internal/trainer_utils#transformers.HfArgumentParser) in Transformers with additional checks on the argument values to make sure that they will work well with AWS Trainium instances.
-- [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
+- [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
 
-The [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the TrainiumTrainer one.
+The [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the NeuronTrainer one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-neuron/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 ```diff
 from transformers import TrainingArguments
-+from optimum.neuron import TrainiumTrainer as Trainer
++from optimum.neuron import NeuronTrainer as Trainer
 
 training_args = TrainingArguments(
   # training arguments...
 )
 
 # A lot of code here
```

### Comparing `optimum-neuron-0.0.7/README.md` & `optimum-neuron-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 -->
 
 # Optimum Neuron
 
-🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls). 
+🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls).
 It provides a set of tools enabling easy model loading, training and inference on single- and multi-Accelerator settings for different downstream tasks.
 The list of officially validated models and tasks is available [here](TODO:). Users can try other models and tasks with only few changes.
 
 ## Install
 To install the latest release of this package:
 
 ```bash
@@ -54,22 +54,22 @@
 
 🤗 Optimum Neuron was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers user while leveraging the complete power of AWS Accelerators**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - TrainiumArgumentParser: inherits the original [HfArgumentParser](https://huggingface.co/docs/transformers/main/en/internal/trainer_utils#transformers.HfArgumentParser) in Transformers with additional checks on the argument values to make sure that they will work well with AWS Trainium instances.
-- [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
+- [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
 
-The [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the TrainiumTrainer one.
+The [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the NeuronTrainer one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-neuron/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 ```diff
 from transformers import TrainingArguments
-+from optimum.neuron import TrainiumTrainer as Trainer
++from optimum.neuron import NeuronTrainer as Trainer
 
 training_args = TrainingArguments(
   # training arguments...
 )
 
 # A lot of code here
```

### Comparing `optimum-neuron-0.0.7/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.8/optimum/commands/export/neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.8/optimum/commands/export/neuronx.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/commands/neuron/base.py` & `optimum-neuron-0.0.8/optimum/commands/neuron/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Defines the root command line class for optimum-neuron."""
 
 from ...utils import logging
 from ..base import BaseOptimumCLICommand, CommandInfo
 from .cache import CustomCacheRepoCommand
+from .subcommands import ConsolidateCommand
 
 
 logger = logging.get_logger()
 logger.setLevel(logging.INFO)
 
 
 class NeuronCommand(BaseOptimumCLICommand):
     COMMAND = CommandInfo(name="neuron", help="Optimum Neuron CLI")
     SUBCOMMANDS = (
         CommandInfo(
             name="cache",
-            help="Manage the Trainium cache.",
+            help="Manage the Neuron cache.",
             subcommand_class=CustomCacheRepoCommand,
         ),
+        CommandInfo(
+            name="consolidate",
+            help="Consolidate checkpoints that were produced during a parallel training setting.",
+            subcommand_class=ConsolidateCommand,
+        ),
     )
```

### Comparing `optimum-neuron-0.0.7/optimum/commands/neuron/cache.py` & `optimum-neuron-0.0.8/optimum/commands/neuron/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines the command line related to dealing with the Trainium cache repo."""
+"""Defines the command line related to dealing with the Neuron cache repo."""
 
 from typing import TYPE_CHECKING
 
 from ...neuron.utils.cache_utils import (
     CACHE_REPO_NAME,
     HF_HOME_CACHE_REPO_FILE,
     create_custom_cache_repo,
@@ -51,26 +51,26 @@
             action="store_true",
             help="If set, the created repo will be public. By default the cache repo is private.",
         )
 
     def run(self):
         repo_url = create_custom_cache_repo(repo_id=self.args.name, private=not self.args.public)
         public_or_private = "public" if self.args.public else "private"
-        logger.info(f"Trainium cache created on the Hugging Face Hub: {repo_url.repo_id} [{public_or_private}].")
-        logger.info(f"Trainium cache name set locally to {repo_url.repo_id} in {HF_HOME_CACHE_REPO_FILE}.")
+        logger.info(f"Neuron cache created on the Hugging Face Hub: {repo_url.repo_id} [{public_or_private}].")
+        logger.info(f"Neuron cache name set locally to {repo_url.repo_id} in {HF_HOME_CACHE_REPO_FILE}.")
 
 
 class SetCustomCacheRepoCommand(BaseOptimumCLICommand):
     @staticmethod
     def parse_args(parser: "ArgumentParser"):
         parser.add_argument("name", type=str, help="The name of the repo to use as remote cache.")
 
     def run(self):
         set_custom_cache_repo_name_in_hf_home(self.args.name)
-        logger.info(f"Trainium cache name set locally to {self.args.name} in {HF_HOME_CACHE_REPO_FILE}.")
+        logger.info(f"Neuron cache name set locally to {self.args.name} in {HF_HOME_CACHE_REPO_FILE}.")
 
 
 class AddToCacheRepoCommand(BaseOptimumCLICommand):
     @staticmethod
     def parse_args(parser: "ArgumentParser"):
         parser.add_argument("-m", "--model", type=str, required=True, help="The name of model or path of the model.")
         parser.add_argument("--task", type=str, required=True, help="The task for which the model should be compiled.")
@@ -213,15 +213,15 @@
         CommandInfo(
             name="create",
             help="Create a model repo on the Hugging Face Hub to store Neuron X compilation files.",
             subcommand_class=CreateCustomCacheRepoCommand,
         ),
         CommandInfo(
             name="set",
-            help="Set the name of the Trainium cache repo to use locally.",
+            help="Set the name of the Neuron cache repo to use locally.",
             subcommand_class=SetCustomCacheRepoCommand,
         ),
         CommandInfo(
             name="add",
             help="Add a model to the cache of your choice.",
             subcommand_class=AddToCacheRepoCommand,
         ),
```

### Comparing `optimum-neuron-0.0.7/optimum/commands/register/register_export.py` & `optimum-neuron-0.0.8/optimum/commands/register/register_export.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.8/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.8/optimum/exporters/neuron/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,10 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .__main__ import main_export, normalize_input_shapes, normalize_stable_diffusion_input_shapes
 from .base import NeuronConfig
 from .convert import export, export_models, validate_model_outputs, validate_models_outputs
-from .utils import build_stable_diffusion_components_mandatory_shapes, get_stable_diffusion_models_for_export
+from .utils import (
+    DiffusersPretrainedConfig,
+    build_stable_diffusion_components_mandatory_shapes,
+    get_stable_diffusion_models_for_export,
+)
```

### Comparing `optimum-neuron-0.0.7/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.8/optimum/exporters/neuron/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Neuron configuration base classes."""
 
+import importlib
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import torch
 
 from ...exporters.base import ExportConfig
-from ...neuron.utils import is_neuron_available
+from ...neuron.utils import is_neuron_available, is_transformers_neuronx_available
 from ...utils import logging
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedModel
 
     from optimum.utils import DummyInputGenerator
@@ -72,14 +73,15 @@
         They are required or not depending on the model the `NeuronConfig` is designed for.
     """
 
     NORMALIZED_CONFIG_CLASS = None
     DUMMY_INPUT_GENERATOR_CLASSES = ()
     ATOL_FOR_VALIDATION: Union[float, Dict[str, float]] = 1e-5
     MANDATORY_AXES = ()
+    MODEL_TYPE = None
 
     _TASK_TO_COMMON_OUTPUTS = {
         "feature-extraction": ["last_hidden_state", "pooler_output"],
         "fill-mask": ["logits"],
         "image-classification": ["logits"],
         "image-segmentation": ["logits", "pred_boxes", "pred_masks"],
         "masked-im": ["logits"],
@@ -95,14 +97,16 @@
         "audio-xvector": ["logits"],
     }
 
     def __init__(
         self,
         config: "PretrainedConfig",
         task: str,
+        compiler_type: Optional[str] = None,
+        compiler_version: Optional[str] = None,
         batch_size: Optional[int] = None,
         dynamic_batch_size: bool = False,
         sequence_length: Optional[int] = None,
         num_choices: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         num_channels: Optional[int] = None,
@@ -139,14 +143,16 @@
         }
         input_shapes = {}
         for name, value in axes_values.items():
             if value is not None:
                 input_shapes[name] = value
             setattr(self, name, value)
         setattr(self, "input_shapes", input_shapes)
+        setattr(self, "compiler_type", compiler_type)
+        setattr(self, "compiler_version", compiler_version)
 
     @classmethod
     def get_mandatory_axes_for_task(cls, task: str) -> Tuple[str]:
         axes = []
         for axis in cls.MANDATORY_AXES:
             if isinstance(axis, tuple):
                 tasks, name = axis
@@ -302,7 +308,59 @@
                             "To extract outputs from a tuple, `eligible_outputs` must be a list of integers only."
                         )
                     outputs = [outputs[i] for i in eligible_outputs]
 
                 return outputs
 
         return ModelWrapper(model, list(dummy_inputs.keys()))
+
+
+class NeuronDecoderConfig(ExportConfig):
+    """
+    Base class for configuring the export of Neuron Decoder models
+
+    Class attributes:
+
+    - NEURONX_CLASS (`str`) -- the name of the transformers-neuronx class to instantiate for the model.
+    It is a full class name defined relatively to the transformers-neuronx module, e.g. `gpt2.model.GPT2ForSampling`
+    [`~optimum.utils.DummyInputGenerator`] specifying how to create dummy inputs.
+    - NEURONX_ARGS (`List[str]`) -- a list of optional arguments to be passed when instantiating the transformers-neuronx
+    model class.
+
+    The NEURONX_CLASS must always be defined in each model configuration.
+    The NEURONX_ARGS list is required only to identify specific parameters passed to the pre_trained method that must not be
+     passed to the transformers checkpoint model during export, but only to the transformers-neuronx model. By default it is empty.
+
+    Args:
+        task (`str`): The task the model should be exported for.
+    """
+
+    NEURONX_CLASS = None
+    NEURONX_ARGS = []
+
+    def __init__(self, task):
+        if not is_transformers_neuronx_available():
+            raise ModuleNotFoundError(
+                "The mandatory transformers-neuronx package is missing. Please install optimum[neuronx]."
+            )
+        module_name, class_name = self.NEURONX_CLASS.rsplit(".", maxsplit=1)
+        module = importlib.import_module(f"transformers_neuronx.{module_name}")
+        self._neuronx_class = getattr(module, class_name, None)
+        if self._neuronx_class is None:
+            raise ImportError(f"{class_name} not found in {module_name}. Please check transformers-neuronx version.")
+
+    def split_kwargs(self, **kwargs):
+        """Splits between kwargs that need to be passed when loading the transformers model during export
+        and those that need to be passed to the neuron optimizer.
+        """
+        model_kwargs = {}
+        neuron_kwargs = {}
+        for arg, value in kwargs.items():
+            if arg in self.NEURONX_ARGS:
+                neuron_kwargs[arg] = value
+            else:
+                model_kwargs[arg] = value
+        return model_kwargs, neuron_kwargs
+
+    @property
+    def neuronx_class(self):
+        return self._neuronx_class
```

### Comparing `optimum-neuron-0.0.7/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.8/optimum/exporters/neuron/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from ...utils import (
     DummyBboxInputGenerator,
     DummyTextInputGenerator,
     DummyVisionInputGenerator,
     logging,
 )
-from .base import NeuronConfig
+from .base import NeuronConfig, NeuronDecoderConfig
 
 
 logger = logging.get_logger(__name__)
 
 
 class TextEncoderNeuronConfig(NeuronConfig):
     """
@@ -49,7 +49,15 @@
 
 class TextAndVisionNeuronConfig(NeuronConfig):
     """
     Handles multi-modal text and vision architectures.
     """
 
     DUMMY_INPUT_GENERATOR_CLASSES = (DummyTextInputGenerator, DummyVisionInputGenerator, DummyBboxInputGenerator)
+
+
+class TextNeuronDecoderConfig(NeuronDecoderConfig):
+    """
+    Handles text decoder architectures.
+    """
+
+    pass
```

### Comparing `optimum-neuron-0.0.7/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.8/optimum/exporters/neuron/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 import numpy as np
 import torch
 from transformers import PretrainedConfig
 
 from ...exporters.error_utils import OutputMatchError, ShapeError
 from ...neuron.utils import (
     convert_neuronx_compiler_args_to_neuron,
-    get_attention_scores,
     is_neuron_available,
     is_neuronx_available,
     store_compilation_config,
 )
 from ...neuron.utils.version_utils import get_neuroncc_version, get_neuronxcc_version
 from ...utils import is_diffusers_available, logging
+from .utils import DiffusersPretrainedConfig
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel
 
     from .base import NeuronConfig
 
@@ -63,15 +63,15 @@
 def validate_models_outputs(
     models_and_neuron_configs: Dict[
         str, Tuple[Union["PreTrainedModel", "ModelMixin", torch.nn.Module], "NeuronConfig"]
     ],
     neuron_named_outputs: List[List[str]],
     output_dir: Path,
     atol: Optional[float] = None,
-    neuron_files_subpaths: Optional[List[str]] = None,
+    neuron_files_subpaths: Optional[Dict[str, str]] = None,
 ):
     """
     Validates the export of several models, by checking that the outputs from both the reference and the exported model match.
     The following method validates the Neuron models exported using the `export_models` method.
 
     Args:
         models_and_neuron_configs (`Dict[str, Tuple[Union[`PreTrainedModel`, `ModelMixin`, `torch.nn.Module`], `NeuronConfig`]]):
@@ -101,15 +101,15 @@
 
     exceptions = []  # run all validations before raising
     neuron_paths = []
     for i, model_name in enumerate(models_and_neuron_configs.keys()):
         submodel, sub_neuron_config = models_and_neuron_configs[model_name]
         ref_submodel = copy.deepcopy(submodel)
         neuron_model_path = (
-            output_dir.joinpath(neuron_files_subpaths[i])
+            output_dir.joinpath(neuron_files_subpaths[model_name])
             if neuron_files_subpaths is not None
             else output_dir.joinpath(model_name + ".neuron")
         )
         neuron_paths.append(neuron_model_path)
         try:
             validate_model_outputs(
                 config=sub_neuron_config,
@@ -157,16 +157,16 @@
     if atol is None:
         if isinstance(config.ATOL_FOR_VALIDATION, dict):
             atol = config.ATOL_FOR_VALIDATION[config.task]
         else:
             atol = config.ATOL_FOR_VALIDATION
 
     input_shapes = {}
-    for axe in config.mandatory_axes:
-        input_shapes[axe] = getattr(config, axe)
+    for axis in config.mandatory_axes:
+        input_shapes[axis] = getattr(config, axis)
     if config.dynamic_batch_size is True:
         input_shapes["batch_size"] *= 2
 
     # Reference outputs
     with torch.no_grad():
         reference_model.eval()
         ref_inputs = config.generate_dummy_inputs(return_tuple=False, **input_shapes)
@@ -252,15 +252,15 @@
 
 
 def export_models(
     models_and_neuron_configs: Dict[
         str, Tuple[Union["PreTrainedModel", "ModelMixin", torch.nn.Module], "NeuronConfig"]
     ],
     output_dir: Path,
-    output_file_names: Optional[List[str]] = None,
+    output_file_names: Optional[Dict[str, str]] = None,
     compiler_kwargs: Optional[Dict[str, Any]] = {},
     configs: Optional[Dict[str, Any]] = {},
 ) -> Tuple[List[List[str]], List[List[str]]]:
     """
     Exports a Pytorch model with multiple component models to separate files.
 
     Args:
@@ -285,15 +285,17 @@
         raise ValueError(
             f"Provided {len(output_file_names)} custom names for the export of {len(models_and_neuron_configs)} models. Please provide the same number of names as models to export."
         )
 
     failed_models = []
     for i, model_name in enumerate(models_and_neuron_configs.keys()):
         submodel, sub_neuron_config = models_and_neuron_configs[model_name]
-        output_file_name = output_file_names[i] if output_file_names is not None else Path(model_name + ".neuron")
+        output_file_name = (
+            output_file_names[model_name] if output_file_names is not None else Path(model_name + ".neuron")
+        )
 
         output_path = output_dir / output_file_name
         output_path.parent.mkdir(parents=True, exist_ok=True)
 
         try:
             neuron_inputs, neuron_outputs = export(
                 model=submodel,
@@ -308,26 +310,29 @@
             elif configs and (model_name in configs.keys()):
                 model_config = configs[model_name]
             else:
                 raise AttributeError("Cannot find model's configuration, please pass it with `configs`.")
 
             if is_diffusers_available() and isinstance(model_config, FrozenDict):
                 model_config = OrderedDict(model_config)
-                model_config = PretrainedConfig.from_dict(model_config)
+                model_config = DiffusersPretrainedConfig.from_dict(model_config)
 
             store_compilation_config(
                 config=model_config,
                 input_shapes=sub_neuron_config.input_shapes,
                 compiler_kwargs=compiler_kwargs,
                 input_names=neuron_inputs,
                 output_names=neuron_outputs,
                 dynamic_batch_size=sub_neuron_config.dynamic_batch_size,
-                neuron_compiler=NEURON_COMPILER_TYPE,
-                neuron_compiler_version=NEURON_COMPILER_VERSION,
+                compiler_type=NEURON_COMPILER_TYPE,
+                compiler_version=NEURON_COMPILER_VERSION,
+                model_type=getattr(sub_neuron_config, "MODEL_TYPE", None),
             )
+            if isinstance(model_config, PretrainedConfig):
+                model_config = DiffusersPretrainedConfig.from_dict(model_config.__dict__)
             model_config.save_pretrained(output_path.parent)
         except Exception as e:
             failed_models.append((i, model_name))
             output_path.parent.rmdir()
             logger.error(
                 f"An error occured when trying to trace {model_name} with the error message: {e}.\n"
                 f"The export is failed and {model_name} neuron model won't be stored."
@@ -398,16 +403,16 @@
     if config.values_override is not None:
         logger.info(f"Overriding {len(config.values_override)} configuration item(s)")
         for override_config_key, override_config_value in config.values_override.items():
             logger.info(f"\t- {override_config_key} -> {override_config_value}")
             setattr(model.config, override_config_key, override_config_value)
 
     input_shapes = {}
-    for axe in config.mandatory_axes:
-        input_shapes[axe] = getattr(config, axe)
+    for axis in config.mandatory_axes:
+        input_shapes[axis] = getattr(config, axis)
 
     dummy_inputs = config.generate_dummy_inputs(**input_shapes)
     dummy_inputs_tuple = tuple(dummy_inputs.values())
     checked_model = config.check_model_inputs_order(model, dummy_inputs)
 
     if auto_cast is not None:
         logger.info(f"Using Neuron: --auto-cast {auto_cast}")
@@ -418,18 +423,15 @@
         logger.info(f"Using Neuron: --auto-cast-type {auto_cast_type}")
         compiler_args.extend(["--auto-cast-type", auto_cast_type])
     else:
         compiler_args = ["--auto-cast", "none"]
 
     # diffusers specific
     if hasattr(config._config, "_class_name") and "unet" in config._config._class_name.lower():
-        from diffusers.models.attention_processor import Attention
-
         compiler_args.extend(["--model-type", "unet-inference"])
-        Attention.get_attention_scores = get_attention_scores
 
     neuron_model = neuronx.trace(checked_model, dummy_inputs_tuple, compiler_args=compiler_args)
 
     if config.dynamic_batch_size is True:
         neuron_model = neuronx.dynamic_batch(neuron_model)
 
     torch.jit.save(neuron_model, output)
@@ -481,16 +483,16 @@
     if config.values_override is not None:
         logger.info(f"Overriding {len(config.values_override)} configuration item(s)")
         for override_config_key, override_config_value in config.values_override.items():
             logger.info(f"\t- {override_config_key} -> {override_config_value}")
             setattr(model.config, override_config_key, override_config_value)
 
     input_shapes = {}
-    for axe in config.mandatory_axes:
-        input_shapes[axe] = getattr(config, axe)
+    for axis in config.mandatory_axes:
+        input_shapes[axis] = getattr(config, axis)
 
     dummy_inputs = config.generate_dummy_inputs(**input_shapes)
     dummy_inputs_tuple = tuple(dummy_inputs.values())
     checked_model = config.check_model_inputs_order(model, dummy_inputs)
     compiler_args = convert_neuronx_compiler_args_to_neuron(auto_cast, auto_cast_type, disable_fast_relayout)
 
     neuron_model = neuron.trace(
```

### Comparing `optimum-neuron-0.0.7/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.8/optimum/exporters/neuron/model_configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     NormalizedTextAndVisionConfig,
     is_diffusers_available,
 )
 from ..tasks import TasksManager
 from .config import (
     TextAndVisionNeuronConfig,
     TextEncoderNeuronConfig,
+    TextNeuronDecoderConfig,
     VisionNeuronConfig,
 )
 
 
 if TYPE_CHECKING:
     if is_diffusers_available():
         from diffusers.models.vae import Decoder as VaeDecoder
@@ -175,92 +176,136 @@
 
     @property
     def outputs(self) -> List[str]:
         return ["logits_per_image", "logits_per_text", "text_embeds", "image_embeds"]
 
 
 @register_in_tasks_manager("clip-text-model", *["feature-extraction"])
-class CLIPTextNeuronConfig(TextEncoderNeuronConfig):
+class CLIPTextWithProjectionNeuronConfig(TextEncoderNeuronConfig):
     ATOL_FOR_VALIDATION = 1e-3
 
     NORMALIZED_CONFIG_CLASS = NormalizedConfig.with_args(
         vocab_size="vocab_size",
         sequence_length="max_position_embeddings",
+        num_layers="num_hidden_layers",
         allow_new=True,
     )
 
     @property
     def inputs(self) -> List[str]:
         return ["input_ids"]
 
     @property
     def outputs(self) -> List[str]:
-        return ["last_hidden_state"]
+        common_outputs = ["text_embeds", "last_hidden_state"]
+
+        if self._normalized_config.output_hidden_states:
+            for i in range(self._normalized_config.num_layers + 1):
+                common_outputs.append(f"hidden_states.{i}")
+
+        return common_outputs
+
+
+@register_in_tasks_manager("clip-text-model", *["stable-diffusion", "feature-extraction"])
+class CLIPTextNeuronConfig(CLIPTextWithProjectionNeuronConfig):
+    MODEL_TYPE = "clip-text-model"
+
+    @property
+    def outputs(self) -> List[str]:
+        common_outputs = ["last_hidden_state", "pooler_output"]
+
+        if self._normalized_config.output_hidden_states:
+            for i in range(self._normalized_config.num_layers + 1):
+                common_outputs.append(f"hidden_states.{i}")
+
+        return common_outputs
 
     def generate_dummy_inputs(self, return_tuple: bool = False, **kwargs):
         dummy_inputs = super().generate_dummy_inputs(**kwargs)
-        dummy_inputs["input_ids"] = dummy_inputs["input_ids"].to(dtype=torch.int32)
+        dummy_inputs["input_ids"] = dummy_inputs["input_ids"]
 
         if return_tuple is True:
             return tuple(dummy_inputs.values())
         else:
             return dummy_inputs
 
     def check_model_inputs_order(self, model, dummy_inputs, forward_with_tuple=False):
         return super().check_model_inputs_order(model, dummy_inputs, forward_with_tuple, eligible_outputs=[0])
 
 
-@register_in_tasks_manager("vae-encoder", *["semantic-segmentation"])
-class VaeEncoderNeuronConfig(VisionNeuronConfig):
-    ATOL_FOR_VALIDATION = 1e-2
+@register_in_tasks_manager("unet", *["stable-diffusion", "semantic-segmentation"])
+class UNetNeuronConfig(VisionNeuronConfig):
+    ATOL_FOR_VALIDATION = 1e-3
+    MANDATORY_AXES = ("batch_size", "sequence_length", "num_channels", "width", "height")
+    MODEL_TYPE = "unet"
 
     NORMALIZED_CONFIG_CLASS = NormalizedConfig.with_args(
-        num_channels="in_channels",
         image_size="sample_size",
+        num_channels="in_channels",
+        hidden_size="cross_attention_dim",
+        vocab_size="norm_num_groups",
         allow_new=True,
     )
 
+    DUMMY_INPUT_GENERATOR_CLASSES = (
+        DummyVisionInputGenerator,
+        DummyTimestepInputGenerator,
+        DummySeq2SeqDecoderTextInputGenerator,
+    )
+
     @property
     def inputs(self) -> List[str]:
-        return ["sample"]
+        common_inputs = ["sample", "timestep", "encoder_hidden_states"]
+
+        # TODO : add text_image, image and image_embeds
+        if getattr(self._normalized_config, "addition_embed_type", None) == "text_time":
+            common_inputs.append("text_embeds")
+            common_inputs.append("time_ids")
+
+        return common_inputs
 
     @property
     def outputs(self) -> List[str]:
-        return ["latent_sample"]
+        return ["sample"]
 
+    def generate_dummy_inputs(self, return_tuple: bool = False, **kwargs):
+        dummy_inputs = super().generate_dummy_inputs(**kwargs)
+        dummy_inputs["timestep"] = dummy_inputs["timestep"].float()
+        dummy_inputs["encoder_hidden_states"] = dummy_inputs["encoder_hidden_states"][0]
 
-@register_in_tasks_manager("vae-decoder", *["semantic-segmentation"])
-class VaeDecoderNeuronConfig(VisionNeuronConfig):
-    ATOL_FOR_VALIDATION = 1e-3
+        if return_tuple is True:
+            return tuple(dummy_inputs.values())
+        else:
+            return dummy_inputs
+
+
+@register_in_tasks_manager("vae-encoder", *["stable-diffusion", "semantic-segmentation"])
+class VaeEncoderNeuronConfig(VisionNeuronConfig):
+    ATOL_FOR_VALIDATION = 1e-2
+    MODEL_TYPE = "vae-encoder"
 
     NORMALIZED_CONFIG_CLASS = NormalizedConfig.with_args(
-        num_channels="latent_channels",
+        num_channels="in_channels",
+        image_size="sample_size",
         allow_new=True,
     )
 
     @property
     def inputs(self) -> List[str]:
-        return ["latent_sample"]
+        return ["sample"]
 
     @property
     def outputs(self) -> List[str]:
-        return ["sample"]
-
-    def check_model_inputs_order(
-        self,
-        model: "VaeDecoder",
-        dummy_inputs: Dict[str, torch.Tensor],
-        **kwargs,
-    ):
-        return super().check_model_inputs_order(model=model, dummy_inputs=dummy_inputs, forward_with_tuple=True)
+        return ["latent_sample"]
 
 
-@register_in_tasks_manager("conv2d", *["semantic-segmentation"])
-class Conv2dNeuronConfig(VisionNeuronConfig):
+@register_in_tasks_manager("vae-decoder", *["stable-diffusion", "semantic-segmentation"])
+class VaeDecoderNeuronConfig(VisionNeuronConfig):
     ATOL_FOR_VALIDATION = 1e-3
+    MODEL_TYPE = "vae-decoder"
 
     NORMALIZED_CONFIG_CLASS = NormalizedConfig.with_args(
         num_channels="latent_channels",
         allow_new=True,
     )
 
     @property
@@ -269,49 +314,18 @@
 
     @property
     def outputs(self) -> List[str]:
         return ["sample"]
 
     def check_model_inputs_order(
         self,
-        model: torch.nn.Module,
+        model: "VaeDecoder",
         dummy_inputs: Dict[str, torch.Tensor],
         **kwargs,
     ):
         return super().check_model_inputs_order(model=model, dummy_inputs=dummy_inputs, forward_with_tuple=True)
 
 
-@register_in_tasks_manager("unet", *["semantic-segmentation"])
-class UNetNeuronConfig(VisionNeuronConfig):
-    ATOL_FOR_VALIDATION = 1e-3
-
-    NORMALIZED_CONFIG_CLASS = NormalizedConfig.with_args(
-        image_size="sample_size",
-        num_channels="in_channels",
-        hidden_size="cross_attention_dim",
-        vocab_size="norm_num_groups",
-        allow_new=True,
-    )
-
-    DUMMY_INPUT_GENERATOR_CLASSES = (
-        DummyVisionInputGenerator,
-        DummyTimestepInputGenerator,
-        DummySeq2SeqDecoderTextInputGenerator,
-    )
-
-    @property
-    def inputs(self) -> List[str]:
-        return ["sample", "timestep", "encoder_hidden_states"]
-
-    @property
-    def outputs(self) -> List[str]:
-        return ["sample"]
-
-    def generate_dummy_inputs(self, return_tuple: bool = False, **kwargs):
-        dummy_inputs = super().generate_dummy_inputs(**kwargs)
-        dummy_inputs["timestep"] = dummy_inputs["timestep"].float()
-        dummy_inputs["encoder_hidden_states"] = dummy_inputs["encoder_hidden_states"][0]
-
-        if return_tuple is True:
-            return tuple(dummy_inputs.values())
-        else:
-            return dummy_inputs
+@register_in_tasks_manager("gpt2", "text-generation")
+class GPT2NeuronConfig(TextNeuronDecoderConfig):
+    NEURONX_ARGS = ["n_positions"]
+    NEURONX_CLASS = "gpt2.model.GPT2ForSampling"
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,49 +15,64 @@
 
 from typing import TYPE_CHECKING
 
 from transformers.utils import _LazyModule
 
 
 _import_structure = {
-    "hf_argparser": ["TrainiumHfArgumentParser"],
-    "trainers": ["TrainiumTrainer", "Seq2SeqTrainiumTrainer"],
-    "training_args": ["TrainiumTrainingArguments", "Seq2SeqTrainiumTrainingArguments"],
+    "hf_argparser": ["NeuronHfArgumentParser"],
+    "trainers": ["NeuronTrainer", "Seq2SeqNeuronTrainer"],
+    "training_args": ["NeuronTrainingArguments", "Seq2SeqNeuronTrainingArguments"],
     "modeling_base": ["NeuronBaseModel"],
     "modeling": [
         "NeuronModelForFeatureExtraction",
         "NeuronModelForMaskedLM",
         "NeuronModelForQuestionAnswering",
         "NeuronModelForSequenceClassification",
         "NeuronModelForTokenClassification",
         "NeuronModelForMultipleChoice",
+        "NeuronModelForCausalLM",
     ],
+    "modeling_diffusion": [
+        "NeuronStableDiffusionPipeline",
+        "NeuronStableDiffusionImg2ImgPipeline",
+        "NeuronStableDiffusionInpaintPipeline",
+    ],
+    "modeling_decoder": ["NeuronDecoderModel"],
     "accelerate": [
         "NeuronAccelerator",
         "NeuronAcceleratorState",
         "NeuronPartialState",
     ],
     "pipelines": ["pipeline"],
 }
 
 if TYPE_CHECKING:
     from .accelerate import NeuronAccelerator, NeuronAcceleratorState, NeuronPartialState
-    from .hf_argparser import TrainiumHfArgumentParser
+    from .hf_argparser import NeuronHfArgumentParser
     from .modeling import (
+        NeuronModelForCausalLM,
         NeuronModelForFeatureExtraction,
         NeuronModelForMaskedLM,
         NeuronModelForMultipleChoice,
         NeuronModelForQuestionAnswering,
         NeuronModelForSequenceClassification,
         NeuronModelForTokenClassification,
     )
     from .modeling_base import NeuronBaseModel
+    from .modeling_decoder import NeuronDecoderModel
+    from .modeling_diffusion import (
+        NeuronStableDiffusionImg2ImgPipeline,
+        NeuronStableDiffusionInpaintPipeline,
+        NeuronStableDiffusionPipeline,
+    )
     from .pipelines import pipeline
-    from .trainers import Seq2SeqTrainiumTrainer, TrainiumTrainer
-    from .training_args import Seq2SeqTrainiumTrainingArguments, TrainiumTrainingArguments
+    from .trainers import NeuronTrainer, Seq2SeqNeuronTrainer
+    from .training_args import NeuronTrainingArguments, Seq2SeqNeuronTrainingArguments
+
 else:
     import sys
 
     sys.modules[__name__] = _LazyModule(
         __name__,
         globals()["__file__"],
         _import_structure,
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/accelerator.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/accelerator.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Custom Accelerator class for Neuron."""
 
+import collections
 import inspect
 import os
 import re
 import shutil
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import torch
 from accelerate import Accelerator
 from accelerate.checkpointing import save_accelerator_state, save_custom_state
 from accelerate.utils import DistributedType
+from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
 from ...utils import logging
-from ..distributed import ParallelizersManager
+from ..distributed import Parallelizer, ParallelizersManager
+from ..distributed.utils import ZeroRedundancyOptimizerCompatibleWithTensorParallelism
 from ..utils import Patcher, is_neuronx_distributed_available, is_torch_xla_available, patch_within_function
 from ..utils.misc import args_and_kwargs_to_kwargs_only
 from .optimizer import NeuronAcceleratedOptimizer
 from .scheduler import NeuronAcceleratedScheduler
 from .state import NeuronAcceleratorState
 from .utils import (
     NeuronDistributedType,
@@ -62,15 +65,15 @@
 
 logger = logging.get_logger(__name__)
 
 
 # TODO: should we do a XLAFSDPNeuronAccelerator instead?
 class NeuronAccelerator(Accelerator):
     # @patch_within_function(("accelerate.accelerator.AcceleratorState", NeuronAcceleratorState))
-    def __init__(self, *args, tp_plugin: Optional[TensorParallelismPlugin] = None, **kwargs):
+    def __init__(self, *args, tp_plugin: Optional[TensorParallelismPlugin] = None, zero_1: bool = False, **kwargs):
         # Patches accelerate.utils.imports.is_tpu_available to match `is_torch_xla_available`
         patch_accelerate_is_tpu_available()
 
         full_kwargs = args_and_kwargs_to_kwargs_only(
             super().__init__, args=args, kwargs=kwargs, include_default_values=True
         )
 
@@ -86,16 +89,23 @@
         elif gradient_accumulation_steps != 1:
             num_steps = gradient_accumulation_steps
             gradient_accumulation_steps = 1
         full_kwargs["gradient_accumulation_plugin"] = gradient_accumulation_plugin
         full_kwargs["gradient_accumulation_steps"] = gradient_accumulation_steps
 
         fsdp_plugin = full_kwargs["fsdp_plugin"]
-        if fsdp_plugin is None and os.environ.get("ACCELERATE_USE_FSDP", "false") == "true":
-            fsdp_plugin = NeuronFullyShardedDataParallelPlugin()
+        if fsdp_plugin is None:
+            if os.environ.get("ACCELERATE_USE_FSDP", "false") == "true":
+                fsdp_plugin = NeuronFullyShardedDataParallelPlugin()
+        elif not isinstance(fsdp_plugin, NeuronFullyShardedDataParallelPlugin):
+            raise ValueError(
+                "The fsdp_plugin must be an instance of NeuronFullyShardedDataParallelPlugin to use XLA FSDP with "
+                f"the NeuronAccelerator, but an instance of {type(fsdp_plugin)} was given here."
+            )
+        self.fsdp_plugin = fsdp_plugin
 
         use_neuronx_distributed_tp = os.environ.get("ACCELERATE_USE_NEURONX_DISTRIBUTED_TP", "false")
         if tp_plugin is None:
             if use_neuronx_distributed_tp == "false":
                 tp_size = 1
             else:
                 tp_size = int(use_neuronx_distributed_tp)
@@ -105,53 +115,113 @@
         if tp_plugin.should_parallelize:
             os.environ["ACCELERATE_USE_NEURONX_DISTRIBUTED_TP"] = "true"
 
         patched_accelerator_state = partial(NeuronAcceleratorState, tp_plugin=tp_plugin)
         with Patcher([("accelerate.accelerator.AcceleratorState", patched_accelerator_state)]):
             super().__init__(**full_kwargs)
 
+        self.zero_1 = zero_1
+
+        if self.fsdp_plugin is not None and self.zero_1:
+            raise ValueError("Either enable XLA ZeRO Stage 1 or XLA FSDP but not both.")
+
+        if self.process_index == -1 and self.zero_1:
+            raise ValueError("XLA ZeRO Stage 1 can only be enabled in a distributed training setting.")
+
         if fsdp_plugin is not None and tp_plugin is not None:
             raise ValueError("It is not possible to both use neuronx_distributed Tensor Parallelism and XLA FSDP.")
 
         if num_steps != 1:
             self.gradient_accumulation_steps = num_steps
 
-    def _prepare_data_loader_for_tp(self, data_loader: torch.utils.data.DataLoader):
+    def _prepare_data_loader_for_tp(self, data_loader: DataLoader) -> DataLoader:
+        # TODO: make it more robust, similar to the prepare_data_loader function in `accelerate`.
+        if isinstance(data_loader.sampler, DistributedSampler):
+            return data_loader
         sampler = DistributedSampler(
             data_loader.dataset,
-            num_replicas=parallel_layers.parallel_state.get_data_parallel_world_size(),
+            num_replicas=parallel_layers.parallel_state.get_data_parallel_size(),
             rank=parallel_layers.parallel_state.get_data_parallel_rank(),
         )
-        data_loader.sampler = sampler
-        return data_loader
+        data_loader_for_tp = DataLoader(
+            data_loader.dataset,
+            batch_size=data_loader.batch_size,
+            sampler=sampler,
+            num_workers=data_loader.num_workers,
+            collate_fn=data_loader.collate_fn,
+            pin_memory=data_loader.pin_memory,
+            drop_last=data_loader.drop_last,
+        )
+        data_loader_for_tp._is_accelerate_prepared = True
+        return data_loader_for_tp
 
-    def prepare_data_loader(self, data_loader: torch.utils.data.DataLoader, device_placement: Optional[bool] = None):
-        if self.tensor_parallel_size > 1:
+    def prepare_data_loader(self, data_loader: DataLoader, device_placement: Optional[bool] = None):
+        if self.state.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
             data_loader = self._prepare_data_loader_for_tp(data_loader)
+        else:
+            # TODO: fix that.
+            return data_loader
         return super().prepare_data_loader(data_loader, device_placement=device_placement)
 
     def _prepare_optimizer_for_tp(self, optimizer: torch.optim.Optimizer, device_placement=None):
-        new_groups = []
-        for param_group in optimizer.param_groups:
-            new_params = []
-            params = param_group["params"]
-            for idx in range(len(params)):
-                for cpu_to_xla in self._model_cpu_parameters_to_xla.values():
-                    new_params.append(cpu_to_xla[id(params[idx])])
-            new_group = {k: v for k, v in param_group.items() if k != "params"}
-            new_group["params"] = new_params
-            new_groups.append(new_group)
+        cpu_parameters_to_xla = collections.ChainMap(*self._model_cpu_parameters_to_xla.values())
+        if not self.zero_1:
+            optimizer = Parallelizer.optimizer_for_tp(optimizer, cpu_parameters_to_xla)
+        else:
+            xla_parameters, _ = Parallelizer.optimizer_cpu_params_to_xla_params(optimizer, cpu_parameters_to_xla)
+            if hasattr(optimizer, "_args_to_recreate"):
+                args, kwargs = optimizer._args_to_recreate
+                args = (xla_parameters,) + args[1:]
+                optimizer._args_to_recreate = (args, kwargs)
+            else:
+                optimizer.param_groups = xla_parameters
+        return optimizer
 
-        new_optimizer = optimizer.__class__(new_groups)
-        return super().prepare_optimizer(new_optimizer, device_placement=device_placement)
+    def _prepare_optimizer_for_zero_1(self, optimizer: torch.optim.Optimizer, device_placement=None):
+        mixed_precision_to_dtype = {
+            "no": torch.float32,
+            "bf16": torch.bfloat16,
+        }
+        optimizer_dtype = mixed_precision_to_dtype.get(self.state.mixed_precision, None)
+        if optimizer_dtype is None:
+            raise ValueError(f"The precision {self.state.mixed_precision} is not supported for ZeRO Stage 1")
+
+        if hasattr(optimizer, "_args_to_recreate"):
+            args, kwargs = optimizer._args_to_recreate
+            params = args[0]
+            defaults = args_and_kwargs_to_kwargs_only(optimizer.__class__, args[1:], kwargs)
+
+            zero_1_optimizer = ZeroRedundancyOptimizerCompatibleWithTensorParallelism(
+                params,
+                optimizer.__class__,
+                optimizer_dtype=optimizer_dtype,
+                pin_layout=False,
+                **defaults,
+            )
+            del optimizer
+        else:
+            logger.warning(
+                f"Creating a ZeroRedundancyOptimizer from {optimizer}, this might change some default values. When "
+                "using ZeRO 1 it is recommended to create the ZeroRedundancyOptimizer yourself to avoid this kind of "
+                "issues."
+            )
+            zero_1_optimizer = ZeroRedundancyOptimizerCompatibleWithTensorParallelism(
+                optimizer.param_groups,
+                optimizer.__class__,
+                optimizer_dtype=optimizer_dtype,
+                pin_layout=False,
+            )
+        return zero_1_optimizer
 
     @patch_within_function(("accelerate.accelerator.AcceleratedOptimizer", NeuronAcceleratedOptimizer))
     def prepare_optimizer(self, optimizer: torch.optim.Optimizer, device_placement: Optional[bool] = None):
         if self.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
-            return self._prepare_optimizer_for_tp(optimizer, device_placement=device_placement)
+            optimizer = self._prepare_optimizer_for_tp(optimizer, device_placement=device_placement)
+        if self.zero_1:
+            optimizer = self._prepare_optimizer_for_zero_1(optimizer, device_placement=device_placement)
         return super().prepare_optimizer(optimizer, device_placement=device_placement)
 
     @patch_within_function(("accelerate.accelerator.AcceleratedScheduler", NeuronAcceleratedScheduler))
     def prepare_scheduler(self, scheduler: "LRScheduler"):
         return super().prepare_scheduler(scheduler)
 
     def prepare_model_for_xla_fsdp(
@@ -225,18 +295,23 @@
         return model
 
     def _prepare_model_for_tp(
         self, model: torch.nn.Module, device_placement: Optional[bool] = None, evaluation_mode: bool = False
     ):
         if not evaluation_mode:
             cpu_ids = [id(v) for v in model.parameters()]
-            model, orig_to_parallel = self.state.tp_plugin.parallelize_model(model, return_orig_to_parallel=True)
+            # TODO: enable self.device (if needed).
+            model = self.state.tp_plugin.parallelize_model(model, return_orig_to_parallel=False, device=None)
+            if os.environ.get("XLA_USE_BF16", "0") == "1":
+                model.to(torch.bfloat16)
+            else:
+                model.to(torch.float32)
             parallel_layers.move_model_to_device(model, self.device)
-            self._model_cpu_parameters_to_xla[id(model)] = dict(zip(cpu_ids, model.parameters()))
             model.tie_weights()
+            self._model_cpu_parameters_to_xla[id(model)] = dict(zip(cpu_ids, model.parameters()))
             device_placement = False
         return super().prepare_model(model, device_placement=device_placement, evaluation_mode=evaluation_mode)
 
     def prepare_model(
         self, model: torch.nn.Module, device_placement: Optional[bool] = None, evaluation_mode: bool = False
     ):
         if self.distributed_type is NeuronDistributedType.XLA_FSDP:
@@ -254,43 +329,43 @@
             self.scaler.scale(loss).backward(**kwargs)
         else:
             loss.backward(**kwargs)
 
     def backward(self, loss, **kwargs):
         if self.distributed_type != DistributedType.DEEPSPEED:
             loss = loss / self.gradient_accumulation_steps
-        if self.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
-            loss = loss / parallel_layers.parallel_state.get_data_parallel_size()
         if self.distributed_type is NeuronDistributedType.XLA_FSDP:
             self.backward_for_xla_fsdp(loss, **kwargs)
         elif self.scaler is not None:
             self.scaler.scale(loss).backward(**kwargs)
         else:
-            # Providing **kwargs causes "Unsupported XLA type 10"
             loss.backward(**kwargs)
 
     def clip_grad_norm_for_xla_fsdp(self, parameters, max_norm, norm_type: int = 2):
         self.unscale_gradients()
         parameters = list(parameters)
         for model in self._models:
             if parameters == list(model.parameters()):
                 return model.clip_grad_norm_(max_norm, norm_type)
 
-    def _clip_grad_norm_for_tp(self, parameters, max_norm, norm_type: int = 2):
+    def _prepare_clip_grad_norm(self, parameters, max_norm, norm_type: int = 2):
         self.unscale_gradients()
         parameters = list(parameters)
         for model in self._models:
             if parameters == list(model.parameters()):
-                return parallel_layers.clip_grad_norm(parameters, max_norm, norm_type=norm_type)
+                for opt in self._optimizers:
+                    # Under this setting, the gradient clipping will be deferred to the optimizer step.
+                    # It will happen after the gradients have been reduced and before the optimizer step.
+                    return opt.prepare_clip_grad_norm(parameters, max_norm, norm_type=norm_type)
 
     def clip_grad_norm_(self, parameters, max_norm, norm_type=2):
         if self.distributed_type is NeuronDistributedType.XLA_FSDP:
             return self.clip_grad_norm_for_xla_fsdp(parameters, max_norm, norm_type=norm_type)
-        elif self.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
-            return self._clip_grad_norm_for_tp(parameters, max_norm, norm_type=norm_type)
+        elif self.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM or self.zero_1:
+            return self._prepare_clip_grad_norm(parameters, max_norm, norm_type=norm_type)
         return super().clip_grad_norm_(parameters, max_norm, norm_type=norm_type)
 
     def clip_grad_value_(self, parameters, clip_value):
         if self.distributed_type is NeuronDistributedType.XLA_FSDP:
             raise Exception("XLA FSDP  does not support `clip_grad_value_`. Use `clip_grad_norm_` instead.")
         return super().clip_grad_value_(parameters, clip_value)
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/scheduler.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/scheduler.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/state.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/state.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/dataclasses.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Custom dataclasses for Neuron."""
 
 import enum
 import os
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Dict, Tuple, Union
+from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union
 
 import torch
 from accelerate.utils.constants import MODEL_NAME, OPTIMIZER_NAME
 from accelerate.utils.dataclasses import FullyShardedDataParallelPlugin
 
 from ...distributed import ParallelizersManager
 from ...utils import is_torch_xla_available
@@ -139,28 +139,31 @@
 
 
 @dataclass
 class TensorParallelismPlugin:
     tensor_parallel_size: int = 1
 
     def __post_init__(self):
-        if self.tensor_parallel_size > 1:
-            raise NotImplementedError("Tensor Parallelism is not supported yet.")
         if self.tensor_parallel_size < 1:
             raise ValueError(f"The tensor parallel size must be >= 1, but {self.tensor_parallel_size} was given here.")
 
     @property
     def should_parallelize(self):
         return self.tensor_parallel_size > 1
 
     def parallelize_model(
-        self, model: "PreTrainedModel", return_orig_to_parallel: bool = False
+        self,
+        model: "PreTrainedModel",
+        return_orig_to_parallel: bool = False,
+        device: Optional["torch.device"] = None,
     ) -> Union["PreTrainedModel", Tuple["PreTrainedModel", Dict[int, "torch.nn.Parameter"]]]:
-        orig_to_parallel = {}
+        orig_to_parallel = {} if return_orig_to_parallel else None
         parallelizer = ParallelizersManager.parallelizer_for_model(model)
         parallelized_model = parallelizer.parallelize(
-            model, orig_to_parallel=orig_to_parallel if return_orig_to_parallel else None
+            model,
+            orig_to_parallel=orig_to_parallel,
+            device=device,
         )
         if return_orig_to_parallel:
             return parallelized_model, orig_to_parallel
         else:
             return parallelized_model
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/misc.py` & `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/distributed/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # coding=utf-8
-# Copyright 2023 The HuggingFace Inc. team. All rights reserved.
+# Copyright 2023 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .base import Parallelizer
-from .parallelizers_manager import ParallelizersManager
+from .base import (
+    pipeline,
+)
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/distributed/encoder_models.py` & `optimum-neuron-0.0.8/optimum/neuron/distributed/encoder_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 """Classes related to `neuronx-distributed` to perform parallelism."""
 
 from typing import TYPE_CHECKING, Dict, Optional
 
 from .base import Parallelizer
 from .parallel_layers import ParallelSelfAttention, ParallelSelfOutput
-from .utils import embedding_to_parallel_embedding
 
 
 if TYPE_CHECKING:
     import torch
     from transformers import PreTrainedModel
 
 
@@ -32,42 +31,59 @@
 
 class BertParallelSelfOutput(ParallelSelfOutput):
     pass
 
 
 class BertParallelizer(Parallelizer):
     @classmethod
-    def parallelize(
-        cls, model: "PreTrainedModel", orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]] = None
+    def _parallelize(
+        cls,
+        model: "PreTrainedModel",
+        orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]],
+        device: Optional["torch.device"] = None,
     ) -> "PreTrainedModel":
-        model.bert.embeddings.word_embeddings = embedding_to_parallel_embedding(model.bert.embeddings.word_embeddings)
         for layer in model.bert.encoder.layer:
             layer.attention.self = BertParallelSelfAttention.transform(
-                layer.attention.self, model.config, orig_to_parallel=orig_to_parallel
+                model,
+                layer.attention.self,
+                orig_to_parallel=orig_to_parallel,
+                device=device,
             )
             layer.attention.output = BertParallelSelfOutput.transform(
-                layer.attention.output, model.config, orig_to_parallel=orig_to_parallel
+                model,
+                layer.attention.output,
+                orig_to_parallel=orig_to_parallel,
+                device=device,
             )
         return model
 
 
 class RobertaParallelSelfAttention(BertParallelSelfAttention):
     pass
 
 
 class RobertaParallelSelfOutput(BertParallelSelfOutput):
     pass
 
 
 class RobertaParallelizer(Parallelizer):
     @classmethod
-    def parallelize(
-        cls, model: "PreTrainedModel", orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]] = None
+    def _parallelize(
+        cls,
+        model: "PreTrainedModel",
+        orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]],
+        device: Optional["torch.device"] = None,
     ) -> "PreTrainedModel":
         for layer in model.roberta.encoder.layer:
             layer.attention.self = RobertaParallelSelfAttention.transform(
-                layer.attention.self, model.config, orig_to_parallel=orig_to_parallel
+                model,
+                layer.attention.self,
+                orig_to_parallel=orig_to_parallel,
+                device=device,
             )
             layer.attention.output = RobertaParallelSelfOutput.transform(
-                layer.attention.output, model.config, orig_to_parallel=orig_to_parallel
+                model,
+                layer.attention.output,
+                orig_to_parallel=orig_to_parallel,
+                device=device,
             )
         return model
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/distributed/parallelizers_manager.py` & `optimum-neuron-0.0.8/optimum/neuron/distributed/parallelizers_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Factory class mapping model architectures to their Parallelizer class."""
 
 import importlib
-from typing import Dict, Type, Union
+from typing import Dict, List, Type, Union
 
 from transformers import PreTrainedModel
 
 from .base import Parallelizer
 
 
 _PARALLELIZER_CLASSES_MODULE_NAMES = ["encoder_models", "decoder_models"]
@@ -55,14 +55,18 @@
             "roberta": "RobertaParallelizer",
             "gpt_neo": "GPTNeoParallelizer",
             "llama": "LlamaParallelizer",
         }
     )
 
     @classmethod
+    def get_supported_model_types(cls) -> List[str]:
+        return list(cls._MODEL_TYPE_TO_PARALLEL_MODEL_CLASS.keys())
+
+    @classmethod
     def _get_model_type(cls, model_type_or_model: Union[str, PreTrainedModel]) -> str:
         if isinstance(model_type_or_model, PreTrainedModel):
             model_type = model_type_or_model.config.model_type
         else:
             model_type = model_type_or_model
         return model_type
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/generation/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/generation/utils.py` & `optimum-neuron-0.0.8/optimum/neuron/generation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1271,15 +1271,15 @@
                 next_token_logits = torch.matmul(one_hot, outputs.logits)
                 next_token_logits = next_token_logits.squeeze(1)
             else:
                 next_token_logits = outputs.logits[:, -1, :]
 
             # pre-process distribution
             # Move to cpu to handle arbitrary logits_processor
-            next_tokens_scores = logits_processor(input_ids[:, :seq_length].to("cpu"), next_token_logits.to("cpu"))
+            next_tokens_scores = logits_processor(input_ids.to("cpu")[:, :seq_length], next_token_logits.to("cpu"))
             next_tokens_scores = next_tokens_scores.to(input_ids.device)
 
             # Store scores, attentions and hidden_states when required
             if return_dict_in_generate:
                 if output_scores:
                     scores += (next_tokens_scores,)
                 if output_attentions:
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.8/optimum/neuron/hf_argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Customizes the HfArgumentParser to add checks for AWS Tranium instances."""
+"""Customizes the HfArgumentParser to add checks for AWS Neuron instances."""
 
 from transformers import HfArgumentParser
 
 from .utils.argument_utils import validate_arg
 
 
-class TrainiumHfArgumentParser(HfArgumentParser):
+class NeuronHfArgumentParser(HfArgumentParser):
     def validate_args(self, args):
         validate_arg(
             args,
             "pad_to_max_length",
             (
                 "pad_to_max_length=False can lead to very poor performance because it can trigger a lot of recompilation "
                 "due to variable sequence length."
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/modeling_base.py` & `optimum-neuron-0.0.8/optimum/neuron/modeling_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 import torch
 from huggingface_hub import HfApi, HfFolder, hf_hub_download
-from packaging import version
 from transformers import AutoConfig, AutoModel
 
 from ..exporters.neuron import export
 from ..exporters.neuron.model_configs import *  # noqa: F403
 from ..exporters.tasks import TasksManager
 from ..modeling_base import OptimizedModel
 from ..utils.save_utils import maybe_load_preprocessors, maybe_save_preprocessors
 from .utils import NEURON_FILE_NAME, is_neuron_available, store_compilation_config
 from .utils.import_utils import is_neuronx_available
-from .utils.version_utils import get_neuroncc_version, get_neuronxcc_version
+from .utils.version_utils import check_compiler_compatibility, get_neuroncc_version, get_neuronxcc_version
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
     from ..exporters.neuron import NeuronConfig
 
@@ -154,34 +153,18 @@
                     f"Too many neuron model files were found in {model_path}, specify which one to load by using the "
                     "file_name argument."
                 )
             else:
                 file_name = neuron_files[0].name
 
         # Check compiler compatibility(compiler type and version) of the saved model vs. system.
-        if hasattr(config, "neuron_compiler"):
-            if config.neuron_compiler == "neuron-cc":
-                compiler_available_fn = is_neuron_available
-                installed_compiler_version_fn = get_neuroncc_version
-            elif config.neuron_compiler == "neuronx-cc":
-                compiler_available_fn = is_neuronx_available
-                installed_compiler_version_fn = get_neuronxcc_version
-            else:
-                raise RuntimeError(f"Pretrained model compiler type {config.neuron_compiler} not recognized.")
-
-            if not compiler_available_fn():
-                raise RuntimeError(
-                    f"Pretrained model was compiled for {config.neuron_compiler}, but {config.neuron_compiler} is not installed."
-                )
-                if hasattr(config, "neuron_compiler_version"):
-                    if version.parse(config.neuron_compiler_version) > version.parse(installed_compiler_version_fn()):
-                        raise RuntimeError(
-                            f"Pretrained model ({config.neuron_compiler}={installed_compiler_version_fn()}) is newer than current compiler ({config.neuron_compiler}={config.neuron_compiler_version}),"
-                            " which may cause runtime incompatabilities."
-                        )
+        if hasattr(config, "neuron") and "compiler_type" in config.neuron:
+            model_compiler_type = config.neuron.get("compiler_type")
+            model_compiler_version = config.neuron.get("compiler_version")
+            check_compiler_compatibility(model_compiler_type, model_compiler_version)
 
         preprocessors = None
         if model_path.is_dir():
             model = NeuronBaseModel.load_model(model_path / file_name)
             new_model_save_dir = model_path
         else:
             model_cache_path = hf_hub_download(
@@ -262,27 +245,40 @@
 
         neuron_config_constructor = TasksManager.get_exporter_config_constructor(
             model=model, exporter="neuron", task=task
         )
 
         input_shapes = {}
         for name in neuron_config_constructor.func.get_mandatory_axes_for_task(task):
-            static_shape = kwargs_shapes.get(name, None) or getattr(config, "neuron_" + name, None)
+            static_shape = kwargs_shapes.get(name, None) or config.neuron.get("static_" + name, None)
             if static_shape is None:
                 raise AttributeError(
                     f"Cannot find the value of `{name}` from arguments nor the `config`. `{name}` is mandatory"
                     " for exporting the model to the neuron format, please set the value explicitly."
                 )
             else:
                 input_shapes[name] = static_shape
         if is_neuron_available() and dynamic_batch_size is True and "batch_size" in input_shapes:
             input_shapes["batch_size"] = 1
             disable_fallback = True  # Turn off the fallback for neuron, otherwise dynamic batching will still fail
 
-        neuron_config = neuron_config_constructor(model.config, dynamic_batch_size=dynamic_batch_size, **input_shapes)
+        if is_neuronx_available():
+            compiler_type = "neuronx-cc"
+            compiler_version = get_neuronxcc_version()
+        else:
+            compiler_type = "neuron-cc"
+            compiler_version = get_neuroncc_version()
+
+        neuron_config = neuron_config_constructor(
+            model.config,
+            dynamic_batch_size=dynamic_batch_size,
+            compiler_type=compiler_type,
+            compiler_version=compiler_version,
+            **input_shapes,
+        )
 
         # Get compilation arguments
         auto_cast_type = None if auto_cast is None else auto_cast_type
         compiler_kwargs = {
             "auto_cast": auto_cast,
             "auto_cast_type": auto_cast_type,
             "disable_fast_relayout": disable_fast_relayout,
@@ -292,30 +288,23 @@
         input_names, output_names = export(
             model=model,
             config=neuron_config,
             output=save_dir_path / NEURON_FILE_NAME,
             **compiler_kwargs,
         )
 
-        # This logic is a bit of a reacharound, using the same logic as in `export()` to determine the cc version
-        if is_neuronx_available():
-            neuron_compiler = "neuronx-cc"
-            neuron_compiler_version = get_neuronxcc_version()
-        else:
-            neuron_compiler = "neuron-cc"
-            neuron_compiler_version = get_neuroncc_version()
         store_compilation_config(
             config,
             input_shapes,
             compiler_kwargs,
             input_names,
             output_names,
             dynamic_batch_size,
-            neuron_compiler,
-            neuron_compiler_version,
+            compiler_type,
+            compiler_version,
         )
 
         config.save_pretrained(save_dir_path)
         maybe_save_preprocessors(model_id, save_dir_path, src_subfolder=subfolder)
 
         return cls._from_pretrained(save_dir_path, config, model_save_dir=save_dir, neuron_config=neuron_config)
 
@@ -347,34 +336,49 @@
 
         # Registers the NeuronModelForXXX classes into the transformers AutoModel classes to avoid warnings when creating
         # a pipeline https://github.com/huggingface/transformers/blob/3d3204c025b6b5de013e07dd364208e28b4d9589/src/transformers/pipelines/base.py#L940
         AutoConfig.register(self.model_type, AutoConfig)
         if hasattr(self.auto_model_class, "register"):
             self.auto_model_class.register(AutoConfig, self.__class__)
 
-    def _neuron_config_init(self, config: "PretrainedConfig") -> "NeuronConfig":
+    @classmethod
+    def _neuron_config_init(cls, config: "PretrainedConfig") -> "NeuronConfig":
         """
         Builds a `NeuronConfig` with an instance of the `PretrainedConfig` and the task.
         """
+        if not hasattr(config, "neuron"):
+            logger.warning(
+                "Unable to identify neuron configuration with the keyword `neuron`, make sure that your config file contains necessary information"
+            )
+            return
+
+        neuron_configs = config.neuron
+        # Fetch compiler information
+        compiler_type = neuron_configs.get("compiler_type")
+        compiler_version = neuron_configs.get("compiler_version")
+
         # Fetch mandatory shapes from config
         compile_shapes = {
-            key.replace("neuron_", ""): value
-            for (key, value) in config.to_diff_dict().items()
-            if key.startswith("neuron_") and not key.startswith("neuron_compiler")  # <-- TODO: is there a better way?
+            key.replace("static_", ""): value
+            for (key, value) in config.to_diff_dict().get("neuron").items()
+            if key.startswith("static_")
         }
 
         # Neuron config constructuor
-        task = TasksManager.infer_task_from_model(self.auto_model_class)
+        task = TasksManager.infer_task_from_model(cls.auto_model_class)
         neuron_config_constructor = TasksManager.get_exporter_config_constructor(
             model_type=config.model_type, exporter="neuron", task=task
         )
 
-        # Build neuron config
         return neuron_config_constructor(
-            config, dynamic_batch_size=getattr(config, "dynamic_batch_size", False), **compile_shapes
+            config,
+            dynamic_batch_size=getattr(config, "dynamic_batch_size", False),
+            compiler_type=compiler_type,
+            compiler_version=compiler_version,
+            **compile_shapes,
         )
 
     @classmethod
     def get_input_static_shapes(cls, neuron_config: "NeuronConfig") -> Dict[str, int]:
         """
         Gets a dictionary of inputs with their valid static shapes.
         """
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/pipelines/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/base.py` & `optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.8/optimum/neuron/trainer_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines custom Trainer callbacks specific to AWS Trainium instances."""
+"""Defines custom Trainer callbacks specific to AWS Neuron instances."""
 
 import inspect
 import json
 import shutil
 import subprocess
 from collections import defaultdict
 from dataclasses import asdict, dataclass
@@ -24,14 +24,15 @@
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import torch
 from transformers import TrainerCallback, TrainerState
 
 from ..utils import logging
+from .utils import is_torch_xla_available
 from .utils.cache_utils import (
     NEURON_COMPILE_CACHE_NAME,
     NeuronHash,
     download_cached_model_from_hub,
     follows_new_cache_naming_convention,
     get_neuron_cache_path,
     list_files_in_neuron_cache,
@@ -40,14 +41,18 @@
     set_neuron_cache_path,
 )
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel, TrainerControl, TrainingArguments
 
+
+if is_torch_xla_available():
+    import torch_xla.core.xla_model as xm
+
 logger = logging.get_logger(__name__)
 
 
 @dataclass
 class NeuronTrainerState(TrainerState):
     last_inputs: Optional[Dict[str, Any]] = None
 
@@ -59,23 +64,29 @@
     @classmethod
     def from_trainer_state(cls, state: TrainerState) -> "NeuronTrainerState":
         neuron_trainer_state = cls(asdict(state))
         neuron_trainer_state.last_inputs = getattr(state, "last_inputs", {})
         return neuron_trainer_state
 
 
-class NeuronCacheCallaback(TrainerCallback):
+class NeuronCacheCallback(TrainerCallback):
     def __init__(
         self,
         tmp_neuron_cache: Optional[TemporaryDirectory] = None,
         original_neuron_cache_path: Optional[Path] = None,
-        only_do_fetching: bool = False,
+        fetch: bool = True,
+        push: bool = True,
+        wait_for_everyone_on_fetch: bool = True,
+        wait_for_everyone_on_push: bool = True,
     ):
         super().__init__()
-        self.only_do_fetching = only_do_fetching
+        self.fetch = fetch
+        self.push = push
+        self.wait_for_everyone_on_fetch = is_torch_xla_available() and wait_for_everyone_on_fetch
+        self.wait_for_everyone_on_push = is_torch_xla_available() and wait_for_everyone_on_push
 
         # Real Neuron compile cache if it exists.
         if original_neuron_cache_path is None:
             self.neuron_cache_path = get_neuron_cache_path()
         else:
             self.neuron_cache_path = original_neuron_cache_path
         self.use_neuron_cache = self.neuron_cache_path is not None
@@ -192,18 +203,20 @@
         if args.fp16:
             data_type = torch.float16
         elif args.bf16:
             data_type = torch.bfloat16
         else:
             data_type = torch.float32
 
-        key = (model, input_shapes, data_type)
+        key_args = (model, input_shapes, data_type)
+        key_kwargs = {"tensor_parallel_size": args.tensor_parallel_size}
+        key = key_args + tuple(key_kwargs.values())
         neuron_hash = self.neuron_hashes.get(key, None)
         if neuron_hash is None:
-            neuron_hash = NeuronHash(*key)
+            neuron_hash = NeuronHash(*key_args, **key_kwargs)
             self.neuron_hashes[key] = neuron_hash
             if try_to_fetch_cached_model:
                 self.try_to_fetch_cached_model(neuron_hash)
         return neuron_hash
 
     def full_path_to_path_in_temporary_cache(self, path: Path):
         return path_after_folder(path, self.tmp_neuron_cache_path.name)
@@ -266,23 +279,26 @@
         if self.use_neuron_cache:
             self._update_cache_stats(self.neuron_cache_path)
 
         for neuron_hash in self.neuron_hash_to_files:
             self.neuron_hash_to_files[neuron_hash] = []
 
     def on_step_middle(self, args: "TrainingArguments", state: TrainerState, control: "TrainerControl", **kwargs):
-        model = kwargs["model"]
-        self.neuron_hash_for_model(args, model, state.last_inputs, try_to_fetch_cached_model=True)
+        if self.fetch:
+            model = kwargs["model"]
+            self.neuron_hash_for_model(args, model, state.last_inputs, try_to_fetch_cached_model=True)
+        if self.wait_for_everyone_on_fetch:
+            xm.rendezvous("wait for everyone after fetching")
 
     def on_step_end(self, args: "TrainingArguments", state: "TrainerState", control: "TrainerControl", **kwargs):
         """
         Event called at the end of a training step. If using gradient accumulation, one training step might take
         several inputs.
         """
-        if not self.only_do_fetching:
+        if self.push:
             model = kwargs["model"]
             state = self.prepare_state(state)
             neuron_hash = self.neuron_hash_for_model(args, model, state.last_inputs, try_to_fetch_cached_model=True)
             diff = self.synchronize_temporary_neuron_cache_state()
             self.neuron_hash_to_files[neuron_hash].extend(diff)
 
     def on_prediction_step(self, args: "TrainingArguments", state: TrainerState, control: "TrainerControl", **kwargs):
@@ -291,16 +307,18 @@
         """
         self.on_step_end(args, state, control, **kwargs)
 
     def on_save(self, args: "TrainingArguments", state: TrainerState, control: "TrainerControl", **kwargs):
         """
         Event called after a checkpoint save.
         """
-        if not self.only_do_fetching:
+        if self.push:
             self.synchronize_temporary_neuron_cache()
+        if self.wait_for_everyone_on_push:
+            xm.rendezvous("wait for everyone after pushing")
 
     def on_train_end(self, args: "TrainingArguments", state: TrainerState, control: "TrainerControl", **kwargs):
         """
         Event called at the end of training.
         """
         self.on_save(args, state, control, **kwargs)
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/trainers.py` & `optimum-neuron-0.0.8/optimum/neuron/trainers.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,48 +8,57 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines Trainer subclasses to perform training on AWS Trainium instances."""
+"""Defines Trainer subclasses to perform training on AWS Neuron instances."""
 
 import contextlib
 import glob
 import os
 import random
 import warnings
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from packaging import version
+from torch.utils.data import DataLoader
 from transformers import PreTrainedModel, Seq2SeqTrainer, Trainer, TrainingArguments
 from transformers.dependency_versions_check import dep_version_check
 from transformers.integrations import is_fairscale_available
 from transformers.trainer import (
     OPTIMIZER_NAME,
     SCHEDULER_NAME,
     TRAINER_STATE_NAME,
+    TRAINING_ARGS_NAME,
 )
 from transformers.trainer_pt_utils import reissue_pt_warnings
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 from transformers.utils import is_sagemaker_mp_enabled
 
 from ..utils import check_if_transformers_greater, logging
 from .accelerate import NeuronAccelerator, NeuronDistributedType
 from .distributed import ParallelizersManager
-from .trainer_callback import NeuronCacheCallaback
-from .utils import DynamicPatch, ModelPatcher, is_torch_xla_available, patch_within_function
+from .distributed.utils import make_optimizer_constructor_lazy
+from .trainer_callback import NeuronCacheCallback
+from .utils import (
+    DynamicPatch,
+    ModelPatcher,
+    is_torch_xla_available,
+    patch_within_function,
+)
 from .utils.cache_utils import get_neuron_cache_path
 from .utils.training_utils import (
     TRANSFORMERS_MIN_VERSION_USE_ACCELERATE,
+    get_model_param_count,
     is_precompilation,
     patch_generation_mixin_to_neuron_generation_mixin,
     patched_finfo,
     prepare_environment_for_neuron,
     skip_first_batches,
 )
 
@@ -91,21 +100,24 @@
 
 
 if os.environ.get("TORCHELASTIC_RUN_ID"):
     import torch_xla.distributed.xla_backend as xbn
 
     if not isinstance(torch.distributed.group.WORLD, xbn.ProcessGroupXla):
         _ORIGINAL_NEURON_CACHE_PATH = get_neuron_cache_path()
-        _TMP_NEURON_CACHE_DIR = NeuronCacheCallaback.create_temporary_neuron_cache(get_neuron_cache_path())
+        if not is_precompilation():
+            _TMP_NEURON_CACHE_DIR = NeuronCacheCallback.create_temporary_neuron_cache(get_neuron_cache_path())
         torch.distributed.init_process_group(backend="xla")
         if not isinstance(torch.distributed.group.WORLD, xbn.ProcessGroupXla):
             raise AssertionError("Failed to initialize torch.distributed process group using XLA backend.")
 
+transformers_get_optimizer_cls_and_kwargs = Trainer.get_optimizer_cls_and_kwargs
+
 
-class AugmentTrainerForTrainiumMixin:
+class AugmentTrainerForNeuronMixin:
     def __init__(self, *args, **kwargs):
         if not isinstance(self, Trainer):
             raise TypeError(f"{self.__class__.__name__} can only be mixed with Trainer subclasses.")
 
         training_args = kwargs.get("args", None)
         if training_args is None and len(args) >= 2:
             training_args = args[1]
@@ -134,25 +146,37 @@
         if self.is_fsdp_enabled and self.args.do_eval:
             raise ValueError("Evaluation is not supported with XLA FSDP yet.")
 
         if self.args.local_rank <= 0:
             logger.setLevel(logging.INFO)
 
         if not is_precompilation():
-            callback = NeuronCacheCallaback(
+            push = self.args.local_rank <= 0
+            fetch = self.args.local_rank <= 0
+
+            callback = NeuronCacheCallback(
                 tmp_neuron_cache=_TMP_NEURON_CACHE_DIR,
                 original_neuron_cache_path=_ORIGINAL_NEURON_CACHE_PATH,
-                only_do_fetching=self.args.local_rank > 0,
+                fetch=fetch,
+                push=push,
+                wait_for_everyone_on_fetch=False,
+                wait_for_everyone_on_push=True,
             )
-            # TODO: re-enable.
             self.add_callback(callback)
 
         # Make the model Neuron-compatible for generation.
         patch_generation_mixin_to_neuron_generation_mixin(self.model)
 
+    @property
+    def tp_enabled(self):
+        return (
+            check_if_transformers_greater("4.30.0")
+            and self.accelerator.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM
+        )
+
     def prepare_args_for_precompilation(self, args: "TrainingArguments"):
         if args.num_train_epochs != 1:
             logger.info("Setting the number of epochs for precompilation to 1.")
             args.num_train_epochs = 1
         if args.max_steps is not None:
             logger.info("Disabling max_steps for precompilation.")
             args.nax_steps = None
@@ -168,14 +192,15 @@
 
     def create_accelerator_and_postprocess(self):
         # create accelerator object
         self.accelerator = NeuronAccelerator(
             deepspeed_plugin=self.args.deepspeed_plugin,
             gradient_accumulation_steps=self.args.gradient_accumulation_steps,
             tp_plugin=self.args.tp_plugin,
+            zero_1=self.args.zero_1,
         )
 
         # deepspeed and accelerate flags covering both trainer args and accelerate launcher
         self.is_deepspeed_enabled = getattr(self.accelerator.state, "deepspeed_plugin", None) is not None
         self.is_fsdp_enabled = getattr(self.accelerator.state, "fsdp_plugin", None) is not None
 
         # post accelerator creation setup
@@ -201,26 +226,57 @@
 
         with ModelPatcher(patching_specs, ignore_missing_attributes=True):
             return super()._wrap_model(model, training=training, dataloader=dataloader)
 
     # TODO: make this cleaner.
     def trigger_on_step_middle_for_neuron_cache_callback(self, model: "PreTrainedModel"):
         for callback in self.callback_handler.callbacks:
-            if isinstance(callback, NeuronCacheCallaback):
+            if isinstance(callback, NeuronCacheCallback):
                 # kwargs might not have everything expected (like metrics) but all we need is here.
                 kwargs = {
                     "model": model,
                     "tokenizer": self.tokenizer,
                     "optimizer": self.optimizer,
                     "lr_scheduler": self.lr_scheduler,
                     "train_dataloader": self.callback_handler.train_dataloader,
                     "eval_dataloader": self.callback_handler.eval_dataloader,
                 }
                 callback.on_step_middle(self.args, self.state, self.control, **kwargs)
 
+    def _prepare_data_loader_with_accelerator(self, data_loader: DataLoader):
+        if not check_if_transformers_greater("4.31.0"):
+            data_loader = self.accelerator.prepare_data_loader(data_loader)
+        return data_loader
+
+    def _get_train_sampler(self) -> Optional[torch.utils.data.Sampler]:
+        if self.tp_enabled:
+            return None
+        return super()._get_train_sampler()
+
+    def get_train_dataloader(self, *args, **kwargs) -> DataLoader:
+        return self._prepare_data_loader_with_accelerator(super().get_train_dataloader(*args, **kwargs))
+
+    def get_eval_dataloader(self, *args, **kwargs) -> DataLoader:
+        return self._prepare_data_loader_with_accelerator(super().get_eval_dataloader(*args, **kwargs))
+
+    def get_test_dataloader(self, *args, **kwargs) -> DataLoader:
+        return self._prepare_data_loader_with_accelerator(super().get_test_dataloader(*args, **kwargs))
+
+    @staticmethod
+    def get_optimizer_cls_and_kwargs(args: TrainingArguments) -> Tuple[Any, Any]:
+        optimizer_cls, optimizer_kwargs = transformers_get_optimizer_cls_and_kwargs(args)
+        lazy_load = args.tp_plugin.should_parallelize or args.zero_1
+        if check_if_transformers_greater("4.30.0") and lazy_load:
+            optimizer_cls = make_optimizer_constructor_lazy(optimizer_cls)
+        return optimizer_cls, optimizer_kwargs
+
+    @patch_within_function(("transformers.Trainer.get_optimizer_cls_and_kwargs", get_optimizer_cls_and_kwargs))
+    def create_optimizer(self):
+        return super().create_optimizer()
+
     def compute_loss(self, model, inputs, return_outputs: bool = False):
         self.state.last_inputs = inputs
         self.trigger_on_step_middle_for_neuron_cache_callback(model)
         return super().compute_loss(model, inputs, return_outputs=return_outputs)
 
     def prediction_step(
         self,
@@ -229,14 +285,26 @@
         prediction_loss_only: bool,
         ignore_keys: Optional[List[str]] = None,
     ) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
         self.state.last_inputs = inputs
         self.trigger_on_step_middle_for_neuron_cache_callback(model)
         return super().prediction_step(model, inputs, prediction_loss_only, ignore_keys=ignore_keys)
 
+    @patch_within_function(("transformers.trainer.get_model_param_count", get_model_param_count))
+    def _inner_training_loop(
+        self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
+    ):
+        return super()._inner_training_loop(
+            batch_size=batch_size,
+            args=args,
+            resume_from_checkpoint=resume_from_checkpoint,
+            trial=trial,
+            ignore_keys_for_eval=ignore_keys_for_eval,
+        )
+
     # def _nested_gather_for_xla_fsdp(self, tensors, name=None):
     #     # if isinstance(tensors, (list, tuple)):
     #     #     return type(tensors)(self._nested_gather_for_xla_fsdp(t, f"{name}_{i}") for i, t in enumerate(tensors))
     #     # if isinstance(tensors, dict):
     #     #     return type(tensors)(
     #     #         {k: self._nested_gather_for_xla_fsdp(t, f"{name}_{i}") for i, (k, t) in enumerate(tensors.items())}
     #     #     )
@@ -271,14 +339,24 @@
         if self.hp_search_backend is None and trial is None:
             self.store_flos()
 
         run_dir = self._get_output_dir(trial=trial)
         output_dir = os.path.join(run_dir, checkpoint_folder)
         os.makedirs(output_dir, exist_ok=True)
 
+        if xm.is_master_ordinal():
+            os.makedirs(output_dir, exist_ok=True)
+            torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
+
+        if self.tokenizer is not None and self.args.should_save:
+            self.tokenizer.save_pretrained(output_dir)
+
+        if isinstance(self.model, PreTrainedModel):
+            self.model.config.save_pretrained(output_dir)
+
         self.accelerator.save_state(output_dir)
 
         # Save scaler
         # TODO: is grad scaling supported with TORCH XLA?
         # reissue_pt_warnings(caught_warnings)
         # if self.do_grad_scaling:
         #     xm.save(self.scaler.state_dict(), os.path.join(output_dir, SCALER_NAME))
@@ -326,15 +404,14 @@
             self._push_from_checkpoint(output_dir)
 
         # Maybe delete some older checkpoints.
         if self.args.should_save:
             self._rotate_checkpoints(use_mtime=True, output_dir=run_dir)
 
     def _save_checkpoint(self, model, trial, metrics=None):
-        # if self.fsdp or self.is_fsdp_enabled:
         if check_if_transformers_greater("4.30.0") and self.accelerator.distributed_type in [
             NeuronDistributedType.XLA_FSDP,
             NeuronDistributedType.TENSOR_PARALLELISM,
         ]:
             return self._save_checkpoint_with_accelerator(model, trial, metrics=metrics)
         return super()._save_checkpoint(model, trial, metrics=metrics)
 
@@ -382,17 +459,17 @@
             args=args,
             resume_from_checkpoint=resume_from_checkpoint,
             trial=trial,
             ignore_keys_for_eval=ignore_keys_for_eval,
         )
 
 
-class TrainiumTrainer(AugmentTrainerForTrainiumMixin, Trainer):
+class NeuronTrainer(AugmentTrainerForNeuronMixin, Trainer):
     """
     Trainer that is suited for performing training on AWS Tranium instances.
     """
 
 
-class Seq2SeqTrainiumTrainer(AugmentTrainerForTrainiumMixin, Seq2SeqTrainer):
+class Seq2SeqNeuronTrainer(AugmentTrainerForNeuronMixin, Seq2SeqTrainer):
     """
     Seq2SeqTrainer that is suited for performing training on AWS Tranium instances.
     """
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/training_args.py` & `optimum-neuron-0.0.8/optimum/neuron/training_args.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines a TrainingArguments class compatible with Trainium."""
+"""Defines a TrainingArguments class compatible with Neuron."""
 
 import io
 import json
 import os
 import warnings
 from dataclasses import dataclass, field
 from datetime import timedelta
@@ -45,15 +45,21 @@
 
     smp.init()
 
 
 logger = logging.get_logger(__name__)
 
 
-class TrainiumTrainingArgumentsMixin:
+@dataclass
+class NeuronTrainingArgumentsMixin:
+    zero_1: bool = field(default=False, metadata={"help": "Whether to use  ZeRO Stage 1 Optimization."})
+    tensor_parallel_size: int = field(
+        default=1, metadata={"help": "The number of replicas the model will be sharded on."}
+    )
+
     def __post_init__(self):
         # Patches accelerate.utils.imports.is_tpu_available to match `is_torch_xla_available`
         patch_accelerate_is_tpu_available()
 
         if self.fsdp != "":
             # Disabling FSDP until next release because it is still very experimental and not validated.
             raise RuntimeError("FSDP is not supported yet.")
@@ -181,20 +187,23 @@
                     torch.cuda.set_device(device)
         return device
 
     @property
     def place_model_on_device(self):
         return not self.tp_plugin.should_parallelize and super().place_model_on_device
 
+    @property
+    def world_size(self):
+        divisor = 1
+        if self.tp_plugin.should_parallelize:
+            divisor = self.tp_plugin.tensor_parallel_size
+        return super().world_size // divisor
+
 
 @dataclass
-class TrainiumTrainingArguments(TrainiumTrainingArgumentsMixin, TrainingArguments):
-    tensor_parallel_size: int = field(
-        default=1, metadata={"help": "The number of replicas the model will be sharded on."}
-    )
+class NeuronTrainingArguments(NeuronTrainingArgumentsMixin, TrainingArguments):
+    pass
 
 
 @dataclass
-class Seq2SeqTrainiumTrainingArguments(TrainiumTrainingArgumentsMixin, Seq2SeqTrainingArguments):
-    tensor_parallel_size: int = field(
-        default=1, metadata={"help": "The number of replicas the model will be sharded on."}
-    )
+class Seq2SeqNeuronTrainingArguments(NeuronTrainingArgumentsMixin, Seq2SeqTrainingArguments):
+    pass
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .argument_utils import convert_neuronx_compiler_args_to_neuron, store_compilation_config
-from .constant import NEURON_FILE_NAME
+from .constant import (
+    DIFFUSION_MODEL_TEXT_ENCODER_NAME,
+    DIFFUSION_MODEL_UNET_NAME,
+    DIFFUSION_MODEL_VAE_DECODER_NAME,
+    DIFFUSION_MODEL_VAE_ENCODER_NAME,
+    NEURON_FILE_NAME,
+)
 from .import_utils import (
     is_accelerate_available,
     is_neuron_available,
     is_neuronx_available,
     is_neuronx_distributed_available,
     is_torch_xla_available,
+    is_transformers_neuronx_available,
 )
 from .optimization_utils import get_attention_scores
 from .patching import DynamicPatch, ModelPatcher, Patcher, patch_everywhere, patch_within_function
 from .training_utils import (
     FirstAndLastDataset,
     is_model_officially_supported,
     is_precompilation,
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/argument_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,33 +139,46 @@
 def store_compilation_config(
     config: Union["PretrainedConfig", OrderedDict],
     input_shapes: Dict[str, int],
     compiler_kwargs: Dict[str, Any],
     input_names: List[str],
     output_names: List[str],
     dynamic_batch_size: bool,
-    neuron_compiler: str,
-    neuron_compiler_version: str,
+    compiler_type: str,
+    compiler_version: str,
+    model_type: Optional[str] = None,
     **kwargs,
 ):
     if isinstance(config, OrderedDict):
         update_func = config.__setitem__
     else:
         update_func = config.__setattr__
+    config_args = {}
 
     # Add neuron version to the config, so it can be checked at load time
-    update_func("neuron_compiler", neuron_compiler)
-    update_func("neuron_compiler_version", neuron_compiler_version)
+    config_args["compiler_type"] = compiler_type
+    config_args["compiler_version"] = compiler_version
 
     # Add input shapes during compilation to the config
-    for axe, shape in input_shapes.items():
-        axe = f"neuron_{axe}"
-        update_func(axe, shape)
+    for axis, shape in input_shapes.items():
+        axis = f"static_{axis}"
+        config_args[axis] = shape
 
-    update_func("dynamic_batch_size", dynamic_batch_size)
+    config_args["dynamic_batch_size"] = dynamic_batch_size
 
     # Add compilation args to the config
     for arg, value in compiler_kwargs.items():
-        update_func(arg, value)
+        config_args[arg] = value
 
-    config.input_names = input_names
-    config.output_names = output_names
+    config_args["input_names"] = input_names
+    config_args["output_names"] = output_names
+
+    update_func("neuron", config_args)
+
+    if hasattr(config, "_diffusers_version"):
+        import diffusers
+
+        update_func("_diffusers_version", diffusers.__version__)
+
+    model_type = getattr(config, "model_type", None) or model_type
+    model_type = str(model_type).replace("_", "-")
+    update_func("model_type", model_type)
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/cache_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def set_custom_cache_repo_name_in_hf_home(repo_id: str, hf_home: str = HF_HOME, check_repo: bool = True):
     hf_home_cache_repo_file = f"{hf_home}/{CACHE_REPO_FILENAME}"
     if check_repo:
         try:
             HfApi().repo_info(repo_id, repo_type="model")
         except Exception as e:
             raise ValueError(
-                f"Could not save the custom Trainium cache repo to be {repo_id} because it does not exist or is "
+                f"Could not save the custom Neuron cache repo to be {repo_id} because it does not exist or is "
                 f"private to you. Complete exception message: {e}."
             )
 
     existing_custom_cache_repo = load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file)
     if existing_custom_cache_repo is not None:
         logger.warning(
             f"A custom cache repo was already registered: {existing_custom_cache_repo}. It will be overwritten to "
@@ -171,17 +171,17 @@
 def get_hf_hub_cache_repos():
     hf_hub_repos = HF_HUB_CACHE_REPOS
 
     saved_custom_cache_repo = load_custom_cache_repo_name_from_hf_home()
     if saved_custom_cache_repo is None:
         warn_once(
             logger,
-            "No Trainium cache name is saved locally. This means that only the official Trainium cache, and "
-            "potentially a cache defined in $CUSTOM_CACHE_REPO will be used. You can create a Trainium cache repo by "
-            "running the following command: `optimum-cli neuron cache create`. If the Trainium cache already exists "
+            "No Neuron cache name is saved locally. This means that only the official Neuron cache, and "
+            "potentially a cache defined in $CUSTOM_CACHE_REPO will be used. You can create a Neuron cache repo by "
+            "running the following command: `optimum-cli neuron cache create`. If the Neuron cache already exists "
             "you can set it by running the following command: `optimum-cli neuron cache set -n [name]`.",
         )
     else:
         hf_hub_repos = [saved_custom_cache_repo] + hf_hub_repos
 
     custom_cache_repo = os.environ.get("CUSTOM_CACHE_REPO", None)
     if custom_cache_repo is not None:
@@ -201,15 +201,15 @@
 
         process_index = xm.get_ordinal()
 
     if process_index == 0 and hf_hub_repos and not has_write_access_to_repo(hf_hub_repos[0]):
         warn_once(
             logger,
             f"You do not have write access to {hf_hub_repos[0]} so you will not be able to push any cached compilation "
-            "files. Please log in and/or use a custom Trainium cache.",
+            "files. Please log in and/or use a custom Neuron cache.",
         )
     return hf_hub_repos
 
 
 def get_neuron_cache_path() -> Optional[Path]:
     # NEURON_CC_FLAGS is the environment variable read by the neuron compiler.
     # Among other things, this is where the cache directory is specified.
@@ -514,28 +514,45 @@
                 min_neuron_compiler_version=min_neuron_compiler_version,
                 default=default,
             )
 
         return constructor
 
     def check_requirements_are_met(self, neuron_compiler_version: str):
+        if self.should_be_inserted_in_hash_dict(neuron_compiler_version) and self.default is None:
+            raise ValueError("A default value must be specified.")
+        # from ..version import __version__
+
+        # optimum_neuron_requirement = True
+        # if self.min_optimum_neuron_version is not None:
+        #     if version.parse(__version__) >= version.parse(self.min_optimum_neuron_version):
+        #         optimum_neuron_requirement = self.default is not None
+
+        # neuron_compiler_requirement = True
+        # if self.min_neuron_compiler_version is not None:
+        #     if version.parse(neuron_compiler_version) >= version.parse(self.min_neuron_compiler_version):
+        #         neuron_compiler_requirement = self.default is not None
+
+        # if not optimum_neuron_requirement or not neuron_compiler_requirement:
+        #     raise ValueError("A default value must be specified.")
+
+    def should_be_inserted_in_hash_dict(self, neuron_compiler_version: str) -> bool:
         from ..version import __version__
 
-        optimum_neuron_requirement = True
+        optimum_neuron_requirement = False
         if self.min_optimum_neuron_version is not None:
-            if version.parse(__version__) >= version.parse(self.min_optimum_neuron_version):
-                optimum_neuron_requirement = self.default is not None
+            optimum_neuron_requirement = version.parse(__version__) >= version.parse(self.min_optimum_neuron_version)
 
-        neuron_compiler_requirement = True
+        neuron_compiler_requirement = False
         if self.min_neuron_compiler_version is not None:
-            if version.parse(neuron_compiler_version) >= version.parse(self.min_neuron_compiler_version):
-                neuron_compiler_requirement = self.default is not None
+            neuron_compiler_requirement = version.parse(neuron_compiler_version) >= version.parse(
+                self.min_neuron_compiler_version
+            )
 
-        if not optimum_neuron_requirement or not neuron_compiler_requirement:
-            raise ValueError("A default value must be specified.")
+        return optimum_neuron_requirement or neuron_compiler_requirement
 
 
 @dataclass(frozen=True)
 class NeuronHash:
     model: "PreTrainedModel"
     input_shapes: Tuple[Tuple[str, Tuple[int, ...]], ...]
     data_type: torch.dtype
@@ -557,17 +574,16 @@
 
     def _insert_potential_unspecified_hash_attribute(
         self, attribute_name: str, attribute: Any, hash_dict: Dict[str, Any]
     ):
         """
         Inserts `attribute` in `hash_dict` only if it is a specified attribute or if it has a default value.
         """
-        if isinstance(attribute, _UnspecifiedHashAttribute):
-            if attribute.default is not None:
-                hash_dict[attribute_name] = attribute
+        if isinstance(attribute, _UnspecifiedHashAttribute) and attribute.should_be_inserted_in_hash_dict:
+            hash_dict[attribute_name] = attribute.default
         else:
             hash_dict[attribute_name] = attribute
 
     @property
     def hash_dict(self) -> Dict[str, Any]:
         hash_dict = asdict(self)
         hash_dict["model"] = hash_dict["model"].state_dict()
@@ -577,18 +593,21 @@
 
         self._insert_potential_unspecified_hash_attribute("tensor_parallel_size", self.tensor_parallel_size, hash_dict)
         self._insert_potential_unspecified_hash_attribute("fsdp", self.fsdp, hash_dict)
 
         return hash_dict
 
     def state_dict_to_bytes(self, state_dict: Dict[str, torch.Tensor]) -> bytes:
+        cast_to_mapping = {
+            torch.bfloat16: torch.float16,
+        }
         bytes_to_join = []
         for name, tensor in state_dict.items():
             memfile = io.BytesIO()
-            np.save(memfile, tensor.cpu().numpy())
+            np.save(memfile, tensor.to(cast_to_mapping.get(tensor.dtype, tensor.dtype)).cpu().numpy())
             bytes_to_join.append(name.encode("utf-8"))
             bytes_to_join.append(memfile.getvalue())
         return b"".join(bytes_to_join)
 
     def compute_sha512_hash(self, *buffers: bytes) -> str:
         hash_ = hashlib.sha512()
         for buffer in buffers:
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/compilation_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/compilation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,17 +281,17 @@
                 "You need to log in the Hugging Face Hub otherwise you will not be able to push anything. "
                 "Please run the following command: huggingface-cli login"
             )
         saved_custom_cache_repo = load_custom_cache_repo_name_from_hf_home()
         custom_cache_repo = os.environ.get("CUSTOM_CACHE_REPO", None)
         if saved_custom_cache_repo is None and custom_cache_repo is None:
             logger.warning(
-                "No custom Trainium cache repo set which means that the official Trainium cache repo will be used. If "
+                "No custom Neuron cache repo set which means that the official Neuron cache repo will be used. If "
                 "you are not a member of the Optimum Neuron Team, this means that you will not be able to push to the "
-                "Hub. Follow the instructions here to set you custom Trainium cache: "
+                "Hub. Follow the instructions here to set you custom Neuron cache: "
                 "https://huggingface.co/docs/optimum-neuron/guides/cache_system#how-to-use-a-private-trainium-model-cache"
             )
 
         main_repo = get_hf_hub_cache_repos()[0]
         has_write_access = has_write_access_to_repo(main_repo)
         if not has_write_access:
             raise RuntimeError(
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/constant.py` & `optimum-neuron-0.0.8/optimum/neuron/distributed/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,10 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Constants used as default values."""
 
-NEURON_FILE_NAME = "model.neuron"
+from .base import Parallelizer
+from .checkpointing import (
+    consolidate_tensor_parallel_checkpoints,
+    consolidate_tensor_parallel_checkpoints_to_unified_checkpoint,
+)
+from .parallelizers_manager import ParallelizersManager
+from .utils import lazy_load_for_parallelism
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/import_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     return found_torch_xla and import_succeeded
 
 
 def is_neuronx_distributed_available() -> bool:
     return importlib.util.find_spec("neuronx_distributed") is not None
 
 
+def is_transformers_neuronx_available() -> bool:
+    return importlib.util.find_spec("transformers_neuronx") is not None
+
+
 def is_accelerate_available(min_version: Optional[str] = MIN_ACCELERATE_VERSION) -> bool:
     _accelerate_available = importlib.util.find_spec("accelerate") is not None
     if min_version is not None:
         if _accelerate_available:
             import accelerate
 
             _accelerate_version = accelerate.__version__
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/optimization_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/patching.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/patching.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,15 +73,26 @@
 
     def process_patching_specs(
         self, patching_specs: Optional[List[Tuple[str, Any]]] = None, ignore_missing_attributes: bool = False
     ):
         proccessed_patching_specs = []
         for orig, patch in patching_specs or []:
             module_qualified_name, attribute_name = orig.rsplit(".", maxsplit=1)
-            module = importlib.import_module(module_qualified_name)
+            try:
+                module = importlib.import_module(module_qualified_name)
+            except ModuleNotFoundError as e:
+                module_qualified_name, module_attribute_containing_attribute_name = module_qualified_name.rsplit(
+                    ".", maxsplit=1
+                )
+                module = importlib.import_module(module_qualified_name)
+                try:
+                    module = getattr(module, module_attribute_containing_attribute_name)
+                except AttributeError:
+                    raise e
+
             module_has_attr = hasattr(module, attribute_name)
             if module_has_attr:
                 attribute = getattr(module, attribute_name)
             elif ignore_missing_attributes and not isinstance(patch, DynamicPatch):
                 attribute = None
             elif isinstance(patch, DynamicPatch):
                 raise ValueError("Cannot ignore missing attribute with a DynamicPatch.")
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.8/optimum/neuron/utils/training_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     MODEL_FOR_SEMANTIC_SEGMENTATION_MAPPING_NAMES,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING_NAMES,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES,
     MODEL_FOR_SPEECH_SEQ_2_SEQ_MAPPING_NAMES,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING_NAMES,
     MODEL_MAPPING_NAMES,
 )
+from transformers.trainer_pt_utils import get_model_param_count as transformers_get_model_param_count
 from transformers.utils.logging import set_verbosity as set_verbosity_transformers
 
 from ...utils.logging import set_verbosity as set_verbosity_optimum
 from ..generation import NeuronGenerationMixin
 from . import is_torch_xla_available
 
 
@@ -226,14 +227,16 @@
     Changes the vanilla `GenerationMixin` class from Transformers to `NeuronGenerationMixin` in the model's
     inheritance. This allows to make the model Neuron-compatible for generation without much hassle.
     """
     to_visit = [model.__class__]
     should_stop = False
     while to_visit and not should_stop:
         cls = to_visit.pop(0)
+        if cls is object:
+            continue
         bases = cls.__bases__
         new_bases = []
         for base in bases:
             to_visit.append(base)
             if base == GenerationMixin:
                 new_bases.append(NeuronGenerationMixin)
                 should_stop = True
@@ -246,15 +249,17 @@
 
 
 def prepare_environment_for_neuron():
     """
     Prepares the system environment for Transformers models training on AWS Neuron.
     """
     # Set compiler flag to compile for transformer model type
-    os.environ["NEURON_CC_FLAGS"] = os.environ.get("NEURON_CC_FLAGS", "") + " --model-type=transformer"
+    os.environ["NEURON_CC_FLAGS"] = (
+        os.environ.get("NEURON_CC_FLAGS", "") + " --model-type=transformer --enable-experimental-O1"
+    )
 
 
 def set_verbosity(verbosity: int):
     set_verbosity_transformers(verbosity)
     set_verbosity_optimum(verbosity)
 
 
@@ -271,7 +276,13 @@
     `torch_xla.distributed`, for XLA FSDP for instance.
     """
     if isinstance(dataloader, (pl.ParallelLoader, pl.PerDeviceLoader)):
         dataloader._loader = skip_first_batches(dataloader._loader, num_batches=num_batches)
     else:
         dataloader = accelerate_skip_first_batches(dataloader, num_batches=num_batches)
     return dataloader
+
+
+def get_model_param_count(model, trainable_only=False):
+    """Wrapper around `transformers.trainer_pt_utils.get_model_param_count` to handle tensor parallelism."""
+    # TODO: make it work for TP
+    return transformers_get_model_param_count(model, trainable_only=trainable_only)
```

### Comparing `optimum-neuron-0.0.7/optimum/neuron/version.py` & `optimum-neuron-0.0.8/optimum/neuron/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

### Comparing `optimum-neuron-0.0.7/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.8/optimum_neuron.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.7
+Version: 0.0.8
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: quality
 Provides-Extra: neuron
 Provides-Extra: neuronx
+Provides-Extra: diffusers
 License-File: LICENSE
 
 <!---
 Copyright 2023 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
@@ -37,15 +38,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 -->
 
 # Optimum Neuron
 
-🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls). 
+🤗 Optimum Neuron is the interface between the 🤗 Transformers library and AWS Accelerators including [AWS Trainium](https://aws.amazon.com/machine-learning/trainium/?nc1=h_ls) and [AWS Inferentia](https://aws.amazon.com/machine-learning/inferentia/?nc1=h_ls).
 It provides a set of tools enabling easy model loading, training and inference on single- and multi-Accelerator settings for different downstream tasks.
 The list of officially validated models and tasks is available [here](TODO:). Users can try other models and tasks with only few changes.
 
 ## Install
 To install the latest release of this package:
 
 ```bash
@@ -79,22 +80,22 @@
 
 🤗 Optimum Neuron was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers user while leveraging the complete power of AWS Accelerators**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - TrainiumArgumentParser: inherits the original [HfArgumentParser](https://huggingface.co/docs/transformers/main/en/internal/trainer_utils#transformers.HfArgumentParser) in Transformers with additional checks on the argument values to make sure that they will work well with AWS Trainium instances.
-- [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
+- [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer): this version trainer takes care of doing the proper checks and changes to the supported models to make them trainable on AWS Trainium instances.
 
-The [TrainiumTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the TrainiumTrainer one.
+The [NeuronTrainer](https://huggingface.co/docs/optimum/neuron/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Trainium will mostly consist in simply swapping the Trainer class for the NeuronTrainer one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-neuron/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 ```diff
 from transformers import TrainingArguments
-+from optimum.neuron import TrainiumTrainer as Trainer
++from optimum.neuron import NeuronTrainer as Trainer
 
 training_args = TrainingArguments(
   # training arguments...
 )
 
 # A lot of code here
```

### Comparing `optimum-neuron-0.0.7/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.8/optimum_neuron.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,60 +4,66 @@
 pyproject.toml
 setup.cfg
 setup.py
 optimum/commands/export/neuron.py
 optimum/commands/export/neuronx.py
 optimum/commands/neuron/base.py
 optimum/commands/neuron/cache.py
+optimum/commands/neuron/subcommands.py
 optimum/commands/register/register_export.py
 optimum/commands/register/register_neuron.py
 optimum/exporters/neuron/__init__.py
 optimum/exporters/neuron/__main__.py
 optimum/exporters/neuron/base.py
 optimum/exporters/neuron/config.py
 optimum/exporters/neuron/convert.py
 optimum/exporters/neuron/model_configs.py
 optimum/exporters/neuron/utils.py
 optimum/neuron/__init__.py
 optimum/neuron/hf_argparser.py
 optimum/neuron/modeling.py
 optimum/neuron/modeling_base.py
+optimum/neuron/modeling_decoder.py
+optimum/neuron/modeling_diffusion.py
 optimum/neuron/trainer_callback.py
 optimum/neuron/trainers.py
 optimum/neuron/training_args.py
 optimum/neuron/version.py
 optimum/neuron/accelerate/__init__.py
 optimum/neuron/accelerate/accelerator.py
 optimum/neuron/accelerate/optimizer.py
 optimum/neuron/accelerate/scheduler.py
 optimum/neuron/accelerate/state.py
 optimum/neuron/accelerate/utils/__init__.py
 optimum/neuron/accelerate/utils/dataclasses.py
 optimum/neuron/accelerate/utils/misc.py
 optimum/neuron/distributed/__init__.py
 optimum/neuron/distributed/base.py
+optimum/neuron/distributed/checkpointing.py
 optimum/neuron/distributed/decoder_models.py
 optimum/neuron/distributed/encoder_models.py
 optimum/neuron/distributed/parallel_layers.py
 optimum/neuron/distributed/parallelizers_manager.py
 optimum/neuron/distributed/utils.py
 optimum/neuron/generation/__init__.py
 optimum/neuron/generation/utils.py
 optimum/neuron/pipelines/__init__.py
+optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py
 optimum/neuron/pipelines/transformers/__init__.py
 optimum/neuron/pipelines/transformers/base.py
 optimum/neuron/utils/__init__.py
 optimum/neuron/utils/argument_utils.py
 optimum/neuron/utils/cache_utils.py
 optimum/neuron/utils/compilation_utils.py
 optimum/neuron/utils/constant.py
 optimum/neuron/utils/import_utils.py
 optimum/neuron/utils/misc.py
 optimum/neuron/utils/optimization_utils.py
 optimum/neuron/utils/patching.py
+optimum/neuron/utils/require_utils.py
 optimum/neuron/utils/testing_utils.py
 optimum/neuron/utils/training_utils.py
 optimum/neuron/utils/version_utils.py
 optimum_neuron.egg-info/PKG-INFO
 optimum_neuron.egg-info/SOURCES.txt
 optimum_neuron.egg-info/dependency_links.txt
 optimum_neuron.egg-info/entry_points.txt
@@ -65,10 +71,11 @@
 optimum_neuron.egg-info/requires.txt
 optimum_neuron.egg-info/top_level.txt
 tests/test_cache_utils.py
 tests/test_compilation_utils.py
 tests/test_examples.py
 tests/test_generate.py
 tests/test_modeling.py
+tests/test_modeling_decoder.py
 tests/test_trainer_callback.py
 tests/test_trainers.py
 tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.7/pyproject.toml` & `optimum-neuron-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/setup.py` & `optimum-neuron-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,37 @@
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
     "transformers >= 4.28.0",
     "accelerate >= 0.20.1",
-    "optimum",
+    "optimum >= 1.8.8",
     "huggingface_hub >= 0.14.0",
     "numpy>=1.18.5, <=1.21.6",
     "protobuf<4",
 ]
 
-TESTS_REQUIRE = ["pytest", "psutil", "parameterized", "GitPython", "sentencepiece", "datasets", "sacremoses"]
+TESTS_REQUIRE = [
+    "pytest",
+    "psutil",
+    "parameterized",
+    "GitPython",
+    "sentencepiece",
+    "datasets",
+    "sacremoses",
+    "diffusers>=0.17.0",
+    "safetensors",
+]
 
 QUALITY_REQUIRES = [
     "black",
     "ruff",
     "isort",
-    # "hf_doc_builder @ git+https://github.com/huggingface/doc-builder.git",
+#    "hf_doc_builder @ git+https://github.com/huggingface/doc-builder.git",
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
     "neuron": [
         "wheel",
@@ -41,17 +51,20 @@
         "protobuf",
         "torchvision",
     ],
     "neuronx": [
         "wheel",
         "neuronx-cc==2.6.*",
         "torch-neuronx",
+        "transformers-neuronx",
         "torch==1.13.1.*",
         "torchvision==0.14.*",
+        "neuronx_distributed",
     ],
+    "diffusers": ["diffusers"],
 }
 
 setup(
     name="optimum-neuron",
     version=__version__,
     description=(
         "Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS "
```

### Comparing `optimum-neuron-0.0.7/tests/test_cache_utils.py` & `optimum-neuron-0.0.8/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/tests/test_compilation_utils.py` & `optimum-neuron-0.0.8/tests/test_compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/tests/test_examples.py` & `optimum-neuron-0.0.8/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/tests/test_generate.py` & `optimum-neuron-0.0.8/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/tests/test_modeling.py` & `optimum-neuron-0.0.8/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.7/tests/test_trainer_callback.py` & `optimum-neuron-0.0.8/tests/test_trainer_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,39 +19,39 @@
 from unittest import TestCase
 
 import torch
 from huggingface_hub import HfApi
 from transformers import TrainingArguments
 from transformers.testing_utils import is_staging_test
 
-from optimum.neuron.trainers import NeuronCacheCallaback
+from optimum.neuron.trainers import NeuronCacheCallback
 from optimum.neuron.utils.cache_utils import (
     NEURON_COMPILE_CACHE_NAME,
     NeuronHash,
     list_files_in_neuron_cache,
     push_to_cache_on_hub,
     set_neuron_cache_path,
 )
 from optimum.neuron.utils.testing_utils import is_trainium_test
 
 from .utils import StagingTestMixin
 
 
 @is_trainium_test
 @is_staging_test
-class NeuronCacheCallabackTestCase(StagingTestMixin, TestCase):
+class NeuronCacheCallbackTestCase(StagingTestMixin, TestCase):
     def test_neuron_hash_for_model(self):
         with TemporaryDirectory() as tmpdirname:
             args = TrainingArguments(tmpdirname)
         model = self.create_tiny_pretrained_model(random_num_linears=True)
         inputs = {
             "x": torch.rand((1,)),
         }
 
-        callback = NeuronCacheCallaback()
+        callback = NeuronCacheCallback()
 
         # We first check that no hashes is in the hash cache already.
         self.assertFalse(callback.neuron_hashes)
 
         callback.neuron_hash_for_model(args, model, inputs)
         neuron_hash = callback.neuron_hashes[(model, (("x", tuple(inputs["x"].shape)),), torch.float32)]
 
@@ -70,15 +70,15 @@
             inputs = {"x": torch.rand((8, 1)).to("xla")}
             print(model(**inputs))
             neuron_hash = NeuronHash(model, (("x", (8, 1)),), torch.float32)
             push_to_cache_on_hub(neuron_hash, Path(tmpdirname) / NEURON_COMPILE_CACHE_NAME)
 
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
-            callback = NeuronCacheCallaback()
+            callback = NeuronCacheCallback()
             args = TrainingArguments(tmpdirname)
             inputs = {"x": torch.rand((24, 1))}
             neuron_hash = callback.neuron_hash_for_model(args, model, inputs)
 
             found_in_cache = callback.try_to_fetch_cached_model(neuron_hash)
             self.assertFalse(found_in_cache, "No model should have been fetched.")
 
@@ -105,15 +105,15 @@
             self.assertNotEqual(files_diff, [])
             self.assertListEqual(files_diff, state_diff)
             self.assertEqual(len(files_diff), len(neuron_cache_files_diff))
 
     def test_synchronize_temporary_neuron_cache_state(self):
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
-            callback = NeuronCacheCallaback()
+            callback = NeuronCacheCallback()
 
             diff = callback.synchronize_temporary_neuron_cache_state()
             self.assertListEqual(diff, [], "The diff should be empty.")
 
             model = self.create_tiny_pretrained_model(random_num_linears=True).to("xla")
             inputs = {"x": torch.rand((8, 1)).to("xla")}
             # No compilation happens if not printing for some reason...
@@ -129,15 +129,15 @@
     def test_synchronize_temporary_neuron_cache(self):
         os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
         model = self.create_tiny_pretrained_model(random_num_linears=True).to("xla")
 
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
             args = TrainingArguments(tmpdirname)
-            callback = NeuronCacheCallaback()
+            callback = NeuronCacheCallback()
 
             callback.synchronize_temporary_neuron_cache()
             files_in_repo = HfApi().list_repo_files(repo_id=self.CUSTOM_PRIVATE_CACHE_REPO)
             files_in_repo = [f for f in files_in_repo if not f.startswith(".")]
             files_in_cache = list_files_in_neuron_cache(callback.neuron_cache_path, only_relevant_files=True)
             self.assertListEqual(files_in_repo, [], "Repo should be empty.")
             self.assertListEqual(files_in_cache, [], "Cache should be empty.")
```

### Comparing `optimum-neuron-0.0.7/tests/test_trainers.py` & `optimum-neuron-0.0.8/tests/test_trainers.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from unittest import TestCase
 
 from huggingface_hub import HfApi, delete_repo
 from huggingface_hub.utils import RepositoryNotFoundError
 from transformers import BertConfig, BertModel, BertTokenizer, TrainingArguments
 from transformers.testing_utils import is_staging_test
 
-from optimum.neuron.trainers import TrainiumTrainer
+from optimum.neuron.trainers import NeuronTrainer
 from optimum.neuron.utils.cache_utils import (
     get_neuron_cache_path,
     list_files_in_neuron_cache,
     remove_ip_adress_from_path,
     set_neuron_cache_path,
 )
 from optimum.neuron.utils.testing_utils import is_trainium_test
@@ -46,15 +46,15 @@
     create_tiny_pretrained_model,
     get_random_string,
 )
 
 
 @is_trainium_test
 @is_staging_test
-class StagingTrainiumTrainerTestCase(StagingTestMixin, TestCase):
+class StagingNeuronTrainerTestCase(StagingTestMixin, TestCase):
     def test_train_and_eval(self):
         os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
 
         # We take a batch size that does not divide the total number of samples.
         num_train_samples = 1000
         per_device_train_batch_size = 32
         dummy_train_dataset = create_dummy_dataset({"x": (1,), "labels": (1,)}, num_train_samples)
@@ -82,15 +82,15 @@
                 do_eval=True,
                 bf16=True,
                 per_device_train_batch_size=per_device_train_batch_size,
                 per_device_eval_batch_size=per_device_eval_batch_size,
                 save_steps=10,
                 num_train_epochs=2,
             )
-            trainer = TrainiumTrainer(
+            trainer = NeuronTrainer(
                 model,
                 args,
                 train_dataset=dummy_train_dataset,
                 eval_dataset=dummy_eval_dataset,
             )
             start = time.time()
             trainer.train()
@@ -118,15 +118,15 @@
                 do_eval=True,
                 bf16=True,
                 per_device_train_batch_size=per_device_train_batch_size,
                 per_device_eval_batch_size=per_device_eval_batch_size,
                 save_steps=10,
                 num_train_epochs=2,
             )
-            trainer = TrainiumTrainer(
+            trainer = NeuronTrainer(
                 clone,
                 args,
                 train_dataset=dummy_train_dataset,
                 eval_dataset=dummy_eval_dataset,
             )
             start = time.time()
             trainer.train()
@@ -307,15 +307,15 @@
                 "Second training should be faster because cached graphs can be used.",
             )
 
         self.remove_model_and_dataset_on_staging_hub(dataset_name, model_name)
 
 
 @is_trainium_test
-class TrainiumTrainerTestCase(TestCase):
+class NeuronTrainerTestCase(TestCase):
     def _test_training_with_fsdp_mode(self, fsdp_mode: str):
         model_name = "prajjwal1/bert-tiny"
         task_name = "sst2"
 
         with TemporaryDirectory() as tmpdirname:
             set_neuron_cache_path(tmpdirname)
             output_1 = Path(tmpdirname) / "out_1"
```

### Comparing `optimum-neuron-0.0.7/tests/test_utils.py` & `optimum-neuron-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

