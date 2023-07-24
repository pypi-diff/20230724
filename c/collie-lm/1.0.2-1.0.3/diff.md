# Comparing `tmp/collie-lm-1.0.2.tar.gz` & `tmp/collie-lm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collie-lm-1.0.2.tar", last modified: Tue Jul 18 09:38:10 2023, max compression
+gzip compressed data, was "collie-lm-1.0.3.tar", last modified: Mon Jul 24 12:10:31 2023, max compression
```

## Comparing `collie-lm-1.0.2.tar` & `collie-lm-1.0.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.936818 collie-lm-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 09:37:55.000000 collie-lm-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 09:38:10.936818 collie-lm-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-18 09:37:55.000000 collie-lm-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.924818 collie-lm-1.0.2/collie/
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.924818 collie-lm-1.0.2/collie/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/callback_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/has_monitor_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/load_best_model_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/topk_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/callbacks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.924818 collie-lm-1.0.2/collie/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/controller/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/controller/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    40946 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/controller/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/controller/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.924818 collie-lm-1.0.2/collie/data/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/data/batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.924818 collie-lm-1.0.2/collie/driver/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/driver/io/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/driver/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/driver/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/driver/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/driver/io/petrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/log/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/log/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/log/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/log/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/log/print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/classify_f1_pre_rec_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/ppl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/metrics/rouge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/chatglm/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/chatglm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35785 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/chatglm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/chatglm2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/chatglm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/chatglm2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/internlm/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/internlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31269 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/internlm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/llama/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36136 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/llama/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/moss/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/moss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36202 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/moss/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.928818 collie-lm-1.0.2/collie/models/moss_moon/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/moss_moon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25535 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/moss_moon/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/models/moss_moon/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28180 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.932818 collie-lm-1.0.2/collie/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/optim/lomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/optim/sophiag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.932818 collie-lm-1.0.2/collie/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    24908 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/metric_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/peft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46874 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/pipeline_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/seq_len_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.932818 collie-lm-1.0.2/collie_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.932818 collie-lm-1.0.2/collie_cli/bullet/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/charDef.py
--rw-r--r--   0 runner    (1001) docker     (123)    25857 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/keyhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/bullet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/collie_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-18 09:37:55.000000 collie-lm-1.0.2/collie_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:38:10.936818 collie-lm-1.0.2/collie_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 09:38:10.000000 collie-lm-1.0.2/collie_lm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:38:10.936818 collie-lm-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-18 09:37:55.000000 collie-lm-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.739993 collie-lm-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 12:10:19.000000 collie-lm-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 12:10:31.735993 collie-lm-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-07-24 12:10:19.000000 collie-lm-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/callback_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/has_monitor_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/load_best_model_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/topk_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/callbacks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/controller/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/controller/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40946 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/controller/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/controller/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/data/batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/driver/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/driver/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/driver/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/driver/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/driver/io/petrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/log/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/log/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/log/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/log/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/log/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/classify_f1_pre_rec_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/ppl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/metrics/rouge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35186 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.731993 collie-lm-1.0.3/collie/models/chatglm/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/chatglm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35564 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/chatglm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/models/chatglm2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/chatglm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52616 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/chatglm2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/models/internlm/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/internlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31024 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/internlm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36705 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/llama/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/models/moss/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35915 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/moss/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/models/moss_moon/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/moss_moon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25535 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/moss_moon/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/models/moss_moon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28504 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/optim/lomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/optim/sophiag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24908 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/metric_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/peft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46874 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/pipeline_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/seq_len_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie_cli/bullet/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/charDef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25857 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/keyhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/bullet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/collie_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-24 12:10:19.000000 collie-lm-1.0.3/collie_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:31.735993 collie-lm-1.0.3/collie_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:10:31.000000 collie-lm-1.0.3/collie_lm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:10:31.739993 collie-lm-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 12:10:20.000000 collie-lm-1.0.3/setup.py
```

### Comparing `collie-lm-1.0.2/LICENSE` & `collie-lm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/README.md` & `collie-lm-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,21 @@
     - [internlm-chat-7b](https://huggingface.co/internlm/internlm-chat-7b)
     - [internlm-chat-7b-8k](https://huggingface.co/internlm/internlm-chat-7b-8k)
 - [LLaMA](https://github.com/facebookresearch/llama)
     - [llama-7b-hf](https://huggingface.co/decapoda-research/llama-7b-hf)
     - [llama-13b-hf](https://huggingface.co/decapoda-research/llama-13b-hf)
     - [llama-30b-hf](https://huggingface.co/decapoda-research/llama-30b-hf)
     - [llama-65b-hf](https://huggingface.co/decapoda-research/llama-65b-hf)
+- [LLaMA-2](https://github.com/facebookresearch/llama)
+    - [Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf)
+    - [Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf)
+    - [Llama-2-70b-hf](https://huggingface.co/meta-llama/Llama-2-70b-hf)
+    - [Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf)
+    - [Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf)
+    - [Llama-2-70b-chat-hf](https://huggingface.co/meta-llama/Llama-2-70b-chat-hf)
 - [OpenLLaMA](https://github.com/openlm-research/open_llama)
     - [open_llama_3b](https://huggingface.co/openlm-research/open_llama_3b)
     - [open_llama_7b](https://huggingface.co/openlm-research/open_llama_7b)
     - [open_llama_13b](https://huggingface.co/openlm-research/open_llama_13b)
     - [open_llama_7b_v2](https://huggingface.co/openlm-research/open_llama_7b_v2)
 - [ChatGLM](https://github.com/THUDM/ChatGLM-6B)
     - [chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
```

#### html2text {}

```diff
@@ -44,25 +44,32 @@
 (https://github.com/InternLM/InternLM) - [internlm-7b](https://huggingface.co/
 internlm/internlm-7b) - [internlm-chat-7b](https://huggingface.co/internlm/
 internlm-chat-7b) - [internlm-chat-7b-8k](https://huggingface.co/internlm/
 internlm-chat-7b-8k) - [LLaMA](https://github.com/facebookresearch/llama) -
 [llama-7b-hf](https://huggingface.co/decapoda-research/llama-7b-hf) - [llama-
 13b-hf](https://huggingface.co/decapoda-research/llama-13b-hf) - [llama-30b-hf]
 (https://huggingface.co/decapoda-research/llama-30b-hf) - [llama-65b-hf](https:
-//huggingface.co/decapoda-research/llama-65b-hf) - [OpenLLaMA](https://
-github.com/openlm-research/open_llama) - [open_llama_3b](https://
-huggingface.co/openlm-research/open_llama_3b) - [open_llama_7b](https://
-huggingface.co/openlm-research/open_llama_7b) - [open_llama_13b](https://
-huggingface.co/openlm-research/open_llama_13b) - [open_llama_7b_v2](https://
-huggingface.co/openlm-research/open_llama_7b_v2) - [ChatGLM](https://
-github.com/THUDM/ChatGLM-6B) - [chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) - [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B) - [chatglm2-6b]
-(https://huggingface.co/THUDM/chatglm2-6b) ## è¯æµ ### ååé | | 7B | 13B
-| 30B | 65B | | ---------- | ---- | ---- | ---- | ---- | | Finetune | 2 | 3 | 6
-| 16 | | LoRA | 1 | 1 | 1 | 2 | | LOMO | 1 | 1 | 1 | 2 |
+//huggingface.co/decapoda-research/llama-65b-hf) - [LLaMA-2](https://
+github.com/facebookresearch/llama) - [Llama-2-7b-hf](https://huggingface.co/
+meta-llama/Llama-2-7b-hf) - [Llama-2-13b-hf](https://huggingface.co/meta-llama/
+Llama-2-13b-hf) - [Llama-2-70b-hf](https://huggingface.co/meta-llama/Llama-2-
+70b-hf) - [Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-
+chat-hf) - [Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-
+chat-hf) - [Llama-2-70b-chat-hf](https://huggingface.co/meta-llama/Llama-2-70b-
+chat-hf) - [OpenLLaMA](https://github.com/openlm-research/open_llama) -
+[open_llama_3b](https://huggingface.co/openlm-research/open_llama_3b) -
+[open_llama_7b](https://huggingface.co/openlm-research/open_llama_7b) -
+[open_llama_13b](https://huggingface.co/openlm-research/open_llama_13b) -
+[open_llama_7b_v2](https://huggingface.co/openlm-research/open_llama_7b_v2) -
+[ChatGLM](https://github.com/THUDM/ChatGLM-6B) - [chatglm-6b](https://
+huggingface.co/THUDM/chatglm-6b) - [ChatGLM2](https://github.com/THUDM/
+ChatGLM2-6B) - [chatglm2-6b](https://huggingface.co/THUDM/chatglm2-6b) ##
+è¯æµ ### ååé | | 7B | 13B | 30B | 65B | | ---------- | ---- | ---- | --
+-- | ---- | | Finetune | 2 | 3 | 6 | 16 | | LoRA | 1 | 1 | 1 | 2 | | LOMO | 1 |
+1 | 1 | 2 |
 æ³¨ï¼å¨ä½¿ç¨Adamä¼åå¨çæåµä¸ï¼åä¸ªæ¨¡åéè¦çæå°çGPUï¼A100ï¼æ°é
 ## å®è£ ```bash pip install git+https://github.com/OpenLMLab/collie.git ```
 ## Dockerå®è£ ## ä½¿ç¨ ### å¿«éå¼å§
 ä¸é¢å°æä¾ä¸ä¸ªä½¿ç¨CoLLiEè®­ç»Mossçæ ·ä¾ï¼åæ¶ä½¿ç¨LOMOä¼åå¨ï¼å¹¶ä¸å¼å¯ZeRO3æ¥éä½æ¾å­æ¶èã
 é£ä¹ï¼è¯·æç§ä¸é¢çæ­¥éª¤å¼å¯ä½ çå¤§æ¨¡åè®­ç»ä¹æå§~ [docs/
 assets/images/mario-running.gif] #### ç¬¬ä¸æ­¥ï¼å¯¼å¥å¿è¦çå ```python
 from transformers import AutoTokenizer from collie.config import CollieConfig
```

### Comparing `collie-lm-1.0.2/collie/__init__.py` & `collie-lm-1.0.3/collie/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     ColumnParallelLinearWithoutBias, LinearWithHiddenStates, \
     ColumnParallelLMHead, GPTLMLoss
 from .utils import progress, setup_distribution, set_seed, env, \
     setup_ds_engine, zero3_load_state_dict, is_zero3_enabled, \
     broadcast_tensor, find_tensors, BaseProvider, GradioProvider, \
     _GenerationStreamer, BaseMonitor, StepTimeMonitor, TGSMonitor, \
     MemoryMonitor, LossMonitor, EvalMonitor, LRMonitor, dict_as_params, \
-        DashProvider, is_static_method, \
-            auto_param_call, NetworkIOMonitor, DiskIOMonitor, \
-                CPUMemoryMonitor, ColliePadder, get_keys_to_not_convert
+    DashProvider, is_static_method, auto_param_call, NetworkIOMonitor, \
+    DiskIOMonitor, CPUMemoryMonitor, ColliePadder, get_keys_to_not_convert, \
+    concat_tensor
 from .module import PipelineGenerationMixin, ColumnParallelLinear, \
     RowParallelLinearWithoutBias, LinearWithHiddenStates, \
     ColumnParallelLMHead, GPTLMLoss
 from .controller import Trainer, Evaluator, EvaluatorForPerplexity, \
     EvaluatorForClassfication, EvaluatorForGeneration, Server
 from .config import CollieConfig
 from .metrics import BaseMetric, DecodeMetric, AccuracyMetric, \
@@ -73,14 +73,15 @@
     'setup_distribution',
     'set_seed',
     'env',
     'setup_ds_engine',
     'zero3_load_state_dict',
     'is_zero3_enabled',
     'broadcast_tensor',
+    'concat_tensor',
     'find_tensors',
     'BaseProvider', 
     'GradioProvider', 
     'BaseMonitor',
     'StepTimeMonitor',
     'TGSMonitor',
     'MemoryMonitor',
```

### Comparing `collie-lm-1.0.2/collie/callbacks/callback.py` & `collie-lm-1.0.3/collie/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/callback_manager.py` & `collie-lm-1.0.3/collie/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/checkpoint_callback.py` & `collie-lm-1.0.3/collie/callbacks/checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/has_monitor_callback.py` & `collie-lm-1.0.3/collie/callbacks/has_monitor_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/load_best_model_callback.py` & `collie-lm-1.0.3/collie/callbacks/load_best_model_callback.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/topk_saver.py` & `collie-lm-1.0.3/collie/callbacks/topk_saver.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/callbacks/utils.py` & `collie-lm-1.0.3/collie/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/config.py` & `collie-lm-1.0.3/collie/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         值。在流水线并行中，该项代表流水线的 micro batch 的数目。
     :param eval_batch_size: 验证时的 batch 大小。在流水线中代表验证时一个 micro
         batch 的大小。
     :param checkpointing: 是否使用梯度检查点，该设置可以节省显存。
     :param use_flash: 是否使用 `FlashAttention <https://github.com/HazyResearch/flash-attention>`_ 。
         仅对部分模型有效。
     :param dropout: :class:`Dropout` 的概率。仅对部分模型有效。
-    :param initization_method: 初始化方法。必须是一个接收一个 ``torch.Tensor`` 
+    :param init_method: 初始化方法。必须是一个接收一个 ``torch.Tensor`` 
         并返回一个 ``torch.Tensor`` 的可调用对象。
     :param low_cpu_mem_usage: 是否在初始化模型时尝试减少 CPU 占用
     :param ds_config: **DeepSpeed** 的配置文件。可以是一个路径或字典。
     :param model_config: 模型设置。一般情况下无需手动设置，而是通过
         :meth:`from_pretrained` 获取，
     :param peft_config: Peft 的配置。
     :param quantization_config: 模型的量化配置
@@ -135,15 +135,15 @@
     )
     dropout: float = field(
         default=0.0,
         metadata={
             "help": "Dropout probability."
         }
     )
-    initization_method: Callable = field(
+    init_method: Callable = field(
         default_factory=lambda: torch.nn.init.uniform_,
         metadata={
             "help": "Initialization method. Possible values are 'none', 'normal', 'xavier_normal', "
             "'xavier_uniform', 'kaiming_normal', 'kaiming_uniform', 'orthogonal', 'sparse', "
             "'eye', 'dirac'. Default is 'none'."
         }
     )
```

### Comparing `collie-lm-1.0.2/collie/controller/evaluator.py` & `collie-lm-1.0.3/collie/controller/evaluator.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/controller/server.py` & `collie-lm-1.0.3/collie/controller/server.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/controller/trainer.py` & `collie-lm-1.0.3/collie/controller/trainer.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/controller/utils.py` & `collie-lm-1.0.3/collie/controller/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/data/batch_sampler.py` & `collie-lm-1.0.3/collie/data/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/data/dataloader.py` & `collie-lm-1.0.3/collie/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/data/dataset.py` & `collie-lm-1.0.3/collie/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,20 +194,19 @@
         return dataset
 
     def save_propressed(self, path: str, shard_size: int = 4):
         shard = io.BytesIO()
         shard_idx = 0
         meta = np.empty((0, 2), int)
         for i in self.indices:
-            labels = self[i][1]
             data = {
-                "tokens": labels["labels"]
+                "tokens": self[i]["input_ids"]
             }
             data.update(
-                {key: value for key, value in labels.items() if key != "labels"})
+                {key: value for key, value in self[i].items() if key != "input_ids"})
             bytes_data = json.dumps(data).encode() + "\n".encode()
             offset = shard.tell()
             length = len(data["tokens"])
             shard.write(bytes_data)
             meta = np.append(meta, np.array([[offset, length]]), axis=0)
             if shard.tell() > shard_size * 1024 * 1024 or i == len(self) - 1:
                 file = f"collie-dataset-shard-{shard_idx}.bin"
@@ -281,16 +280,23 @@
                     "output": ["类别1", "类别2", "类别3"],
                     "target": 0
                 },
                 ...
             ]
     """
     
-    def __init__(self, style: str="harness", *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, 
+                 dataset: Sequence[Dict],
+                 tokenizer: Optional[PreTrainedTokenizer] = None,
+                 add_special_tokens: bool = True,
+                 shuffle: bool = False,
+                 seed: int = 1024,
+                 max_length: int=-1, 
+                 style: str="harness"):
+        super().__init__(dataset=dataset, tokenizer=tokenizer, add_special_tokens=add_special_tokens, shuffle=shuffle, seed=seed, max_length=max_length)
         assert style.lower() in ("harness", "helm"), "Style can only be one of `harness` or `helm`"
         self.style = style.lower()
 
     def __getitem__(self, index) -> Tuple:
         if index > len(self):
             raise IndexError("Index out of range.")
         index = self.indices[index]
```

### Comparing `collie-lm-1.0.2/collie/driver/io/base.py` & `collie-lm-1.0.3/collie/driver/io/base.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/driver/io/file.py` & `collie-lm-1.0.3/collie/driver/io/file.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/driver/io/petrel.py` & `collie-lm-1.0.3/collie/driver/io/petrel.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/log/handler.py` & `collie-lm-1.0.3/collie/log/handler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/log/logger.py` & `collie-lm-1.0.3/collie/log/logger.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/log/print.py` & `collie-lm-1.0.3/collie/log/print.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/accuracy.py` & `collie-lm-1.0.3/collie/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/base.py` & `collie-lm-1.0.3/collie/metrics/base.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/bleu.py` & `collie-lm-1.0.3/collie/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/classify_f1_pre_rec_metric.py` & `collie-lm-1.0.3/collie/metrics/classify_f1_pre_rec_metric.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/decode.py` & `collie-lm-1.0.3/collie/metrics/decode.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/ppl.py` & `collie-lm-1.0.3/collie/metrics/ppl.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/metrics/rouge.py` & `collie-lm-1.0.3/collie/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/models/base.py` & `collie-lm-1.0.3/collie/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from transformers.generation.utils import GenerationConfig
 from transformers.utils import ContextManagers
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 from collie.module import PipelineModel, GPTLMLoss
 from collie.config import CollieConfig, load_config
 from collie.log import logger
 from collie.utils import setup_distribution, is_zero3_enabled, env, \
-    dict_as_params, get_keys_to_not_convert
+    dict_as_params, get_keys_to_not_convert, concat_tensor
 
 class CollieModelForCausalLM(nn.Module, GenerationMixin):
     """
     **CoLLiE** 的基础模型。如果要实现新的模型，必须继承该基类。
 
     ``CollieModelForCausalLM`` 统一了非流水线模型和流水线模型的接口，并且可以执行
     生成任务。
@@ -180,19 +180,19 @@
                         data_parallel_group=parallel_state.get_data_parallel_group(),
                         config_dict_or_path=config.ds_config  # config is necessary for bf16
                     ))
                 with ContextManagers(contexts):
                     if param.device == torch.device("meta"):
                         set_module_tensor_to_device(
                             module=model, tensor_name=name, device="cpu" if param.device == torch.device("meta") else param.device,
-                            value=config.initization_method(torch.empty((*param.data.size(),),dtype=config.model_config.torch_dtype)),
+                            value=config.init_method(torch.empty((*param.data.size(),),dtype=config.model_config.torch_dtype)),
                             dtype=config.model_config.torch_dtype
                         )
                     else:
-                        param.data = config.initization_method(torch.zeros_like(param.data)).to(config.model_config.torch_dtype).to(param.device)
+                        param.data = config.init_method(torch.zeros_like(param.data)).to(config.model_config.torch_dtype).to(param.device)
         if kwargs.get("get_peft", True) and config.peft_config.peft_type is not None:
             model = get_peft_model(model, config.peft_config)
             model.print_trainable_parameters()
         # set model dtype to deepspeed dtype under zero3, because the model is initialized with deepspeed.zero.Init()
         # if is_zero3_enabled(config):
         #     if 'fp16' in config.ds_config and config.ds_config['fp16']['enabled']:
         #         ds_dtype = torch.float16
@@ -519,41 +519,33 @@
                 start_pos_old = 0
                 end_pos_old = 0
                 start_pos_new = 0
                 end_pos_new = 0
             if is_zero3_enabled(self.collie_config):
                 with deepspeed.zero.GatheredParameters([new_embedding.weight, embedding.weight], modifier_rank=0):
                     if env.tp_size > 1 and isinstance(new_embedding, tensor_parallel.VocabParallelEmbedding):
-                        weights_list = [embedding.weight.clone() for _ in range(env.tp_size)]
-                        dist.all_gather(weights_list, embedding.weight, group=parallel_state.get_tensor_model_parallel_group())
-                        embedding.weight = nn.Parameter(torch.concat(weights_list, dim=0))
+                        weights_list = [embedding.weight.clone().cuda() for _ in range(env.tp_size)]
+                        dist.all_gather(weights_list, embedding.weight.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                        embedding.weight = nn.Parameter(concat_tensor(weights_list, dim=0))
                     if env.dp_rank == 0:
                         new_embedding.weight.data[start_pos_new:end_pos_new, :] \
                             = embedding.weight.data[start_pos_old:end_pos_old, :]
                         if end_pos_new < (new_num_tokens // env.tp_size):
-                            initization_method = self.collie_config.initization_method
-                            if self.collie_config.initization_method_params is not None:
-                                initization_method = initization_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :],
-                                                                        **self.collie_config.initization_method_params)
-                            else:
-                                initization_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :])
+                            init_method = self.collie_config.init_method
+                            init_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :])
             else:
                 if env.tp_size > 1 and isinstance(new_embedding, tensor_parallel.VocabParallelEmbedding):
-                    weights_list = [embedding.weight.clone() for _ in range(env.tp_size)]
-                    dist.all_gather(weights_list, embedding.weight, group=parallel_state.get_tensor_model_parallel_group())
-                    embedding.weight = nn.Parameter(torch.concat(weights_list, dim=0))
+                    weights_list = [embedding.weight.clone().cuda() for _ in range(env.tp_size)]
+                    dist.all_gather(weights_list, embedding.weight.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                    embedding.weight = nn.Parameter(concat_tensor(weights_list, dim=0))
                 new_embedding.weight.data[start_pos_new:end_pos_new, :] \
                     = embedding.weight.data[start_pos_old:end_pos_old, :]
                 if end_pos_new < (new_num_tokens // env.tp_size):
-                    initization_method = self.collie_config.initization_method
-                    if self.collie_config.initization_method_params is not None:
-                        initization_method = initization_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :],
-                                                                **self.collie_config.initization_method_params)
-                    else:
-                        initization_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :])
+                    init_method = self.collie_config.init_method
+                    init_method(new_embedding.weight[end_pos_new:new_num_tokens // env.tp_size, :])
             self.set_input_embedding(embedding_name, new_embedding)
         if lm_head is not None:
             if embedding is not None and id(lm_head.weight) == id(embedding.weight):
                 lm_head.weight = new_embedding.weight
                 return
             with deepspeed.zero.Init(data_parallel_group=parallel_state.get_data_parallel_group(), enabled=is_zero3_enabled(self.collie_config)):
                 if hasattr(lm_head, "dict_as_params_input_keys") and \
@@ -586,65 +578,51 @@
                 end_pos_old = 0
                 start_pos_new = 0
                 end_pos_new = 0
             if is_zero3_enabled(self.collie_config):
                 with deepspeed.zero.GatheredParameters([new_lm_head.weight, lm_head.weight] + \
                     [new_lm_head.bias, lm_head.bias] if lm_head.bias is not None else [], modifier_rank=0):
                     if env.tp_size > 1 and isinstance(new_lm_head, tensor_parallel.ColumnParallelLinear):
-                        weights_list = [lm_head.weight.clone() for _ in range(env.tp_size)]
-                        dist.all_gather(weights_list, lm_head.weight, group=parallel_state.get_tensor_model_parallel_group())
-                        lm_head.weight = nn.Parameter(torch.concat(weights_list, dim=0))
+                        weights_list = [lm_head.weight.clone().cuda() for _ in range(env.tp_size)]
+                        dist.all_gather(weights_list, lm_head.weight.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                        lm_head.weight = nn.Parameter(concat_tensor(weights_list, dim=0))
                         if lm_head.bias is not None:
-                            bias_list = [lm_head.bias.clone() for _ in range(env.tp_size)]
-                            dist.all_gather(bias_list, lm_head.bias, group=parallel_state.get_tensor_model_parallel_group())
-                            lm_head.bias = nn.Parameter(torch.concat(bias_list, dim=0))
+                            bias_list = [lm_head.bias.clone().cuda() for _ in range(env.tp_size)]
+                            dist.all_gather(bias_list, lm_head.bias.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                            lm_head.bias = nn.Parameter(concat_tensor(bias_list, dim=0))
                     if env.dp_rank == 0:
                         new_lm_head.weight.data[start_pos_new:end_pos_new, :] \
                             = lm_head.weight.data[start_pos_old:end_pos_old, :]
                         if lm_head.bias is not None:
                             new_lm_head.bias.data[start_pos_new:end_pos_new] \
                                 = lm_head.bias.data[start_pos_old:end_pos_old]
                         if end_pos_new < (new_num_tokens // env.tp_size):
-                            initization_method = self.collie_config.initization_method
-                            if self.collie_config.initization_method_params is not None:
-                                initization_method = initization_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :],
-                                                                        **self.collie_config.initization_method_params)
-                                if lm_head.bias is not None:
-                                    initization_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size],
-                                                        **self.collie_config.initization_method_params)
-                            else:
-                                initization_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :])
-                                if lm_head.bias is not None:
-                                    initization_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size])
+                            init_method = self.collie_config.init_method
+                            init_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :])
+                            if lm_head.bias is not None:
+                                init_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size])
             else:
                 if env.tp_size > 1 and isinstance(new_lm_head, tensor_parallel.ColumnParallelLinear):
-                    weights_list = [lm_head.weight.clone() for _ in range(env.tp_size)]
-                    dist.all_gather(weights_list, lm_head.weight, group=parallel_state.get_tensor_model_parallel_group())
-                    lm_head.weight = nn.Parameter(torch.concat(weights_list, dim=0))
+                    weights_list = [lm_head.weight.clone().cuda() for _ in range(env.tp_size)]
+                    dist.all_gather(weights_list, lm_head.weight.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                    lm_head.weight = nn.Parameter(concat_tensor(weights_list, dim=0))
                     if lm_head.bias is not None:
                         bias_list = [lm_head.bias.clone() for _ in range(env.tp_size)]
-                        dist.all_gather(bias_list, lm_head.bias, group=parallel_state.get_tensor_model_parallel_group())
-                        lm_head.bias = nn.Parameter(torch.concat(bias_list, dim=0))
+                        dist.all_gather(bias_list, lm_head.bias.cuda(), group=parallel_state.get_tensor_model_parallel_group())
+                        lm_head.bias = nn.Parameter(concat_tensor(bias_list, dim=0))
                 new_lm_head.weight.data[start_pos_new:end_pos_new, :] \
                     = lm_head.weight.data[start_pos_old:end_pos_old, :]
                 if lm_head.bias is not None:
                     new_lm_head.bias.data[start_pos_new:end_pos_new] \
                         = lm_head.bias.data[start_pos_old:end_pos_old]
                 if end_pos_new < (new_num_tokens // env.tp_size):
-                    initization_method = self.collie_config.initization_method
-                    if self.collie_config.initization_method_params is not None:
-                        initization_method = initization_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :],
-                                                                **self.collie_config.initization_method_params)
-                        if lm_head.bias is not None:
-                            initization_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size],
-                                                **self.collie_config.initization_method_params)
-                    else:
-                        initization_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :])
-                        if lm_head.bias is not None:
-                            initization_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size])
+                    init_method = self.collie_config.init_method
+                    init_method(new_lm_head.weight[end_pos_new:new_num_tokens // env.tp_size, :])
+                    if lm_head.bias is not None:
+                            init_method(new_lm_head.bias[end_pos_new:new_num_tokens // env.tp_size])
             self.set_lm_head(lm_head_name, new_lm_head)
 
 
     def get_input_embedding(self):
         for name, module in self.named_children():
             if isinstance(module, (nn.Embedding, tensor_parallel.VocabParallelEmbedding)):
                 return name, module
```

### Comparing `collie-lm-1.0.2/collie/models/chatglm/model.py` & `collie-lm-1.0.3/collie/models/chatglm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     FlashAttention = None
 
 from collie.log.logger import logger
 from collie.config import CollieConfig
 from collie.models.base import CollieModelForCausalLM
 from collie.driver.io import IODriver
 from collie.module import ColumnParallelLinearWithoutBias, RowParallelLinearWithoutBias, ColumnParallelLMHead
-from collie.utils import progress, env, dict_as_params
+from collie.utils import progress, env, dict_as_params, concat_tensor
 
 from typing import Any, Union, Optional
 from collections import OrderedDict
 from transformers.modeling_utils import dtype_byte_size
 from transformers.modeling_utils import PretrainedConfig
 from transformers.modeling_outputs import CausalLMOutputWithPast
 
@@ -296,15 +296,15 @@
         )
         self.lm_head = ColumnParallelLinearWithoutBias(
             self.config.hidden_size,
             self.config.vocab_size,
             bias=False
         )
         # GenerationMixin 需要的额外参数
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config.is_decoder=True
         self.main_input_name = "input_ids"
 
     def forward(self, input_ids: torch.Tensor, **kwargs):
         attention_mask = kwargs.get("attention_mask", None)
         past_key_values=self._get_past_key_values(self.layers)
         if past_key_values is not None and not self.training:
             input_ids = input_ids[:, -1:]
@@ -621,36 +621,33 @@
         with progress(rank_order, desc="Saving model", disable=int(os.environ.get("RANK", "0")) != 0) as pbar:
             for rank in pbar:
                 if env.dp_rank == 0 \
                     and (env.pp_rank == rank
                          or not process_exclusion):
                     if config.tp_size > 1:
                         for key in sorted(list(state_dict.keys())):
-                            device = state_dict[key].device
                             tensor_list = None
                             if env.tp_rank == 0:
                                 tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
                             dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
                             if env.tp_rank == 0:
                                 filte_list = ["query_key_value.weight", "query_key_value.bias", "dense_h_to_4h.weight", "dense_h_to_4h.bias", "word_embeddings.weight", "lm_head.weight"]
                                 need_split = any([key.endswith(filte) for filte in filte_list])
                                 if env.pp_size > 1:
                                     # embedding 层和 lm_head 都需要切
                                     need_split = need_split or int(key.split(".")[0]) == max(parts) - 1
                                     need_split = need_split or int(key.split(".")[0]) == min(parts)
                                 if need_split:
-                                    state_dict[key] = torch.cat(tensor_list, dim=0).detach().clone().to(device)
-                                    del tensor_list
+                                    state_dict[key] = concat_tensor(tensor_list, dim=0)
                                     if process_exclusion:
                                         # CPU 内存回收（速度很慢）
                                         gc.collect()
                                 elif key.endswith("dense.weight") \
                                     or key.endswith("dense_4h_to_4.weight.weight"):
-                                        state_dict[key] = torch.cat(tensor_list, dim=1).detach().clone().to(device)
-                                        del tensor_list
+                                        state_dict[key] = concat_tensor(tensor_list, dim=1)
                                         if process_exclusion:
                                             # CPU 内存回收（速度很慢）
                                             gc.collect()
                     if env.tp_rank == 0:
                         # Save gathered weights
                         if env.is_pipeline:
                             ckpt_name = f"pytorch_model-{env.pp_rank+1:05d}-of-{config.pp_size:05d}.bin"
```

### Comparing `collie-lm-1.0.2/collie/models/chatglm2/model.py` & `collie-lm-1.0.3/collie/models/chatglm2/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     FlashAttention = None
 
 from collie.log.logger import logger
 from collie.config import CollieConfig
 from collie.models.base import CollieModelForCausalLM
 from collie.driver.io import IODriver
 from collie.module import ColumnParallelLinearWithoutBias, RowParallelLinearWithoutBias, ColumnParallelLMHead
-from collie.utils import progress, env, dict_as_params
+from collie.utils import progress, env, dict_as_params, concat_tensor
 
 from typing import Any, Union, Optional
 from collections import OrderedDict
 from transformers.modeling_utils import dtype_byte_size
 from transformers.modeling_utils import PretrainedConfig
 from transformers.modeling_outputs import CausalLMOutputWithPast
  
@@ -513,15 +513,15 @@
         )
         self.lm_head = ColumnParallelLinearWithoutBias(
             self.config.hidden_size,
             self.config.padded_vocab_size,
             bias=False
         )
         # GenerationMixin 需要的额外参数
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config.is_decoder=True
         self.main_input_name = "input_ids"
 
     def forward(self, input_ids: torch.Tensor, **kwargs):
         _, seq_length = input_ids.shape
         attention_mask = kwargs.get("attention_mask", None)
         full_attention_mask = kwargs.get("full_attention_mask", None)
         
@@ -938,15 +938,14 @@
         dst = parallel_state.get_tensor_model_parallel_src_rank()
         with progress(rank_order, desc="Saving model", disable=int(os.environ.get("RANK", "0")) != 0) as pbar:
             for rank in pbar:
                 if env.dp_rank == 0 \
                     and (env.pp_rank == rank
                          or not process_exclusion):
                     for key in sorted(list(state_dict.keys())):
-                        device = state_dict[key].device
                         tensor_list = None
                         if env.tp_rank == 0:
                             tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
                         dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
                         if env.tp_rank == 0:
                             need_column_list = ["query_layer.weight", "query_layer.bias", "key_layer.weight", "key_layer.bias", "value_layer.weight", "value_layer.bias", "word_embeddings.weight",
                                     "lm_head.weight", "dense_h_to_4h_up_proj.weight", "dense_h_to_4h_down_proj.weight"]
@@ -956,22 +955,20 @@
                             if env.pp_size > 1:
                                 # embedding 层和 lm_head 都需要切
                                 try:
                                     need_column_split = need_column_split or int(key.split(".")[0]) == max(parts) - 1 or int(key.split(".")[0]) == min(parts)
                                 except:
                                     pass
                             if need_column_split:
-                                state_dict[key] = torch.cat(tensor_list, dim=0).detach().clone().to(device)
-                                del tensor_list
+                                state_dict[key] = concat_tensor(tensor_list, dim=0)
                                 if process_exclusion:
                                     # CPU 内存回收（速度很慢）
                                     gc.collect()
                             elif need_row_split:
-                                state_dict[key] = torch.cat(tensor_list, dim=1).detach().clone().to(device)
-                                del tensor_list
+                                state_dict[key] = concat_tensor(tensor_list, dim=1)
                                 if process_exclusion:
                                     # CPU 内存回收（速度很慢）
                                     gc.collect()
                     if env.tp_rank == 0:
                         # Save gathered weights
                         if env.is_pipeline:
                             ckpt_name = f"pytorch_model-{env.pp_rank+1:05d}-of-{config.pp_size:05d}.bin"
```

### Comparing `collie-lm-1.0.2/collie/models/internlm/model.py` & `collie-lm-1.0.3/collie/models/internlm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from flash_attn.flash_attention import FlashAttention
 except ModuleNotFoundError:
     FlashAttention = None
 
 from collie.log.logger import logger
 from collie.config import load_config
 from collie.config import CollieConfig
-from collie.utils import progress, env, dict_as_params
+from collie.utils import progress, env, dict_as_params, concat_tensor
 from collie.driver.io import IODriver
 from collie.models.base import CollieModelForCausalLM
 from collie.module import ColumnParallelLinearWithoutBias, RowParallelLinearWithoutBias, ColumnParallelLMHead
 
 from typing import Union, Optional, Tuple
 from collections import OrderedDict
 from transformers.modeling_utils import dtype_byte_size
@@ -243,15 +243,15 @@
         )
         self.lm_head = ColumnParallelLinearWithoutBias(
             self.collie_config.hidden_size,
             self.collie_config.vocab_size,
             bias=False
         )
         # GenerationMixin 需要的额外参数
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config.is_decoder=True
         if config.model_config.tie_word_embeddings:
             self.lm_head.weight = self.embed_tokens.weight
         self.main_input_name = "input_ids"
 
     def forward(self, 
                 input_ids: Optional[torch.Tensor] = None, 
                 attention_mask: Optional[torch.Tensor] = None, 
@@ -525,15 +525,14 @@
         dst = parallel_state.get_tensor_model_parallel_src_rank()
         with progress(rank_order, desc="Saving model", disable=int(os.environ.get("RANK", "0")) != 0) as pbar:
             for rank in pbar:
                 if env.dp_rank == 0 \
                     and (env.pp_rank == rank
                          or not process_exclusion):
                     for key in sorted(list(state_dict.keys())):
-                        device = state_dict[key].device
                         tensor_list = None
                         if env.tp_rank == 0:
                             tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
                         dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
                         if env.tp_rank == 0:
                             if key.endswith("q_proj.weight") \
                                 or key.endswith("q_proj.bias") \
@@ -541,25 +540,23 @@
                                         or key.endswith("k_proj.bias") \
                                             or key.endswith("v_proj.weight") \
                                                 or key.endswith("v_proj.bias") \
                                                     or key.endswith("gate_proj.weight") \
                                                         or key.endswith("up_proj.weight") \
                                                             or key.endswith("embed_tokens.weight") \
                                                                 or key.endswith("lm_head.weight"):
-                                                                    state_dict[key] = torch.cat(tensor_list, dim=0).detach().clone().to(device)
+                                                                    state_dict[key] = concat_tensor(tensor_list, dim=0)
                                                                     if key.endswith("q_proj.weight")  or key.endswith("k_proj.weight"):
                                                                         state_dict[key] = reshape_wq_wk(state_dict[key])
-                                                                    del tensor_list
                                                                     if process_exclusion:
                                                                         # CPU 内存回收（速度很慢）
                                                                         gc.collect()
                             elif key.endswith("o_proj.weight") \
                                 or key.endswith("down_proj.weight"):
-                                    state_dict[key] = torch.cat(tensor_list, dim=1).detach().clone().to(device)
-                                    del tensor_list
+                                    state_dict[key] = concat_tensor(tensor_list, dim=1)
                                     if process_exclusion:
                                         # CPU 内存回收（速度很慢）
                                         gc.collect()
                     if env.tp_rank == 0:
                         # Save gathered weights
                         if env.is_pipeline:
                             ckpt_name = f"pytorch_model-{env.pp_rank+1:05d}-of-{config.pp_size:05d}.bin"
```

### Comparing `collie-lm-1.0.2/collie/models/llama/model.py` & `collie-lm-1.0.3/collie/models/moss/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from flash_attn.flash_attention import FlashAttention
 except ModuleNotFoundError:
     FlashAttention = None
 
 from collie.log.logger import logger
 from collie.config import load_config
 from collie.config import CollieConfig
-from collie.utils import progress, env, dict_as_params
+from collie.utils import progress, env, dict_as_params, concat_tensor
 from collie.driver.io import IODriver
 from collie.models.base import CollieModelForCausalLM
 from collie.module import ColumnParallelLinearWithoutBias, RowParallelLinearWithoutBias, ColumnParallelLMHead
 
 from typing import Union, Optional, Tuple
 from collections import OrderedDict
 from transformers.modeling_utils import dtype_byte_size
@@ -75,15 +75,15 @@
     def forward(self, hidden_states):
         variance = hidden_states.to(torch.float32).pow(2).mean(-1, keepdim=True)
         hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
         if self.weight.dtype in [torch.float16, torch.bfloat16]:
             hidden_states = hidden_states.to(self.weight.dtype)
         return hidden_states * self.weight
 
-class LlamaLayer(nn.Module):
+class MossLayer(nn.Module):
     def __init__(self, config: CollieConfig) -> None:
         super().__init__()
         self.config = config
         self.self_attn = nn.ModuleDict(
             {
                 "q_proj": ColumnParallelLinearWithoutBias(
                     config.hidden_size,
@@ -223,35 +223,35 @@
                 inputs.get("attention_mask", None)
             )
         else:
             inputs["hidden_states"] = self._forward(**inputs)
         return inputs
 
 
-class LlamaForCausalLM(CollieModelForCausalLM):
+class MossForCausalLM(CollieModelForCausalLM):
     
     def __init__(self, config: CollieConfig) -> None:
         super().__init__(config)
         self.embed_tokens = tensor_parallel.VocabParallelEmbedding(
             self.collie_config.vocab_size,
             self.collie_config.hidden_size
         )
         self.layers = nn.ModuleList(
-            [LlamaLayer(self.collie_config) for _ in range(self.collie_config.num_hidden_layers)])
+            [MossLayer(self.collie_config) for _ in range(self.collie_config.num_hidden_layers)])
         self.norm = RMSNormalize(
             dim=self.collie_config.hidden_size,
             eps=self.collie_config.rms_norm_eps
         )
         self.lm_head = ColumnParallelLinearWithoutBias(
             self.collie_config.hidden_size,
             self.collie_config.vocab_size,
             bias=False
         )
         # GenerationMixin 需要的额外参数
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config.is_decoder=True
         if config.model_config.tie_word_embeddings:
             self.lm_head.weight = self.embed_tokens.weight
         self.main_input_name = "input_ids"
 
     def forward(self, 
                 input_ids: Optional[torch.Tensor] = None, 
                 attention_mask: Optional[torch.Tensor] = None, 
@@ -304,15 +304,15 @@
         if config.model_config.tie_word_embeddings:
             return [TiedLayerSpec(
                 "embed_tokens",
                 dict_as_params(input_keys="input_ids", output_keys="hidden_states"),
                 tensor_parallel.VocabParallelEmbedding,
                 config.vocab_size,
                 config.hidden_size),
-                *[LayerSpec(LlamaLayer, config)
+                *[LayerSpec(MossLayer, config)
                 for _ in range(config.num_hidden_layers)],
                 LayerSpec(dict_as_params(input_keys="hidden_states", output_keys="hidden_states"), RMSNormalize,
                         dim=config.hidden_size,
                         eps=config.rms_norm_eps),
                 TiedLayerSpec(
                 "embed_tokens",
                 dict_as_params(input_keys="hidden_states", output_keys="logits"),
@@ -323,15 +323,15 @@
             ]
         else:
             return [LayerSpec(
                 dict_as_params(input_keys="input_ids", output_keys="hidden_states"),
                 tensor_parallel.VocabParallelEmbedding,
                 config.vocab_size,
                 config.hidden_size),
-                *[LayerSpec(LlamaLayer, config)
+                *[LayerSpec(MossLayer, config)
                 for _ in range(config.num_hidden_layers)],
                 LayerSpec(dict_as_params(input_keys="hidden_states", output_keys="hidden_states"), RMSNormalize,
                         dim=config.hidden_size,
                         eps=config.rms_norm_eps),
                 LayerSpec(
                 dict_as_params(input_keys="hidden_states", output_keys="logits"),
                 ColumnParallelLMHead,
@@ -590,40 +590,38 @@
         dst = parallel_state.get_tensor_model_parallel_src_rank()
         with progress(rank_order, desc="Saving model", disable=int(os.environ.get("RANK", "0")) != 0) as pbar:
             for rank in pbar:
                 if env.dp_rank == 0 \
                     and (env.pp_rank == rank
                          or not process_exclusion):
                     for key in sorted(list(state_dict.keys())):
-                        device = state_dict[key].device
                         tensor_list = None
                         if env.tp_size > 1:
                             if env.tp_rank == 0:
                                 tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
                             dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
                             if env.tp_rank == 0:
                                 filte_list = ["q_proj.weight", "q_proj.weight", "k_proj.weight", "v_proj.weight", "gate_proj.weight", "up_proj.weight", "embed_tokens.weight", "lm_head.weight"]
                                 need_split = any([key.endswith(filte) for filte in filte_list])
                                 if env.pp_size > 1:
                                     # embedding 层和 lm_head 都需要切
                                     need_split = need_split or int(key.split(".")[0]) == max(parts) - 1
                                     need_split = need_split or int(key.split(".")[0]) == min(parts)
+
                                 if need_split:
-                                    state_dict[key] = torch.cat(tensor_list, dim=0).detach().clone().to(device)
+                                    state_dict[key] = concat_tensor(tensor_list, dim=0)
                                     if key.endswith("q_proj.weight")  or key.endswith("k_proj.weight"):
                                         state_dict[key] = reshape_wq_wk(state_dict[key])
-                                    del tensor_list
                                     if process_exclusion:
                                         # CPU 内存回收（速度很慢）
                                         gc.collect()
                                                             
                                 elif key.endswith("o_proj.weight") \
                                     or key.endswith("down_proj.weight"):
-                                        state_dict[key] = torch.cat(tensor_list, dim=1).detach().clone().to(device)
-                                        del tensor_list
+                                        state_dict[key] = concat_tensor(tensor_list, dim=1)
                                         if process_exclusion:
                                             # CPU 内存回收（速度很慢）
                                             gc.collect()
                             if not key.startswith("lm_head.weight"):
                                 state_dict[f"model.{key}"] = state_dict.pop(key)
                     if env.tp_rank == 0:
                         # Save gathered weights
```

### Comparing `collie-lm-1.0.2/collie/models/moss/model.py` & `collie-lm-1.0.3/collie/models/llama/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 from deepspeed.pipe import LayerSpec, TiedLayerSpec
 from deepspeed.accelerator import get_accelerator
 
 import math
 from einops import rearrange
 
 try:
-    from flash_attn.flash_attention import FlashAttention
+    from flash_attn.modules.mha import SelfAttention as FlashAttention
 except ModuleNotFoundError:
     FlashAttention = None
 
 from collie.log.logger import logger
 from collie.config import load_config
 from collie.config import CollieConfig
-from collie.utils import progress, env, dict_as_params
+from collie.utils import progress, env, dict_as_params, concat_tensor
 from collie.driver.io import IODriver
 from collie.models.base import CollieModelForCausalLM
 from collie.module import ColumnParallelLinearWithoutBias, RowParallelLinearWithoutBias, ColumnParallelLMHead
 
-from typing import Union, Optional
+from typing import Union, Optional, Tuple
 from collections import OrderedDict
 from transformers.modeling_utils import dtype_byte_size
 from transformers.modeling_utils import PretrainedConfig
 from transformers.modeling_outputs import CausalLMOutputWithPast
 
 class RotaryPositionEmbedding(nn.Module):
     def __init__(self, head_dim: int) -> None:
@@ -52,15 +52,15 @@
         query = torch.view_as_complex(
             query.float().reshape(*query.shape[:-1], -1, 2))
         key = torch.view_as_complex(
             key.float().reshape(*key.shape[:-1], -1, 2))
         freqs = torch.outer(torch.arange(
             (2 ** 16) * 2, device=self.inv_freq.device), self.inv_freq).float()
         freqs_cis = torch.polar(torch.ones_like(freqs), freqs)[
-            start_pos: start_pos + seq_len].to(query)
+            start_pos: start_pos + seq_len]
         shape = [d if i == 1 or i == query.ndim -
                  1 else 1 for i, d in enumerate(query.shape)]
         freqs_cis = freqs_cis.view(*shape)
         query = torch.view_as_real(query * freqs_cis).flatten(3)
         key = torch.view_as_real(key * freqs_cis).flatten(3)
         return query.type(t), key.type(t)
 
@@ -75,43 +75,51 @@
     def forward(self, hidden_states):
         variance = hidden_states.to(torch.float32).pow(2).mean(-1, keepdim=True)
         hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
         if self.weight.dtype in [torch.float16, torch.bfloat16]:
             hidden_states = hidden_states.to(self.weight.dtype)
         return hidden_states * self.weight
 
-class MossLayer(nn.Module):
+class LlamaLayer(nn.Module):
     def __init__(self, config: CollieConfig) -> None:
         super().__init__()
         self.config = config
+        if hasattr(config, "num_key_value_heads"):
+            # llama2 (transformers >= 4.31.0)
+            self.num_key_value_heads = config.num_key_value_heads
+        else:
+            self.num_key_value_heads = config.num_attention_heads
+        self.num_key_value_groups = config.num_attention_heads // self.num_key_value_heads
+        self.num_heads = config.num_attention_heads
+        self.head_dim = config.hidden_size // config.num_attention_heads
         self.self_attn = nn.ModuleDict(
             {
                 "q_proj": ColumnParallelLinearWithoutBias(
                     config.hidden_size,
-                    config.hidden_size,
+                    self.num_heads * self.head_dim,
                     bias=False,
                     gather_output=False,
                     init_method=lambda x: x
                 ),
                 "k_proj": ColumnParallelLinearWithoutBias(
                     config.hidden_size,
-                    config.hidden_size,
+                    self.num_key_value_heads * self.head_dim,
                     bias=False,
                     gather_output=False,
                     init_method=lambda x: x
                 ),
                 "v_proj": ColumnParallelLinearWithoutBias(
                     config.hidden_size,
-                    config.hidden_size,
+                    self.num_key_value_heads * self.head_dim,
                     bias=False,
                     gather_output=False,
                     init_method=lambda x: x
                 ),
                 "o_proj": RowParallelLinearWithoutBias(
-                    config.hidden_size,
+                    self.num_heads * self.head_dim,
                     config.hidden_size,
                     bias=False,
                     input_is_parallel=True,
                     init_method=lambda x: x
                 ),
                 "rotary_emb": RotaryPositionEmbedding(
                     self.config.hidden_size // self.config.num_attention_heads)
@@ -145,75 +153,77 @@
             )
         })
         self.post_attention_layernorm = RMSNormalize(
             dim=config.hidden_size,
             eps=config.rms_norm_eps
         )
         # 务必保持变量名一致
-        self.use_cache = False
+        self.use_cache = self.config.model_config.use_cache
         self.past_key_values = None
         self.hidden_states = None
 
     def _forward(self, 
                  hidden_states: torch.Tensor,
                  attention_mask: Optional[torch.Tensor] = None, **kwargs):
         if not self.training:
             self.hidden_states = hidden_states
         else:
             self.hidden_states = None
         assert hidden_states.ndim == 3, f"hidden_states.shape must be (B, N, H), but got {hidden_states.shape}"
         batch_size, seq_len, _ = hidden_states.shape
-        head_dim = self.config.hidden_size // self.config.num_attention_heads
         _hidden_states = self.input_layernorm(hidden_states)
         query, key, value = self.self_attn["q_proj"](_hidden_states), self.self_attn["k_proj"](
             _hidden_states), self.self_attn["v_proj"](_hidden_states)
-        query, key, value = rearrange(query, "b n (h d) -> b n h d", d=head_dim), \
-            rearrange(key, "b n (h d) -> b n h d", d=head_dim), \
-            rearrange(value, "b n (h d) -> b n h d", d=head_dim)
-        if self.past_key_values is not None and self.use_cache:
-            start_pos = self.past_key_values[0].shape[1]
+        query, key, value = rearrange(query, "b n (h d) -> b n h d", d=self.head_dim), \
+            rearrange(key, "b n (h d) -> b n h d", d=self.head_dim), \
+            rearrange(value, "b n (h d) -> b n h d", d=self.head_dim)
+        if self.past_key_values is not None:
+            start_pos = self.past_key_values.shape[3]
         else:
-            self.past_key_values = None
             start_pos = 0
         query, key = self.self_attn["rotary_emb"](query, key, seq_len, start_pos)
-        if self.use_cache:
-            if self.past_key_values is not None:
-                query = torch.cat([self.past_key_values[0], query], dim=1)
-                key = torch.cat([self.past_key_values[0], key], dim=1)
-                value = torch.cat([self.past_key_values[1], value], dim=1)
-            if not self.training:
-                self.past_key_values = [key, value]
+        if self.past_key_values is not None:
+            query = torch.cat([self.past_key_values[0].permute([0, 2, 1, 3]), query], dim=1)
+            key = torch.cat([self.past_key_values[0].permute([0, 2, 1, 3]), key], dim=1)
+            value = torch.cat([self.past_key_values[1].permute([0, 2, 1, 3]), value], dim=1)
+        if self.use_cache and not self.training:
+            self.past_key_values = torch.stack((key.permute([0, 2, 1, 3]), value.permute([0, 2, 1, 3])), dim=0)
+        key = torch.repeat_interleave(key, dim=1, repeats=self.num_key_value_groups)
+        value = torch.repeat_interleave(value, dim=1, repeats=self.num_key_value_groups)
         attention_mask = attention_mask if attention_mask is not None else torch.ones((query.shape[0], query.shape[1])).to(hidden_states.device)
         if self.config.use_flash:
             assert FlashAttention is not None, \
                 "Detected flash_attn is not installed. See https://github.com/HazyResearch/flash-attention"
             qkv = torch.stack([query, key, value], dim=2)
-            output, _ = FlashAttention()(qkv, key_padding_mask=attention_mask, causal=True)
+            output = FlashAttention()(qkv, key_padding_mask=attention_mask.bool(), causal=True)
+            """ flash_attn_2 note: 
+                from flash_attn.modules.mha import SelfAttention as FlashAttention
+                require attention_mask as a bool tensor
+                replace 'output, _ =' as 'output =' 
+            """
             output = rearrange(output, "b n h d -> b n (h d)")
-            output = F.dropout(output, p=self.config.dropout,
-                               training=self.training)
         else:
             query, key, value = query.permute(0, 2, 1, 3), key.permute(
                 0, 2, 1, 3), value.permute(0, 2, 1, 3)
             attention_score = torch.matmul(query, key.transpose(
-                2, 3)) / math.sqrt(head_dim)
+                2, 3)) / math.sqrt(self.head_dim)
             if seq_len + start_pos > 1:
                 mask = torch.full((1, 1, seq_len + start_pos, seq_len + start_pos), float("-inf"))
                 mask = torch.triu(mask, diagonal=1).to(
                     attention_score.device)
                 attention_score = attention_score + mask
             key_padding_mask = (1.0 - attention_mask.unsqueeze(1).unsqueeze(2)) * torch.finfo(
                 attention_score.dtype).min
             attention_score = F.softmax(
                 attention_score + key_padding_mask, dim=-1).type_as(value)
             output = torch.matmul(attention_score, value)
             output = output.transpose(1, 2).contiguous().view(
                 batch_size, seq_len + start_pos, -1)
-            output = F.dropout(output, p=self.config.dropout,
-                               training=self.training)
+        output = F.dropout(output, p=self.config.dropout,
+                            training=self.training)
         output = output[:, start_pos:, :]
         hidden_states = hidden_states + self.self_attn["o_proj"](output)
         _hidden_states = self.post_attention_layernorm(hidden_states)
         hidden_states = hidden_states + F.dropout(self.mlp["down_proj"](F.silu(self.mlp["gate_proj"](
             _hidden_states)) * self.mlp["up_proj"](_hidden_states)), p=self.config.dropout, training=self.training)
         return hidden_states
 
@@ -225,47 +235,55 @@
                 inputs.get("attention_mask", None)
             )
         else:
             inputs["hidden_states"] = self._forward(**inputs)
         return inputs
 
 
-class MossForCausalLM(CollieModelForCausalLM):
+class LlamaForCausalLM(CollieModelForCausalLM):
     
     def __init__(self, config: CollieConfig) -> None:
         super().__init__(config)
         self.embed_tokens = tensor_parallel.VocabParallelEmbedding(
             self.collie_config.vocab_size,
             self.collie_config.hidden_size
         )
         self.layers = nn.ModuleList(
-            [MossLayer(self.collie_config) for _ in range(self.collie_config.num_hidden_layers)])
+            [LlamaLayer(self.collie_config) for _ in range(self.collie_config.num_hidden_layers)])
         self.norm = RMSNormalize(
             dim=self.collie_config.hidden_size,
             eps=self.collie_config.rms_norm_eps
         )
         self.lm_head = ColumnParallelLinearWithoutBias(
             self.collie_config.hidden_size,
             self.collie_config.vocab_size,
             bias=False
         )
         # GenerationMixin 需要的额外参数
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config.is_decoder=True
         if config.model_config.tie_word_embeddings:
             self.lm_head.weight = self.embed_tokens.weight
         self.main_input_name = "input_ids"
 
-    def forward(self, input_ids: Optional[torch.Tensor] = None, attention_mask: Optional[torch.Tensor] = None, **kwargs):
+    def forward(self, 
+                input_ids: Optional[torch.Tensor] = None, 
+                attention_mask: Optional[torch.Tensor] = None, 
+                past_key_values: Optional[Tuple[torch.Tensor]] = None,
+                **kwargs):
         inputs = {"input_ids": input_ids}
         if attention_mask is not None:
             inputs["attention_mask"] = attention_mask
         if input_ids == None:
             inputs["hidden_states"] = kwargs['inputs_embeds']
         else:
             inputs["hidden_states"] = self.embed_tokens(inputs["input_ids"])
+        if past_key_values is not None:
+            self._set_past_key_values(self.layers, past_key_values)
+        else:
+            self._clean_past_key_values(self.layers)
         all_hidden_states = ()
         for layer in self.layers:
             all_hidden_states += (inputs["hidden_states"],)
             inputs.update(layer(inputs))
         inputs["hidden_states"] = self.norm(inputs["hidden_states"])
         all_hidden_states += (inputs["hidden_states"], )
         inputs["logits"] = self.lm_head(inputs["hidden_states"])
@@ -273,31 +291,22 @@
             loss=None,
             logits=inputs["logits"],
             past_key_values=self._get_past_key_values(self.layers),
             hidden_states=all_hidden_states,
             attentions=None
         )
 
-    def prepare_inputs_for_generation(self,
-                                      input_ids: torch.Tensor,
-                                      past_key_values: Optional[list] = None,
-                                      attention_mask: Optional[torch.Tensor] = None,
-                                      **kwargs):
-        self._set_use_cache(self.layers, kwargs.get("use_cache", self.generation_config.use_cache))
-        if past_key_values is None:
-            self._clean_past_key_values(self.layers)
-        else:
-            input_ids = input_ids[:, -1].unsqueeze(-1)
-            self._set_past_key_values(self.layers, past_key_values)
-        return {"input_ids": input_ids, "attention_mask": attention_mask, "past_key_values": past_key_values}
-
     def clean(self):
         self._clean_hidden_states([*self.layers, self.lm_head])
         self._clean_past_key_values(self.layers)
         self._set_use_cache(self.layers, False)
+        
+    def set_cache(self, use_cache, past_key_values):
+        self._set_use_cache(self.layers, use_cache)
+        self._set_past_key_values(self.layers, past_key_values)
 
     @classmethod
     def pipeline_layers(cls, config: CollieConfig):
         """
         Get layers of pipeline.
 
         :return: list
@@ -307,15 +316,15 @@
         if config.model_config.tie_word_embeddings:
             return [TiedLayerSpec(
                 "embed_tokens",
                 dict_as_params(input_keys="input_ids", output_keys="hidden_states"),
                 tensor_parallel.VocabParallelEmbedding,
                 config.vocab_size,
                 config.hidden_size),
-                *[LayerSpec(MossLayer, config)
+                *[LayerSpec(LlamaLayer, config)
                 for _ in range(config.num_hidden_layers)],
                 LayerSpec(dict_as_params(input_keys="hidden_states", output_keys="hidden_states"), RMSNormalize,
                         dim=config.hidden_size,
                         eps=config.rms_norm_eps),
                 TiedLayerSpec(
                 "embed_tokens",
                 dict_as_params(input_keys="hidden_states", output_keys="logits"),
@@ -326,15 +335,15 @@
             ]
         else:
             return [LayerSpec(
                 dict_as_params(input_keys="input_ids", output_keys="hidden_states"),
                 tensor_parallel.VocabParallelEmbedding,
                 config.vocab_size,
                 config.hidden_size),
-                *[LayerSpec(MossLayer, config)
+                *[LayerSpec(LlamaLayer, config)
                 for _ in range(config.num_hidden_layers)],
                 LayerSpec(dict_as_params(input_keys="hidden_states", output_keys="hidden_states"), RMSNormalize,
                         dim=config.hidden_size,
                         eps=config.rms_norm_eps),
                 LayerSpec(
                 dict_as_params(input_keys="hidden_states", output_keys="logits"),
                 ColumnParallelLMHead,
@@ -593,44 +602,44 @@
         dst = parallel_state.get_tensor_model_parallel_src_rank()
         with progress(rank_order, desc="Saving model", disable=int(os.environ.get("RANK", "0")) != 0) as pbar:
             for rank in pbar:
                 if env.dp_rank == 0 \
                     and (env.pp_rank == rank
                          or not process_exclusion):
                     for key in sorted(list(state_dict.keys())):
-                        device = state_dict[key].device
                         tensor_list = None
-                        if env.tp_rank == 0:
-                            tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
-                        dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
-                        if env.tp_rank == 0:
-                            filte_list = ["q_proj.weight", "q_proj.weight", "k_proj.weight", "v_proj.weight", "gate_proj.weight", "up_proj.weight", "embed_tokens.weight", "lm_head.weight"]
-                            need_split = any([key.endswith(filte) for filte in filte_list])
-                            if env.pp_size > 1:
-                                # embedding 层和 lm_head 都需要切
-                                need_split = need_split or int(key.split(".")[0]) == max(parts) - 1
-                                need_split = need_split or int(key.split(".")[0]) == min(parts)
-                            if need_split:
-                                state_dict[key] = torch.cat(tensor_list, dim=0).detach().clone().to(device)
-                                if key.endswith("q_proj.weight")  or key.endswith("k_proj.weight"):
-                                    state_dict[key] = reshape_wq_wk(state_dict[key])
-                                del tensor_list
-                                if process_exclusion:
-                                    # CPU 内存回收（速度很慢）
-                                    gc.collect()
-                                                        
-                            elif key.endswith("o_proj.weight") \
-                                or key.endswith("down_proj.weight"):
-                                    state_dict[key] = torch.cat(tensor_list, dim=1).detach().clone().to(device)
-                                    del tensor_list
+                        if env.tp_size > 1:
+                            if env.tp_rank == 0:
+                                tensor_list = [torch.zeros_like(state_dict[key]).to(state_dict[key].dtype).cuda() for _ in range(config.tp_size)]
+                            dist.gather(state_dict[key].cuda(), dst=dst, gather_list=tensor_list, group=env.tp_group)
+                            if env.tp_rank == 0:
+                                filte_list = ["q_proj.weight", "q_proj.weight", "k_proj.weight", "v_proj.weight", "gate_proj.weight", "up_proj.weight", "embed_tokens.weight", "lm_head.weight"]
+                                need_split = any([key.endswith(filte) for filte in filte_list])
+                                if env.pp_size > 1:
+                                    # embedding 层和 lm_head 都需要切
+                                    need_split = need_split or int(key.split(".")[0]) == max(parts) - 1
+                                    need_split = need_split or int(key.split(".")[0]) == min(parts)
+
+                                if need_split:
+                                    state_dict[key] = concat_tensor(tensor_list, dim=0)
+                                    
                                     if process_exclusion:
                                         # CPU 内存回收（速度很慢）
                                         gc.collect()
-                            if not key.startswith("lm_head.weight"):
-                                state_dict[f"model.{key}"] = state_dict.pop(key)
+                                                            
+                                elif key.endswith("o_proj.weight") \
+                                    or key.endswith("down_proj.weight"):
+                                        state_dict[key] = concat_tensor(tensor_list, dim=1)
+                                        if process_exclusion:
+                                            # CPU 内存回收（速度很慢）
+                                            gc.collect()
+                        if key.endswith("q_proj.weight")  or key.endswith("k_proj.weight"):
+                            state_dict[key] = reshape_wq_wk(state_dict[key])
+                        if not key.startswith("lm_head.weight"):
+                            state_dict[f"model.{key}"] = state_dict.pop(key)
                     if env.tp_rank == 0:
                         # Save gathered weights
                         if env.is_pipeline:
                             ckpt_name = f"pytorch_model-{env.pp_rank+1:05d}-of-{config.pp_size:05d}.bin"
                             total_size = 0
                             weight_map = {}
                             for name, weight in state_dict.items():
```

### Comparing `collie-lm-1.0.2/collie/models/moss_moon/model.py` & `collie-lm-1.0.3/collie/models/moss_moon/model.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/models/moss_moon/utils.py` & `collie-lm-1.0.3/collie/models/moss_moon/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gc
 
 import torch
 from torch import distributed as dist
 from transformers.modeling_utils import dtype_byte_size
-from collie.utils import env
+from collie.utils import env, concat_tensor
 
 def create_sinusoidal_positions(num_pos: int, dim: int) -> torch.Tensor:
     inv_freq = 1.0 / (10000 ** (torch.arange(0, dim, 2) / dim))
     sinusoid_inp = torch.einsum("i , j -> i j", torch.arange(num_pos, dtype=torch.float), inv_freq).float()
     return torch.cat((torch.sin(sinusoid_inp), torch.cos(sinusoid_inp)), dim=1)
 
 def rotate_every_two(x: torch.Tensor) -> torch.Tensor:
@@ -170,21 +170,21 @@
         chunk_dim = _tp_split_dim(name)
         if chunk_dim is None:
             continue
         # gather to tp_rank 0
         gather_list = [torch.empty_like(param) for _ in range(tp_size)]
         dist.all_gather(gather_list, param, group=tp_group)
         if tp_rank == 0:
-            tensor = torch.concat(gather_list, dim=chunk_dim)
+            tensor = concat_tensor(gather_list)
             del state_dict[name]
+            del gather_list_cpu
             state_dict[name] = tensor
         else:
             del gather_list
             del state_dict[name]
-
         if process_exclusion:
             # CPU 内存回收（速度很慢）
             gc.collect()
 
     return state_dict
 
 def _state_dict_to_save(state_dict, tp_rank, tp_size, tp_group,
```

### Comparing `collie-lm-1.0.2/collie/module.py` & `collie-lm-1.0.3/collie/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     重写 ``transformers`` 提供的 ``GenerationMixin`` 以支持 **CoLLie** 中的流水线
     模型。
 
     :param engine: `DeepSpeedEngine` 实例，可由 :meth:`~collie.utils.\
         setup_ds_engine` 函数生成
     """
     def __init__(self) -> None:
-        self.config = PretrainedConfig(is_decoder=True)
+        self.config = self.collie_config.model_config
+        self.config.is_decoder=True
         self.generation_config = GenerationConfig()
         self.main_input_name = "input_ids"
         self.device = torch.device("cuda")
         self.engine_container = []
         self.layers = None
         self._find_layers()
         self.is_contrastive_search = False
@@ -570,23 +571,29 @@
             return None, None
         for name, layer in enumerate(reversed(self.forward_funcs)):
             if isinstance(layer, (ColumnParallelLinear, nn.Linear)):
                 return len(self.forward_funcs) - name - 1, layer
         return None, None
     
     def set_input_embedding(self, name, embedding):
-        if self.get_input_embedding()[1] is not None and self.get_input_embedding()[1] in list(self.tied_modules.values()):
-            key = list(self.tied_modules.keys())[list(self.tied_modules.values()).index(self.get_input_embedding()[1])]
-            self.tied_modules[key] = embedding
+        if self.get_input_embedding()[1] is not None:
+            if self.get_input_embedding()[1] in list(self.tied_modules.values()):
+                key = list(self.tied_modules.keys())[list(self.tied_modules.values()).index(self.get_input_embedding()[1])]
+                self.tied_modules[key] = embedding
+            elif self.get_input_embedding()[1] in list(self._modules.values()):
+                self.add_module(str(name), embedding)
         self.forward_funcs[name] = embedding
-        
+
     def set_lm_head(self, name, lm_head):
-        if self.get_lm_head()[1] is not None and self.get_lm_head()[1] in list(self.tied_modules.values()):
-            key = list(self.tied_modules.keys())[list(self.tied_modules.values()).index(self.get_lm_head()[1])]
-            self.tied_modules[key] = lm_head
+        if self.get_lm_head()[1] is not None:
+            if self.get_lm_head()[1] in list(self.tied_modules.values()):
+                key = list(self.tied_modules.keys())[list(self.tied_modules.values()).index(self.get_lm_head()[1])]
+                self.tied_modules[key] = lm_head
+            elif self.get_lm_head()[1] in list(self._modules.values()):
+                self.add_module(str(name), lm_head)
         self.forward_funcs[name] = lm_head
         
     def tie_weights(self):
         pass
     
     def skip_input_embedding(self):
         input_embedding = self.get_input_embedding()[1]
```

### Comparing `collie-lm-1.0.2/collie/optim/adan.py` & `collie-lm-1.0.3/collie/optim/adan.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/optim/lion.py` & `collie-lm-1.0.3/collie/optim/lion.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/optim/lomo.py` & `collie-lm-1.0.3/collie/optim/lomo.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/optim/sophiag.py` & `collie-lm-1.0.3/collie/optim/sophiag.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/__init__.py` & `collie-lm-1.0.3/collie/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .dist_utils import (setup_distribution, set_seed, env, setup_ds_engine,
                          zero3_load_state_dict, is_zero3_enabled,
                          broadcast_tensor)
 from .utils import find_tensors, progress, dictToObj, apply_to_collection, dict_as_params, \
-    is_static_method, auto_param_call, get_keys_to_not_convert
+    is_static_method, auto_param_call, get_keys_to_not_convert, concat_tensor
 from .data_provider import BaseProvider, GradioProvider, _GenerationStreamer, DashProvider
 from .metric_wrapper import _MetricsWrapper
 from .monitor import BaseMonitor, StepTimeMonitor, _MultiMonitors, TGSMonitor, MemoryMonitor, \
     LossMonitor, EvalMonitor, LRMonitor, NetworkIOMonitor, DiskIOMonitor, CPUMemoryMonitor
 from .padder import ColliePadder
 
 __all__ = [
@@ -24,14 +24,15 @@
     "progress",
     "dict_as_params",
     "dictToObj",
     "apply_to_collection",
     "is_static_method",
     "auto_param_call",
     "get_keys_to_not_convert",
+    "concat_tensor",
 
     # data_provider
     "BaseProvider",
     "GradioProvider",
     "_GenerationStreamer",
     "DashProvider",
```

### Comparing `collie-lm-1.0.2/collie/utils/data_provider.py` & `collie-lm-1.0.3/collie/utils/data_provider.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/dist_utils.py` & `collie-lm-1.0.3/collie/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/metric_wrapper.py` & `collie-lm-1.0.3/collie/utils/metric_wrapper.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/monitor.py` & `collie-lm-1.0.3/collie/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/padder.py` & `collie-lm-1.0.3/collie/utils/padder.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/peft_utils.py` & `collie-lm-1.0.3/collie/utils/peft_utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/pipeline_engine.py` & `collie-lm-1.0.3/collie/utils/pipeline_engine.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/rich_progress.py` & `collie-lm-1.0.3/collie/utils/rich_progress.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/seq_len_to_mask.py` & `collie-lm-1.0.3/collie/utils/seq_len_to_mask.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie/utils/utils.py` & `collie-lm-1.0.3/collie/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import torch
 
 from collie.log.logger import logger
 from .rich_progress import f_rich_progress
 
 __all__ = ["find_tensors", "progress", "dictToObj", "apply_to_collection", 
            "dict_as_params", "initization_mapping", "is_static_method", 
-           "auto_param_call", "get_keys_to_not_convert"]
+           "auto_param_call", "get_keys_to_not_convert", "concat_tensor"]
 
 def find_tensors():
     """
     打印出垃圾回收区的所有张量。
 
     Adopted from https://discuss.pytorch.org/t/how-to-debug-causes-of-gpu-memory-leaks/6741/3
     """
@@ -31,14 +31,27 @@
     for obj in gc.get_objects():
         try:
             if torch.is_tensor(obj) or (hasattr(obj, 'data') and torch.is_tensor(obj.data)):
                 print(type(obj), obj.size(), obj.dtype, obj.device)
         except:
             pass
 
+
+def concat_tensor(tensor_list, dim=0):
+    """
+    拼接 ``tensor_list`` 中的张量，并且在拼接时将张量转移到 cpu 上来避免显存的增加。
+
+    :return: 拼接后位于 cpu 上的张量
+    """
+    tensor_list_cpu = [t.detach().cpu().clone() for t in tensor_list]
+    tensor_list.clear()
+    # del tensor_list
+    ret = torch.cat(tensor_list_cpu, dim=dim)
+    return ret
+
         
 class progress:
     """包装了 ``rich`` 进度条的类。
 
     .. code-block::
 
         for batch in progress(dataloader):
```

### Comparing `collie-lm-1.0.2/collie_cli/bullet/charDef.py` & `collie-lm-1.0.3/collie_cli/bullet/charDef.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/client.py` & `collie-lm-1.0.3/collie_cli/bullet/client.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/colors.py` & `collie-lm-1.0.3/collie_cli/bullet/colors.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/cursor.py` & `collie-lm-1.0.3/collie_cli/bullet/cursor.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/keyhandler.py` & `collie-lm-1.0.3/collie_cli/bullet/keyhandler.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/styles.py` & `collie-lm-1.0.3/collie_cli/bullet/styles.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/bullet/utils.py` & `collie-lm-1.0.3/collie_cli/bullet/utils.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/collie_cli.py` & `collie-lm-1.0.3/collie_cli/collie_cli.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/config.py` & `collie-lm-1.0.3/collie_cli/config.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_cli/run.py` & `collie-lm-1.0.3/collie_cli/run.py`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/collie_lm.egg-info/SOURCES.txt` & `collie-lm-1.0.3/collie_lm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collie-lm-1.0.2/setup.py` & `collie-lm-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt", encoding="utf-8") as f:
     reqs = f.read()
 
 setup(
     name="collie-lm",
-    version="1.0.2",
+    version="1.0.3",
     description="CoLLiE: Collaborative Tuning of Large Language Models in an Efficient Way",
     author="OpenLMLab",
     author_email="yanhang@pjlab.org.cn",
     packages=find_packages(),
     install_requires=reqs.splitlines(),
     python_requires=">=3.8",
     entry_points={
```

