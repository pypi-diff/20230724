# Comparing `tmp/waffle_hub-0.2.7.tar.gz` & `tmp/waffle_hub-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.7.tar", last modified: Wed Jul 19 12:10:25 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.8.tar", last modified: Mon Jul 24 12:49:30 2023, max compression
```

## Comparing `waffle_hub-0.2.7.tar` & `waffle_hub-0.2.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/
--rw-r--r--   0 lhj       (1001) lhj       (1001)    35149 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/LICENSE
--rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/MANIFEST.in
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/PKG-INFO
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3314 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/README.md
--rw-r--r--   0 lhj       (1001) lhj       (1001)      386 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/requirements.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)       38 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/setup.cfg
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2935 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/setup.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/tests/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8814 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    18878 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_dataset.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4581 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_ddp.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    12951 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2292 2023-07-19 12:09:36.000000 waffle_hub-0.2.7/waffle_hub/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/dataset/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       53 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/dataset/adapter/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      419 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     7146 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6516 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/coco.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     9006 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/transformers.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    14273 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/yolo.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      633 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    50432 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/dataset.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/experimental/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8261 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2986 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/serve.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       39 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       75 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    10199 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4515 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      129 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1913 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     5446 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       77 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2220 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/config.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     9156 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    10543 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       74 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6999 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/config.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    13208 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      585 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    57365 2023-07-19 12:09:24.000000 waffle_hub-0.2.7/waffle_hub/hub/hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/model/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/model/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    13900 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/model/wrapper.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/schema/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      345 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1236 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/base_schema.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1745 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/configs.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      954 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/data.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      378 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/evaluate.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/schema/fields/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    17259 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/annotation.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1722 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/base_field.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     7283 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/category.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3137 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/image.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      537 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/result.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/utils/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3462 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/base_cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3694 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/callback.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1686 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/conversion.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8726 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/data.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4200 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/draw.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4420 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/evaluate.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6049 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/metric_logger.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      631 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/process.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub.egg-info/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/PKG-INFO
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2276 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/SOURCES.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)        1 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/dependency_links.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)      224 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/entry_points.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)      308 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/requires.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)       11 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/top_level.txt
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    35149 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/LICENSE
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/MANIFEST.in
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3314 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/README.md
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      386 2023-07-24 11:38:49.000000 waffle_hub-0.2.8/requirements.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       38 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/setup.cfg
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2935 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/setup.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/tests/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8814 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/tests/test_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    20016 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/tests/test_dataset.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4581 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/tests/test_ddp.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    12951 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/tests/test_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2292 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/waffle_hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/dataset/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       53 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/dataset/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/dataset/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      419 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7146 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6516 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/coco.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9006 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/transformers.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    14273 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/yolo.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      633 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    57191 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/waffle_hub/dataset/dataset.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/experimental/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8261 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2986 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/serve.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       39 2023-07-18 04:05:20.000000 waffle_hub-0.2.8/waffle_hub/hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/hub/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       75 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10199 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4515 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      129 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1913 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     5446 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       77 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2220 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9156 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10543 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       74 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6999 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13208 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      585 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    57365 2023-07-23 12:16:26.000000 waffle_hub-0.2.8/waffle_hub/hub/hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/model/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/waffle_hub/hub/model/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13900 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/model/wrapper.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/schema/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      345 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/schema/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1236 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/base_schema.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1745 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/schema/configs.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      954 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/schema/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      378 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/evaluate.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/schema/fields/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    17259 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/annotation.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1722 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/base_field.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7283 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/category.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3137 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/image.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      537 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/result.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/utils/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/waffle_hub/utils/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3462 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/base_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3694 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/callback.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1686 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/conversion.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8726 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/utils/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4200 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/draw.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4420 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/evaluate.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6049 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/metric_logger.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      631 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/process.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub.egg-info/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2276 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        1 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      224 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/entry_points.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      308 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/requires.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       11 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.7/LICENSE` & `waffle_hub-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/PKG-INFO` & `waffle_hub-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.7
+Version: 0.2.8
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.7 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.8 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.7/README.md` & `waffle_hub-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/setup.py` & `waffle_hub-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/tests/test_cli.py` & `waffle_hub-0.2.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/tests/test_dataset.py` & `waffle_hub-0.2.8/tests/test_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -146,16 +146,31 @@
     dataset: Dataset = Dataset.new(name="test_new", task=TaskType.OBJECT_DETECTION, root_dir=tmpdir)
     assert Path(dataset.dataset_dir).exists()
 
     dataset.delete()
     assert not Path(dataset.dataset_dir).exists()
 
 
-def _load(dataset_name, root_dir):
-    Dataset.load(dataset_name, root_dir=root_dir)
+def _index(dataset_name, root_dir):
+    dataset = Dataset.load(dataset_name, root_dir=root_dir)
+
+    assert len(dataset.image_dict) == len(dataset.get_images())
+    assert len(dataset.unlabeled_image_dict) == len(dataset.get_images(labeled=False))
+    assert len(dataset.annotation_dict) == len(dataset.get_annotations())
+    assert len(dataset.prediction_dict) == len(dataset.get_predictions())
+    assert len(dataset.category_dict) == len(dataset.get_categories())
+
+    assert sum(map(len, dataset.image_to_annotations.values())) == len(dataset.get_annotations())
+    assert sum(map(len, dataset.image_to_predictions.values())) == len(dataset.get_predictions())
+    assert len(dataset.annotation_to_image.values()) == len(dataset.get_annotations())
+    assert len(dataset.prediction_to_image.values()) == len(dataset.get_predictions())
+    # assert sum(map(len, dataset.category_to_images.values())) == len(dataset.get_images())
+    assert len(dataset.category_name_to_category) == len(dataset.get_categories())
+    assert sum(map(len, dataset.category_to_annotations.values())) == len(dataset.get_annotations())
+    assert sum(map(len, dataset.category_to_predictions.values())) == len(dataset.get_predictions())
 
 
 def _clone(dataset_name, root_dir):
     Dataset.clone(
         src_name=dataset_name,
         name="clone_" + dataset_name,
         src_root_dir=root_dir,
@@ -257,15 +272,15 @@
     assert len(dataset.get_images(labeled=False)) == unlabeled_image_num
 
 
 def _total_dummy(
     dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
 ):
     _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
 def test_dummy(tmpdir):
     for task in [
@@ -316,15 +331,15 @@
     assert len(val_ids) == 20
     assert len(test_ids) == 20
     assert len(dataset.get_images()) == 100
 
 
 def _total_coco(dataset_name, task: TaskType, coco_path, root_dir):
     _from_coco(dataset_name, task, coco_path, root_dir)
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
 @pytest.mark.parametrize(
     "task", [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]
@@ -346,15 +361,15 @@
     )
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 60
     assert len(val_ids) == 20
     assert len(test_ids) == 20
     assert len(dataset.get_images()) == 100
 
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, TaskType.CLASSIFICATION, root_dir)
 
 
 def test_yolo_object_detection(yolo_object_detection_path: Path, tmpdir: Path):
     dataset_name = "yolo_object_detection"
@@ -369,15 +384,15 @@
     )
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 60
     assert len(val_ids) == 20
     assert len(test_ids) == 20
     assert len(dataset.get_images()) == 100
 
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, TaskType.OBJECT_DETECTION, root_dir)
 
 
 def test_yolo_instance_segmentation(yolo_instance_segmentation_path: Path, tmpdir: Path):
     dataset_name = "yolo_instance_segmentation"
@@ -392,15 +407,15 @@
     )
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 60
     assert len(val_ids) == 20
     assert len(test_ids) == 20
     assert len(dataset.get_images()) == 100
 
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, TaskType.INSTANCE_SEGMENTATION, root_dir)
 
 
 # test autocare_dlt
 def _from_autocare_dlt(dataset_name, task: TaskType, coco_path, root_dir):
@@ -412,15 +427,15 @@
         root_dir=root_dir,
     )
     assert dataset.dataset_info_file.exists()
 
 
 def _total_autocare_dlt(dataset_name, task: TaskType, coco_path, root_dir):
     _from_autocare_dlt(dataset_name, task, coco_path, root_dir)
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
 @pytest.mark.parametrize(
     "task", [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.TEXT_RECOGNITION]
@@ -442,15 +457,15 @@
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 80
     assert len(dataset.get_images()) == 100
 
 
 def _total_transformers(dataset_name, task: TaskType, transformers_path, root_dir):
     _from_transformers(dataset_name, task, transformers_path, root_dir)
-    _load(dataset_name, root_dir)
+    _index(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
 def test_transformers(transformers_detection_path, transformers_classification_path, tmpdir):
     _total_transformers(
```

### Comparing `waffle_hub-0.2.7/tests/test_ddp.py` & `waffle_hub-0.2.8/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/tests/test_hub.py` & `waffle_hub-0.2.8/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/__init__.py` & `waffle_hub-0.2.8/waffle_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 import enum
 from collections import OrderedDict
 
 BACKEND_MAP = OrderedDict(
     {
         "ultralytics": {
```

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/adapter/autocare_dlt.py` & `waffle_hub-0.2.8/waffle_hub/dataset/adapter/autocare_dlt.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.8/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/adapter/transformers.py` & `waffle_hub-0.2.8/waffle_hub/dataset/adapter/transformers.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.8/waffle_hub/dataset/adapter/yolo.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/cli.py` & `waffle_hub-0.2.8/waffle_hub/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.8/waffle_hub/dataset/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import logging
 import os
 import random
 import shutil
 import warnings
-from collections import Counter, defaultdict
+from collections import Counter, OrderedDict, defaultdict
 from functools import cached_property
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Union
 
 import PIL.Image
 import tqdm
@@ -297,68 +297,101 @@
     def test_set_file(self) -> Path:
         return self.set_dir / Dataset.TEST_SET_FILE_NAME
 
     @cached_property
     def unlabeled_set_file(self) -> Path:
         return self.set_dir / Dataset.UNLABELED_SET_FILE_NAME
 
-    def get_category_names(self) -> list[str]:
-        return [category.name for category in self.categories]
+    # dataset indexes
+    @property
+    def image_dict(self) -> dict[int, Image]:
+        if not hasattr(self, "__image_dict"):
+            self.create_index()
+        return self.__image_dict
 
-    def get_image_to_annotations(self) -> dict[int, list[Annotation]]:
-        image_to_annotations = defaultdict(list)
-        for annotation in self.get_annotations():
-            image_to_annotations[annotation.image_id].append(annotation)
-        return dict(image_to_annotations)
+    @property
+    def unlabeled_image_dict(self) -> dict[int, Image]:
+        if not hasattr(self, "__unlabeled_image_dict"):
+            self.create_index()
+        return self.__unlabeled_image_dict
 
-    def get_category_to_annotations(self) -> dict[int, list[Annotation]]:
-        category_to_annotations = defaultdict(list)
-        category_name_to_id = {
-            category.name: category.category_id for category in self.get_categories()
-        }
-        for annotation in self.get_annotations():
-            if self.task == TaskType.TEXT_RECOGNITION:
-                texts = annotation.caption
-                characters = set(texts)
-                for char in characters:
-                    category_to_annotations[category_name_to_id[char]].append(annotation)
-            else:
-                category_to_annotations[annotation.category_id].append(annotation)
-        return dict(category_to_annotations)
+    @property
+    def annotation_dict(self) -> dict[int, Annotation]:
+        if not hasattr(self, "__annotation_dict"):
+            self.create_index()
+        return self.__annotation_dict
 
-    def get_category_to_images(self) -> dict[int, list[Image]]:
-        category_to_images = category_to_images = {c.category_id: [] for c in self.get_categories()}
-        category_name_to_id = {
-            category.name: category.category_id for category in self.get_categories()
-        }
-        for image_id, annotations in self.get_image_to_annotations().items():
-            image = self.get_images([image_id])[0]
-            if self.task == TaskType.TEXT_RECOGNITION:
-                texts = map(lambda a: a.caption, annotations)
-                character_count = Counter("".join(texts))
-                for k in character_count:
-                    category_to_images[category_name_to_id[k]].append(image)
-            else:
-                category_ids = map(lambda a: a.category_id, annotations)
-                category_count = Counter(category_ids)
-                category_to_images[category_count.most_common(1)[0][0]].append(image)
-        return dict(category_to_images)
+    @property
+    def prediction_dict(self) -> dict[int, Annotation]:
+        if not hasattr(self, "__prediction_dict"):
+            self.create_index()
+        return self.__prediction_dict
 
-    def get_num_images_per_category(self) -> dict[int, int]:
-        self.num_images_per_category = {
-            category_id: len(images) for category_id, images in self.get_category_to_images().items()
-        }
-        return self.num_images_per_category
+    @property
+    def category_dict(self) -> dict[int, Category]:
+        if not hasattr(self, "__category_dict"):
+            self.create_index()
+        return self.__category_dict
 
-    def get_num_annotations_per_category(self) -> dict[int, int]:
-        num_annotations_per_category = {
-            category_id: len(annotations)
-            for category_id, annotations in self.get_category_to_annotations().items()
-        }
-        return num_annotations_per_category
+    @property
+    def image_to_annotations(self) -> dict[int, list[Annotation]]:
+        if not hasattr(self, "__image_to_annotations"):
+            self.create_index()
+        return self.__image_to_annotations
+
+    @property
+    def image_to_predictions(self) -> dict[int, list[Annotation]]:
+        if not hasattr(self, "__image_to_predictions"):
+            self.create_index()
+        return self.__image_to_predictions
+
+    @property
+    def annotation_to_image(self) -> dict[int, Image]:
+        if not hasattr(self, "__annotation_to_image"):
+            self.create_index()
+        return self.__annotation_to_image
+
+    @property
+    def prediction_to_image(self) -> dict[int, Image]:
+        if not hasattr(self, "__prediction_to_image"):
+            self.create_index()
+        return self.__prediction_to_image
+
+    @property
+    def category_to_images(self) -> dict[int, list[Image]]:
+        if not hasattr(self, "__category_to_images"):
+            self.create_index()
+        return self.__category_to_images
+
+    @property
+    def category_to_unique_images(self) -> dict[int, list[Image]]:
+        if not hasattr(self, "__category_to_unique_images"):
+            self.create_index()
+        return self.__category_to_unique_images
+
+    @property
+    def category_name_to_category(self) -> dict[str, Category]:
+        if not hasattr(self, "__category_name_to_category"):
+            self.create_index()
+        return self.__category_name_to_category
+
+    @property
+    def category_to_annotations(self) -> dict[int, list[Annotation]]:
+        if not hasattr(self, "__category_to_annotations"):
+            self.create_index()
+        return self.__category_to_annotations
+
+    @property
+    def category_to_predictions(self) -> dict[int, list[Annotation]]:
+        if not hasattr(self, "__category_to_predictions"):
+            self.create_index()
+        return self.__category_to_predictions
+
+    def get_category_names(self) -> list[str]:
+        return [category.name for category in self.categories]
 
     # factories
     @classmethod
     def new(
         cls,
         name: str,
         task: str,
@@ -440,14 +473,15 @@
         try:
             src_ds = Dataset.load(src_name, src_root_dir)
 
             ds = Dataset.new(name=name, task=src_ds.task, root_dir=root_dir)
             io.copy_files_to_directory(src_ds.dataset_dir, ds.dataset_dir, create_directory=True)
             ds.save_dataset_info()
 
+            ds.create_index()
             return ds
         except Exception as e:
             if (root_dir / name).exists():
                 io.remove_directory(root_dir / name)
             raise e
 
     @classmethod
@@ -577,14 +611,15 @@
                     )
                     PIL.Image.new("RGB", (100, 100)).save(ds.raw_image_dir / file_name)
 
         except Exception as e:
             ds.delete()
             raise e
 
+        ds.create_index()
         return ds
 
     @classmethod
     def load(cls, name: str, root_dir: str = None) -> "Dataset":
         """
         Load Dataset.
         This method loads an existing dataset.
@@ -605,15 +640,18 @@
             Dataset: Dataset Class
         """
         root_dir = Dataset.parse_root_dir(root_dir)
         dataset_info_file = root_dir / name / Dataset.DATASET_INFO_FILE_NAME
         if not dataset_info_file.exists():
             raise FileNotFoundError(f"{dataset_info_file} has not been created.")
         dataset_info = DatasetInfo.load(dataset_info_file)
-        return cls(**dataset_info.to_dict(), root_dir=root_dir)
+
+        ds = cls(**dataset_info.to_dict(), root_dir=root_dir)
+        ds.create_index()
+        return ds
 
     @classmethod
     def merge(
         cls,
         name: str,
         root_dir: str,
         src_names: list[str],
@@ -673,15 +711,15 @@
                         new_category_id = len(categoryname2id) + 1
                         categoryname2id[category.name] = new_category_id
 
                         new_category = copy.deepcopy(category)
                         new_category.category_id = new_category_id
                         merged_ds.add_categories([new_category])
 
-                for image_id, annotations in src_ds.get_image_to_annotations().items():
+                for image_id, annotations in src_ds.image_to_annotations.items():
                     image = src_ds.get_images([image_id])[0]
 
                     # merge - images
                     is_new_image = False
                     if image.file_name not in filename2id:
                         is_new_image = True
 
@@ -717,15 +755,17 @@
                             merged_ds.add_annotations([new_annotation])
 
         except Exception as e:
             if merged_ds.dataset_dir.exists():
                 io.remove_directory(merged_ds.dataset_dir)
             raise e
 
-        return Dataset.load(name, root_dir)
+        ds = Dataset.load(name, root_dir)
+        ds.create_index()
+        return ds
 
     @classmethod
     def from_coco(
         cls,
         name: str,
         task: str,
         coco_file: Union[str, list[str]],
@@ -793,14 +833,15 @@
             # TODO: add unlabeled set
             io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         except Exception as e:
             ds.delete()
             raise e
 
+        ds.create_index()
         return ds
 
     @classmethod
     def from_autocare_dlt(
         cls,
         name: str,
         task: str,
@@ -864,14 +905,15 @@
             # TODO: add unlabeled set
             io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         except Exception as e:
             ds.delete()
             raise e
 
+        ds.create_index()
         return ds
 
     @classmethod
     def from_yolo(
         cls,
         name: str,
         task: str,
@@ -902,14 +944,15 @@
         try:
             import_yolo(ds, yolo_root_dir, yaml_path)
 
         except Exception as e:
             ds.delete()
             raise e
 
+        ds.create_index()
         return ds
 
     @classmethod
     def from_transformers(
         cls,
         name: str,
         task: str,
@@ -944,14 +987,15 @@
             # TODO: add unlabeled set
             io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         except Exception as e:
             ds.delete()
             raise e
 
+        ds.create_index()
         return ds
 
     @classmethod
     def sample(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
         """
         Import sample Dataset.
 
@@ -988,14 +1032,15 @@
                 coco_root_dir=str(temp_dir / "images"),
             )
         except Exception as e:
             raise e
         finally:
             shutil.rmtree(temp_dir)
 
+        ds.create_index()
         return ds
 
     @classmethod
     def get_dataset_list(cls, root_dir: str = None) -> list[str]:
         """
         Get dataset name list in root_dir.
 
@@ -1178,32 +1223,153 @@
             return [
                 Annotation.from_json(f, self.task)
                 for f in self.prediction_dir.glob(f"{image_id}/*.json")
             ]
         else:
             return [Annotation.from_json(f, self.task) for f in self.prediction_dir.glob("*/*.json")]
 
+    def get_num_images_per_category(self) -> dict[int, int]:
+        self.num_images_per_category = {
+            category_id: len(images) for category_id, images in self.category_to_images.items()
+        }
+        return self.num_images_per_category
+
+    def get_num_annotations_per_category(self) -> dict[int, int]:
+        num_annotations_per_category = {
+            category_id: len(annotations)
+            for category_id, annotations in self.category_to_annotations.items()
+        }
+        return num_annotations_per_category
+
+    def create_index(self):
+        """Create index for faster search."""
+        self.__image_dict = OrderedDict()
+        self.__unlabeled_image_dict = OrderedDict()
+        self.__annotation_dict = OrderedDict()
+        self.__prediction_dict = OrderedDict()
+        self.__category_dict = OrderedDict()
+        self.__image_to_annotations = OrderedDict()
+        self.__image_to_predictions = OrderedDict()
+        self.__annotation_to_image = OrderedDict()
+        self.__prediction_to_image = OrderedDict()
+        self.__category_to_images = OrderedDict()
+        self.__category_to_unique_images = OrderedDict()
+        self.__category_name_to_category = OrderedDict()
+        self.__category_to_annotations = OrderedDict()
+        self.__category_to_predictions = OrderedDict()
+
+        logger.info("Creating index for faster search")
+
+        for image in self.get_images():
+            self.__image_dict[image.image_id] = image  # image_id: image
+            self.__image_to_annotations[image.image_id] = []
+            self.__image_to_predictions[image.image_id] = []
+
+        for annotation in self.get_annotations():
+            self.__annotation_dict[
+                annotation.annotation_id
+            ] = annotation  # annotation_id: annotation
+            self.__image_to_annotations[annotation.image_id].append(
+                annotation
+            )  # image_id: [annotations]
+            self.__annotation_to_image[annotation.annotation_id] = self.__image_dict[
+                annotation.image_id
+            ]  # annotation_id: image
+
+        for prediction in self.get_predictions():
+            self.__prediction_dict[
+                prediction.annotation_id
+            ] = prediction  # annotation_id: prediction
+            self.__image_to_predictions[prediction.image_id].append(
+                prediction
+            )  # image_id: [predictions]
+            self.__prediction_to_image[prediction.annotation_id] = self.__image_dict[
+                prediction.image_id
+            ]  # prediction_id: image
+
+        for category in self.get_categories():
+            self.__category_dict[category.category_id] = category  # category_id: category
+            self.__category_name_to_category[category.name] = category  # category_name: category
+            self.__category_to_unique_images[category.category_id] = []  # category_id: image
+            self.__category_to_images[category.category_id] = set()
+            self.__category_to_annotations[category.category_id] = []
+
+        for annotation in self.__annotation_dict.values():
+            if self.task == TaskType.TEXT_RECOGNITION:
+                chars = set(annotation.caption)
+                for char in chars:
+                    category_id = self.__category_name_to_category[char].category_id
+                    self.__category_to_annotations[category_id].append(annotation)
+                    self.__category_to_images[category_id].add(
+                        self.__annotation_to_image[annotation.annotation_id]
+                    )
+            else:
+                self.__category_to_annotations[annotation.category_id].append(
+                    annotation
+                )  # category_id: [annotations]
+                self.__category_to_images[annotation.category_id].add(
+                    self.__annotation_to_image[annotation.annotation_id]
+                )  # category_id: {images}
+
+        for image_id, annotations in self.__image_to_annotations.items():
+            if self.task == TaskType.TEXT_RECOGNITION:
+                most_common_category = Counter(
+                    sum([list(annotation.caption) for annotation in annotations], [])
+                ).most_common(1)[0][0]
+                most_common_category_id = self.__category_name_to_category[
+                    most_common_category
+                ].category_id
+                self.__category_to_unique_images[most_common_category_id].append(
+                    self.__image_dict[image_id]
+                )
+            else:
+                most_common_category_id = Counter(
+                    [annotation.category_id for annotation in annotations]
+                ).most_common(1)[0][0]
+                self.__category_to_unique_images[most_common_category_id].append(
+                    self.__image_dict[image_id]
+                )
+
+        for category_id, images in self.__category_to_images.items():
+            self.__category_to_images[category_id] = list(images)
+
+        for prediction in self.__prediction_dict.values():
+            self.__category_to_predictions[prediction.category_id].append(
+                prediction
+            )  # category_id: [predictions]
+
+        for image in self.get_images(labeled=False):
+            self.__unlabeled_image_dict[image.image_id] = image  # unlabeled_image_id: image
+
+        logger.info("Creating index done")
+
     # add
-    def add_images(self, images: list[Image]):
+    def add_images(self, images: Union[Image, list[Image]]):
         """Add "Image"s to dataset.
 
         Args:
-            images (list[Image]): list of "Image"s
+            images (Union[Image, list[Image]]): list of "Image"s
         """
+        if not isinstance(images, list):
+            images = [images]
+
         for item in images:
             item_id = item.image_id
             item_path = self.image_dir / f"{item_id}.json"
             io.save_json(item.to_dict(), item_path)
 
-    def add_categories(self, categories: list[Category]):
+    def add_categories(self, categories: Union[Category, list[Category]]):
         """Add "Category"s to dataset.
 
         Args:
-            categories (list[Category]): list of "Category"s
+            categories (Union[Category, list[Category]]): list of "Category"s
         """
+        if not isinstance(categories, list):
+            categories = [categories]
+
         category_names_list = [category.name for category in categories]
         category_names = set(category_names_list)
         if (
             len(category_names) != len(category_names_list)
             or set(self.get_category_names()) & category_names
         ):
             raise ValueError("Category names should be unique")
@@ -1211,36 +1377,47 @@
         for item in categories:
             item_id = item.category_id
             item_path = self.category_dir / f"{item_id}.json"
             io.save_json(item.to_dict(), item_path)
 
         self.save_dataset_info()
 
-    def add_annotations(self, annotations: list[Annotation]):
+    def add_annotations(self, annotations: Union[Annotation, list[Annotation]]):
         """Add "Annotation"s to dataset.
 
         Args:
-            annotations (list[Annotation]): list of "Annotation"s
+            annotations (Union[Annotation, list[Annotation]]): list of "Annotation"s
         """
+        if not isinstance(annotations, list):
+            annotations = [annotations]
+
         categories = self.get_category_names()
         for item in annotations:
             if self.task == TaskType.TEXT_RECOGNITION:
                 for char in item.caption:
                     if char not in categories:
                         raise ValueError(f"Category '{char}' is not in dataset")
             item_path = self.annotation_dir / f"{item.image_id}" / f"{item.annotation_id}.json"
             io.save_json(item.to_dict(), item_path, create_directory=True)
 
-    def add_predictions(self, predictions: list[Annotation]):
+    def add_predictions(self, predictions: Union[Annotation, list[Annotation]]):
         """Add "Annotation"s to dataset.
 
         Args:
-            annotations (list[Annotation]): list of "Annotation"s
+            annotations (Union[Annotation, list[Annotation]]): list of "Annotation"s
         """
+        if not isinstance(predictions, list):
+            predictions = [predictions]
+
+        categories = self.get_category_names()
         for item in predictions:
+            if self.task == TaskType.TEXT_RECOGNITION:
+                for char in item.caption:
+                    if char not in categories:
+                        raise ValueError(f"Category '{char}' is not in dataset")
             item_path = self.prediction_dir / f"{item.image_id}" / f"{item.annotation_id}.json"
             io.save_json(item.to_dict(), item_path, create_directory=True)
 
     # functions
     def split(
         self,
         train_ratio: float,
@@ -1289,15 +1466,15 @@
         if method == SplitMethod.RANDOM:
             random.seed(seed)
 
             train_ids = []
             val_ids = []
             test_ids = []
 
-            for category_id, images in self.get_category_to_images().items():
+            for category_id, images in self.__category_to_unique_images.items():
                 image_num = len(images)
                 image_ids = list(map(lambda x: x.image_id, images))
                 random.shuffle(image_ids)
 
                 # flatten images to one list [cat]
                 train_num = max(int(image_num * train_ratio), 1)
                 val_num = max(int(image_num * val_ratio), 1)
```

### Comparing `waffle_hub-0.2.7/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.8/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.8/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/cli.py` & `waffle_hub-0.2.8/waffle_hub/hub/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/hub.py` & `waffle_hub-0.2.8/waffle_hub/hub/hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.8/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.8/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/configs.py` & `waffle_hub-0.2.8/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/data.py` & `waffle_hub-0.2.8/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.8/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.8/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.8/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.8/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/schema/result.py` & `waffle_hub-0.2.8/waffle_hub/schema/result.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/base_cli.py` & `waffle_hub-0.2.8/waffle_hub/utils/base_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/callback.py` & `waffle_hub-0.2.8/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.8/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/data.py` & `waffle_hub-0.2.8/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/draw.py` & `waffle_hub-0.2.8/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.8/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/metric_logger.py` & `waffle_hub-0.2.8/waffle_hub/utils/metric_logger.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub/utils/process.py` & `waffle_hub-0.2.8/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.7/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.8/waffle_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.7
+Version: 0.2.8
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.7 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.8 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.7/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.8/waffle_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

