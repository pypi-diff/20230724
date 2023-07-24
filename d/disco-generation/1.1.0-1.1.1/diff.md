# Comparing `tmp/disco-generation-1.1.0.tar.gz` & `tmp/disco-generation-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disco-generation-1.1.0.tar", last modified: Fri Jun 30 14:27:55 2023, max compression
+gzip compressed data, was "disco-generation-1.1.1.tar", last modified: Mon Jul 24 14:11:52 2023, max compression
```

## Comparing `disco-generation-1.1.0.tar` & `disco-generation-1.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.212954 disco-generation-1.1.0/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21077 2023-05-09 12:38:18.000000 disco-generation-1.1.0/LICENSE
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3586 2023-06-30 14:27:55.211954 disco-generation-1.1.0/PKG-INFO
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.080955 disco-generation-1.1.0/disco/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      173 2023-06-30 09:33:57.000000 disco-generation-1.1.0/disco/__init__.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.099955 disco-generation-1.1.0/disco/distributions/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      438 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     5295 2023-06-09 09:08:25.000000 disco-generation-1.1.0/disco/distributions/base_distribution.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1986 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/context_distribution.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2431 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/dataset_context_distribution.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      538 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/distribution.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     9812 2023-06-14 14:05:23.000000 disco-generation-1.1.0/disco/distributions/lm_distribution.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1441 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/distributions/single_context_distribution.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.112955 disco-generation-1.1.0/disco/metrics/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      175 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1052 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/base.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1843 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/js.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1571 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/kl.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1372 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/metrics/tv.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.124955 disco-generation-1.1.0/disco/samplers/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      259 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1951 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/accumulation_sampler.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     6839 2023-06-21 14:04:06.000000 disco-generation-1.1.0/disco/samplers/quasi_rejection_sampler.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      401 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/samplers/sampler.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.138954 disco-generation-1.1.0/disco/scorers/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      361 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1476 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/boolean_scorer.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1978 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/exponential_scorer.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1299 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/pipeline_scorer.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2437 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/positive_scorer.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1163 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/scorers/scorer.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.153954 disco-generation-1.1.0/disco/tuners/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      279 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1127 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/cdpg_tuner.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1020 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/dpg_tuner.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1153 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/fcdpg_tuner.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1161 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/fdpg_tuner.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.168954 disco-generation-1.1.0/disco/tuners/loggers/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      118 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      982 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/base.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      854 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/console.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3020 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/json.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1991 2023-06-14 12:51:08.000000 disco-generation-1.1.0/disco/tuners/loggers/neptune.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1430 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/loggers/wandb.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.184954 disco-generation-1.1.0/disco/tuners/losses/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      225 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      249 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/losses/base.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2235 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/js.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2123 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/tuners/losses/kl.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2261 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/reverse_kl.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2125 2023-05-25 09:00:48.000000 disco-generation-1.1.0/disco/tuners/losses/tv.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21279 2023-06-21 14:04:06.000000 disco-generation-1.1.0/disco/tuners/tuner.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.195954 disco-generation-1.1.0/disco/utils/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      234 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/__init__.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      893 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/device.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1155 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/helpers.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2145 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/moving_average.py
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      655 2023-05-25 09:00:37.000000 disco-generation-1.1.0/disco/utils/observable.py
-drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-06-30 14:27:55.208954 disco-generation-1.1.0/disco_generation.egg-info/
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3586 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/PKG-INFO
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1591 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/SOURCES.txt
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        1 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/dependency_links.txt
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       76 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/requires.txt
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        6 2023-06-30 14:27:54.000000 disco-generation-1.1.0/disco_generation.egg-info/top_level.txt
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       38 2023-06-30 14:27:55.213954 disco-generation-1.1.0/setup.cfg
--rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3881 2023-06-30 13:55:16.000000 disco-generation-1.1.0/setup.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.348917 disco-generation-1.1.1/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21077 2023-05-09 12:38:18.000000 disco-generation-1.1.1/LICENSE
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3212 2023-07-24 14:11:52.346917 disco-generation-1.1.1/PKG-INFO
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.173919 disco-generation-1.1.1/disco/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      173 2023-07-24 14:06:03.000000 disco-generation-1.1.1/disco/__init__.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.196918 disco-generation-1.1.1/disco/distributions/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      438 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/distributions/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     5295 2023-06-09 09:08:25.000000 disco-generation-1.1.1/disco/distributions/base_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1986 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/distributions/context_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2431 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/distributions/dataset_context_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      538 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/distributions/distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    12806 2023-07-24 14:05:28.000000 disco-generation-1.1.1/disco/distributions/lm_distribution.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1441 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/distributions/single_context_distribution.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.212918 disco-generation-1.1.1/disco/metrics/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      175 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/metrics/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1052 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/metrics/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1843 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/metrics/js.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1571 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/metrics/kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1372 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/metrics/tv.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.227918 disco-generation-1.1.1/disco/samplers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      259 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/samplers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1951 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/samplers/accumulation_sampler.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     6839 2023-07-13 13:42:02.000000 disco-generation-1.1.1/disco/samplers/quasi_rejection_sampler.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      401 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/samplers/sampler.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.248918 disco-generation-1.1.1/disco/scorers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      361 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1476 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/boolean_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1978 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/exponential_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1299 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/pipeline_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2437 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/positive_scorer.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1163 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/scorers/scorer.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.269918 disco-generation-1.1.1/disco/tuners/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      279 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1127 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/cdpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1020 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/dpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1153 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/fcdpg_tuner.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1161 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/fdpg_tuner.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.289917 disco-generation-1.1.1/disco/tuners/loggers/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      118 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/loggers/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      982 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/loggers/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      854 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/loggers/console.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3020 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/loggers/json.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1991 2023-06-14 12:51:08.000000 disco-generation-1.1.1/disco/tuners/loggers/neptune.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1430 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/loggers/wandb.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.310917 disco-generation-1.1.1/disco/tuners/losses/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      225 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/losses/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      249 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/losses/base.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2235 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/losses/js.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2123 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/tuners/losses/kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2261 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/losses/reverse_kl.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2125 2023-05-25 09:00:48.000000 disco-generation-1.1.1/disco/tuners/losses/tv.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)    21279 2023-07-13 13:42:02.000000 disco-generation-1.1.1/disco/tuners/tuner.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.327917 disco-generation-1.1.1/disco/utils/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      234 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/utils/__init__.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      893 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/utils/device.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1155 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/utils/helpers.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     2145 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/utils/moving_average.py
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)      655 2023-05-25 09:00:37.000000 disco-generation-1.1.1/disco/utils/observable.py
+drwxr-xr-x   0 gkruszew (1809414312) domain users (1809400513)        0 2023-07-24 14:11:52.343917 disco-generation-1.1.1/disco_generation.egg-info/
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3212 2023-07-24 14:11:51.000000 disco-generation-1.1.1/disco_generation.egg-info/PKG-INFO
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     1591 2023-07-24 14:11:51.000000 disco-generation-1.1.1/disco_generation.egg-info/SOURCES.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        1 2023-07-24 14:11:51.000000 disco-generation-1.1.1/disco_generation.egg-info/dependency_links.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       76 2023-07-24 14:11:51.000000 disco-generation-1.1.1/disco_generation.egg-info/requires.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)        6 2023-07-24 14:11:51.000000 disco-generation-1.1.1/disco_generation.egg-info/top_level.txt
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)       38 2023-07-24 14:11:52.349917 disco-generation-1.1.1/setup.cfg
+-rw-r--r--   0 gkruszew (1809414312) domain users (1809400513)     3555 2023-07-24 14:05:51.000000 disco-generation-1.1.1/setup.py
```

### Comparing `disco-generation-1.1.0/LICENSE` & `disco-generation-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/PKG-INFO` & `disco-generation-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,48 @@
-Metadata-Version: 2.1
-Name: disco-generation
-Version: 1.1.0
-Summary: A toolkit for distributional control of generative models
-Home-page: https://github.com/naver/disco
-Author: Naver Labs Europe
-Author-email: jos.rozen@naverlabs.com
-License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0
-Description: The 🕺🏽 **disco** toolkit allows to control language models and other generative systems to match human preferences while avoiding catastrophic forgetting.
-        
-        To achieve this, **disco** decouples the problem of expressing _what_ properties the model should have from _how_ to actually get the desired model as separate steps.
-        
-        **Step 1: ⚓ We express how the target distribution *should* be**
-        
-        First, we define some feature over the generated samples that matters to us. It can be anything we can compute. For example, on a language model it can be as simple as whether the generated text contains a certain word or as complex as the compilability of some generated piece of code. Importantly, there is no need for the feature to be differentiable.
-        
-        Then, we can express our preferences on the target distribution by deciding how prevalent the feature should be. For example, we might want to ask that a certain word appears 50% of the time when sampling from the model; or that 100% of the generated code is compilable. The resulting target distribution is expressed as an energy-based model or EBM, which is an unnormalized probability distribution that respects the desired moments while avoiding catastrophic forgetting, as a result of having minimal KL divergence to the original model.
-        
-        The resulting representation of the target distribution can *score* samples, but cannot directly be used to *generate* them.
-        
-        **Step 2: 🎯 Approximate the target distribution**
-        
-        To generate samples from the target distribution we can tune a model to approximate it. We do this by minimizing the divergence to the target distribution. While techniques such as reinforcement learning from human feedback (RLHF) are restricted to using one kind of divergence only (specifically, reverse KL divergence), **disco** is more general, allowing the use of the full class of f-divergences, including both forward and reverse KL divergence, Jensen-Shannon, and total variation distance.
-        
-        **Step 3: 💬 Generate content that matches the preferences**
-        
-        The resulting model can generate samples directly from a close approximation of the target distribution. Furthermore, it can be used jointly with Quasi-Rejection Sampling (QRS), a Monte Carlo sampling technique that allows the generation of samples that are even more representative of the target distribution.
-        Alternatively, it is then possible to use decoding methods such as nucleus sampling, top-k sampling, or beam search, which would return samples from a further updated target distribution.
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Free for non-commercial use
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
+# disco
+# Copyright (C) 2022-present NAVER Corp.
+# Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
+
+from setuptools import setup, find_packages
+
+setup(
+    name='disco-generation',
+    version='1.1.1',
+    description='A toolkit for distributional control of generative models',
+    url='https://github.com/naver/disco',
+    author='Naver Labs Europe', author_email='jos.rozen@naverlabs.com',
+    license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0',
+    long_description="""The 🕺🏽 **disco** toolkit allows to control the properties of the generations by language models and other generative systems to match human preferences while avoiding catastrophic forgetting.
+
+To achieve this in **disco**, we first represent in what ways we want to update original model as a target distribution and then, generate samples from this new distribution through a combination of learning or monte-carlo methods, as follows.
+
+**Step 1: We express how the target distribution *should* be**
+
+To have a handle on the generative model, we define some feature over the generated samples. It can be anything we can compute. For example, on a language model it can be as simple as whether the generated text contains a certain word or as complex as the compilability of some generated piece of code. Importantly, there is no need for the feature to be differentiable.  
+Then, we can express our preferences on the target distribution by defining the target *moments* of this feature. For example, we might want to ask that a certain word appears 50% of the time when sampling from the model; or that 100% of the generated code is compilable. The resulting target distribution is expressed as an energy-based model or EBM, which is an unnormalized probability distribution that respects the desired moments while avoiding catastrophic forgetting, as a result of having minimal KL divergence to the original model.  
+This representation of the target distribution can *score* samples, but cannot directly be used to *generate* them.
+
+**Step 2: We generate samples from the target distribution**
+
+To generate samples from the target distribution, if not perfectly, we can tune a model to approximate it. The resulting model can generate samples directly from a close approximation of the target distribution. Furthermore, it can be used jointly with Quasi-Rejection Sampling (QRS), a Monte Carlo sampling technique that allows the generation of samples that are even more representative of the target distribution.  
+Alternatively, it is then possible to use decoding methods such as nucleus sampling, top-k sampling, or beam search, which would return samples from a further updated target distribution.""",
+    long_description_content_type='text/markdown',
+    packages=find_packages(include=['disco', 'disco.*']),
+    python_requires='>=3.8, <3.11',
+    install_requires=['torch', 'transformers',
+            'numpy', 'scipy',
+            'datasets', 'spacy',
+            'notebook',
+            'neptune-client', 'wandb'],
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Science/Research',
+        'License :: Free for non-commercial use',
+        'Operating System :: POSIX :: Linux',
+        'Operating System :: MacOS',
+        'Operating System :: Microsoft :: Windows',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+)
```

### Comparing `disco-generation-1.1.0/disco/distributions/base_distribution.py` & `disco-generation-1.1.1/disco/distributions/base_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/distributions/context_distribution.py` & `disco-generation-1.1.1/disco/distributions/context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/distributions/dataset_context_distribution.py` & `disco-generation-1.1.1/disco/distributions/dataset_context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/distributions/distribution.py` & `disco-generation-1.1.1/disco/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/distributions/lm_distribution.py` & `disco-generation-1.1.1/disco/distributions/lm_distribution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # disco
 # Copyright (C) 2022-present NAVER Corp.
 # Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license
 
 import torch
-from transformers import AutoTokenizer, AutoModelForCausalLM, AutoModelForSeq2SeqLM
+import copy
+from transformers import AutoTokenizer, AutoModelForCausalLM, AutoModelForSeq2SeqLM, LogitsProcessorList
 
 from collections import namedtuple
 
 from .base_distribution import BaseDistribution
 from disco.utils.helpers import get_token_first_indices
 
 
@@ -24,15 +25,15 @@
             length=40, device="cpu",
             **config
         ):
         """
         Parameters
         ----------
         model: string
-            Transformers' name of a causal or seq2seq language model 
+            Transformers' name of a causal or seq2seq language model
         tokenizer: string
             Transformers' name for the related tokenizer
         auto: class
             auto class from Transformers, default is AutoModelForCausalLM
             but AutoModelForSeq2SeqLM is also valid
         freeze: boolean
             flag to eventually (not) freeze the network's parameters
@@ -43,15 +44,15 @@
         config: kwarg
             parameters and values passed to transformers' ```generate(…)```
         """
 
         self.tokenizer= AutoTokenizer.from_pretrained(tokenizer if tokenizer else model)
         assert auto in [AutoModelForCausalLM, AutoModelForSeq2SeqLM], "only AutoModel, AutoModelForCausalLM and AutoModelForSeq2SeqLM are valid options."
         self._load_network(auto, model)
-    
+
         self.device = device
         self.network.to(self.device)
         self.network.eval() # to make sure scoring is consistent
         if freeze:
             self.freeze(True)
 
         self.length = length
@@ -84,15 +85,15 @@
         """Freeze (or unfreeze) parameters for gradient computation.
 
         Parameters
         ----------
         frozen: boolean (True)
             state to transition to, default is to freeze
         """
- 
+
         self.network.requires_grad_(not frozen)
 
     def log_score(self, samples, context="", grad=False, sum=True):
         """Computes log-probabilities for the samples according
         to the language model network in the given context
 
         Parameters
@@ -106,139 +107,198 @@
         sum: boolean
             flag to eventually return token-level tensor of scores
 
         Returns
         -------
         tensor of log-probabilities
         """
-
         assert self.scorable, "this distribution's parameters make it unscorable."
         shapes = set([s.token_ids.shape for s in samples])
         assert 1 == len(shapes), "sequences of token_ids should have the same shape, but got: {shapes}."
 
-        device = self.device
+        if self.network.config.is_encoder_decoder:
+            assert context is not None and context != "", "context (encoder input) is mandatory for encoder-decoder models"
+        elif not context:
+            context = self.tokenizer.bos_token
 
-        if not self.network.config.is_encoder_decoder:
-            context = self.tokenizer.bos_token if "" == context else context
         tokenized_context = self.tokenizer([context] * len(samples), return_tensors="pt", add_special_tokens=True)
-        tokenized_context["input_ids"] = tokenized_context["input_ids"].to(device)
-        tokenized_context["attention_mask"] = tokenized_context["attention_mask"].to(device)
+        tokenized_context["input_ids"] = tokenized_context["input_ids"].to(self.device)
+        tokenized_context["attention_mask"] = tokenized_context["attention_mask"].to(self.device)
 
         tokenized_samples = dict()
-        tokenized_samples["input_ids"] = torch.stack([sample.token_ids for sample in samples]).to(device)
+        tokenized_samples["input_ids"] = torch.stack([sample.token_ids for sample in samples]).to(self.device)
+
+        tokenized_samples = self._discount_padding_tokens(tokenized_samples)
+
+        input_ids, encoder_input_ids, forward_kwargs, labels, prompt_length, last  = \
+                self._get_forward_inputs(tokenized_context, tokenized_samples, samples)
+
+        if grad:
+            outputs = self.network(**forward_kwargs, labels=labels)
+        else:
+            with torch.no_grad():
+                outputs = self.network(**forward_kwargs, labels=labels)
+
+        all_logits = outputs.logits[:, prompt_length:last, :] # [n_samples, length, vocab]
+
+        all_logits = self._process_and_warp_logits(all_logits, input_ids, encoder_input_ids)
+
+        all_logprobs = all_logits.log_softmax(-1)
+
+        seq_logprobs = torch.gather(
+                all_logprobs, 2, tokenized_samples["input_ids"][:, :, None]
+            ).squeeze(-1) # [n_samples, length]
+
+        seq_logprobs = torch.where(1 == tokenized_samples["attention_mask"], seq_logprobs, torch.tensor(0.).to(self.device))
+
+        return seq_logprobs.sum(dim=1) if sum else seq_logprobs
 
+    def _discount_padding_tokens(self, tokenized_samples):
         first_eos_indices = get_token_first_indices(
                 tokenized_samples["input_ids"],
                 self.tokenizer.eos_token_id
             )
         tokenized_samples["attention_mask"] = torch.where(
                 self.tokenizer.pad_token_id == tokenized_samples["input_ids"],
                 0, 1
             )
         for i, ix in enumerate(first_eos_indices):
             if None != self.network.config.forced_bos_token_id and\
                 self.network.config.forced_bos_token_id == tokenized_samples["input_ids"][i][0]:
                     tokenized_samples["attention_mask"][i][0] = 0
             else:
                 tokenized_samples["attention_mask"][i][0] = 1  # at least score one token
-            if ix != -1:  # if there is an eos token
-                tokenized_samples["attention_mask"][i][ix] = 1  # score first eos token
+            if ix != -1:  # if there is an pad token
+                tokenized_samples["attention_mask"][i][ix] = 1  # score first pad token
                 tokenized_samples["attention_mask"][i][ix + 1:] = 0  # ignore everything after it
-        tokenized_samples["attention_mask"] = tokenized_samples["attention_mask"].to(device)
+        tokenized_samples["attention_mask"] = tokenized_samples["attention_mask"].to(self.device)
+        return tokenized_samples
 
+
+    def _get_forward_inputs(self, tokenized_context, tokenized_samples, samples):
         if self.network.config.is_encoder_decoder:
-            shift = None
-            last = None
-            inputs = tokenized_context
-            labels = tokenized_samples["input_ids"]
+            prompt_length = None
+            last = -1
+            encoder_input_ids = tokenized_context["input_ids"]
+            input_ids = tokenized_samples["input_ids"]
+            forward_kwargs = {
+                "input_ids": encoder_input_ids,
+                "decoder_input_ids": input_ids,
+            }
+            input_ids, forward_kwargs = self.network._prepare_decoder_input_ids_for_generation(len(samples),
+                "decoder_input_ids",
+                forward_kwargs)
+            forward_kwargs['decoder_input_ids'] = input_ids
+            labels = forward_kwargs["decoder_input_ids"]
         else:
-            shift = tokenized_context["input_ids"].shape[-1] - 1
+            prompt_length = tokenized_context["input_ids"].shape[-1] - 1
             last = -1
-            inputs = {
-                "input_ids": torch.cat((tokenized_context["input_ids"], tokenized_samples["input_ids"]), 1),
+            encoder_input_ids = None
+            input_ids = torch.cat((tokenized_context["input_ids"], tokenized_samples["input_ids"]), 1)
+            forward_kwargs = {
+                "input_ids": input_ids,
                 "attention_mask": torch.cat((tokenized_context["attention_mask"], tokenized_samples["attention_mask"]), 1)
             }
-            labels = inputs["input_ids"]
+            labels = forward_kwargs["input_ids"]
 
-        if grad:
-            outputs = self.network(**inputs, labels=labels)
-        else:
-            with torch.no_grad():
-                outputs = self.network(**inputs, labels=labels)
-    
-        all_logprobs = outputs.logits[:, shift:last, :].log_softmax(-1) # [n_samples, length, vocab]
-        seq_logprobs = torch.gather(
-                all_logprobs, 2, tokenized_samples["input_ids"][:, :, None]
-            ).squeeze(-1) # [n_samples, length]
+        return input_ids, encoder_input_ids, forward_kwargs, labels, prompt_length, last
 
-        seq_logprobs = torch.where(1 == tokenized_samples["attention_mask"], seq_logprobs, torch.tensor(0.).to(device))
 
-        return seq_logprobs.sum(dim=1) if sum else seq_logprobs 
+    def _process_and_warp_logits(self, all_logits, input_ids, encoder_input_ids):
+        generation_config = copy.deepcopy(self.network.generation_config)
+        generation_config.update(**self.params)
+
+        logits_warper = self.network._get_logits_warper(generation_config)
+
+        logits_processor = self.network._get_logits_processor(
+            generation_config=generation_config,
+            input_ids_seq_length=input_ids.shape[-1],
+            encoder_input_ids=encoder_input_ids,
+            prefix_allowed_tokens_fn=None,
+            logits_processor=LogitsProcessorList()
+        )
+
+        for i in range(all_logits.shape[1]): # [n_samples, length, vocab]
+            all_logits[:,i,:] = logits_processor(input_ids[:,:i+1], all_logits[:,i,:])
+            all_logits[:,i,:] = logits_warper(input_ids[:,:i+1], all_logits[:,i,:])
+
+        return all_logits
 
     def sample(self, context="", sampling_size=32, sum=True):
         """Samples sequences from the language model in the given context
-        
+
         Parameters
         ----------
         context: text
             contextual text for which to sample
         sampling_size: int
             number of sequences to sample
         sum: Boolean
             flag to eventually return token-level tensor of scores
-        
+
         Returns
         -------
         tuple of (list of Sample(tokens, text), tensor of logprobs)
         """
-    
-        if not self.network.config.is_encoder_decoder and not context:
+        if self.network.config.is_encoder_decoder:
+            assert context is not None and context != "", "context (encoder input) is mandatory for encoder-decoder models"
+        elif not context:
             context = self.tokenizer.bos_token
+
         input_ids = self.tokenizer([context] * sampling_size, return_tensors="pt", add_special_tokens=True).input_ids.to(self.device)
         n_context_tokens = input_ids.shape[-1]
 
+        generate_kwargs = dict(self.params)
+
+        # encoder-decoder models have a hard-coded prompt with the context used for the encoder
+        # In contrast, decoder-only models use the context as a prompt.
         if self.network.config.is_encoder_decoder:
-            shift = 1
+            prompt_length = 1
             last = None
+            torch.tensor([self.tokenizer.bos_token_id] * sampling_size).unsqueeze(-1).to(self.device)
+            decoder_input_ids, generate_kwargs = self.network._prepare_decoder_input_ids_for_generation(sampling_size,
+                    "decoder_input_ids",
+                    generate_kwargs)
+            generate_kwargs["decoder_input_ids"] = decoder_input_ids
         else:
-            shift = n_context_tokens
+            prompt_length = n_context_tokens
             last = None
 
         outputs = self.network.generate(input_ids,
             output_scores=True, return_dict_in_generate=True,
             max_new_tokens=self.length,
-            do_sample=True, **self.params)
+            do_sample=True, **generate_kwargs)
 
         all_logprobs = torch.stack(outputs.scores, dim=1).log_softmax(-1)  # [sampling_size, length, vocab]
         token_seq_logprobs = torch.gather(
-                all_logprobs, 2, outputs.sequences[:, shift:last][:, :, None]
+                all_logprobs, 2, outputs.sequences[:, prompt_length:last][:, :, None]
             ).squeeze(-1) # [sampling_size, length]
 
         # we need to zero the (log-)scores of extra <eos>
         first_eos_indices = get_token_first_indices(
-                outputs.sequences[:, shift:last],  # starting at 1 to skip an eventual bos token
+                outputs.sequences[:, prompt_length:last],  # starting at 1 to skip an eventual bos token
                 self.tokenizer.eos_token_id
             )
         non_pad_tokens = torch.cat(
-                (outputs.sequences[:, shift:last][:, 0].unsqueeze(1),
+                (outputs.sequences[:, prompt_length:last][:, 0].unsqueeze(1),
                 torch.where(
-                        self.tokenizer.pad_token_id == outputs.sequences[:, shift:last][:, 1:],
+                        self.tokenizer.pad_token_id == outputs.sequences[:, prompt_length:last][:, 1:],
                         -1,
-                        outputs.sequences[:, shift:last][:, 1:])
+                        outputs.sequences[:, prompt_length:last][:, 1:])
                     ),
                 dim=1
             )
         non_pad_log_scores = torch.where(-1 != non_pad_tokens, token_seq_logprobs, torch.tensor(0.).to(self.device))
         for i, ix in enumerate(first_eos_indices):
             non_pad_log_scores[i][0] = token_seq_logprobs[i][0]  # at least score one token
             if ix != -1: # if there an eos token
                 non_pad_log_scores[i][ix] = token_seq_logprobs[i][ix]  # keep the first eos scores
                 non_pad_log_scores[i][ix + 1:] = 0. # ignore everything after eos
-        
+
         seq_logprobs = non_pad_log_scores.sum(dim=1) if sum else non_pad_log_scores
 
-        output_tokens = outputs.sequences[:, shift:] # [sampling_size, length]
+        output_tokens = outputs.sequences[:, prompt_length:] # [sampling_size, length]
 
         return (
                 [TextSample(ots, self.tokenizer.decode(ots)) for ots in output_tokens],
                 seq_logprobs
             )
```

### Comparing `disco-generation-1.1.0/disco/distributions/single_context_distribution.py` & `disco-generation-1.1.1/disco/distributions/single_context_distribution.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/metrics/base.py` & `disco-generation-1.1.1/disco/metrics/base.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/metrics/js.py` & `disco-generation-1.1.1/disco/metrics/js.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/metrics/kl.py` & `disco-generation-1.1.1/disco/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/metrics/tv.py` & `disco-generation-1.1.1/disco/metrics/tv.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/samplers/accumulation_sampler.py` & `disco-generation-1.1.1/disco/samplers/accumulation_sampler.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/samplers/quasi_rejection_sampler.py` & `disco-generation-1.1.1/disco/samplers/quasi_rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/scorers/boolean_scorer.py` & `disco-generation-1.1.1/disco/scorers/boolean_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/scorers/exponential_scorer.py` & `disco-generation-1.1.1/disco/scorers/exponential_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/scorers/pipeline_scorer.py` & `disco-generation-1.1.1/disco/scorers/pipeline_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/scorers/positive_scorer.py` & `disco-generation-1.1.1/disco/scorers/positive_scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/scorers/scorer.py` & `disco-generation-1.1.1/disco/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/cdpg_tuner.py` & `disco-generation-1.1.1/disco/tuners/cdpg_tuner.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/dpg_tuner.py` & `disco-generation-1.1.1/disco/tuners/dpg_tuner.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/fcdpg_tuner.py` & `disco-generation-1.1.1/disco/tuners/fcdpg_tuner.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/fdpg_tuner.py` & `disco-generation-1.1.1/disco/tuners/fdpg_tuner.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/loggers/base.py` & `disco-generation-1.1.1/disco/tuners/loggers/base.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/loggers/console.py` & `disco-generation-1.1.1/disco/tuners/loggers/console.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/loggers/json.py` & `disco-generation-1.1.1/disco/tuners/loggers/json.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/loggers/neptune.py` & `disco-generation-1.1.1/disco/tuners/loggers/neptune.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/loggers/wandb.py` & `disco-generation-1.1.1/disco/tuners/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/losses/js.py` & `disco-generation-1.1.1/disco/tuners/losses/js.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/losses/kl.py` & `disco-generation-1.1.1/disco/tuners/losses/kl.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/losses/reverse_kl.py` & `disco-generation-1.1.1/disco/tuners/losses/reverse_kl.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/losses/tv.py` & `disco-generation-1.1.1/disco/tuners/losses/tv.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/tuners/tuner.py` & `disco-generation-1.1.1/disco/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/utils/device.py` & `disco-generation-1.1.1/disco/utils/device.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/utils/helpers.py` & `disco-generation-1.1.1/disco/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/utils/moving_average.py` & `disco-generation-1.1.1/disco/utils/moving_average.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco/utils/observable.py` & `disco-generation-1.1.1/disco/utils/observable.py`

 * *Files identical despite different names*

### Comparing `disco-generation-1.1.0/disco_generation.egg-info/SOURCES.txt` & `disco-generation-1.1.1/disco_generation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

