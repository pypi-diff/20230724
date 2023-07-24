# Comparing `tmp/hyfi-1.8.3.tar.gz` & `tmp/hyfi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.8.3.tar", max compression
+gzip compressed data, was "hyfi-1.9.0.tar", max compression
```

## Comparing `hyfi-1.8.3.tar` & `hyfi-1.9.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-23 20:11:17.358103 hyfi-1.8.3/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-23 20:11:17.358103 hyfi-1.8.3/README.md
--rw-r--r--   0        0        0     4853 2023-07-23 20:11:48.852087 hyfi-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     4168 2023-07-23 20:11:17.362104 hyfi-1.8.3/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-23 20:11:17.362104 hyfi-1.8.3/src/hyfi/__click__.py
--rw-r--r--   0        0        0     1183 2023-07-23 20:11:17.362104 hyfi-1.8.3/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-23 20:11:48.756082 hyfi-1.8.3/src/hyfi/_version.py
--rw-r--r--   0        0        0     1497 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24360 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      193 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0     1053 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      955 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      876 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      738 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      338 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     4683 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10023 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5514 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3266 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5695 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-23 20:11:17.366105 hyfi-1.8.3/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    19642 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4327 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8383 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5822 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7164 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1184 2023-07-23 20:11:17.370106 hyfi-1.8.3/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 11:17:34.959035 hyfi-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-24 11:17:34.959035 hyfi-1.9.0/README.md
+-rw-r--r--   0        0        0     4852 2023-07-24 11:18:08.798650 hyfi-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4346 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0     1213 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 11:18:08.702639 hyfi-1.9.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1497 2023-07-24 11:17:34.963035 hyfi-1.9.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24454 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0     1053 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      955 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      876 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      738 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      338 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5784 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10023 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5783 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3344 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5744 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-24 11:17:34.967035 hyfi-1.9.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    19733 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4327 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8383 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5822 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7164 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1184 2023-07-24 11:17:34.971036 hyfi-1.9.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.9.0/PKG-INFO
```

### Comparing `hyfi-1.8.3/LICENSE` & `hyfi-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/README.md` & `hyfi-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/pyproject.toml` & `hyfi-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.8.3"
+version = "1.9.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
-hyfi = 'hyfi.__cli__:hydra_main'
+hyfi = 'hyfi.__cli__:hyfi_main'
 hyfi-run = 'hyfi.__click__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
 pydantic = "2.0.3"
```

### Comparing `hyfi-1.8.3/src/hyfi/__cli__.py` & `hyfi-1.9.0/src/hyfi/__cli__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     HyFI.terminate()
 
 
 def hyfi_main(
     config_path: Optional[str] = None,
     config_name: Optional[str] = None,
     overrides: Optional[List[str]] = None,
+    plugins: Optional[List[str]] = None,
 ) -> None:
     """
     Main function for the command line interface of Hydra
 
     Args:
         config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
@@ -73,42 +74,46 @@
     """
     if search_path := __global_hyfi__.user_config_path:
         sys.argv.append(f"--config-dir={search_path}")
     if not config_path:
         config_path = __global_hyfi__.config_module_path
     if not config_name:
         config_name = __global_hyfi__.config_name
+    if not plugins:
+        plugins = __global_hyfi__.plugins
     if __global_hyfi__.__package_name__ != __hyfi_package_name__:
         overrides = overrides or []
         override = f"about={__global_hyfi__.__package_name__}"
         if override not in overrides:
             overrides.append(override)
             logger.debug(
                 "Overriding `about` config group with `%s`",
                 __global_hyfi__.__package_name__,
             )
     hyfi_hydra_main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
         overrides=overrides,
+        plugins=plugins,
     )(cli_main)()
 
 
 def hydra_main(
     config_path: Optional[str] = None,
     config_name: Optional[str] = None,
     overrides: Optional[List[str]] = None,
+    plugins: Optional[List[str]] = None,
 ) -> None:
     """
     Main function for the command line interface of Hydra
 
     Args:
         config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
-    hyfi_main(config_path, config_name, overrides)
+    hyfi_main(config_path, config_name, overrides, plugins)
```

### Comparing `hyfi-1.8.3/src/hyfi/__click__.py` & `hyfi-1.9.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/__init__.py` & `hyfi-1.9.0/src/hyfi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "hydra_main",
     "hyfi_main",
     "HyFI",
     "H",
     "HI",
     "LOGGING",
     "__hydra_version_base__",
+    "initialize_global_hyfi",
 ]
 
 
 def initialize_global_hyfi(
     package_name: str,
     version: str,
 ) -> None:
```

### Comparing `hyfi-1.8.3/src/hyfi/about/__init__.py` & `hyfi-1.9.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/batch/__init__.py` & `hyfi-1.9.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/__init__.py` & `hyfi-1.9.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.9.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/cache_file.py` & `hyfi-1.9.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/common.py` & `hyfi-1.9.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/file_lock.py` & `hyfi-1.9.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/meta.py` & `hyfi-1.9.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/progress.py` & `hyfi-1.9.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.9.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.9.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.9.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.9.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.9.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/testing.py` & `hyfi-1.9.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/cached_path/util.py` & `hyfi-1.9.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/composer/__init__.py` & `hyfi-1.9.0/src/hyfi/composer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,26 +199,28 @@
         return self._cfg_
 
     @staticmethod
     def hydra_compose(
         root_config_name: Optional[str] = None,
         config_module: Optional[str] = None,
         overrides: Optional[List[str]] = None,
+        plugins: Optional[List[str]] = None,
     ):
         is_initialized = GlobalHydra.instance().is_initialized()  # type: ignore
         config_module = config_module or __global_hyfi__.hyfi_config_module
         logger.debug("config_module: %s", config_module)
         if is_initialized:
             # Hydra is already initialized.
             logger.debug("Hydra is already initialized")
             cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         else:
             with hyfi_hydra.initialize_config(
                 config_module=config_module,
                 config_dir=__global_hyfi__.hyfi_user_config_path,
+                plugins=__global_hyfi__.plugins,
                 version_base=__hydra_version_base__,
             ):
                 cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         return cfg
 
     @staticmethod
     def split_config_group(
```

### Comparing `hyfi-1.8.3/src/hyfi/composer/base.py` & `hyfi-1.9.0/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/composer/pydantic.py` & `hyfi-1.9.0/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.9.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.9.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/copier/__init__.py` & `hyfi-1.9.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/core/__init__.py` & `hyfi-1.9.0/src/hyfi/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+"""
+    HyFI Core Module
+"""
+import importlib
 import os
 from pathlib import Path
+from typing import Any, List, Optional
 
 from pydantic import BaseModel
 
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
@@ -36,34 +41,62 @@
 
     Attributes:
     __package_name__ (str): The name of the package.
     __package_path__ (str): The path to the package root folder.
     __config_name__ (str): The name of the configuration module.
     __config_path__ (str): The path to the configuration module.
     __user_config_path__ (str): The path to the user configuration directory.
+    __plugins__ (List[Any]): A list of plugins to load.
     __version__ (str): The version number of the package.
     """
 
     __package_name__: str = __hyfi_package_name__
     __package_path__: str = __hyfi_package_path__
     __config_name__: str = __hyfi_config_name__
     __config_path__: str = __hyfi_config_path__
     __user_config_path__: str = "config"
+    __plugins__: Optional[List[str]] = None
     __version__: str = __hyfi_version__()
 
     def initialize(
         self,
         package_name: str = __hyfi_name__,
         version: str = __hyfi_version__(),
+        plugins: Optional[List[str]] = None,
     ) -> None:
         """
         Initializes the global HyFI instance.
         """
         self.__package_name__ = package_name
         self.__version__ = version
+        if plugins:
+            self.__plugins__ = self.get_plugins(plugins)
+
+    @property
+    def plugins(self) -> Optional[List[str]]:
+        """Returns the list of plugins to load."""
+        return self.__plugins__
+
+    def get_plugins(self, plugins: List[str]) -> List[str]:
+        """Returns the list of plugins to load."""
+        _plugins = []
+        for plugin in plugins:
+            H = self._safe_import_module(plugin)
+            if H and getattr(H, "config_module", None):
+                _plugins.append(H.config_module)
+        return _plugins
+
+    @staticmethod
+    def _safe_import_module(module_name: str) -> Any:
+        """Safely imports a module."""
+        try:
+            return importlib.import_module(module_name).HyFI
+        except ImportError:
+            logger.debug("Failed to import module: %s", module_name)
+            return None
 
     @property
     def version(self) -> str:
         """Returns the version number of the package."""
         return self.__version__
 
     @property
```

### Comparing `hyfi-1.8.3/src/hyfi/core/config.py` & `hyfi-1.9.0/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/core/hydra/__init__.py` & `hyfi-1.9.0/src/hyfi/core/hydra/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 import copy
 import os
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from hydra import version
 from hydra._internal.config_search_path_impl import ConfigSearchPathImpl
 from hydra._internal.hydra import Hydra
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.core.global_hydra import GlobalHydra
 from hydra.core.singleton import Singleton
@@ -65,14 +65,15 @@
         job_name: the value for hydra.job.name (default is 'app')
     """
 
     def __init__(
         self,
         config_module: str,
         config_dir: Optional[str] = None,
+        plugins: Optional[List[str]] = None,
         job_name: str = "app",
         version_base: Optional[str] = _UNSPECIFIED_,
     ) -> None:
         self._gh_backup = get_gh_backup()
 
         version.setbase(version_base)
 
@@ -80,15 +81,15 @@
         # may have unexpected meaning. best to force an absolute path to avoid confusion.
         # Can consider using hydra.utils.to_absolute_path() to convert it at a future point if there is demand.
         if config_dir and not os.path.isabs(config_dir):
             raise HydraException(
                 "initialize_config_dir() requires an absolute config_dir as input"
             )
         csp = create_config_search_path(
-            config_module=config_module, search_path_dir=config_dir
+            config_module=config_module, search_path_dir=config_dir, plugins=plugins
         )
         Hydra.create_main_hydra2(task_name=job_name, config_search_path=csp)
 
     def __enter__(self, *args: Any, **kwargs: Any) -> None:
         ...
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
@@ -103,36 +104,42 @@
         logger.debug(
             "Not adding empty path to Hydra's config search path for `%s`", provider
         )
         return
     for sp_item in search_path.get_path():
         if sp_item.path == path:
             logger.debug(
-                "Not adding `%s` to Hydra's config search path, it was already added by `%s`",
+                "Not adding `%s` to Hydra's config search path for `%s` because it is already there by `%s`",
                 path,
+                provider,
                 sp_item.provider,
             )
             return
     logger.debug("Adding `%s` to Hydra's config search path for `%s`", path, provider)
     search_path.append(provider, path)
 
 
 def create_config_search_path(
     config_module: Optional[str],
     search_path_dir: Optional[str],
+    plugins: Optional[List[str]],
 ) -> ConfigSearchPath:
     from hydra.core.plugins import Plugins
     from hydra.plugins.search_path_plugin import SearchPathPlugin
 
     search_path = ConfigSearchPathImpl()
     search_path.append("hydra", "pkg://hydra.conf")
 
     # addiing hyfi's config module to the search path should come before the other modules
     append_search_path("hyfi", f"pkg://{__hyfi_config_module_path__}", search_path)
 
+    if plugins:
+        for plugin in plugins:
+            append_search_path("hyfi-plugin", f"pkg://{plugin}", search_path)
+
     if config_module:
         path = (
             config_module
             if config_module.startswith("pkg://")
             else f"pkg://{config_module}"
             if "." in config_module
             else ""
```

### Comparing `hyfi-1.8.3/src/hyfi/core/hydra/main.py` & `hyfi-1.9.0/src/hyfi/core/hydra/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 def main(
     config_path: Optional[str] = _UNSPECIFIED_,
     config_name: Optional[str] = None,
     version_base: Optional[str] = _UNSPECIFIED_,
     overrides: Optional[List[str]] = None,
+    plugins: Optional[List[str]] = None,
 ) -> Callable[[TaskFunction], Any]:
     """
     :param config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
@@ -71,12 +72,13 @@
                 # multiple times (--multirun)
                 _run_hydra(
                     args=args,
                     args_parser=args_parser,
                     task_function=task_function,
                     config_path=config_path,
                     config_name=config_name,
+                    plugins=plugins,
                 )
 
         return decorated_main
 
     return main_decorator
```

### Comparing `hyfi-1.8.3/src/hyfi/core/hydra/utils.py` & `hyfi-1.9.0/src/hyfi/core/hydra/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 import argparse
 import logging.config
 import os
 import sys
-from typing import Optional
+from typing import List, Optional
 
 from hydra._internal.utils import (
     _run_app,
     detect_calling_file_or_module_from_stack_frame,
     detect_calling_file_or_module_from_task_function,
     detect_task_name,
     run_and_report,
@@ -21,14 +21,15 @@
 
 def _run_hydra(
     args: argparse.Namespace,
     args_parser: argparse.ArgumentParser,
     task_function: TaskFunction,
     config_path: Optional[str],
     config_name: Optional[str],
+    plugins: Optional[List[str]],
     caller_stack_depth: int = 2,
 ) -> None:
     from hydra._internal.hydra import Hydra
     from hydra.core.global_hydra import GlobalHydra
 
     if args.config_name is not None:
         config_name = args.config_name
@@ -44,15 +45,15 @@
         (
             calling_file,
             calling_module,
         ) = detect_calling_file_or_module_from_stack_frame(caller_stack_depth + 1)
     task_name = detect_task_name(calling_file, calling_module)
 
     abs_config_dir = os.path.abspath(args.config_dir) if args.config_dir else None
-    search_path = create_config_search_path(config_path, abs_config_dir)
+    search_path = create_config_search_path(config_path, abs_config_dir, plugins)
     # validate_config_path(config_path)
     # search_path = create_automatic_config_search_path(
     #     calling_file, calling_module, config_path
     # )
 
     # def add_conf_dir() -> None:
     #     if args.config_dir is not None:
```

### Comparing `hyfi-1.8.3/src/hyfi/dotenv/__init__.py` & `hyfi-1.9.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/graphics/__init__.py` & `hyfi-1.9.0/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/graphics/collage.py` & `hyfi-1.9.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/graphics/motion.py` & `hyfi-1.9.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/graphics/utils.py` & `hyfi-1.9.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/joblib/__init__.py` & `hyfi-1.9.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/joblib/batch/apply.py` & `hyfi-1.9.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.9.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.9.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/main/__init__.py` & `hyfi-1.9.0/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,18 @@
     LOGGING,
     NBs,
     PIPELINEs,
     PKGs,
 ):
     """Primary class for the hyfi config package"""
 
-    config = __global_config__
+    global_config = __global_config__
+    global_hyfi = __global_hyfi__
     SpeicialKeys = SpecialKeys
+    config_module = __global_hyfi__.config_module
     __version__ = __hyfi_version__()
     __hyfi_path__ = __hyfi_path__()
     __home_path__ = __home_path__()
     __package_name__ = __package_name__()
     __package_path__ = __package_path__()
     __app_version__ = __app_version__()
```

### Comparing `hyfi-1.8.3/src/hyfi/path/__init__.py` & `hyfi-1.9.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/path/base.py` & `hyfi-1.9.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/path/batch.py` & `hyfi-1.9.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/path/dirnames.py` & `hyfi-1.9.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/path/task.py` & `hyfi-1.9.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/pipe/__init__.py` & `hyfi-1.9.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/pipe/datasets.py` & `hyfi-1.9.0/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/pipe/test.py` & `hyfi-1.9.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/pipeline/__init__.py` & `hyfi-1.9.0/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/pipeline/configs.py` & `hyfi-1.9.0/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/project/__init__.py` & `hyfi-1.9.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/task/__init__.py` & `hyfi-1.9.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/task/batch.py` & `hyfi-1.9.0/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/conf.py` & `hyfi-1.9.0/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/contexts.py` & `hyfi-1.9.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/datasets.py` & `hyfi-1.9.0/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/envs.py` & `hyfi-1.9.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/funcs.py` & `hyfi-1.9.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/gpumon.py` & `hyfi-1.9.0/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/iolibs.py` & `hyfi-1.9.0/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/logging.py` & `hyfi-1.9.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/notebooks.py` & `hyfi-1.9.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/utils/packages.py` & `hyfi-1.9.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/src/hyfi/workflow/__init__.py` & `hyfi-1.9.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.8.3/PKG-INFO` & `hyfi-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.8.3
+Version: 1.9.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

