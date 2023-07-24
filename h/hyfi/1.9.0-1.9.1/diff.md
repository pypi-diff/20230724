# Comparing `tmp/hyfi-1.9.0.tar.gz` & `tmp/hyfi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.9.0.tar", max compression
+gzip compressed data, was "hyfi-1.9.1.tar", max compression
```

## Comparing `hyfi-1.9.0.tar` & `hyfi-1.9.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-24 11:17:34.959035 hyfi-1.9.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-24 11:17:34.959035 hyfi-1.9.0/README.md
--rw-r--r--   0        0        0     4852 2023-07-24 11:18:08.798650 hyfi-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     4346 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0     1213 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-24 11:18:08.702639 hyfi-1.9.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     1497 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24454 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      193 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0     1053 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      955 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      876 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      738 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      338 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5784 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10023 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5783 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3344 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5744 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    19733 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4327 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8383 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5822 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7164 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1184 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 13:05:22.373607 hyfi-1.9.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-24 13:05:22.373607 hyfi-1.9.1/README.md
+-rw-r--r--   0        0        0     4852 2023-07-24 13:06:03.249880 hyfi-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4346 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0     1213 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 13:06:03.137879 hyfi-1.9.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1497 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24454 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0     1053 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      955 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      876 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      738 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      338 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 13:05:22.381607 hyfi-1.9.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5562 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10023 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5671 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3344 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5744 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    19817 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4327 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8383 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5822 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-24 13:05:22.385607 hyfi-1.9.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7916 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1184 2023-07-24 13:05:22.389607 hyfi-1.9.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.9.1/PKG-INFO
```

### Comparing `hyfi-1.9.0/LICENSE` & `hyfi-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/README.md` & `hyfi-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/pyproject.toml` & `hyfi-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.9.0"
+version = "1.9.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.9.0/src/hyfi/__cli__.py` & `hyfi-1.9.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/__click__.py` & `hyfi-1.9.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/__init__.py` & `hyfi-1.9.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/about/__init__.py` & `hyfi-1.9.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/batch/__init__.py` & `hyfi-1.9.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.9.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.9.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.9.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/common.py` & `hyfi-1.9.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.9.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/meta.py` & `hyfi-1.9.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/progress.py` & `hyfi-1.9.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.9.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.9.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.9.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.9.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.9.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/testing.py` & `hyfi-1.9.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/cached_path/util.py` & `hyfi-1.9.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/composer/__init__.py` & `hyfi-1.9.1/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/composer/base.py` & `hyfi-1.9.1/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/composer/pydantic.py` & `hyfi-1.9.1/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.9.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.9.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/copier/__init__.py` & `hyfi-1.9.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/core/__init__.py` & `hyfi-1.9.1/src/hyfi/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 from pathlib import Path
 from typing import Any, List, Optional
 
 from pydantic import BaseModel
 
 from hyfi.utils.logging import LOGGING
+from hyfi.utils.packages import PKGs
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 __hydra_default_config_group_value__ = "__init__"
 __hyfi_name__: str = "HyFI"
 __hyfi_config_path__ = "conf"
@@ -76,28 +77,20 @@
         """Returns the list of plugins to load."""
         return self.__plugins__
 
     def get_plugins(self, plugins: List[str]) -> List[str]:
         """Returns the list of plugins to load."""
         _plugins = []
         for plugin in plugins:
-            H = self._safe_import_module(plugin)
-            if H and getattr(H, "config_module", None):
-                _plugins.append(H.config_module)
+            plugin = plugin.split(".")[0]
+            config_module = f"{plugin}.{self.__config_path__}"
+            if PKGs.is_importable(config_module):
+                _plugins.append(config_module)
         return _plugins
 
-    @staticmethod
-    def _safe_import_module(module_name: str) -> Any:
-        """Safely imports a module."""
-        try:
-            return importlib.import_module(module_name).HyFI
-        except ImportError:
-            logger.debug("Failed to import module: %s", module_name)
-            return None
-
     @property
     def version(self) -> str:
         """Returns the version number of the package."""
         return self.__version__
 
     @property
     def config_module(self) -> str:
```

### Comparing `hyfi-1.9.0/src/hyfi/core/config.py` & `hyfi-1.9.1/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/core/hydra/__init__.py` & `hyfi-1.9.1/src/hyfi/core/hydra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,15 @@
     """Returns the path to the caller module's config folder"""
     caller_module_name = PKGs.get_caller_module_name()
     config_module = caller_module_name.split(".")[0]
     config_module_path = f"{config_module}.{config_path}"
     if config_module_path == __hyfi_config_module_path__:
         return config_module_path
     # check if the config module is importable
-    try:
-        __import__(config_module_path)
-        return config_module_path
-    except ImportError:
-        logger.debug("Config module not found: %s", config_module_path)
-    return ""
+    return config_module_path if PKGs.is_importable(config_module_path) else ""
 
 
 _UNSPECIFIED_: Any = object()
 
 
 class initialize_config:
     """
```

### Comparing `hyfi-1.9.0/src/hyfi/core/hydra/main.py` & `hyfi-1.9.1/src/hyfi/core/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/core/hydra/utils.py` & `hyfi-1.9.1/src/hyfi/core/hydra/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.9.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/graphics/__init__.py` & `hyfi-1.9.1/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/graphics/collage.py` & `hyfi-1.9.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/graphics/motion.py` & `hyfi-1.9.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/graphics/utils.py` & `hyfi-1.9.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/joblib/__init__.py` & `hyfi-1.9.1/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.9.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.9.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.9.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/main/__init__.py` & `hyfi-1.9.1/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,21 +101,24 @@
     def __init__(self) -> None:
         raise NotImplementedError("Use one of the static construction functions")
 
     @staticmethod
     def initialize_global_hyfi(
         package_name: str,
         version: str,
+        plugins: Optional[List[str]] = None,
     ) -> None:
         """
         Initializes the global HyFI instance.
 
         This function should be called before any other HyFI function.
         """
-        __global_hyfi__.initialize(package_name=package_name, version=version)
+        __global_hyfi__.initialize(
+            package_name=package_name, version=version, plugins=plugins
+        )
 
     @staticmethod
     def about(**args) -> None:
         """Print the about information"""
         __global_config__.print_about(**args)
 
     @staticmethod
```

### Comparing `hyfi-1.9.0/src/hyfi/path/__init__.py` & `hyfi-1.9.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/path/base.py` & `hyfi-1.9.1/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/path/batch.py` & `hyfi-1.9.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/path/dirnames.py` & `hyfi-1.9.1/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/path/task.py` & `hyfi-1.9.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/pipe/__init__.py` & `hyfi-1.9.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/pipe/datasets.py` & `hyfi-1.9.1/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/pipe/test.py` & `hyfi-1.9.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.9.1/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/pipeline/configs.py` & `hyfi-1.9.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/project/__init__.py` & `hyfi-1.9.1/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/task/__init__.py` & `hyfi-1.9.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/task/batch.py` & `hyfi-1.9.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/conf.py` & `hyfi-1.9.1/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/contexts.py` & `hyfi-1.9.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/datasets.py` & `hyfi-1.9.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/envs.py` & `hyfi-1.9.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/funcs.py` & `hyfi-1.9.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/gpumon.py` & `hyfi-1.9.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/iolibs.py` & `hyfi-1.9.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/logging.py` & `hyfi-1.9.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/notebooks.py` & `hyfi-1.9.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/src/hyfi/utils/packages.py` & `hyfi-1.9.1/src/hyfi/utils/packages.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module provides utilities for loading library packages and dependencies."""
 import importlib
 import inspect
 import os
 import subprocess
 import sys
 from pathlib import Path
+from typing import Any
 
 from hyfi.utils.iolibs import IOLIBs
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 
@@ -199,10 +200,30 @@
 
     @staticmethod
     def viewsource(obj: str) -> None:
         """Print the source code of the object."""
         print(PKGs.getsource(obj))
 
     @staticmethod
-    def get_caller_module_name() -> str:
+    def get_caller_module_name(caller_stack_depth: int = 2) -> str:
         """Get the name of the module that called this function."""
-        return inspect.getmodule(inspect.stack()[2][0]).__name__  # type: ignore
+        try:
+            return inspect.getmodule(inspect.stack()[caller_stack_depth + 1][0]).__name__  # type: ignore
+        except Exception as e:
+            logger.error(
+                f"Error getting caller module name at depth {caller_stack_depth}: {e}"
+            )
+            return ""
+
+    @staticmethod
+    def is_importable(module_name: str) -> bool:
+        module_spec = importlib.util.find_spec(module_name)  # type: ignore
+        return module_spec is not None
+
+    @staticmethod
+    def safe_import_module(module_name: str) -> Any:
+        """Safely imports a module."""
+        try:
+            return importlib.import_module(module_name)
+        except ImportError:
+            logger.debug("Failed to import module: %s", module_name)
+            return None
```

### Comparing `hyfi-1.9.0/src/hyfi/workflow/__init__.py` & `hyfi-1.9.1/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.9.0/PKG-INFO` & `hyfi-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.9.0
+Version: 1.9.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

