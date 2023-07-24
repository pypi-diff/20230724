# Comparing `tmp/shrike-2.0.0.dev4.tar.gz` & `tmp/shrike-2.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-2.0.0.dev4.tar", last modified: Fri Jul 21 02:17:37 2023, max compression
+gzip compressed data, was "shrike-2.0.0.dev5.tar", last modified: Mon Jul 24 19:23:42 2023, max compression
```

## Comparing `shrike-2.0.0.dev4.tar` & `shrike-2.0.0.dev5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/_core/
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/eyesoff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/distributed/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/cluster_auto_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/dask.py
--rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/mpi_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/distributed/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/canary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.734986 shrike-2.0.0.dev4/shrike/pipeline/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.742987 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/spec.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    38725 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/federated_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/module_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    20768 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/ray_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    75663 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v1/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/pipeline/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/pipeline/v2/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.746986 shrike-2.0.0.dev4/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-21 02:13:33.000000 shrike-2.0.0.dev4/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 02:17:37.738986 shrike-2.0.0.dev4/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-21 02:17:37.000000 shrike-2.0.0.dev4/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.323448 shrike-2.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-24 19:23:42.319448 shrike-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 19:23:42.323448 shrike-2.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.303448 shrike-2.0.0.dev5/shrike/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.303448 shrike-2.0.0.dev5/shrike/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/_core/eyesoff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.303448 shrike-2.0.0.dev5/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.307448 shrike-2.0.0.dev5/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.307448 shrike-2.0.0.dev5/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.307448 shrike-2.0.0.dev5/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.311448 shrike-2.0.0.dev5/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41143 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.311448 shrike-2.0.0.dev5/shrike/distributed/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/distributed/cluster_auto_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/distributed/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/distributed/mpi_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/distributed/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.315448 shrike-2.0.0.dev5/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/canary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.299448 shrike-2.0.0.dev5/shrike/pipeline/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.315448 shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    38725 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/module_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20768 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/pipeline_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/ray_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.319448 shrike-2.0.0.dev5/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/pipeline_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/testing/pipeline_class_test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.319448 shrike-2.0.0.dev5/shrike/pipeline/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v1/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v1/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75663 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v1/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.319448 shrike-2.0.0.dev5/shrike/pipeline/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v2/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v2/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/pipeline/v2/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.319448 shrike-2.0.0.dev5/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-24 19:18:37.000000 shrike-2.0.0.dev5/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:23:42.303448 shrike-2.0.0.dev5/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-24 19:23:41.000000 shrike-2.0.0.dev5/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-24 19:23:42.000000 shrike-2.0.0.dev5/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 19:23:41.000000 shrike-2.0.0.dev5/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-24 19:23:41.000000 shrike-2.0.0.dev5/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-24 19:23:41.000000 shrike-2.0.0.dev5/shrike.egg-info/top_level.txt
```

### Comparing `shrike-2.0.0.dev4/LICENSE` & `shrike-2.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/NOTICE.txt` & `shrike-2.0.0.dev5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/PKG-INFO` & `shrike-2.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev4
+Version: 2.0.0.dev5
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev4/README.md` & `shrike-2.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/setup.py` & `shrike-2.0.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/_core/eyesoff.py` & `shrike-2.0.0.dev5/shrike/_core/eyesoff.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/_core/testing.py` & `shrike-2.0.0.dev5/shrike/_core/testing.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/_core/utils.py` & `shrike-2.0.0.dev5/shrike/_core/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/build/commands/prepare.py` & `shrike-2.0.0.dev5/shrike/build/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/build/commands/register.py` & `shrike-2.0.0.dev5/shrike/build/commands/register.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/build/core/command_line.py` & `shrike-2.0.0.dev5/shrike/build/core/command_line.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/build/core/configuration.py` & `shrike-2.0.0.dev5/shrike/build/core/configuration.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/build/utils/utils.py` & `shrike-2.0.0.dev5/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/__init__.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/argparser_utils.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/argparser_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/data_conversions.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/exceptions.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/logging.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
             # log the data
             if run is not None and category == DataCategory.PUBLIC:
                 if step:
                     run.log(name=name, value=value, description=description, step=step)
                 else:
                     run.log(name=name, value=value, description=description)
             self.info(
-                f"NumbericMetric  | {name}:{step} | {value}",
+                f"NumberMetric  | {name}:{step} | {value}",
                 category=category,
             )
 
             return
 
         # collect dataframes
         if is_vaex_dataframe(value):
```

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/progress.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/progress.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/compliant_logging/system_info.py` & `shrike-2.0.0.dev5/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/distributed/cluster_auto_setup.py` & `shrike-2.0.0.dev5/shrike/distributed/cluster_auto_setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/distributed/dask.py` & `shrike-2.0.0.dev5/shrike/distributed/dask.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/distributed/mpi_driver.py` & `shrike-2.0.0.dev5/shrike/distributed/mpi_driver.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/distributed/ray.py` & `shrike-2.0.0.dev5/shrike/distributed/ray.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/__init__.py` & `shrike-2.0.0.dev5/shrike/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/canary_helper.py` & `shrike-2.0.0.dev5/shrike/pipeline/canary_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/run.py` & `shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/run.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/components/fedavg/spec.yaml` & `shrike-2.0.0.dev5/shrike/pipeline/components/fedavg/spec.yaml`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/federated_learning.py` & `shrike-2.0.0.dev5/shrike/pipeline/federated_learning.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/module_helper_base.py` & `shrike-2.0.0.dev5/shrike/pipeline/module_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/pipeline_config.py` & `shrike-2.0.0.dev5/shrike/pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/pipeline_helper_base.py` & `shrike-2.0.0.dev5/shrike/pipeline/pipeline_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/ray_actor.py` & `shrike-2.0.0.dev5/shrike/pipeline/ray_actor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/telemetry_utils.py` & `shrike-2.0.0.dev5/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/testing/components.py` & `shrike-2.0.0.dev5/shrike/pipeline/testing/components.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/testing/importer.py` & `shrike-2.0.0.dev5/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/testing/module_run_tests.py` & `shrike-2.0.0.dev5/shrike/pipeline/testing/module_run_tests.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-2.0.0.dev5/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/testing/pipeline_class_test_v2.py` & `shrike-2.0.0.dev5/shrike/pipeline/testing/pipeline_class_test_v2.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v1/aml_connect.py` & `shrike-2.0.0.dev5/shrike/pipeline/v1/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v1/module_helper.py` & `shrike-2.0.0.dev5/shrike/pipeline/v1/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v1/pipeline_helper.py` & `shrike-2.0.0.dev5/shrike/pipeline/v1/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v2/aml_connect.py` & `shrike-2.0.0.dev5/shrike/pipeline/v2/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v2/module_helper.py` & `shrike-2.0.0.dev5/shrike/pipeline/v2/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/pipeline/v2/pipeline_helper.py` & `shrike-2.0.0.dev5/shrike/pipeline/v2/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike/spark/spark_net.py` & `shrike-2.0.0.dev5/shrike/spark/spark_net.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike.egg-info/PKG-INFO` & `shrike-2.0.0.dev5/shrike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev4
+Version: 2.0.0.dev5
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev4/shrike.egg-info/SOURCES.txt` & `shrike-2.0.0.dev5/shrike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev4/shrike.egg-info/requires.txt` & `shrike-2.0.0.dev5/shrike.egg-info/requires.txt`

 * *Files identical despite different names*

