# Comparing `tmp/MetaFEDOT-0.0.2.tar.gz` & `tmp/MetaFEDOT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaFEDOT-0.0.2.tar", last modified: Thu Jul 20 07:01:09 2023, max compression
+gzip compressed data, was "MetaFEDOT-0.0.3.tar", last modified: Mon Jul 24 19:40:10 2023, max compression
```

## Comparing `MetaFEDOT-0.0.2.tar` & `MetaFEDOT-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,51 @@
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.932928 MetaFEDOT-0.0.2/
--rw-r--r--   0 hex       (1000) hex       (1000)     1567 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.2/LICENSE
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.912928 MetaFEDOT-0.0.2/MetaFEDOT.egg-info/
--rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-20 07:01:09.000000 MetaFEDOT-0.0.2/MetaFEDOT.egg-info/PKG-INFO
--rw-r--r--   0 hex       (1000) hex       (1000)     1538 2023-07-20 07:01:09.000000 MetaFEDOT-0.0.2/MetaFEDOT.egg-info/SOURCES.txt
--rw-r--r--   0 hex       (1000) hex       (1000)        1 2023-07-20 07:01:09.000000 MetaFEDOT-0.0.2/MetaFEDOT.egg-info/dependency_links.txt
--rw-r--r--   0 hex       (1000) hex       (1000)       12 2023-07-20 07:01:09.000000 MetaFEDOT-0.0.2/MetaFEDOT.egg-info/top_level.txt
--rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-20 07:01:09.932928 MetaFEDOT-0.0.2/PKG-INFO
--rw-r--r--   0 hex       (1000) hex       (1000)     2362 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.2/README.md
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.912928 MetaFEDOT-0.0.2/meta_automl/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/__init__.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.912928 MetaFEDOT-0.0.2/meta_automl/data_preparation/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     2171 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/data_manager.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1748 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/dataset.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.912928 MetaFEDOT-0.0.2/meta_automl/data_preparation/datasets_loaders/
--rw-r--r--   0 hex       (1000) hex       (1000)      120 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/datasets_loaders/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)      790 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/datasets_loaders/datasets_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1880 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.922928 MetaFEDOT-0.0.2/meta_automl/data_preparation/meta_features_extractors/
--rw-r--r--   0 hex       (1000) hex       (1000)      105 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/meta_features_extractors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1055 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     2209 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py
--rw-r--r--   0 hex       (1000) hex       (1000)      395 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/model.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.922928 MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/
--rw-r--r--   0 hex       (1000) hex       (1000)      168 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     6510 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)     3154 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py
--rw-r--r--   0 hex       (1000) hex       (1000)      259 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/models_loader.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.922928 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/
--rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/__init__.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.932928 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/datasets_similarity_assessors/
--rw-r--r--   0 hex       (1000) hex       (1000)      173 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/datasets_similarity_assessors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)      407 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/datasets_similarity_assessors/datasets_similarity_assessor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     2356 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/datasets_similarity_assessors/predict_proba_similarity_assessors.py
-drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-20 07:01:09.932928 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/model_advisors/
--rw-r--r--   0 hex       (1000) hex       (1000)      241 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/model_advisors/__init__.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1337 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py
--rw-r--r--   0 hex       (1000) hex       (1000)     1537 2023-07-17 07:12:35.000000 MetaFEDOT-0.0.2/meta_automl/meta_algorithm/model_advisors/model_advisor.py
--rw-r--r--   0 hex       (1000) hex       (1000)       86 2023-07-19 19:28:59.000000 MetaFEDOT-0.0.2/pyproject.toml
--rw-r--r--   0 hex       (1000) hex       (1000)      214 2023-07-20 06:58:53.000000 MetaFEDOT-0.0.2/requirements.txt
--rw-r--r--   0 hex       (1000) hex       (1000)      599 2023-07-20 07:01:09.932928 MetaFEDOT-0.0.2/setup.cfg
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/
+-rw-r--r--   0 hex       (1000) hex       (1000)     1567 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.3/LICENSE
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/MetaFEDOT.egg-info/
+-rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 19:40:10.000000 MetaFEDOT-0.0.3/MetaFEDOT.egg-info/PKG-INFO
+-rw-r--r--   0 hex       (1000) hex       (1000)     1941 2023-07-24 19:40:10.000000 MetaFEDOT-0.0.3/MetaFEDOT.egg-info/SOURCES.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)        1 2023-07-24 19:40:10.000000 MetaFEDOT-0.0.3/MetaFEDOT.egg-info/dependency_links.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)       12 2023-07-24 19:40:10.000000 MetaFEDOT-0.0.3/MetaFEDOT.egg-info/top_level.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)     2832 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/PKG-INFO
+-rw-r--r--   0 hex       (1000) hex       (1000)     2362 2023-07-17 07:12:34.000000 MetaFEDOT-0.0.3/README.md
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/data_preparation/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/data_preparation/dataset/
+-rw-r--r--   0 hex       (1000) hex       (1000)      193 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/dataset/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      986 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/dataset/custom_dataset.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1095 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/dataset/dataset_base.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1906 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/dataset/openml_dataset.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/data_preparation/datasets_loaders/
+-rw-r--r--   0 hex       (1000) hex       (1000)      103 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/datasets_loaders/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      425 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/datasets_loaders/datasets_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1450 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3357 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/datasets_train_test_split.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/data_preparation/file_system/
+-rw-r--r--   0 hex       (1000) hex       (1000)      543 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/file_system/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3508 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/file_system/cache.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      483 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/file_system/cache_properties.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      578 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/file_system/file_system.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.101997 MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      105 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1153 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     2809 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      422 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/model.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/
+-rw-r--r--   0 hex       (1000) hex       (1000)      168 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     6384 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     3119 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      259 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/models_loader.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/
+-rw-r--r--   0 hex       (1000) hex       (1000)        0 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/__init__.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/datasets_similarity_assessors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      181 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/datasets_similarity_assessors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)      407 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/datasets_similarity_assessors/datasets_similarity_assessor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     2149 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py
+drwxr-xr-x   0 hex       (1000) hex       (1000)        0 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/
+-rw-r--r--   0 hex       (1000) hex       (1000)      241 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/__init__.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1707 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)     1647 2023-07-24 15:51:06.000000 MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/model_advisor.py
+-rw-r--r--   0 hex       (1000) hex       (1000)       88 2023-07-24 15:50:01.000000 MetaFEDOT-0.0.3/pyproject.toml
+-rw-r--r--   0 hex       (1000) hex       (1000)      154 2023-07-24 15:51:48.000000 MetaFEDOT-0.0.3/requirements.txt
+-rw-r--r--   0 hex       (1000) hex       (1000)      599 2023-07-24 19:40:10.111997 MetaFEDOT-0.0.3/setup.cfg
```

### Comparing `MetaFEDOT-0.0.2/LICENSE` & `MetaFEDOT-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.2/MetaFEDOT.egg-info/PKG-INFO` & `MetaFEDOT-0.0.3/MetaFEDOT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaFEDOT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for meta-optimisation in AutoML tasks
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 Project-URL: Homepage, https://github.com/ITMO-NSS-team/MetaFEDOT
 Project-URL: Bug Tracker, https://github.com/ITMO-NSS-team/MetaFEDOT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MetaFEDOT-0.0.2/MetaFEDOT.egg-info/SOURCES.txt` & `MetaFEDOT-0.0.3/MetaFEDOT.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,34 @@
 setup.cfg
 MetaFEDOT.egg-info/PKG-INFO
 MetaFEDOT.egg-info/SOURCES.txt
 MetaFEDOT.egg-info/dependency_links.txt
 MetaFEDOT.egg-info/top_level.txt
 meta_automl/__init__.py
 meta_automl/data_preparation/__init__.py
-meta_automl/data_preparation/data_manager.py
-meta_automl/data_preparation/dataset.py
+meta_automl/data_preparation/datasets_train_test_split.py
 meta_automl/data_preparation/model.py
+meta_automl/data_preparation/dataset/__init__.py
+meta_automl/data_preparation/dataset/custom_dataset.py
+meta_automl/data_preparation/dataset/dataset_base.py
+meta_automl/data_preparation/dataset/openml_dataset.py
 meta_automl/data_preparation/datasets_loaders/__init__.py
 meta_automl/data_preparation/datasets_loaders/datasets_loader.py
 meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py
+meta_automl/data_preparation/file_system/__init__.py
+meta_automl/data_preparation/file_system/cache.py
+meta_automl/data_preparation/file_system/cache_properties.py
+meta_automl/data_preparation/file_system/file_system.py
 meta_automl/data_preparation/meta_features_extractors/__init__.py
 meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py
 meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py
 meta_automl/data_preparation/models_loaders/__init__.py
 meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py
 meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py
 meta_automl/data_preparation/models_loaders/models_loader.py
 meta_automl/meta_algorithm/__init__.py
 meta_automl/meta_algorithm/datasets_similarity_assessors/__init__.py
 meta_automl/meta_algorithm/datasets_similarity_assessors/datasets_similarity_assessor.py
-meta_automl/meta_algorithm/datasets_similarity_assessors/predict_proba_similarity_assessors.py
+meta_automl/meta_algorithm/datasets_similarity_assessors/model_based_similarity_assessors.py
 meta_automl/meta_algorithm/model_advisors/__init__.py
 meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py
 meta_automl/meta_algorithm/model_advisors/model_advisor.py
```

### Comparing `MetaFEDOT-0.0.2/PKG-INFO` & `MetaFEDOT-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaFEDOT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for meta-optimisation in AutoML tasks
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 Project-URL: Homepage, https://github.com/ITMO-NSS-team/MetaFEDOT
 Project-URL: Bug Tracker, https://github.com/ITMO-NSS-team/MetaFEDOT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `MetaFEDOT-0.0.2/README.md` & `MetaFEDOT-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `MetaFEDOT-0.0.2/meta_automl/data_preparation/datasets_loaders/openml_datasets_loader.py` & `MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/pymfe_extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 from __future__ import annotations
 
-from typing import List, Union
+import logging
+from typing import List, Union, Dict, Any
 
-import openml
+import pandas as pd
+from pymfe.mfe import MFE
 
-from meta_automl.data_preparation.dataset import DatasetCache, Dataset
-from meta_automl.data_preparation.datasets_loaders import DatasetsLoader
-
-OpenMLDatasetID = Union[str, int]
-
-
-class OpenMLDatasetsLoader(DatasetsLoader):
-
-    def __init__(self):
-        self.dataset_sources = []
-
-    def load(self, dataset_sources: List[OpenMLDatasetID]) -> List[DatasetCache]:
-        self.dataset_sources = dataset_sources
-
-        datasets = []
-        # TODO: Optimize like this
-        #  https://github.com/openml/automlbenchmark/commit/a09dc8aee96178dd14837d9e1cd519d1ec63f804
-        for source in self.dataset_sources:
-            dataset = self.load_single(source)
-            datasets.append(dataset)
-        return datasets
-
-    def load_single(self, source: OpenMLDatasetID):
-        return self.get_openml_dataset(source)
-
-    def get_openml_dataset(self, dataset_id: OpenMLDatasetID, force_download: bool = False) -> DatasetCache:
-        openml_dataset = openml.datasets.get_dataset(dataset_id, download_data=False, download_qualities=False)
-        name = openml_dataset.name.lower()
-        dataset_cache_path = self.data_manager.get_dataset_cache_path(name)
-        if dataset_cache_path.exists() and not force_download:
-            dataset_cache = DatasetCache(name, dataset_cache_path)
-        else:
-            dataset_id = openml_dataset.id
-            X, y, categorical_indicator, attribute_names = openml_dataset.get_data(
-                target=openml_dataset.default_target_attribute,
-                dataset_format='array'
-            )
-            dataset = Dataset(name, X, y, categorical_indicator, attribute_names, _id=dataset_id)
-            dataset_cache = dataset.dump_to_cache(dataset_cache_path)
-        return dataset_cache
+from meta_automl.data_preparation.dataset import DatasetBase, DatasetIDType
+from meta_automl.data_preparation.datasets_loaders import DatasetsLoader, OpenMLDatasetsLoader
+from meta_automl.data_preparation.meta_features_extractors import MetaFeaturesExtractor
+
+
+class PymfeExtractor(MetaFeaturesExtractor):
+    default_params = {'groups': 'default'}
+
+    def __init__(self, extractor_params: Dict[str, Any] = None, datasets_loader: DatasetsLoader = None):
+        self.extractor_params = extractor_params if extractor_params is not None else self.default_params
+        self._datasets_loader = datasets_loader or OpenMLDatasetsLoader()
+        self._extractor = MFE(**self.extractor_params)
+
+    @property
+    def datasets_loader(self) -> DatasetsLoader:
+        if not self._datasets_loader:
+            raise ValueError("Datasets loader not provided!")
+        return self._datasets_loader
+
+    def extract(self, datasets_or_ids: List[Union[DatasetBase, DatasetIDType]],
+                fill_input_nans: bool = False, use_cached: bool = True, update_cached: bool = True) -> pd.DataFrame:
+        meta_features = {}
+        meta_feature_names = self._extractor.extract_metafeature_names()
+
+        for dataset in datasets_or_ids:
+            if not isinstance(dataset, DatasetBase):
+                dataset = self._datasets_loader.load_single(dataset)
+
+            logging.critical(f'Extracting meta features of the dataset {dataset}...')
+            if (use_cached and
+                    (mfs := self._get_meta_features_cache(dataset.id_, meta_feature_names))):
+                meta_features[dataset.id_] = mfs
+            else:
+                loaded_dataset = dataset.get_data(dataset_format='array')
+                cat_cols = [i for i, val in enumerate(loaded_dataset.categorical_indicator) if val]
+                x = loaded_dataset.x
+                y = loaded_dataset.y
+                if fill_input_nans:
+                    x = self.fill_nans(x)
+                mfe = self._extractor.fit(x, y, cat_cols=cat_cols)
+                feature_names, dataset_features = mfe.extract(out_type=tuple)
+                mfs = dict(zip(feature_names, dataset_features))
+                if update_cached:
+                    self._update_meta_features_cache(dataset.id_, mfs)
+                meta_features[dataset.id_] = mfs
+        meta_features = pd.DataFrame.from_dict(meta_features, orient='index')
+        return meta_features
+
+    @staticmethod
+    def fill_nans(x):
+        if not isinstance(x, pd.DataFrame):
+            x = pd.DataFrame(x)
+        x = x.fillna(x.median())
+        return x.to_numpy()
```

### Comparing `MetaFEDOT-0.0.2/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py` & `MetaFEDOT-0.0.3/meta_automl/data_preparation/meta_features_extractors/meta_features_extractor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
-from abc import abstractmethod
-from typing import Optional, Iterable, Dict, Any, Type
+from abc import abstractmethod, ABC
+from typing import Optional, Iterable, Dict, Any
 
 import pandas as pd
 
-from meta_automl.data_preparation.data_manager import DataManager
+from meta_automl.data_preparation.dataset import DatasetIDType
+from meta_automl.data_preparation.file_system import (CacheOperator, get_local_meta_features,
+                                                      update_local_meta_features)
 
 
-class MetaFeaturesExtractor:
-    DEFAULT_PARAMS: Optional[Dict[str, Any]] = None
-    SOURCE: Optional[str] = None
-    data_manager: Type[DataManager] = DataManager
+class MetaFeaturesExtractor(ABC, CacheOperator):
+    default_params: Optional[Dict[str, Any]] = None
 
     @abstractmethod
     def extract(self, datasets) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def _get_meta_features_cache(self, dataset_name: str, meta_feature_names: Iterable[str]):
-        cache = self.data_manager.get_meta_features_dict(dataset_name, self.SOURCE)
+    def _get_meta_features_cache(self, dataset_id: DatasetIDType, meta_feature_names: Iterable[str]):
+        cache = get_local_meta_features(self.__class__, str(dataset_id))
         if set(meta_feature_names) ^ cache.keys():
             return None
         else:
             return {mf_name: cache[mf_name] for mf_name in meta_feature_names}
 
-    def _update_meta_features_cache(self, dataset_name: str, meta_features_dict: Dict[str, Any]):
-        self.data_manager.update_meta_features_dict(dataset_name, self.SOURCE, meta_features_dict)
+    def _update_meta_features_cache(self, dataset_id: DatasetIDType, meta_features_dict: Dict[str, Any]):
+        update_local_meta_features(self.__class__, dataset_id, meta_features_dict)
```

### Comparing `MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py` & `MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/fedot_pipelines_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,73 +10,72 @@
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.quality_metrics_repository import ClassificationMetricsEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum
 from fedot.core.validation.split import tabular_cv_generator
 from golem.core.log import default_log
 from tqdm import tqdm
 
-from meta_automl.data_preparation.data_manager import PathType
-from meta_automl.data_preparation.dataset import DatasetCache
+from meta_automl.data_preparation.file_system import PathType
+from meta_automl.data_preparation.dataset import DatasetBase
 from meta_automl.data_preparation.datasets_loaders import DatasetsLoader, OpenMLDatasetsLoader
 from meta_automl.data_preparation.model import Model
 from meta_automl.data_preparation.models_loaders import ModelsLoader
 
 
 def evaluate_classification_fedot_pipeline(pipeline, input_data):
     cv_folds = partial(tabular_cv_generator, input_data, folds=5)
     objective_eval = PipelineObjectiveEvaluate(MetricsObjective(ClassificationMetricsEnum.ROCAUC), cv_folds,
                                                eval_n_jobs=-1)
     fitness = objective_eval(pipeline)
     return fitness
 
 
-def get_n_best_fedot_performers(dataset_cache: DatasetCache, pipelines: List[Pipeline], datasets_loader: DatasetsLoader,
-                                n_best: int = 1) -> List[Model]:
-    loaded_dataset = datasets_loader.cache_to_memory(dataset_cache)
-    X, y_test = loaded_dataset.x, loaded_dataset.y
+def get_n_best_fedot_performers(dataset: DatasetBase, pipelines: List[Pipeline], n_best: int = 1) -> List[Model]:
+    data = dataset.get_data()
+    X, y_test = data.x, data.y
     input_data = InputData(idx=np.arange(0, len(X)), features=X, target=y_test, data_type=DataTypesEnum.table,
                            task=Task(TaskTypesEnum.classification))
     fitnesses = []
     models = []
     metric_name = 'roc_auc'
     for pipeline in tqdm(pipelines, desc='Evaluating pipelines'):
         fitness = evaluate_classification_fedot_pipeline(pipeline, input_data)
         fitnesses.append(fitness)
-        models.append(Model(pipeline, fitness, metric_name, dataset_cache))
+        models.append(Model(pipeline, fitness, metric_name, dataset))
 
     best_models = [models.pop(np.argmax(fitnesses)) for _ in range(min(n_best, len(pipelines)))]
     return best_models
 
 
 class FEDOTPipelinesLoader(ModelsLoader):
-    def __init__(self, datasets_to_load: Union[List[Union[DatasetCache, str]], Literal['auto']] = 'auto',
+    def __init__(self, datasets_to_load: Union[List[Union[DatasetBase, str]], Literal['auto']] = 'auto',
                  candidate_pipelines: Optional[List[List[Pipeline]]] = None,
                  candidate_pipeline_paths: Optional[List[List[PathType]]] = None,
                  launch_dir: Optional[PathType] = None,
                  datasets_loader: Optional[DatasetsLoader] = None):
 
         self.log = default_log(self)
 
-        self.datasets_loader = datasets_loader or OpenMLDatasetsLoader()
+        self.datasets_loader = datasets_loader or OpenMLDatasetsLoader(allow_names=True)
 
         self.launch_dir: Path = Path(launch_dir) if isinstance(launch_dir, str) else launch_dir
 
-        self._datasets: List[DatasetCache] = (self._define_datasets() if datasets_to_load == 'auto'
-                                              else self._dataset_names_to_cache(datasets_to_load))
+        self._datasets: List[DatasetBase] = (self._define_datasets() if datasets_to_load == 'auto'
+                                             else self._get_datasets_from_names(datasets_to_load))
 
         self.candidate_pipelines = candidate_pipelines
 
         if self.candidate_pipelines is None:
             candidate_pipeline_paths = candidate_pipeline_paths or self._define_pipeline_paths()
             self._import_pipelines(candidate_pipeline_paths)
 
     def load(self, datasets: Union[List[str], Literal['auto']] = 'auto', n_best: int = 1) -> List[List[Model]]:
         if datasets != 'auto':
-            datasets = self._dataset_names_to_cache(datasets)
-            difference = set(d.name for d in datasets) - set(self.dataset_names)
+            datasets = self._get_datasets_from_names(datasets)
+            difference = set(d.name for d in datasets) - set(self.dataset_ids)
             if difference:
                 raise ValueError(f'Results for these datasets are not available: {difference}.')
         else:
             datasets = self._datasets
 
         models = []
         for dataset, candidate_pipelines in tqdm(list(zip(datasets, self.candidate_pipelines)),
@@ -85,47 +84,46 @@
             models.append(best_performers)
         return models
 
     def _define_pipeline_paths(self) -> List[List[Path]]:
         if not self.launch_dir:
             raise ValueError('Launch dir or model paths must be provided!')
 
-        dataset_names = self.dataset_names
-        datasets_models_paths = dict(zip(dataset_names, [[]] * len(dataset_names)))
+        dataset_ids = self.dataset_ids
+        datasets_models_paths = dict(zip(dataset_ids, [[]] * len(dataset_ids)))
 
-        for dataset_name in tqdm(dataset_names, desc='Defining model paths', unit='dataset'):
+        for dataset_name in tqdm(dataset_ids, desc='Defining model paths', unit='dataset'):
             for model_path in self.launch_dir.joinpath(dataset_name).glob(r'FEDOT*\*\*\launch_*.json'):
                 datasets_models_paths[dataset_name].append(model_path)
 
         return [datasets_models_paths[dataset.name] for dataset in self._datasets]
 
     def _import_pipelines(self, candidate_pipeline_paths: List[List[PathType]]):
         candidate_pipelines = []
         for dataset, paths in tqdm(list(zip(self._datasets, candidate_pipeline_paths)),
                                    desc='Importing pipelines', unit='dataset'):
             candidates_for_dataset = [Pipeline.from_serialized(str(p)) for p in paths]
             if not candidates_for_dataset:
-                self.log.warning(f'No pipelines found for the dataset "{dataset.name}".')
+                self.log.warning(f'No pipelines found for the dataset "{dataset}".')
             candidate_pipelines.append(candidates_for_dataset)
         self.candidate_pipelines = candidate_pipelines
 
-    def _define_datasets(self) -> List[DatasetCache]:
+    def _define_datasets(self) -> List[DatasetBase]:
         if not self.launch_dir:
             raise ValueError('Launch dir or datasets must be provided!')
 
         datasets = list({p.parents[2].name for p in self.launch_dir.glob(r'*\FEDOT*\*\launch_0')})
         datasets.sort()
-        datasets = self._dataset_names_to_cache(datasets)
+        datasets = self._get_datasets_from_names(datasets)
         return datasets
 
     @property
-    def dataset_names(self):
-        return [d.name if isinstance(d, DatasetCache) else d for d in self._datasets]
+    def dataset_ids(self):
+        return [d.name if isinstance(d, DatasetBase) else d for d in self._datasets]
 
-    @staticmethod
-    def _dataset_names_to_cache(datasets: List[Union[str, DatasetCache]]) -> List[DatasetCache]:
+    def _get_datasets_from_names(self, datasets: List[Union[str, DatasetBase]]) -> List[DatasetBase]:
         new_list = []
         for dataset in datasets:
-            if isinstance(dataset, str):
-                dataset = DatasetCache(dataset)
+            if not isinstance(dataset, DatasetBase):
+                dataset = self.datasets_loader.load_single(dataset)
             new_list.append(dataset)
         return new_list
```

### Comparing `MetaFEDOT-0.0.2/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py` & `MetaFEDOT-0.0.3/meta_automl/data_preparation/models_loaders/knowledge_base_models_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,53 +3,54 @@
 from pathlib import Path
 from typing import Union, Literal, Optional, Sequence, List
 
 import pandas as pd
 from fedot.core.pipelines.pipeline import Pipeline
 from golem.core.optimisers.fitness import SingleObjFitness
 
-from meta_automl.data_preparation.data_manager import DataManager
-from meta_automl.data_preparation.dataset import DatasetCache
+
+from meta_automl.data_preparation.dataset import OpenMLDataset
+from meta_automl.data_preparation.file_system import get_data_dir
 from meta_automl.data_preparation.model import Model
 from meta_automl.data_preparation.models_loaders import ModelsLoader
 
-DEFAULT_KNOWLEDGE_BASE_PATH = DataManager.get_data_dir().joinpath('knowledge_base_0')
+DEFAULT_KNOWLEDGE_BASE_PATH = get_data_dir() / 'knowledge_base_0'
 
 
 class KnowledgeBaseModelsLoader(ModelsLoader):
     def __init__(self, knowledge_base_path: Union[str, PathLike] = DEFAULT_KNOWLEDGE_BASE_PATH):
         self.knowledge_base_path: Path = Path(knowledge_base_path)
         self.df_knowledge_base: Optional[pd.DataFrame] = None
         self.df_datasets: Optional[pd.DataFrame] = None
 
-    def load(self, dataset_names: Optional[Sequence[str]] = None,
+    def load(self, dataset_ids: Optional[Sequence[str]] = None,
              fitness_metric: str = 'f1') -> List[Model]:
         if self.df_knowledge_base is None:
             knowledge_base_split_file = self.knowledge_base_path.joinpath('knowledge_base.csv')
             self.df_knowledge_base = pd.read_csv(knowledge_base_split_file)
 
-        if dataset_names is None:
-            dataset_names = self.parse_datasets()['dataset_name']
+        if dataset_ids is None:
+            dataset_ids = self.parse_datasets()['dataset_id']
 
         df_knowledge_base = self.df_knowledge_base
-        df_knowledge_base = df_knowledge_base[df_knowledge_base['dataset_name'].isin(dataset_names)]
+        df_knowledge_base = df_knowledge_base[df_knowledge_base['dataset_id'].isin(dataset_ids)]
 
         cached_datasets = {}
-        for name in dataset_names:
-            cached_datasets[name] = DatasetCache(name)
+        for id_ in dataset_ids:
+            cached_datasets[id_] = OpenMLDataset(id_)
 
         models = []
         for _, row in df_knowledge_base.iterrows():
             pipeline = Pipeline()
             pipeline.log.setLevel(logging.CRITICAL)
             predictor = pipeline.load(str(self.knowledge_base_path.joinpath(row['model_path'])))
             metric_value = row[fitness_metric]
             fitness = SingleObjFitness(metric_value)
             metadata = dict(row)
-            dataset_cache = cached_datasets[row['dataset_name']]
+            dataset_cache = cached_datasets[row['dataset_id']]
             model = Model(predictor, fitness, fitness_metric, dataset_cache, metadata)
             models.append(model)
         return models
 
     def parse_datasets(
             self, train_test: Literal['train', 'test', 'all'] = 'all',
             task_type: Literal['classification', 'regression', 'ts_forecasting'] = 'classification') -> pd.DataFrame:
```

### Comparing `MetaFEDOT-0.0.2/meta_automl/meta_algorithm/datasets_similarity_assessors/predict_proba_similarity_assessors.py` & `MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/model_advisor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,42 @@
-from typing import Optional, Dict, Any, List, Iterable
+from abc import abstractmethod
+from typing import List, Dict, Iterable, Sequence
 
-import numpy as np
 import pandas as pd
-from sklearn.neighbors import KNeighborsClassifier
 
-from meta_automl.meta_algorithm.datasets_similarity_assessors.datasets_similarity_assessor import \
-    DatasetsSimilarityAssessor
+from meta_automl.data_preparation.dataset import DatasetIDType
+from meta_automl.data_preparation.model import Model
+from meta_automl.meta_algorithm.datasets_similarity_assessors import DatasetsSimilarityAssessor
 
 
-class PredictProbaSimilarityAssessor(DatasetsSimilarityAssessor):
-    def __init__(self, model, n_best: int = 1):
-        self._inner_model = model
-        self.n_best = n_best
+class ModelAdvisor:
 
-    @property
-    def datasets(self) -> List[str]:
-        return self._inner_model.classes_
+    @abstractmethod
+    def predict(self, *args, **kwargs) -> List[List[Model]]:
+        raise NotImplementedError()
+
+
+class SimpleSimilarityModelAdvisor(ModelAdvisor):
+    def __init__(self, fitted_similarity_assessor: DatasetsSimilarityAssessor):
+        self.similarity_assessor = fitted_similarity_assessor
+        self.best_models: Dict[DatasetIDType, Sequence[Model]] = {}
 
     @property
-    def feature_names(self) -> List[str]:
-        return self._inner_model.feature_names_in_
+    def datasets(self):
+        return self.similarity_assessor.datasets
 
-    @staticmethod
-    def preprocess_meta_features(meta_features: pd.DataFrame) -> pd.DataFrame:
-        return meta_features.dropna(axis=1, how='any')
-
-    def _preprocess_predict_features(self, meta_features: pd.DataFrame) -> pd.DataFrame:
-        return meta_features[self.feature_names]
-
-    def fit(self, meta_features: pd.DataFrame, datasets: Iterable[str]):
-        meta_features = self.preprocess_meta_features(meta_features)
-        self._inner_model.fit(meta_features, datasets)
-
-    def predict_proba(self, meta_features: pd.DataFrame) -> List[List[float]]:
-        return self._inner_model.predict_proba(meta_features)
-
-    def predict(self, meta_features: pd.DataFrame) -> List[List[str]]:
-        meta_features = self._preprocess_predict_features(meta_features)
-        predict_probs = self.predict_proba(meta_features)
-        final_prediction = []
-        for probabilities in predict_probs:
-            probabilities = list(probabilities)
-            predictions = []
-            for _ in range(self.n_best):
-                predicted_class_idx = np.argmax(probabilities)
-                predicted_class = self.datasets[predicted_class_idx]
-                predictions.append(predicted_class)
-                probabilities.pop(predicted_class_idx)
-            final_prediction.append(predictions)
-
-        return final_prediction
-
-
-class KNNSimilarityAssessor(PredictProbaSimilarityAssessor):
-    def __init__(self, model_params: Optional[Dict[str, Any]] = None, n_best: int = 1):
-        model_params = model_params or dict()
-        model = KNeighborsClassifier(**model_params)
-        super().__init__(model, n_best)
+    def fit(self, dataset_names_to_best_pipelines: Dict[DatasetIDType, Sequence[Model]]):
+        self.best_models.update(dataset_names_to_best_pipelines)
+        return self
+
+    def predict(self, meta_features: pd.DataFrame) -> List[List[Model]]:
+        assessor_predictions = self.similarity_assessor.predict(meta_features)
+        advised_pipelines = []
+        for similar_datasets in assessor_predictions:
+            advised_pipelines.append(self._predict_single(similar_datasets))
+        return advised_pipelines
+
+    def _predict_single(self, similar_dataset_ids: Iterable[DatasetIDType]) -> List[Model]:
+        dataset_pipelines = []
+        for dataset_id in similar_dataset_ids:
+            dataset_pipelines += list(self.best_models.get(dataset_id))
+        return dataset_pipelines
```

### Comparing `MetaFEDOT-0.0.2/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py` & `MetaFEDOT-0.0.3/meta_automl/meta_algorithm/model_advisors/diverse_fedot_pipeline_advisor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import Callable, List, Iterable
+from typing import Callable, List, Iterable, Optional
 
 from fedot.core.pipelines.pipeline import Pipeline
 from golem.core.dag.linked_graph import get_distance_between
 
 from meta_automl.data_preparation.model import Model
 from meta_automl.meta_algorithm.datasets_similarity_assessors import DatasetsSimilarityAssessor
 from meta_automl.meta_algorithm.model_advisors import SimpleSimilarityModelAdvisor
 
 
 class DiverseFEDOTPipelineAdvisor(SimpleSimilarityModelAdvisor):
     def __init__(self,
                  fitted_similarity_assessor: DatasetsSimilarityAssessor,
-                 minimal_distance: int = 1,
-                 distance_func: Callable[[Pipeline, Pipeline], int] = get_distance_between):
+                 n_best_to_advise: Optional[int] = None,
+                 minimal_distance: float = 1,
+                 distance_func: Callable[[Pipeline, Pipeline], float] = get_distance_between):
         super().__init__(fitted_similarity_assessor)
         self.minimal_distance = minimal_distance
+        self.n_best_to_advise = n_best_to_advise
         self.distance_func = distance_func
 
     def _predict_single(self, similar_dataset_names: Iterable[str]) -> List[Model]:
         dataset_advice = super()._predict_single(similar_dataset_names)
         first_model = dataset_advice[0]
         diverse_dataset_advice = [first_model]
         for model in dataset_advice[1:]:
             if self.distance_func(first_model.predictor, model.predictor) > self.minimal_distance:
                 diverse_dataset_advice.append(model)
+
+        if self.n_best_to_advise is not None:
+            diverse_dataset_advice = list(sorted(diverse_dataset_advice, key=lambda m: m.fitness, reverse=True))
+            diverse_dataset_advice = diverse_dataset_advice[:self.n_best_to_advise]
         return diverse_dataset_advice
```

### Comparing `MetaFEDOT-0.0.2/setup.cfg` & `MetaFEDOT-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MetaFEDOT
-version = 0.0.2
+version = 0.0.3
 author = NSS Lab
 author_email = itmo.nss.team@gmail.com
 description = Framework for meta-optimisation in AutoML tasks
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

