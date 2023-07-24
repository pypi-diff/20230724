# Comparing `tmp/MetaFEDOT-0.0.4.tar.gz` & `tmp/MetaFEDOT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaFEDOT-0.0.4.tar", last modified: Mon Jul 24 19:52:55 2023, max compression
+gzip compressed data, was "MetaFEDOT-0.0.5.tar", last modified: Mon Jul 24 20:09:12 2023, max compression
```

## Comparing `MetaFEDOT-0.0.4.tar` & `MetaFEDOT-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/
--rw-r--r--   0 hex       (1000) hex       (1000)     1567 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.4/LICENSE
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/
--rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 19:52:55.000000 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/PKG-INFO
--rw-r--r--   0 hex       (1000) hex       (1000)     1973 2023-07-24 19:52:55.000000 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/SOURCES.txt
--rw-r--r--   0 hex       (1000) hex       (1000)        1 2023-07-24 19:52:55.000000 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/dependency_links.txt
--rw-r--r--   0 hex       (1000) hex       (1000)      146 2023-07-24 19:52:55.000000 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/requires.txt
--rw-r--r--   0 hex       (1000) hex       (1000)       12 2023-07-24 19:52:55.000000 MetaFEDOT-0.0.4/MetaFEDOT.egg-info/top_level.txt
--rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/PKG-INFO
--rw-r--r--   0 hex       (1000) hex       (1000)     2362 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.4/README.md
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/__init__.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/__init__.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/
--rw-r--r--   0 hex       (1000) hex       (1000)      193 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)      986 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/custom_dataset.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1095 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/dataset_base.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1906 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/openml_dataset.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_loaders/
--rw-r--r--   0 hex       (1000) hex       (1000)      103 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_loaders/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)      425 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_loaders/datasets_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1450 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)     3357 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_train_test_split.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/
--rw-r--r--   0 hex       (1000) hex       (1000)      543 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     3508 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/cache.py
--rw-r--r--   0 hex       (1000) hex       (1000)      483 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/cache_properties.py
--rw-r--r--   0 hex       (1000) hex       (1000)      578 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/file_system.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/
--rw-r--r--   0 hex       (1000) hex       (1000)      105 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1153 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     2809 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py
--rw-r--r--   0 hex       (1000) hex       (1000)      422 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/model.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/
--rw-r--r--   0 hex       (1000) hex       (1000)      168 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     6384 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)     3119 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)      259 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/models_loader.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/__init__.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/datasets_similarity_assessors/
--rw-r--r--   0 hex       (1000) hex       (1000)      181 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/datasets_similarity_assessors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)      407 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/datasets_similarity_assessors/datasets_similarity_assessor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     2149 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/
--rw-r--r--   0 hex       (1000) hex       (1000)      241 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1707 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1647 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/model_advisor.py
--rw-r--r--   0 hex       (1000) hex       (1000)       88 2023-07-24 19:51:57.000000 MetaFEDOT-0.0.4/pyproject.toml
--rw-r--r--   0 hex       (1000) hex       (1000)      154 2023-07-24 15:51:48.000000 MetaFEDOT-0.0.4/requirements.txt
--rw-r--r--   0 hex       (1000) hex       (1000)      641 2023-07-24 19:52:55.041786 MetaFEDOT-0.0.4/setup.cfg
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/
+-rw-r--r--   0 hex       (1000) hex       (1000)     1567 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.5/LICENSE
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.661503 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/
+-rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 20:09:12.000000 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/PKG-INFO
+-rw-r--r--   0 hex       (1000) hex       (1000)     1982 2023-07-24 20:09:12.000000 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/SOURCES.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)        1 2023-07-24 20:09:12.000000 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/dependency_links.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)      146 2023-07-24 20:09:12.000000 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/requires.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)       12 2023-07-24 20:09:12.000000 MetaFEDOT-0.0.5/MetaFEDOT.egg-info/top_level.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/PKG-INFO
+-rw-r--r--   0 hex       (1000) hex       (1000)     2362 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.5/README.md
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.661503 MetaFEDOT-0.0.5/meta_automl/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/
+-rw-r--r--   0 hex       (1000) hex       (1000)      193 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      986 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/custom_dataset.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1095 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/dataset_base.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1906 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/openml_dataset.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_loaders/
+-rw-r--r--   0 hex       (1000) hex       (1000)      103 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_loaders/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      425 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_loaders/datasets_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1450 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3357 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_train_test_split.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/
+-rw-r--r--   0 hex       (1000) hex       (1000)      543 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3508 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/cache.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      483 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/cache_properties.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      578 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/file_system.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      105 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1153 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     2809 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      422 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/model.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/
+-rw-r--r--   0 hex       (1000) hex       (1000)      168 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     6384 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3119 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      259 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/models_loader.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/datasets_similarity_assessors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      181 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/datasets_similarity_assessors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      407 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/datasets_similarity_assessors/datasets_similarity_assessor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     2149 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      241 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1707 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1647 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/model_advisor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)       88 2023-07-24 19:51:57.000000 MetaFEDOT-0.0.5/pyproject.toml
+-rw-r--r--   0 hex       (1000) hex       (1000)      154 2023-07-24 15:51:48.000000 MetaFEDOT-0.0.5/requirements.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)      641 2023-07-24 20:09:12.671503 MetaFEDOT-0.0.5/setup.cfg
+-rw-r--r--   0 hex       (1000) hex       (1000)       60 2023-07-24 20:08:48.000000 MetaFEDOT-0.0.5/setup.py
```

### Comparing `MetaFEDOT-0.0.4/LICENSE` & `MetaFEDOT-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/MetaFEDOT.egg-info/PKG-INFO` & `MetaFEDOT-0.0.5/MetaFEDOT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaFEDOT
-Version: 0.0.4
+Version: 0.0.5
 Summary: Framework for meta-optimisation in AutoML tasks
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 Project-URL: Homepage, https://github.com/ITMO-NSS-team/MetaFEDOT
 Project-URL: Bug Tracker, https://github.com/ITMO-NSS-team/MetaFEDOT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MetaFEDOT-0.0.4/MetaFEDOT.egg-info/SOURCES.txt` & `MetaFEDOT-0.0.5/MetaFEDOT.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
+setup.py
 MetaFEDOT.egg-info/PKG-INFO
 MetaFEDOT.egg-info/SOURCES.txt
 MetaFEDOT.egg-info/dependency_links.txt
 MetaFEDOT.egg-info/requires.txt
 MetaFEDOT.egg-info/top_level.txt
 meta_automl/__init__.py
 meta_automl/data_preparation/__init__.py
```

### Comparing `MetaFEDOT-0.0.4/PKG-INFO` & `MetaFEDOT-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaFEDOT
-Version: 0.0.4
+Version: 0.0.5
 Summary: Framework for meta-optimisation in AutoML tasks
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 Project-URL: Homepage, https://github.com/ITMO-NSS-team/MetaFEDOT
 Project-URL: Bug Tracker, https://github.com/ITMO-NSS-team/MetaFEDOT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MetaFEDOT-0.0.4/README.md` & `MetaFEDOT-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/custom_dataset.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/dataset_base.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/dataset_base.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/dataset/openml_dataset.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/dataset/openml_dataset.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/datasets_train_test_split.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/datasets_train_test_split.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/__init__.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/cache.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/cache.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/file_system/file_system.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/file_system/file_system.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py` & `MetaFEDOT-0.0.5/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py` & `MetaFEDOT-0.0.5/meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py` & `MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/meta_automl/meta_algorithm/model_advisors/model_advisor.py` & `MetaFEDOT-0.0.5/meta_automl/meta_algorithm/model_advisors/model_advisor.py`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.4/setup.cfg` & `MetaFEDOT-0.0.5/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MetaFEDOT
-version = 0.0.4
+version = 0.0.5
 author = NSS Lab
 author_email = itmo.nss.team@gmail.com
 description = Framework for meta-optimisation in AutoML tasks
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

