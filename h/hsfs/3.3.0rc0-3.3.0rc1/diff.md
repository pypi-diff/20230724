# Comparing `tmp/hsfs-3.3.0rc0.tar.gz` & `tmp/hsfs-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.3.0rc0.tar", last modified: Mon Jul  3 11:50:55 2023, max compression
+gzip compressed data, was "hsfs-3.3.0rc1.tar", last modified: Mon Jul 24 11:26:28 2023, max compression
```

## Comparing `hsfs-3.3.0rc0.tar` & `hsfs-3.3.0rc1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.165521 hsfs-3.3.0rc0/
--rw-r--r--   0     1006     1006       40 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     7742 2023-07-03 11:50:55.165521 hsfs-3.3.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     5539 2023-07-03 11:50:54.000000 hsfs-3.3.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.145522 hsfs-3.3.0rc0/hsfs/
--rw-r--r--   0     1006     1006     1182 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.149522 hsfs-3.3.0rc0/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     6622 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/client/base.py
--rw-r--r--   0     1006     1006     2090 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11621 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/client/external.py
--rw-r--r--   0     1006     1006     7924 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006     1536 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/code.py
--rw-r--r--   0     1006     1006    18899 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.149522 hsfs-3.3.0rc0/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1487 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5143 2023-06-30 06:14:21.000000 hsfs-3.3.0rc0/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     3158 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1731 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2151 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1577 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    26740 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3331 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.165521 hsfs-3.3.0rc0/hsfs/core/
--rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006    10185 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/arrow_flight_client.py
--rw-r--r--   0     1006     1006     3688 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     3291 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3509 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     1030 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1609 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4060 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9792 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     5331 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    13467 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6610 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    13066 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006     1238 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006     9739 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    24309 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5023 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11701 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1211 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1077 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     4285 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2004 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2047 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     1530 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006      898 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     1981 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/spine_group_engine.py
--rw-r--r--   0     1006     1006     4204 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006     8159 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     2325 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6357 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    12422 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     2297 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    19974 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.165521 hsfs-3.3.0rc0/hsfs/engine/
--rw-r--r--   0     1006     1006     2244 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    50175 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    44416 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006    23594 2023-06-26 14:55:39.000000 hsfs-3.3.0rc0/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6857 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/feature.py
--rw-r--r--   0     1006     1006   118825 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3937 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1985 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    69498 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/feature_store.py
--rw-r--r--   0     1006     1006   106306 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8633 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     1449 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     2893 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3313 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    41656 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1850 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/tag.py
--rw-r--r--   0     1006     1006    35625 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     3771 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2758 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8929 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2179 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     3491 2023-06-05 14:18:50.000000 hsfs-3.3.0rc0/hsfs/user.py
--rw-r--r--   0     1006     1006    12670 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/util.py
--rw-r--r--   0     1006     1006     7519 2023-06-19 21:22:26.000000 hsfs-3.3.0rc0/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      631 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2023-07-03 11:50:55.145522 hsfs-3.3.0rc0/hsfs.egg-info/
--rw-r--r--   0     1006     1006     7742 2023-07-03 11:50:54.000000 hsfs-3.3.0rc0/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2870 2023-07-03 11:50:55.000000 hsfs-3.3.0rc0/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-07-03 11:50:54.000000 hsfs-3.3.0rc0/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      830 2023-07-03 11:50:54.000000 hsfs-3.3.0rc0/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2023-07-03 11:50:54.000000 hsfs-3.3.0rc0/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-07-03 11:50:55.165521 hsfs-3.3.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     3074 2023-07-03 11:50:50.000000 hsfs-3.3.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.294640 hsfs-3.3.0rc1/
+-rw-r--r--   0     1006     1006       40 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0     1006     1006     7742 2023-07-24 11:26:28.294640 hsfs-3.3.0rc1/PKG-INFO
+-rw-r--r--   0     1006     1006     5539 2023-07-24 11:26:27.000000 hsfs-3.3.0rc1/README.md
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.266641 hsfs-3.3.0rc1/hsfs/
+-rw-r--r--   0     1006     1006     1182 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.270641 hsfs-3.3.0rc1/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     6622 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     2090 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11621 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     7924 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1536 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/code.py
+-rw-r--r--   0     1006     1006    18899 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.274641 hsfs-3.3.0rc1/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1487 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5143 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     3158 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1731 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2151 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1577 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    26964 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3331 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.294640 hsfs-3.3.0rc1/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006    10201 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/arrow_flight_client.py
+-rw-r--r--   0     1006     1006     3688 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     3291 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3509 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     1030 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1609 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4060 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9792 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     5331 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    13467 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6610 2023-07-14 08:54:50.000000 hsfs-3.3.0rc1/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    13066 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006     1238 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006     9739 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    24309 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5023 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11701 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1211 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1077 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     4285 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2004 2023-07-14 08:54:50.000000 hsfs-3.3.0rc1/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2047 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     1530 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006      898 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     1981 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/spine_group_engine.py
+-rw-r--r--   0     1006     1006     4204 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006     8159 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     2325 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6357 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    12422 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     2297 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    19974 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.294640 hsfs-3.3.0rc1/hsfs/engine/
+-rw-r--r--   0     1006     1006     2244 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    50176 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    44416 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006    23594 2023-06-26 14:55:39.000000 hsfs-3.3.0rc1/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6857 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/feature.py
+-rw-r--r--   0     1006     1006   119054 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3937 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1985 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    69498 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006   108097 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8633 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     1449 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     2893 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3313 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    41656 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1850 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/tag.py
+-rw-r--r--   0     1006     1006    35625 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     3771 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2758 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8929 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2179 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     3491 2023-06-05 14:18:50.000000 hsfs-3.3.0rc1/hsfs/user.py
+-rw-r--r--   0     1006     1006    12670 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/util.py
+-rw-r--r--   0     1006     1006     7519 2023-06-19 21:22:26.000000 hsfs-3.3.0rc1/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2023-07-24 11:26:28.266641 hsfs-3.3.0rc1/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     7742 2023-07-24 11:26:28.000000 hsfs-3.3.0rc1/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2870 2023-07-24 11:26:28.000000 hsfs-3.3.0rc1/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-07-24 11:26:28.000000 hsfs-3.3.0rc1/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      830 2023-07-24 11:26:28.000000 hsfs-3.3.0rc1/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2023-07-24 11:26:28.000000 hsfs-3.3.0rc1/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-07-24 11:26:28.294640 hsfs-3.3.0rc1/setup.cfg
+-rw-r--r--   0     1006     1006     3074 2023-07-24 11:26:23.000000 hsfs-3.3.0rc1/setup.py
```

### Comparing `hsfs-3.3.0rc0/PKG-INFO` & `hsfs-3.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.3.0rc0
+Version: 3.3.0rc1
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc0
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc1
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.3.0rc0 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.3.0rc1 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc0
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc1
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.3.0rc0/README.md` & `hsfs-3.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/__init__.py` & `hsfs-3.3.0rc1/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/__init__.py` & `hsfs-3.3.0rc1/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/auth.py` & `hsfs-3.3.0rc1/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/base.py` & `hsfs-3.3.0rc1/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/exceptions.py` & `hsfs-3.3.0rc1/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/external.py` & `hsfs-3.3.0rc1/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/client/hopsworks.py` & `hsfs-3.3.0rc1/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/code.py` & `hsfs-3.3.0rc1/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/connection.py` & `hsfs-3.3.0rc1/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/__init__.py` & `hsfs-3.3.0rc1/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.3.0rc1/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/filter.py` & `hsfs-3.3.0rc1/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/fs_query.py` & `hsfs-3.3.0rc1/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.3.0rc1/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/join.py` & `hsfs-3.3.0rc1/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.3.0rc1/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/query.py` & `hsfs-3.3.0rc1/hsfs/constructor/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,19 @@
             however, you can use the Query API to create Feature Views/Training
             Data containing External Feature Groups.
 
         # Arguments
             online: Read from online storage. Defaults to `False`.
             dataframe_type: DataFrame type to return. Defaults to `"default"`.
             read_options: Dictionary of read options for Spark in spark engine.
-                Only for python engine: Use key "hive_config" to pass a dictionary of hive or tez configurations.
-                For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
+                Only for python engine:
+                * key `"use_hive"` and value `True` to read query with Hive instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
+                * key "hive_config" to pass a dictionary of hive or tez configurations.
+                  For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 Defaults to `{}`.
 
         # Returns
             `DataFrame`: DataFrame depending on the chosen type.
         """
         if not read_options:
             read_options = {}
```

### Comparing `hsfs-3.3.0rc0/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.3.0rc1/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/__init__.py` & `hsfs-3.3.0rc1/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/arrow_flight_client.py` & `hsfs-3.3.0rc1/hsfs/core/arrow_flight_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
                 self._initialize_connection()
             except Exception as e:
                 self._disable(str(e))
 
     def _disable(self, message):
         self._is_enabled = False
         warnings.warn(
-            f"Could not establish connection to FlyingDuck. ({message}) "
+            f"Could not establish connection to ArrowFlight Server. ({message}) "
             f"Will fall back to hive/spark for this session. "
-            f"If the error persists, you can disable FlyingDuck "
+            f"If the error persists, you can disable using ArrowFlight "
             f"by changing the cluster configuration (set 'enable_flyingduck'='false')."
         )
 
     def _initialize_connection(self):
         self._client = client.get_instance()
 
         if isinstance(self._client, client.external.Client):
@@ -173,15 +173,15 @@
                     and "Please register client certificates first." in message
                 ):
                     self = args[0]
                     self._register_certificates()
                     return method(*args, **kw)
                 else:
                     raise FeatureStoreException(
-                        "Could not read data using FlyingDuck. "
+                        "Could not read data using ArrowFlight. "
                         "If the issue persists, "
                         'use read_options={"use_hive": True} instead.'
                     ) from e
 
         return afs_error_handler_wrapper
 
     def _get_dataset(self, descriptor):
```

### Comparing `hsfs-3.3.0rc0/hsfs/core/builtin_transformation_function.py` & `hsfs-3.3.0rc1/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/code_api.py` & `hsfs-3.3.0rc1/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/code_engine.py` & `hsfs-3.3.0rc1/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/dataset_api.py` & `hsfs-3.3.0rc1/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.3.0rc1/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/execution.py` & `hsfs-3.3.0rc1/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/expectation_api.py` & `hsfs-3.3.0rc1/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/expectation_engine.py` & `hsfs-3.3.0rc1/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/expectation_suite_api.py` & `hsfs-3.3.0rc1/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/expectation_suite_engine.py` & `hsfs-3.3.0rc1/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/explicit_provenance.py` & `hsfs-3.3.0rc1/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/external_feature_group_engine.py` & `hsfs-3.3.0rc1/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_group_api.py` & `hsfs-3.3.0rc1/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_group_base_engine.py` & `hsfs-3.3.0rc1/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_group_engine.py` & `hsfs-3.3.0rc1/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_store_api.py` & `hsfs-3.3.0rc1/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_view_api.py` & `hsfs-3.3.0rc1/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/feature_view_engine.py` & `hsfs-3.3.0rc1/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/great_expectation_engine.py` & `hsfs-3.3.0rc1/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/hosts_api.py` & `hsfs-3.3.0rc1/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/hudi_engine.py` & `hsfs-3.3.0rc1/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/ingestion_job.py` & `hsfs-3.3.0rc1/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/ingestion_job_conf.py` & `hsfs-3.3.0rc1/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/inode.py` & `hsfs-3.3.0rc1/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/job.py` & `hsfs-3.3.0rc1/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/job_api.py` & `hsfs-3.3.0rc1/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/job_configuration.py` & `hsfs-3.3.0rc1/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/kafka_api.py` & `hsfs-3.3.0rc1/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/project_api.py` & `hsfs-3.3.0rc1/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/query_constructor_api.py` & `hsfs-3.3.0rc1/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/services_api.py` & `hsfs-3.3.0rc1/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/spine_group_engine.py` & `hsfs-3.3.0rc1/hsfs/core/spine_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/statistics_api.py` & `hsfs-3.3.0rc1/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/statistics_engine.py` & `hsfs-3.3.0rc1/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/storage_connector_api.py` & `hsfs-3.3.0rc1/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/tags_api.py` & `hsfs-3.3.0rc1/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/training_dataset_api.py` & `hsfs-3.3.0rc1/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/training_dataset_engine.py` & `hsfs-3.3.0rc1/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.3.0rc1/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/transformation_function_api.py` & `hsfs-3.3.0rc1/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/transformation_function_engine.py` & `hsfs-3.3.0rc1/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/validation_report_api.py` & `hsfs-3.3.0rc1/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/validation_report_engine.py` & `hsfs-3.3.0rc1/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/validation_result_api.py` & `hsfs-3.3.0rc1/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/validation_result_engine.py` & `hsfs-3.3.0rc1/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/variable_api.py` & `hsfs-3.3.0rc1/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/core/vector_server.py` & `hsfs-3.3.0rc1/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/decorators.py` & `hsfs-3.3.0rc1/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/engine/__init__.py` & `hsfs-3.3.0rc1/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/engine/python.py` & `hsfs-3.3.0rc1/hsfs/engine/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         feature_store,
         dataframe_type,
         schema=None,
         hive_config=None,
     ):
         if arrow_flight_client.get_instance().is_flyingduck_query_object(sql_query):
             result_df = util.run_with_loading_animation(
-                "Reading data from Hopsworks, using FlyingDuck",
+                "Reading data from Hopsworks, using ArrowFlight",
                 arrow_flight_client.get_instance().read_query,
                 sql_query,
             )
         else:
             with self._create_hive_connection(
                 feature_store, hive_config=hive_config
             ) as hive_conn:
```

### Comparing `hsfs-3.3.0rc0/hsfs/engine/spark.py` & `hsfs-3.3.0rc1/hsfs/engine/spark.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/expectation_suite.py` & `hsfs-3.3.0rc1/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/feature.py` & `hsfs-3.3.0rc1/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/feature_group.py` & `hsfs-3.3.0rc1/hsfs/feature_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -2934,4494 +2934,4508 @@
 0000b750: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
 0000b760: 6e63 6528 6578 7065 6374 6174 696f 6e5f  nce(expectation_
 0000b770: 7375 6974 652c 2045 7870 6563 7461 7469  suite, Expectati
 0000b780: 6f6e 5375 6974 6529 3a0a 2020 2020 2020  onSuite):.      
 0000b790: 2020 2020 2020 746d 705f 6578 7065 6374        tmp_expect
 0000b7a0: 6174 696f 6e5f 7375 6974 6520 3d20 6578  ation_suite = ex
 0000b7b0: 7065 6374 6174 696f 6e5f 7375 6974 652e  pectation_suite.
-0000b7c0: 746f 5f6a 736f 6e5f 6469 6374 2829 0a20  to_json_dict(). 
-0000b7d0: 2020 2020 2020 2020 2020 2074 6d70 5f65             tmp_e
-0000b7e0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000b7f0: 5b22 6665 6174 7572 6567 726f 7570 5f69  ["featuregroup_i
-0000b800: 6422 5d20 3d20 7365 6c66 2e5f 6964 0a20  d"] = self._id. 
-0000b810: 2020 2020 2020 2020 2020 2074 6d70 5f65             tmp_e
-0000b820: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000b830: 5b22 6665 6174 7572 6573 746f 7265 5f69  ["featurestore_i
-0000b840: 6422 5d20 3d20 7365 6c66 2e5f 6665 6174  d"] = self._feat
-0000b850: 7572 655f 7374 6f72 655f 6964 0a20 2020  ure_store_id.   
-0000b860: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-0000b870: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000b880: 203d 2045 7870 6563 7461 7469 6f6e 5375   = ExpectationSu
-0000b890: 6974 6528 2a2a 746d 705f 6578 7065 6374  ite(**tmp_expect
-0000b8a0: 6174 696f 6e5f 7375 6974 6529 0a20 2020  ation_suite).   
-0000b8b0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000b8c0: 616e 6365 2865 7870 6563 7461 7469 6f6e  ance(expectation
-0000b8d0: 5f73 7569 7465 2c20 6765 2e63 6f72 652e  _suite, ge.core.
-0000b8e0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-0000b8f0: 652e 4578 7065 6374 6174 696f 6e53 7569  e.ExpectationSui
-0000b900: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
-0000b910: 2073 656c 662e 5f65 7870 6563 7461 7469   self._expectati
-0000b920: 6f6e 5f73 7569 7465 203d 2045 7870 6563  on_suite = Expec
-0000b930: 7461 7469 6f6e 5375 6974 6528 0a20 2020  tationSuite(.   
-0000b940: 2020 2020 2020 2020 2020 2020 202a 2a65               **e
-0000b950: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000b960: 2e74 6f5f 6a73 6f6e 5f64 6963 7428 292c  .to_json_dict(),
-0000b970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b980: 2066 6561 7475 7265 5f73 746f 7265 5f69   feature_store_i
-0000b990: 643d 7365 6c66 2e5f 6665 6174 7572 655f  d=self._feature_
-0000b9a0: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
-0000b9b0: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-0000b9c0: 655f 6772 6f75 705f 6964 3d73 656c 662e  e_group_id=self.
-0000b9d0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000b9e0: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-0000b9f0: 6973 696e 7374 616e 6365 2865 7870 6563  isinstance(expec
-0000ba00: 7461 7469 6f6e 5f73 7569 7465 2c20 6469  tation_suite, di
-0000ba10: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-0000ba20: 2074 6d70 5f65 7870 6563 7461 7469 6f6e   tmp_expectation
-0000ba30: 5f73 7569 7465 203d 2065 7870 6563 7461  _suite = expecta
-0000ba40: 7469 6f6e 5f73 7569 7465 2e63 6f70 7928  tion_suite.copy(
-0000ba50: 290a 2020 2020 2020 2020 2020 2020 746d  ).            tm
-0000ba60: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
-0000ba70: 6974 655b 2266 6561 7475 7265 5f73 746f  ite["feature_sto
-0000ba80: 7265 5f69 6422 5d20 3d20 7365 6c66 2e5f  re_id"] = self._
-0000ba90: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
-0000baa0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-0000bab0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-0000bac0: 7465 5b22 6665 6174 7572 655f 6772 6f75  te["feature_grou
-0000bad0: 705f 6964 225d 203d 2073 656c 662e 5f69  p_id"] = self._i
-0000bae0: 640a 2020 2020 2020 2020 2020 2020 7365  d.            se
-0000baf0: 6c66 2e5f 6578 7065 6374 6174 696f 6e5f  lf._expectation_
-0000bb00: 7375 6974 6520 3d20 4578 7065 6374 6174  suite = Expectat
-0000bb10: 696f 6e53 7569 7465 282a 2a74 6d70 5f65  ionSuite(**tmp_e
-0000bb20: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000bb30: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-0000bb40: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000bb50: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000bb60: 2020 2020 2020 7365 6c66 2e5f 6578 7065        self._expe
-0000bb70: 6374 6174 696f 6e5f 7375 6974 6520 3d20  ctation_suite = 
-0000bb80: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
-0000bb90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000bba0: 6169 7365 2054 7970 6545 7272 6f72 280a  aise TypeError(.
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2254 6865 2061 7267 756d 656e 7420 6065  "The argument `e
-0000bbd0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000bbe0: 6020 6861 7320 746f 2062 6520 604e 6f6e  ` has to be `Non
-0000bbf0: 6560 206f 6620 7479 7065 2060 4578 7065  e` of type `Expe
-0000bc00: 6374 6174 696f 6e53 7569 7465 6020 6f72  ctationSuite` or
-0000bc10: 2060 6469 6374 602c 2062 7574 2069 7320   `dict`, but is 
-0000bc20: 6f66 2074 7970 653a 2060 7b7d 6022 2e66  of type: `{}`".f
-0000bc30: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0000bc40: 2020 2020 2020 2020 2020 2074 7970 6528             type(
-0000bc50: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-0000bc60: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000bc70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bc80: 2029 0a0a 2020 2020 4070 726f 7065 7274   )..    @propert
-0000bc90: 790a 2020 2020 6465 6620 6f6e 6c69 6e65  y.    def online
-0000bca0: 5f65 6e61 626c 6564 2873 656c 6629 3a0a  _enabled(self):.
-0000bcb0: 2020 2020 2020 2020 2222 2253 6574 7469          """Setti
-0000bcc0: 6e67 2069 6620 7468 6520 6665 6174 7572  ng if the featur
-0000bcd0: 6520 6772 6f75 7020 6973 2061 7661 696c  e group is avail
-0000bce0: 6162 6c65 2069 6e20 6f6e 6c69 6e65 2073  able in online s
-0000bcf0: 746f 7261 6765 2e22 2222 0a20 2020 2020  torage.""".     
-0000bd00: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000bd10: 6f6e 6c69 6e65 5f65 6e61 626c 6564 0a0a  online_enabled..
-0000bd20: 2020 2020 406f 6e6c 696e 655f 656e 6162      @online_enab
-0000bd30: 6c65 642e 7365 7474 6572 0a20 2020 2064  led.setter.    d
-0000bd40: 6566 206f 6e6c 696e 655f 656e 6162 6c65  ef online_enable
-0000bd50: 6428 7365 6c66 2c20 6f6e 6c69 6e65 5f65  d(self, online_e
-0000bd60: 6e61 626c 6564 293a 0a20 2020 2020 2020  nabled):.       
-0000bd70: 2073 656c 662e 5f6f 6e6c 696e 655f 656e   self._online_en
-0000bd80: 6162 6c65 6420 3d20 6f6e 6c69 6e65 5f65  abled = online_e
-0000bd90: 6e61 626c 6564 0a0a 2020 2020 4070 726f  nabled..    @pro
-0000bda0: 7065 7274 790a 2020 2020 6465 6620 7375  perty.    def su
-0000bdb0: 626a 6563 7428 7365 6c66 293a 0a20 2020  bject(self):.   
-0000bdc0: 2020 2020 2022 2222 5375 626a 6563 7420       """Subject 
-0000bdd0: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
-0000bde0: 726f 7570 2e22 2222 0a20 2020 2020 2020  roup.""".       
-0000bdf0: 2069 6620 7365 6c66 2e5f 7375 626a 6563   if self._subjec
-0000be00: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
-0000be10: 2020 2020 2020 2023 2063 6163 6865 2074         # cache t
-0000be20: 6865 2073 6368 656d 610a 2020 2020 2020  he schema.      
-0000be30: 2020 2020 2020 7365 6c66 2e5f 7375 626a        self._subj
-0000be40: 6563 7420 3d20 7365 6c66 2e5f 6665 6174  ect = self._feat
-0000be50: 7572 655f 6772 6f75 705f 656e 6769 6e65  ure_group_engine
-0000be60: 2e67 6574 5f73 7562 6a65 6374 2873 656c  .get_subject(sel
-0000be70: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
-0000be80: 6e20 7365 6c66 2e5f 7375 626a 6563 740a  n self._subject.
-0000be90: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000bea0: 2020 2064 6566 2061 7672 6f5f 7363 6865     def avro_sche
-0000beb0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
-0000bec0: 2020 2222 2241 7672 6f20 7363 6865 6d61    """Avro schema
-0000bed0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-0000bee0: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
-0000bef0: 726f 7570 2e22 2222 0a20 2020 2020 2020  roup.""".       
-0000bf00: 2072 6574 7572 6e20 7365 6c66 2e73 7562   return self.sub
-0000bf10: 6a65 6374 5b22 7363 6865 6d61 225d 0a0a  ject["schema"]..
-0000bf20: 2020 2020 6465 6620 6765 745f 636f 6d70      def get_comp
-0000bf30: 6c65 785f 6665 6174 7572 6573 2873 656c  lex_features(sel
-0000bf40: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
-0000bf50: 6574 7572 6e73 2074 6865 206e 616d 6573  eturns the names
-0000bf60: 206f 6620 616c 6c20 6665 6174 7572 6573   of all features
-0000bf70: 2077 6974 6820 6120 636f 6d70 6c65 7820   with a complex 
-0000bf80: 6461 7461 2074 7970 6520 696e 2074 6869  data type in thi
-0000bf90: 730a 2020 2020 2020 2020 6665 6174 7572  s.        featur
-0000bfa0: 6520 6772 6f75 702e 0a0a 2020 2020 2020  e group...      
-0000bfb0: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
-0000bfc0: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
-0000bfd0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
-0000bfe0: 636f 6d70 6c65 785f 6474 7970 655f 6665  complex_dtype_fe
-0000bff0: 6174 7572 6573 203d 2066 672e 6765 745f  atures = fg.get_
-0000c000: 636f 6d70 6c65 785f 6665 6174 7572 6573  complex_features
-0000c010: 2829 0a20 2020 2020 2020 2020 2020 2060  ().            `
-0000c020: 6060 0a20 2020 2020 2020 2022 2222 0a20  ``.        """. 
-0000c030: 2020 2020 2020 2072 6574 7572 6e20 5b66         return [f
-0000c040: 2e6e 616d 6520 666f 7220 6620 696e 2073  .name for f in s
-0000c050: 656c 662e 6665 6174 7572 6573 2069 6620  elf.features if 
-0000c060: 662e 6973 5f63 6f6d 706c 6578 2829 5d0a  f.is_complex()].
-0000c070: 0a20 2020 2064 6566 205f 6765 745f 656e  .    def _get_en
-0000c080: 636f 6465 645f 6176 726f 5f73 6368 656d  coded_avro_schem
-0000c090: 6128 7365 6c66 293a 0a20 2020 2020 2020  a(self):.       
-0000c0a0: 2063 6f6d 706c 6578 5f66 6561 7475 7265   complex_feature
-0000c0b0: 7320 3d20 7365 6c66 2e67 6574 5f63 6f6d  s = self.get_com
-0000c0c0: 706c 6578 5f66 6561 7475 7265 7328 290a  plex_features().
-0000c0d0: 2020 2020 2020 2020 7363 6865 6d61 203d          schema =
-0000c0e0: 206a 736f 6e2e 6c6f 6164 7328 7365 6c66   json.loads(self
-0000c0f0: 2e61 7672 6f5f 7363 6865 6d61 290a 0a20  .avro_schema).. 
-0000c100: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
-0000c110: 2069 6e20 7363 6865 6d61 5b22 6669 656c   in schema["fiel
-0000c120: 6473 225d 3a0a 2020 2020 2020 2020 2020  ds"]:.          
-0000c130: 2020 6966 2066 6965 6c64 5b22 6e61 6d65    if field["name
-0000c140: 225d 2069 6e20 636f 6d70 6c65 785f 6665  "] in complex_fe
-0000c150: 6174 7572 6573 3a0a 2020 2020 2020 2020  atures:.        
-0000c160: 2020 2020 2020 2020 6669 656c 645b 2274          field["t
-0000c170: 7970 6522 5d20 3d20 5b22 6e75 6c6c 222c  ype"] = ["null",
-0000c180: 2022 6279 7465 7322 5d0a 0a20 2020 2020   "bytes"]..     
-0000c190: 2020 2073 6368 656d 615f 7320 3d20 6a73     schema_s = js
-0000c1a0: 6f6e 2e64 756d 7073 2873 6368 656d 6129  on.dumps(schema)
-0000c1b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000c1c0: 2020 2020 2020 2020 2020 6176 726f 2e73            avro.s
-0000c1d0: 6368 656d 612e 7061 7273 6528 7363 6865  chema.parse(sche
-0000c1e0: 6d61 5f73 290a 2020 2020 2020 2020 6578  ma_s).        ex
-0000c1f0: 6365 7074 2061 7672 6f2e 7363 6865 6d61  cept avro.schema
-0000c200: 2e53 6368 656d 6150 6172 7365 4578 6365  .SchemaParseExce
-0000c210: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-0000c220: 2020 2020 2020 2020 7261 6973 6520 4665          raise Fe
-0000c230: 6174 7572 6553 746f 7265 4578 6365 7074  atureStoreExcept
-0000c240: 696f 6e28 2246 6169 6c65 6420 746f 2063  ion("Failed to c
-0000c250: 6f6e 7374 7275 6374 2041 7672 6f20 5363  onstruct Avro Sc
-0000c260: 6865 6d61 3a20 7b7d 222e 666f 726d 6174  hema: {}".format
-0000c270: 2865 2929 0a20 2020 2020 2020 2072 6574  (e)).        ret
-0000c280: 7572 6e20 7363 6865 6d61 5f73 0a0a 2020  urn schema_s..  
-0000c290: 2020 6465 6620 5f67 6574 5f66 6561 7475    def _get_featu
-0000c2a0: 7265 5f61 7672 6f5f 7363 6865 6d61 2873  re_avro_schema(s
-0000c2b0: 656c 662c 2066 6561 7475 7265 5f6e 616d  elf, feature_nam
-0000c2c0: 6529 3a0a 2020 2020 2020 2020 666f 7220  e):.        for 
-0000c2d0: 6669 656c 6420 696e 206a 736f 6e2e 6c6f  field in json.lo
-0000c2e0: 6164 7328 7365 6c66 2e61 7672 6f5f 7363  ads(self.avro_sc
-0000c2f0: 6865 6d61 295b 2266 6965 6c64 7322 5d3a  hema)["fields"]:
-0000c300: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c310: 6669 656c 645b 226e 616d 6522 5d20 3d3d  field["name"] ==
-0000c320: 2066 6561 7475 7265 5f6e 616d 653a 0a20   feature_name:. 
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000c340: 6574 7572 6e20 6a73 6f6e 2e64 756d 7073  eturn json.dumps
-0000c350: 2866 6965 6c64 5b22 7479 7065 225d 290a  (field["type"]).
-0000c360: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000c370: 2020 2064 6566 2066 6561 7475 7265 7328     def features(
-0000c380: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000c390: 2222 5363 6865 6d61 2069 6e66 6f72 6d61  ""Schema informa
-0000c3a0: 7469 6f6e 2e22 2222 0a20 2020 2020 2020  tion.""".       
-0000c3b0: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
-0000c3c0: 6174 7572 6573 0a0a 2020 2020 4066 6561  atures..    @fea
-0000c3d0: 7475 7265 732e 7365 7474 6572 0a20 2020  tures.setter.   
-0000c3e0: 2064 6566 2066 6561 7475 7265 7328 7365   def features(se
-0000c3f0: 6c66 2c20 6e65 775f 6665 6174 7572 6573  lf, new_features
-0000c400: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000c410: 5f66 6561 7475 7265 7320 3d20 6e65 775f  _features = new_
-0000c420: 6665 6174 7572 6573 0a0a 0a63 6c61 7373  features...class
-0000c430: 2046 6561 7475 7265 4772 6f75 7028 4665   FeatureGroup(Fe
-0000c440: 6174 7572 6547 726f 7570 4261 7365 293a  atureGroupBase):
-0000c450: 0a20 2020 2043 4143 4845 445f 4645 4154  .    CACHED_FEAT
-0000c460: 5552 455f 4752 4f55 5020 3d20 2243 4143  URE_GROUP = "CAC
-0000c470: 4845 445f 4645 4154 5552 455f 4752 4f55  HED_FEATURE_GROU
-0000c480: 5022 0a20 2020 2053 5452 4541 4d5f 4645  P".    STREAM_FE
-0000c490: 4154 5552 455f 4752 4f55 5020 3d20 2253  ATURE_GROUP = "S
-0000c4a0: 5452 4541 4d5f 4645 4154 5552 455f 4752  TREAM_FEATURE_GR
-0000c4b0: 4f55 5022 0a20 2020 2045 4e54 4954 595f  OUP".    ENTITY_
-0000c4c0: 5459 5045 203d 2022 6665 6174 7572 6567  TYPE = "featureg
-0000c4d0: 726f 7570 7322 0a0a 2020 2020 6465 6620  roups"..    def 
-0000c4e0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0000c4f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000c500: 6e61 6d65 2c0a 2020 2020 2020 2020 7665  name,.        ve
-0000c510: 7273 696f 6e2c 0a20 2020 2020 2020 2066  rsion,.        f
-0000c520: 6561 7475 7265 7374 6f72 655f 6964 2c0a  eaturestore_id,.
-0000c530: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000c540: 696f 6e3d 2222 2c0a 2020 2020 2020 2020  ion="",.        
-0000c550: 7061 7274 6974 696f 6e5f 6b65 793d 4e6f  partition_key=No
-0000c560: 6e65 2c0a 2020 2020 2020 2020 7072 696d  ne,.        prim
-0000c570: 6172 795f 6b65 793d 4e6f 6e65 2c0a 2020  ary_key=None,.  
-0000c580: 2020 2020 2020 6875 6469 5f70 7265 636f        hudi_preco
-0000c590: 6d62 696e 655f 6b65 793d 4e6f 6e65 2c0a  mbine_key=None,.
-0000c5a0: 2020 2020 2020 2020 6665 6174 7572 6573          features
-0000c5b0: 746f 7265 5f6e 616d 653d 4e6f 6e65 2c0a  tore_name=None,.
-0000c5c0: 2020 2020 2020 2020 6372 6561 7465 643d          created=
-0000c5d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6372  None,.        cr
-0000c5e0: 6561 746f 723d 4e6f 6e65 2c0a 2020 2020  eator=None,.    
-0000c5f0: 2020 2020 6964 3d4e 6f6e 652c 0a20 2020      id=None,.   
-0000c600: 2020 2020 2066 6561 7475 7265 733d 4e6f       features=No
-0000c610: 6e65 2c0a 2020 2020 2020 2020 6c6f 6361  ne,.        loca
-0000c620: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 2020  tion=None,.     
-0000c630: 2020 206f 6e6c 696e 655f 656e 6162 6c65     online_enable
-0000c640: 643d 4661 6c73 652c 0a20 2020 2020 2020  d=False,.       
-0000c650: 2074 696d 655f 7472 6176 656c 5f66 6f72   time_travel_for
-0000c660: 6d61 743d 4e6f 6e65 2c0a 2020 2020 2020  mat=None,.      
-0000c670: 2020 7374 6174 6973 7469 6373 5f63 6f6e    statistics_con
-0000c680: 6669 673d 4e6f 6e65 2c0a 2020 2020 2020  fig=None,.      
-0000c690: 2020 6f6e 6c69 6e65 5f74 6f70 6963 5f6e    online_topic_n
-0000c6a0: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-0000c6b0: 2020 6576 656e 745f 7469 6d65 3d4e 6f6e    event_time=Non
-0000c6c0: 652c 0a20 2020 2020 2020 2073 7472 6561  e,.        strea
-0000c6d0: 6d3d 4661 6c73 652c 0a20 2020 2020 2020  m=False,.       
-0000c6e0: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-0000c6f0: 7465 3d4e 6f6e 652c 0a20 2020 2020 2020  te=None,.       
-0000c700: 2070 6172 656e 7473 3d4e 6f6e 652c 0a20   parents=None,. 
-0000c710: 2020 2020 2020 2068 7265 663d 4e6f 6e65         href=None
-0000c720: 2c0a 2020 2020 2020 2020 6465 6c74 615f  ,.        delta_
-0000c730: 7374 7265 616d 6572 5f6a 6f62 5f63 6f6e  streamer_job_con
-0000c740: 663d 4e6f 6e65 2c0a 2020 2020 293a 0a20  f=None,.    ):. 
-0000c750: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-0000c760: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000c770: 2020 2020 2066 6561 7475 7265 7374 6f72       featurestor
-0000c780: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-0000c790: 2020 6c6f 6361 7469 6f6e 2c0a 2020 2020    location,.    
-0000c7a0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
-0000c7b0: 6d65 3d65 7665 6e74 5f74 696d 652c 0a20  me=event_time,. 
-0000c7c0: 2020 2020 2020 2020 2020 206f 6e6c 696e             onlin
-0000c7d0: 655f 656e 6162 6c65 643d 6f6e 6c69 6e65  e_enabled=online
-0000c7e0: 5f65 6e61 626c 6564 2c0a 2020 2020 2020  _enabled,.      
-0000c7f0: 2020 2020 2020 6964 3d69 642c 0a20 2020        id=id,.   
-0000c800: 2020 2020 2020 2020 2065 7870 6563 7461           expecta
-0000c810: 7469 6f6e 5f73 7569 7465 3d65 7870 6563  tion_suite=expec
-0000c820: 7461 7469 6f6e 5f73 7569 7465 2c0a 2020  tation_suite,.  
-0000c830: 2020 2020 2020 2020 2020 6f6e 6c69 6e65            online
-0000c840: 5f74 6f70 6963 5f6e 616d 653d 6f6e 6c69  _topic_name=onli
-0000c850: 6e65 5f74 6f70 6963 5f6e 616d 652c 0a20  ne_topic_name,. 
-0000c860: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000c870: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
-0000c880: 7374 6f72 655f 6e61 6d65 203d 2066 6561  store_name = fea
-0000c890: 7475 7265 7374 6f72 655f 6e61 6d65 0a20  turestore_name. 
-0000c8a0: 2020 2020 2020 2073 656c 662e 5f64 6573         self._des
-0000c8b0: 6372 6970 7469 6f6e 203d 2064 6573 6372  cription = descr
-0000c8c0: 6970 7469 6f6e 0a20 2020 2020 2020 2073  iption.        s
-0000c8d0: 656c 662e 5f63 7265 6174 6564 203d 2063  elf._created = c
-0000c8e0: 7265 6174 6564 0a20 2020 2020 2020 2073  reated.        s
-0000c8f0: 656c 662e 5f63 7265 6174 6f72 203d 2075  elf._creator = u
-0000c900: 7365 722e 5573 6572 2e66 726f 6d5f 7265  ser.User.from_re
-0000c910: 7370 6f6e 7365 5f6a 736f 6e28 6372 6561  sponse_json(crea
-0000c920: 746f 7229 0a20 2020 2020 2020 2073 656c  tor).        sel
-0000c930: 662e 5f76 6572 7369 6f6e 203d 2076 6572  f._version = ver
-0000c940: 7369 6f6e 0a20 2020 2020 2020 2073 656c  sion.        sel
-0000c950: 662e 5f6e 616d 6520 3d20 6e61 6d65 0a20  f._name = name. 
-0000c960: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
-0000c970: 7475 7265 7320 3d20 5b0a 2020 2020 2020  tures = [.      
-0000c980: 2020 2020 2020 6665 6174 7572 652e 4665        feature.Fe
-0000c990: 6174 7572 652e 6672 6f6d 5f72 6573 706f  ature.from_respo
-0000c9a0: 6e73 655f 6a73 6f6e 2866 6561 7429 2069  nse_json(feat) i
-0000c9b0: 6620 6973 696e 7374 616e 6365 2866 6561  f isinstance(fea
-0000c9c0: 742c 2064 6963 7429 2065 6c73 6520 6665  t, dict) else fe
-0000c9d0: 6174 0a20 2020 2020 2020 2020 2020 2066  at.            f
-0000c9e0: 6f72 2066 6561 7420 696e 2028 6665 6174  or feat in (feat
-0000c9f0: 7572 6573 206f 7220 5b5d 290a 2020 2020  ures or []).    
-0000ca00: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
-0000ca10: 656c 662e 5f74 696d 655f 7472 6176 656c  elf._time_travel
-0000ca20: 5f66 6f72 6d61 7420 3d20 280a 2020 2020  _format = (.    
-0000ca30: 2020 2020 2020 2020 7469 6d65 5f74 7261          time_tra
-0000ca40: 7665 6c5f 666f 726d 6174 2e75 7070 6572  vel_format.upper
-0000ca50: 2829 2069 6620 7469 6d65 5f74 7261 7665  () if time_trave
-0000ca60: 6c5f 666f 726d 6174 2069 7320 6e6f 7420  l_format is not 
-0000ca70: 4e6f 6e65 2065 6c73 6520 4e6f 6e65 0a20  None else None. 
-0000ca80: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000ca90: 2020 7365 6c66 2e5f 7374 7265 616d 203d    self._stream =
-0000caa0: 2073 7472 6561 6d0a 2020 2020 2020 2020   stream.        
-0000cab0: 7365 6c66 2e5f 7061 7265 6e74 7320 3d20  self._parents = 
-0000cac0: 7061 7265 6e74 730a 2020 2020 2020 2020  parents.        
-0000cad0: 7365 6c66 2e5f 6465 6c74 6173 7472 6561  self._deltastrea
-0000cae0: 6d65 725f 6a6f 6263 6f6e 6620 3d20 6465  mer_jobconf = de
-0000caf0: 6c74 615f 7374 7265 616d 6572 5f6a 6f62  lta_streamer_job
-0000cb00: 5f63 6f6e 660a 0a20 2020 2020 2020 2073  _conf..        s
-0000cb10: 656c 662e 5f62 6163 6b66 696c 6c5f 6a6f  elf._backfill_jo
-0000cb20: 6220 3d20 4e6f 6e65 0a0a 2020 2020 2020  b = None..      
-0000cb30: 2020 6966 2073 656c 662e 5f69 643a 0a20    if self._id:. 
-0000cb40: 2020 2020 2020 2020 2020 2023 2069 6e69             # ini
-0000cb50: 7469 616c 697a 6564 2062 7920 6261 636b  tialized by back
-0000cb60: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
-0000cb70: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
-0000cb80: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0000cb90: 2020 2020 2066 6561 742e 6e61 6d65 2066       feat.name f
-0000cba0: 6f72 2066 6561 7420 696e 2073 656c 662e  or feat in self.
-0000cbb0: 5f66 6561 7475 7265 7320 6966 2066 6561  _features if fea
-0000cbc0: 742e 7072 696d 6172 7920 6973 2054 7275  t.primary is Tru
-0000cbd0: 650a 2020 2020 2020 2020 2020 2020 5d0a  e.            ].
-0000cbe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cbf0: 2e5f 7061 7274 6974 696f 6e5f 6b65 7920  ._partition_key 
-0000cc00: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0000cc10: 2020 2020 6665 6174 2e6e 616d 6520 666f      feat.name fo
-0000cc20: 7220 6665 6174 2069 6e20 7365 6c66 2e5f  r feat in self._
-0000cc30: 6665 6174 7572 6573 2069 6620 6665 6174  features if feat
-0000cc40: 2e70 6172 7469 7469 6f6e 2069 7320 5472  .partition is Tr
-0000cc50: 7565 0a20 2020 2020 2020 2020 2020 205d  ue.            ]
-0000cc60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000cc70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000cc80: 2020 7469 6d65 5f74 7261 7665 6c5f 666f    time_travel_fo
-0000cc90: 726d 6174 2069 7320 6e6f 7420 4e6f 6e65  rmat is not None
-0000cca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ccb0: 2061 6e64 2074 696d 655f 7472 6176 656c   and time_travel
-0000ccc0: 5f66 6f72 6d61 742e 7570 7065 7228 2920  _format.upper() 
-0000ccd0: 3d3d 2022 4855 4449 220a 2020 2020 2020  == "HUDI".      
-0000cce0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-0000ccf0: 6c66 2e5f 6665 6174 7572 6573 0a20 2020  lf._features.   
-0000cd00: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-0000cd10: 2020 2020 2020 2020 2020 2020 2320 6875              # hu
-0000cd20: 6469 2070 7265 636f 6d62 696e 6520 6b65  di precombine ke
-0000cd30: 7920 6973 2061 6c77 6179 7320 6120 7369  y is always a si
-0000cd40: 6e67 6c65 2066 6561 7475 7265 0a20 2020  ngle feature.   
-0000cd50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000cd60: 662e 5f68 7564 695f 7072 6563 6f6d 6269  f._hudi_precombi
-0000cd70: 6e65 5f6b 6579 203d 205b 0a20 2020 2020  ne_key = [.     
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000cd90: 6561 742e 6e61 6d65 0a20 2020 2020 2020  eat.name.       
-0000cda0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000cdb0: 2066 6561 7420 696e 2073 656c 662e 5f66   feat in self._f
-0000cdc0: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
-0000cdd0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0000cde0: 6561 742e 6875 6469 5f70 7265 636f 6d62  eat.hudi_precomb
-0000cdf0: 696e 655f 6b65 7920 6973 2054 7275 650a  ine_key is True.
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-0000ce20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000ce30: 2020 2020 2020 2073 656c 662e 5f68 7564         self._hud
-0000ce40: 695f 7072 6563 6f6d 6269 6e65 5f6b 6579  i_precombine_key
-0000ce50: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-0000ce60: 2020 2020 2073 656c 662e 7374 6174 6973       self.statis
-0000ce70: 7469 6373 5f63 6f6e 6669 6720 3d20 7374  tics_config = st
-0000ce80: 6174 6973 7469 6373 5f63 6f6e 6669 670a  atistics_config.
-0000ce90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000cea0: 2020 2020 2020 2020 2020 2023 2069 6e69             # ini
-0000ceb0: 7469 616c 697a 6564 2062 7920 7573 6572  tialized by user
-0000cec0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-0000ced0: 6f72 2070 7974 686f 6e20 656e 6769 6e65  or python engine
-0000cee0: 2077 6520 616c 7761 7973 2075 7365 2073   we always use s
-0000cef0: 7472 6561 6d20 6665 6174 7572 6520 6772  tream feature gr
-0000cf00: 6f75 700a 2020 2020 2020 2020 2020 2020  oup.            
-0000cf10: 6966 2065 6e67 696e 652e 6765 745f 7479  if engine.get_ty
-0000cf20: 7065 2829 203d 3d20 2270 7974 686f 6e22  pe() == "python"
-0000cf30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cf40: 2020 7365 6c66 2e5f 7374 7265 616d 203d    self._stream =
-0000cf50: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000cf60: 2020 2320 666f 7220 7374 7265 616d 2066    # for stream f
-0000cf70: 6561 7475 7265 2067 726f 7570 2074 696d  eature group tim
-0000cf80: 6520 7472 6176 656c 2066 6f72 6d61 7420  e travel format 
-0000cf90: 6973 2061 6c77 6179 7320 4855 4449 0a20  is always HUDI. 
-0000cfa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000cfb0: 6c66 2e5f 7374 7265 616d 3a0a 2020 2020  lf._stream:.    
-0000cfc0: 2020 2020 2020 2020 2020 2020 6578 7065              expe
-0000cfd0: 6374 6564 5f66 6f72 6d61 7420 3d20 2248  cted_format = "H
-0000cfe0: 5544 4922 0a20 2020 2020 2020 2020 2020  UDI".           
-0000cff0: 2020 2020 2069 6620 7365 6c66 2e5f 7469       if self._ti
-0000d000: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
-0000d010: 2021 3d20 6578 7065 6374 6564 5f66 6f72   != expected_for
-0000d020: 6d61 743a 0a20 2020 2020 2020 2020 2020  mat:.           
-0000d030: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-0000d040: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d070: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-0000d080: 6865 2070 726f 7669 6465 6420 7469 6d65  he provided time
-0000d090: 2074 7261 7665 6c20 666f 726d 6174 2060   travel format `
-0000d0a0: 7b7d 6020 6861 7320 6265 656e 206f 7665  {}` has been ove
-0000d0b0: 7277 7269 7474 656e 2022 0a20 2020 2020  rwritten ".     
-0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0d0: 2020 2020 2020 2022 6265 6361 7573 6520         "because 
-0000d0e0: 5374 7265 616d 2065 6e61 626c 6564 2066  Stream enabled f
-0000d0f0: 6561 7475 7265 2067 726f 7570 7320 6f6e  eature groups on
-0000d100: 6c79 2073 7570 706f 7274 2060 7b7d 6022  ly support `{}`"
-0000d110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d120: 2020 2020 2020 2020 2029 2e66 6f72 6d61           ).forma
-0000d130: 7428 7365 6c66 2e5f 7469 6d65 5f74 7261  t(self._time_tra
-0000d140: 7665 6c5f 666f 726d 6174 2c20 6578 7065  vel_format, expe
-0000d150: 6374 6564 5f66 6f72 6d61 7429 2c0a 2020  cted_format),.  
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 2020 2020 2020 7574 696c 2e46 6561 7475        util.Featu
-0000d180: 7265 4772 6f75 7057 6172 6e69 6e67 2c0a  reGroupWarning,.
-0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000d1b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000d1c0: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
-0000d1d0: 6174 203d 2065 7870 6563 7465 645f 666f  at = expected_fo
-0000d1e0: 726d 6174 0a0a 2020 2020 2020 2020 2020  rmat..          
-0000d1f0: 2020 7365 6c66 2e70 7269 6d61 7279 5f6b    self.primary_k
-0000d200: 6579 203d 2070 7269 6d61 7279 5f6b 6579  ey = primary_key
-0000d210: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d220: 662e 7061 7274 6974 696f 6e5f 6b65 7920  f.partition_key 
-0000d230: 3d20 7061 7274 6974 696f 6e5f 6b65 790a  = partition_key.
-0000d240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d250: 2e5f 6875 6469 5f70 7265 636f 6d62 696e  ._hudi_precombin
-0000d260: 655f 6b65 7920 3d20 280a 2020 2020 2020  e_key = (.      
-0000d270: 2020 2020 2020 2020 2020 6875 6469 5f70            hudi_p
-0000d280: 7265 636f 6d62 696e 655f 6b65 792e 6c6f  recombine_key.lo
-0000d290: 7765 7228 290a 2020 2020 2020 2020 2020  wer().          
-0000d2a0: 2020 2020 2020 6966 2068 7564 695f 7072        if hudi_pr
-0000d2b0: 6563 6f6d 6269 6e65 5f6b 6579 2069 7320  ecombine_key is 
-0000d2c0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000d2d0: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
-0000d2e0: 662e 5f74 696d 655f 7472 6176 656c 5f66  f._time_travel_f
-0000d2f0: 6f72 6d61 7420 6973 206e 6f74 204e 6f6e  ormat is not Non
-0000d300: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000d310: 2020 616e 6420 7365 6c66 2e5f 7469 6d65    and self._time
-0000d320: 5f74 7261 7665 6c5f 666f 726d 6174 203d  _travel_format =
-0000d330: 3d20 2248 5544 4922 0a20 2020 2020 2020  = "HUDI".       
-0000d340: 2020 2020 2020 2020 2065 6c73 6520 4e6f           else No
-0000d350: 6e65 0a20 2020 2020 2020 2020 2020 2029  ne.            )
-0000d360: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d370: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
-0000d380: 6669 6720 3d20 7374 6174 6973 7469 6373  fig = statistics
-0000d390: 5f63 6f6e 6669 670a 0a20 2020 2020 2020  _config..       
-0000d3a0: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-0000d3b0: 726f 7570 5f65 6e67 696e 6520 3d20 6665  roup_engine = fe
-0000d3c0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-0000d3d0: 6e65 2e46 6561 7475 7265 4772 6f75 7045  ne.FeatureGroupE
-0000d3e0: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
-0000d3f0: 2020 2066 6561 7475 7265 7374 6f72 655f     featurestore_
-0000d400: 6964 0a20 2020 2020 2020 2029 0a20 2020  id.        ).   
-0000d410: 2020 2020 2073 656c 662e 5f68 7265 6620       self._href 
-0000d420: 3d20 6872 6566 0a0a 2020 2020 2020 2020  = href..        
-0000d430: 2320 6361 6368 6520 666f 7220 6f70 7469  # cache for opti
-0000d440: 6d69 7a65 6420 7772 6974 6573 0a20 2020  mized writes.   
-0000d450: 2020 2020 2073 656c 662e 5f6b 6166 6b61       self._kafka
-0000d460: 5f70 726f 6475 6365 7220 3d20 4e6f 6e65  _producer = None
-0000d470: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-0000d480: 6561 7475 7265 5f77 7269 7465 7273 203d  eature_writers =
-0000d490: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000d4a0: 6c66 2e5f 7772 6974 6572 203d 204e 6f6e  lf._writer = Non
-0000d4b0: 650a 0a20 2020 2064 6566 2072 6561 6428  e..    def read(
-0000d4c0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000d4d0: 2020 2020 2020 2077 616c 6c63 6c6f 636b         wallclock
-0000d4e0: 5f74 696d 653a 204f 7074 696f 6e61 6c5b  _time: Optional[
-0000d4f0: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
-0000d500: 6461 7465 7469 6d65 2c20 6461 7465 5d5d  datetime, date]]
-0000d510: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000d520: 206f 6e6c 696e 653a 204f 7074 696f 6e61   online: Optiona
-0000d530: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-0000d540: 0a20 2020 2020 2020 2064 6174 6166 7261  .        datafra
-0000d550: 6d65 5f74 7970 653a 204f 7074 696f 6e61  me_type: Optiona
-0000d560: 6c5b 7374 725d 203d 2022 6465 6661 756c  l[str] = "defaul
-0000d570: 7422 2c0a 2020 2020 2020 2020 7265 6164  t",.        read
-0000d580: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-0000d590: 616c 5b64 6963 745d 203d 207b 7d2c 0a20  al[dict] = {},. 
-0000d5a0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000d5b0: 220a 2020 2020 2020 2020 5265 6164 2074  ".        Read t
-0000d5c0: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-0000d5d0: 2069 6e74 6f20 6120 6461 7461 6672 616d   into a datafram
-0000d5e0: 652e 0a0a 2020 2020 2020 2020 5265 6164  e...        Read
-0000d5f0: 7320 7468 6520 6665 6174 7572 6520 6772  s the feature gr
-0000d600: 6f75 7020 6279 2064 6566 6175 6c74 2066  oup by default f
-0000d610: 726f 6d20 7468 6520 6f66 666c 696e 6520  rom the offline 
-0000d620: 7374 6f72 6167 6520 6173 2053 7061 726b  storage as Spark
-0000d630: 2044 6174 6146 7261 6d65 0a20 2020 2020   DataFrame.     
-0000d640: 2020 206f 6e20 486f 7073 776f 726b 7320     on Hopsworks 
-0000d650: 616e 6420 4461 7461 6272 6963 6b73 2c20  and Databricks, 
-0000d660: 616e 6420 6173 2050 616e 6461 7320 6461  and as Pandas da
-0000d670: 7461 6672 616d 6520 6f6e 2041 5753 2053  taframe on AWS S
-0000d680: 6167 656d 616b 6572 2061 6e64 2070 7572  agemaker and pur
-0000d690: 650a 2020 2020 2020 2020 5079 7468 6f6e  e.        Python
-0000d6a0: 2065 6e76 6972 6f6e 6d65 6e74 732e 0a0a   environments...
-0000d6b0: 2020 2020 2020 2020 5365 7420 606f 6e6c          Set `onl
-0000d6c0: 696e 6560 2074 6f20 6054 7275 6560 2074  ine` to `True` t
-0000d6d0: 6f20 7265 6164 2066 726f 6d20 7468 6520  o read from the 
-0000d6e0: 6f6e 6c69 6e65 2073 746f 7261 6765 2c20  online storage, 
-0000d6f0: 6f72 2063 6861 6e67 650a 2020 2020 2020  or change.      
-0000d700: 2020 6064 6174 6166 7261 6d65 5f74 7970    `dataframe_typ
-0000d710: 6560 2074 6f20 7265 6164 2061 7320 6120  e` to read as a 
-0000d720: 6469 6666 6572 656e 7420 666f 726d 6174  different format
-0000d730: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-0000d740: 7861 6d70 6c65 2022 5265 6164 2066 6561  xample "Read fea
-0000d750: 7475 7265 2067 726f 7570 2061 7320 6f66  ture group as of
-0000d760: 206c 6174 6573 7420 7374 6174 653a 220a   latest state:".
-0000d770: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-0000d780: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-0000d790: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-0000d7a0: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-0000d7b0: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-0000d7c0: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-0000d7d0: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-0000d7e0: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-0000d7f0: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-0000d800: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
-0000d810: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-0000d820: 6f75 7028 2e2e 2e29 0a20 2020 2020 2020  oup(...).       
-0000d830: 2020 2020 2066 672e 7265 6164 2829 0a20       fg.read(). 
-0000d840: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-0000d850: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-0000d860: 706c 6520 2252 6561 6420 6665 6174 7572  ple "Read featur
-0000d870: 6520 6772 6f75 7020 6173 206f 6620 7370  e group as of sp
-0000d880: 6563 6966 6963 2070 6f69 6e74 2069 6e20  ecific point in 
-0000d890: 7469 6d65 3a22 0a20 2020 2020 2020 2020  time:".         
-0000d8a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-0000d8b0: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
-0000d8c0: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-0000d8d0: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
-0000d8e0: 290a 2020 2020 2020 2020 2020 2020 6667  ).            fg
-0000d8f0: 2e72 6561 6428 2232 3032 302d 3130 2d32  .read("2020-10-2
-0000d900: 3020 3037 3a33 343a 3131 2229 0a20 2020  0 07:34:11").   
-0000d910: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
-0000d920: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
-0000d930: 730a 2020 2020 2020 2020 2020 2020 7761  s.            wa
-0000d940: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4966  llclock_time: If
-0000d950: 2073 7065 6369 6669 6564 2077 696c 6c20   specified will 
-0000d960: 7265 7472 6965 7665 2066 6561 7475 7265  retrieve feature
-0000d970: 2067 726f 7570 2061 7320 6f66 2073 7065   group as of spe
-0000d980: 6369 6669 6320 706f 696e 7420 696e 2074  cific point in t
-0000d990: 696d 652e 2044 6566 6175 6c74 7320 746f  ime. Defaults to
-0000d9a0: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
-0000d9b0: 2020 2020 2020 2020 2049 6620 6e6f 7420           If not 
-0000d9c0: 7370 6563 6966 6965 642c 2077 696c 6c20  specified, will 
-0000d9d0: 7265 7475 726e 2061 7320 6f66 206d 6f73  return as of mos
-0000d9e0: 7420 7265 6365 6e74 2074 696d 652e 0a20  t recent time.. 
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000da00: 7472 696e 6773 2073 686f 756c 6420 6265  trings should be
-0000da10: 2066 6f72 6d61 7474 6564 2069 6e20 6f6e   formatted in on
-0000da20: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-0000da30: 6e67 2066 6f72 6d61 7473 2060 2559 2d25  ng formats `%Y-%
-0000da40: 6d2d 2564 602c 2060 2559 2d25 6d2d 2564  m-%d`, `%Y-%m-%d
-0000da50: 2025 4860 2c20 6025 592d 256d 2d25 6420   %H`, `%Y-%m-%d 
-0000da60: 2548 3a25 4d60 2c20 6025 592d 256d 2d25  %H:%M`, `%Y-%m-%
-0000da70: 6420 2548 3a25 4d3a 2553 602c 0a20 2020  d %H:%M:%S`,.   
-0000da80: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000da90: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-0000daa0: 2553 2e25 6660 2e0a 2020 2020 2020 2020  %S.%f`..        
-0000dab0: 2020 2020 6f6e 6c69 6e65 3a20 626f 6f6c      online: bool
-0000dac0: 2c20 6f70 7469 6f6e 616c 2e20 4966 2060  , optional. If `
-0000dad0: 5472 7565 6020 7265 6164 2066 726f 6d20  True` read from 
-0000dae0: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-0000daf0: 746f 7265 2c20 6465 6661 756c 7473 0a20  tore, defaults. 
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000db10: 6f20 6046 616c 7365 602e 0a20 2020 2020  o `False`..     
-0000db20: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-0000db30: 5f74 7970 653a 2073 7472 2c20 6f70 7469  _type: str, opti
-0000db40: 6f6e 616c 2e20 506f 7373 6962 6c65 2076  onal. Possible v
-0000db50: 616c 7565 7320 6172 6520 6022 6465 6661  alues are `"defa
-0000db60: 756c 7422 602c 2060 2273 7061 726b 2260  ult"`, `"spark"`
-0000db70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000db80: 2020 6022 7061 6e64 6173 2260 2c20 6022    `"pandas"`, `"
-0000db90: 6e75 6d70 7922 6020 6f72 2060 2270 7974  numpy"` or `"pyt
-0000dba0: 686f 6e22 602c 2064 6566 6175 6c74 7320  hon"`, defaults 
-0000dbb0: 746f 2060 2264 6566 6175 6c74 2260 2e0a  to `"default"`..
-0000dbc0: 2020 2020 2020 2020 2020 2020 7265 6164              read
-0000dbd0: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-0000dbe0: 6f6e 616c 206f 7074 696f 6e73 2061 7320  onal options as 
-0000dbf0: 6b65 792f 7661 6c75 6520 7061 6972 7320  key/value pairs 
-0000dc00: 746f 2070 6173 7320 746f 2074 6865 2065  to pass to the e
-0000dc10: 7865 6375 7469 6f6e 2065 6e67 696e 652e  xecution engine.
-0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc30: 2046 6f72 2073 7061 726b 2065 6e67 696e   For spark engin
-0000dc40: 653a 2044 6963 7469 6f6e 6172 7920 6f66  e: Dictionary of
-0000dc50: 2072 6561 6420 6f70 7469 6f6e 7320 666f   read options fo
-0000dc60: 7220 5370 6172 6b2e 0a20 2020 2020 2020  r Spark..       
-0000dc70: 2020 2020 2020 2020 2046 6f72 2070 7974           For pyt
-0000dc80: 686f 6e20 656e 6769 6e65 3a0a 2020 2020  hon engine:.    
-0000dc90: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
-0000dca0: 7920 6022 6869 7665 5f63 6f6e 6669 6722  y `"hive_config"
-0000dcb0: 6020 746f 2070 6173 7320 6120 6469 6374  ` to pass a dict
-0000dcc0: 696f 6e61 7279 206f 6620 6869 7665 206f  ionary of hive o
-0000dcd0: 7220 7465 7a20 636f 6e66 6967 7572 6174  r tez configurat
-0000dce0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000dcf0: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-0000dd00: 706c 653a 2060 7b22 6869 7665 5f63 6f6e  ple: `{"hive_con
-0000dd10: 6669 6722 3a20 7b22 6869 7665 2e74 657a  fig": {"hive.tez
-0000dd20: 2e63 7075 2e76 636f 7265 7322 3a20 322c  .cpu.vcores": 2,
-0000dd30: 2022 7465 7a2e 6772 6f75 7069 6e67 2e73   "tez.grouping.s
-0000dd40: 706c 6974 2d63 6f75 6e74 223a 2022 3322  plit-count": "3"
-0000dd50: 7d7d 600a 2020 2020 2020 2020 2020 2020  }}`.            
-0000dd60: 2020 2020 2a20 6b65 7920 6022 7061 6e64      * key `"pand
-0000dd70: 6173 5f74 7970 6573 2260 2061 6e64 2076  as_types"` and v
-0000dd80: 616c 7565 2060 5472 7565 6020 746f 2072  alue `True` to r
-0000dd90: 6574 7269 6576 6520 636f 6c75 6d6e 7320  etrieve columns 
-0000dda0: 6173 2050 616e 6461 7320 6e75 6c6c 6162  as Pandas nullab
-0000ddb0: 6c65 2074 7970 6573 0a20 2020 2020 2020  le types.       
-0000ddc0: 2020 2020 2020 2020 2020 2072 6174 6865             rathe
-0000ddd0: 7220 7468 616e 206e 756d 7079 2f6f 626a  r than numpy/obj
-0000dde0: 6563 7428 7374 7269 6e67 2920 7479 7065  ect(string) type
-0000ddf0: 7320 2865 7870 6572 696d 656e 7461 6c29  s (experimental)
-0000de00: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000de10: 2020 2020 2873 6565 2068 7474 7073 3a2f      (see https:/
-0000de20: 2f70 616e 6461 732e 7079 6461 7461 2e6f  /pandas.pydata.o
-0000de30: 7267 2f64 6f63 732f 7573 6572 5f67 7569  rg/docs/user_gui
-0000de40: 6465 2f69 6e74 6567 6572 5f6e 612e 6874  de/integer_na.ht
-0000de50: 6d6c 292e 0a20 2020 2020 2020 2020 2020  ml)..           
-0000de60: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-0000de70: 2060 7b7d 602e 0a0a 2020 2020 2020 2020   `{}`...        
-0000de80: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-0000de90: 2020 2020 2020 6044 6174 6146 7261 6d65        `DataFrame
-0000dea0: 603a 2054 6865 2073 7061 726b 2064 6174  `: The spark dat
-0000deb0: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
-0000dec0: 6720 7468 6520 6665 6174 7572 6520 6461  g the feature da
-0000ded0: 7461 2e0a 2020 2020 2020 2020 2020 2020  ta..            
-0000dee0: 6070 7973 7061 726b 2e44 6174 6146 7261  `pyspark.DataFra
-0000def0: 6d65 602e 2041 2053 7061 726b 2044 6174  me`. A Spark Dat
-0000df00: 6146 7261 6d65 2e0a 2020 2020 2020 2020  aFrame..        
-0000df10: 2020 2020 6070 616e 6461 732e 4461 7461      `pandas.Data
-0000df20: 4672 616d 6560 2e20 4120 5061 6e64 6173  Frame`. A Pandas
-0000df30: 2044 6174 6146 7261 6d65 2e0a 2020 2020   DataFrame..    
-0000df40: 2020 2020 2020 2020 606e 756d 7079 2e6e          `numpy.n
-0000df50: 6461 7272 6179 602e 2041 2074 776f 2d64  darray`. A two-d
-0000df60: 696d 656e 7369 6f6e 616c 204e 756d 7079  imensional Numpy
-0000df70: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
-0000df80: 2020 2020 606c 6973 7460 2e20 4120 7477      `list`. A tw
-0000df90: 6f2d 6469 6d65 6e73 696f 6e61 6c20 5079  o-dimensional Py
-0000dfa0: 7468 6f6e 206c 6973 742e 0a0a 2020 2020  thon list...    
-0000dfb0: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-0000dfc0: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-0000dfd0: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-0000dfe0: 2e52 6573 7441 5049 4572 726f 7260 2e20  .RestAPIError`. 
-0000dff0: 4e6f 2064 6174 6120 6973 2061 7661 696c  No data is avail
-0000e000: 6162 6c65 2066 6f72 2066 6561 7475 7265  able for feature
-0000e010: 2067 726f 7570 2077 6974 6820 7468 6973   group with this
-0000e020: 2063 6f6d 6d69 7420 6461 7465 2c20 4966   commit date, If
-0000e030: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
-0000e040: 626c 6564 2e0a 2020 2020 2020 2020 2222  bled..        ""
-0000e050: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-0000e060: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-0000e070: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-0000e080: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-0000e090: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-0000e0a0: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-0000e0b0: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-0000e0c0: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-0000e0d0: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-0000e0e0: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e100: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-0000e110: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-0000e120: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-0000e130: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000e140: 2020 2020 6966 2077 616c 6c63 6c6f 636b      if wallclock
-0000e150: 5f74 696d 653a 0a20 2020 2020 2020 2020  _time:.         
-0000e160: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-0000e170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e180: 2e73 656c 6563 745f 616c 6c28 290a 2020  .select_all().  
-0000e190: 2020 2020 2020 2020 2020 2020 2020 2e61                .a
-0000e1a0: 735f 6f66 2877 616c 6c63 6c6f 636b 5f74  s_of(wallclock_t
-0000e1b0: 696d 6529 0a20 2020 2020 2020 2020 2020  ime).           
-0000e1c0: 2020 2020 202e 7265 6164 280a 2020 2020       .read(.    
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 6f6e 6c69 6e65 2c0a 2020 2020 2020 2020  online,.        
-0000e1f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000e200: 6672 616d 655f 7479 7065 2c0a 2020 2020  frame_type,.    
-0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e220: 7265 6164 5f6f 7074 696f 6e73 2c0a 2020  read_options,.  
-0000e230: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000e240: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e250: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000e260: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e270: 656c 662e 7365 6c65 6374 5f61 6c6c 2829  elf.select_all()
-0000e280: 2e72 6561 6428 0a20 2020 2020 2020 2020  .read(.         
-0000e290: 2020 2020 2020 206f 6e6c 696e 652c 0a20         online,. 
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000e2b0: 6174 6166 7261 6d65 5f74 7970 652c 0a20  ataframe_type,. 
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e2d0: 6561 645f 6f70 7469 6f6e 732c 0a20 2020  ead_options,.   
-0000e2e0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000e2f0: 6465 6620 7265 6164 5f63 6861 6e67 6573  def read_changes
-0000e300: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000e310: 2020 2020 2020 2020 7374 6172 745f 7761          start_wa
-0000e320: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 556e  llclock_time: Un
-0000e330: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
-0000e340: 7465 7469 6d65 2c20 6461 7465 5d2c 0a20  tetime, date],. 
-0000e350: 2020 2020 2020 2065 6e64 5f77 616c 6c63         end_wallc
-0000e360: 6c6f 636b 5f74 696d 653a 2055 6e69 6f6e  lock_time: Union
-0000e370: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
-0000e380: 696d 652c 2064 6174 655d 2c0a 2020 2020  ime, date],.    
-0000e390: 2020 2020 7265 6164 5f6f 7074 696f 6e73      read_options
-0000e3a0: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-0000e3b0: 203d 207b 7d2c 0a20 2020 2029 3a0a 2020   = {},.    ):.  
-0000e3c0: 2020 2020 2020 2222 2252 6561 6473 2075        """Reads u
-0000e3d0: 7064 6174 6573 206f 6620 7468 6973 2066  pdates of this f
-0000e3e0: 6561 7475 7265 2074 6861 7420 6f63 6375  eature that occu
-0000e3f0: 7272 6564 2062 6574 7765 656e 2073 7065  rred between spe
-0000e400: 6369 6669 6564 2070 6f69 6e74 7320 696e  cified points in
-0000e410: 2074 696d 652e 0a0a 2020 2020 2020 2020   time...        
-0000e420: 2121 2120 7761 726e 696e 6720 2244 6570  !!! warning "Dep
-0000e430: 7265 6361 7465 6422 0a20 2020 2020 2020  recated".       
-0000e440: 2020 2020 2020 2020 2020 2020 2060 7265               `re
-0000e450: 6164 5f63 6861 6e67 6573 6020 6d65 7468  ad_changes` meth
-0000e460: 6f64 2069 7320 6465 7072 6563 6174 6564  od is deprecated
-0000e470: 2e20 5573 650a 2020 2020 2020 2020 2020  . Use.          
-0000e480: 2020 2020 2020 2020 2020 6061 735f 6f66            `as_of
-0000e490: 2865 6e64 5f77 616c 6c63 6c6f 636b 5f74  (end_wallclock_t
-0000e4a0: 696d 652c 2065 7863 6c75 6465 5f75 6e74  ime, exclude_unt
-0000e4b0: 696c 3d73 7461 7274 5f77 616c 6c63 6c6f  il=start_wallclo
-0000e4c0: 636b 5f74 696d 6529 2e72 6561 6428 7265  ck_time).read(re
-0000e4d0: 6164 5f6f 7074 696f 6e73 3d72 6561 645f  ad_options=read_
-0000e4e0: 6f70 7469 6f6e 7329 600a 2020 2020 2020  options)`.      
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000e500: 7374 6561 642e 0a0a 2020 2020 2020 2020  stead...        
-0000e510: 5468 6973 2066 756e 6374 696f 6e20 6f6e  This function on
-0000e520: 6c79 2077 6f72 6b73 206f 6e20 6665 6174  ly works on feat
-0000e530: 7572 6520 6772 6f75 7073 2077 6974 6820  ure groups with 
-0000e540: 6048 5544 4960 2074 696d 6520 7472 6176  `HUDI` time trav
-0000e550: 656c 2066 6f72 6d61 742e 0a0a 2020 2020  el format...    
-0000e560: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
-0000e570: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0000e580: 745f 7761 6c6c 636c 6f63 6b5f 7469 6d65  t_wallclock_time
-0000e590: 3a20 5374 6172 7420 7469 6d65 206f 6620  : Start time of 
-0000e5a0: 7468 6520 7469 6d65 2074 7261 7665 6c20  the time travel 
-0000e5b0: 7175 6572 792e 2053 7472 696e 6773 2073  query. Strings s
-0000e5c0: 686f 756c 6420 6265 2066 6f72 6d61 7474  hould be formatt
-0000e5d0: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-0000e5e0: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-0000e5f0: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-0000e600: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-0000e610: 592d 256d 2d25 6420 2548 3a25 4d60 2c0a  Y-%m-%d %H:%M`,.
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-0000e640: 2553 602c 206f 7220 6025 592d 256d 2d25  %S`, or `%Y-%m-%
-0000e650: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-0000e660: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-0000e670: 7761 6c6c 636c 6f63 6b5f 7469 6d65 3a20  wallclock_time: 
-0000e680: 456e 6420 7469 6d65 206f 6620 7468 6520  End time of the 
-0000e690: 7469 6d65 2074 7261 7665 6c20 7175 6572  time travel quer
-0000e6a0: 792e 2053 7472 696e 6773 2073 686f 756c  y. Strings shoul
-0000e6b0: 6420 6265 2066 6f72 6d61 7474 6564 2069  d be formatted i
-0000e6c0: 6e20 6f6e 6520 6f66 2074 6865 2066 6f6c  n one of the fol
-0000e6d0: 6c6f 7769 6e67 2066 6f72 6d61 7473 2060  lowing formats `
-0000e6e0: 2559 2d25 6d2d 2564 602c 2060 2559 2d25  %Y-%m-%d`, `%Y-%
-0000e6f0: 6d2d 2564 2025 4860 2c20 6025 592d 256d  m-%d %H`, `%Y-%m
-0000e700: 2d25 6420 2548 3a25 4d60 2c0a 2020 2020  -%d %H:%M`,.    
-0000e710: 2020 2020 2020 2020 2020 2020 6025 592d              `%Y-
-0000e720: 256d 2d25 6420 2548 3a25 4d3a 2553 602c  %m-%d %H:%M:%S`,
-0000e730: 206f 7220 6025 592d 256d 2d25 6420 2548   or `%Y-%m-%d %H
-0000e740: 3a25 4d3a 2553 2e25 6660 2e0a 2020 2020  :%M:%S.%f`..    
-0000e750: 2020 2020 2020 2020 7265 6164 5f6f 7074          read_opt
-0000e760: 696f 6e73 3a20 4164 6469 7469 6f6e 616c  ions: Additional
-0000e770: 206f 7074 696f 6e73 2061 7320 6b65 792f   options as key/
-0000e780: 7661 6c75 6520 7061 6972 7320 746f 2070  value pairs to p
-0000e790: 6173 7320 746f 2074 6865 2065 7865 6375  ass to the execu
-0000e7a0: 7469 6f6e 2065 6e67 696e 652e 0a20 2020  tion engine..   
-0000e7b0: 2020 2020 2020 2020 2020 2020 2046 6f72               For
-0000e7c0: 2073 7061 726b 2065 6e67 696e 653a 2044   spark engine: D
-0000e7d0: 6963 7469 6f6e 6172 7920 6f66 2072 6561  ictionary of rea
-0000e7e0: 6420 6f70 7469 6f6e 7320 666f 7220 5370  d options for Sp
-0000e7f0: 6172 6b2e 0a20 2020 2020 2020 2020 2020  ark..           
-0000e800: 2020 2020 2046 6f72 2070 7974 686f 6e20       For python 
-0000e810: 656e 6769 6e65 3a0a 2020 2020 2020 2020  engine:.        
-0000e820: 2020 2020 2020 2020 2a20 6b65 7920 6022          * key `"
-0000e830: 6869 7665 5f63 6f6e 6669 6722 6020 746f  hive_config"` to
-0000e840: 2070 6173 7320 6120 6469 6374 696f 6e61   pass a dictiona
-0000e850: 7279 206f 6620 6869 7665 206f 7220 7465  ry of hive or te
-0000e860: 7a20 636f 6e66 6967 7572 6174 696f 6e73  z configurations
-0000e870: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e880: 2020 2020 466f 7220 6578 616d 706c 653a      For example:
-0000e890: 2060 7b22 6869 7665 5f63 6f6e 6669 6722   `{"hive_config"
-0000e8a0: 3a20 7b22 6869 7665 2e74 657a 2e63 7075  : {"hive.tez.cpu
-0000e8b0: 2e76 636f 7265 7322 3a20 322c 2022 7465  .vcores": 2, "te
-0000e8c0: 7a2e 6772 6f75 7069 6e67 2e73 706c 6974  z.grouping.split
-0000e8d0: 2d63 6f75 6e74 223a 2022 3322 7d7d 600a  -count": "3"}}`.
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 4465 6661 756c 7473 2074 6f20 607b 7d60  Defaults to `{}`
-0000e900: 2e0a 0a20 2020 2020 2020 2023 2052 6574  ...        # Ret
-0000e910: 7572 6e73 0a20 2020 2020 2020 2020 2020  urns.           
-0000e920: 2060 4461 7461 4672 616d 6560 2e20 5468   `DataFrame`. Th
-0000e930: 6520 7370 6172 6b20 6461 7461 6672 616d  e spark datafram
-0000e940: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-0000e950: 2069 6e63 7265 6d65 6e74 616c 2063 6861   incremental cha
-0000e960: 6e67 6573 206f 660a 2020 2020 2020 2020  nges of.        
-0000e970: 2020 2020 6665 6174 7572 6520 6461 7461      feature data
-0000e980: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
-0000e990: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-0000e9a0: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
-0000e9b0: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
-0000e9c0: 7272 6f72 602e 2020 4e6f 2064 6174 6120  rror`.  No data 
-0000e9d0: 6973 2061 7661 696c 6162 6c65 2066 6f72  is available for
-0000e9e0: 2066 6561 7475 7265 2067 726f 7570 2077   feature group w
-0000e9f0: 6974 6820 7468 6973 2063 6f6d 6d69 7420  ith this commit 
-0000ea00: 6461 7465 2e0a 2020 2020 2020 2020 2020  date..          
-0000ea10: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
-0000ea20: 7863 6570 7469 6f6e 732e 4665 6174 7572  xceptions.Featur
-0000ea30: 6553 746f 7265 4578 6365 7074 696f 6e60  eStoreException`
-0000ea40: 2e20 4966 2074 6865 2066 6561 7475 7265  . If the feature
-0000ea50: 2067 726f 7570 2064 6f65 7320 6e6f 7420   group does not 
-0000ea60: 6861 7665 2060 4855 4449 6020 7469 6d65  have `HUDI` time
-0000ea70: 2074 7261 7665 6c20 666f 726d 6174 0a20   travel format. 
-0000ea80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ea90: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-0000eaa0: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
-0000eab0: 6563 745f 616c 6c28 290a 2020 2020 2020  ect_all().      
-0000eac0: 2020 2020 2020 2e70 756c 6c5f 6368 616e        .pull_chan
-0000ead0: 6765 7328 7374 6172 745f 7761 6c6c 636c  ges(start_wallcl
-0000eae0: 6f63 6b5f 7469 6d65 2c20 656e 645f 7761  ock_time, end_wa
-0000eaf0: 6c6c 636c 6f63 6b5f 7469 6d65 290a 2020  llclock_time).  
-0000eb00: 2020 2020 2020 2020 2020 2e72 6561 6428            .read(
-0000eb10: 4661 6c73 652c 2022 6465 6661 756c 7422  False, "default"
-0000eb20: 2c20 7265 6164 5f6f 7074 696f 6e73 290a  , read_options).
-0000eb30: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000eb40: 6566 2073 686f 7728 7365 6c66 2c20 6e3a  ef show(self, n:
-0000eb50: 2069 6e74 2c20 6f6e 6c69 6e65 3a20 4f70   int, online: Op
-0000eb60: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
-0000eb70: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
-0000eb80: 2222 5368 6f77 2074 6865 2066 6972 7374  ""Show the first
-0000eb90: 2060 6e60 2072 6f77 7320 6f66 2074 6865   `n` rows of the
-0000eba0: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-0000ebb0: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-0000ebc0: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-0000ebd0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-0000ebe0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-0000ebf0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-0000ec00: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-0000ec10: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-0000ec20: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-0000ec30: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-0000ec40: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-0000ec50: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
-0000ec60: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
-0000ec70: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
-0000ec80: 2020 2020 2020 2020 2020 2023 206d 616b             # mak
-0000ec90: 6520 6120 7175 6572 7920 616e 6420 7368  e a query and sh
-0000eca0: 6f77 2074 6f70 2035 2072 6f77 730a 2020  ow top 5 rows.  
-0000ecb0: 2020 2020 2020 2020 2020 6667 2e73 656c            fg.sel
-0000ecc0: 6563 7428 5b27 6461 7465 272c 2777 6565  ect(['date','wee
-0000ecd0: 6b6c 795f 7361 6c65 7327 2c27 6973 5f68  kly_sales','is_h
-0000ece0: 6f6c 6964 6179 275d 292e 7368 6f77 2835  oliday']).show(5
-0000ecf0: 290a 2020 2020 2020 2020 2020 2020 6060  ).            ``
-0000ed00: 600a 0a20 2020 2020 2020 2023 2041 7267  `..        # Arg
-0000ed10: 756d 656e 7473 0a20 2020 2020 2020 2020  uments.         
-0000ed20: 2020 206e 3a20 696e 742e 204e 756d 6265     n: int. Numbe
-0000ed30: 7220 6f66 2072 6f77 7320 746f 2073 686f  r of rows to sho
-0000ed40: 772e 0a20 2020 2020 2020 2020 2020 206f  w..            o
-0000ed50: 6e6c 696e 653a 2062 6f6f 6c2c 206f 7074  nline: bool, opt
-0000ed60: 696f 6e61 6c2e 2049 6620 6054 7275 6560  ional. If `True`
-0000ed70: 2072 6561 6420 6672 6f6d 206f 6e6c 696e   read from onlin
-0000ed80: 6520 6665 6174 7572 6520 7374 6f72 652c  e feature store,
-0000ed90: 2064 6566 6175 6c74 730a 2020 2020 2020   defaults.      
-0000eda0: 2020 2020 2020 2020 2020 746f 2060 4661            to `Fa
-0000edb0: 6c73 6560 2e0a 2020 2020 2020 2020 2222  lse`..        ""
-0000edc0: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-0000edd0: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-0000ede0: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-0000edf0: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-0000ee00: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-0000ee10: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-0000ee20: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-0000ee30: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-0000ee40: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-0000ee50: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-0000ee60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ee70: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-0000ee80: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-0000ee90: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-0000eea0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000eeb0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000eec0: 7365 6c65 6374 5f61 6c6c 2829 2e73 686f  select_all().sho
-0000eed0: 7728 6e2c 206f 6e6c 696e 6529 0a0a 2020  w(n, online)..  
-0000eee0: 2020 6465 6620 7361 7665 280a 2020 2020    def save(.    
-0000eef0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000ef00: 2020 6665 6174 7572 6573 3a20 556e 696f    features: Unio
-0000ef10: 6e5b 0a20 2020 2020 2020 2020 2020 2070  n[.            p
-0000ef20: 642e 4461 7461 4672 616d 652c 0a20 2020  d.DataFrame,.   
-0000ef30: 2020 2020 2020 2020 2054 7970 6556 6172           TypeVar
-0000ef40: 2822 7079 7370 6172 6b2e 7371 6c2e 4461  ("pyspark.sql.Da
-0000ef50: 7461 4672 616d 6522 292c 2020 2320 6e6f  taFrame"),  # no
-0000ef60: 7161 3a20 4638 3231 0a20 2020 2020 2020  qa: F821.       
-0000ef70: 2020 2020 2054 7970 6556 6172 2822 7079       TypeVar("py
-0000ef80: 7370 6172 6b2e 5244 4422 292c 2020 2320  spark.RDD"),  # 
-0000ef90: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-0000efa0: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
-0000efb0: 792c 0a20 2020 2020 2020 2020 2020 204c  y,.            L
-0000efc0: 6973 745b 6665 6174 7572 652e 4665 6174  ist[feature.Feat
-0000efd0: 7572 655d 2c0a 2020 2020 2020 2020 5d20  ure],.        ] 
-0000efe0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000eff0: 7772 6974 655f 6f70 7469 6f6e 733a 204f  write_options: O
-0000f000: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
-0000f010: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
-0000f020: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-0000f030: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-0000f040: 616c 5b44 6963 745b 416e 792c 2041 6e79  al[Dict[Any, Any
-0000f050: 5d5d 203d 207b 7d2c 0a20 2020 2020 2020  ]] = {},.       
-0000f060: 2077 6169 743a 2062 6f6f 6c20 3d20 4661   wait: bool = Fa
-0000f070: 6c73 652c 0a20 2020 2029 3a0a 2020 2020  lse,.    ):.    
-0000f080: 2020 2020 2222 2250 6572 7369 7374 2074      """Persist t
-0000f090: 6865 206d 6574 6164 6174 6120 616e 6420  he metadata and 
-0000f0a0: 6d61 7465 7269 616c 697a 6520 7468 6520  materialize the 
-0000f0b0: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
-0000f0c0: 2074 6865 2066 6561 7475 7265 2073 746f   the feature sto
-0000f0d0: 7265 2e0a 0a20 2020 2020 2020 2021 2121  re...        !!!
-0000f0e0: 2077 6172 6e69 6e67 2022 4368 616e 6765   warning "Change
-0000f0f0: 6420 696e 2033 2e33 2e30 220a 2020 2020  d in 3.3.0".    
-0000f100: 2020 2020 2020 2020 6069 6e73 6572 7460          `insert`
-0000f110: 2061 6e64 2060 7361 7665 6020 6d65 7468   and `save` meth
-0000f120: 6f64 7320 6172 6520 6e6f 7720 6173 796e  ods are now asyn
-0000f130: 6320 6279 2064 6566 6175 6c74 2069 6e20  c by default in 
-0000f140: 6e6f 6e2d 7370 6172 6b20 636c 6965 6e74  non-spark client
-0000f150: 732e 0a20 2020 2020 2020 2020 2020 2054  s..            T
-0000f160: 6f20 6163 6869 6576 6520 7468 6520 6f6c  o achieve the ol
-0000f170: 6420 6265 6861 7669 6f75 722c 2073 6574  d behaviour, set
-0000f180: 2060 7761 6974 6020 6172 6775 6d65 6e74   `wait` argument
-0000f190: 2074 6f20 6054 7275 6560 2e0a 0a20 2020   to `True`...   
-0000f1a0: 2020 2020 2043 616c 6c69 6e67 2060 7361       Calling `sa
-0000f1b0: 7665 6020 6372 6561 7465 7320 7468 6520  ve` creates the 
-0000f1c0: 6d65 7461 6461 7461 2066 6f72 2074 6865  metadata for the
-0000f1d0: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-0000f1e0: 6e20 7468 6520 6665 6174 7572 6520 7374  n the feature st
-0000f1f0: 6f72 652e 0a20 2020 2020 2020 2049 6620  ore..        If 
-0000f200: 6120 4461 7461 4672 616d 652c 2052 4444  a DataFrame, RDD
-0000f210: 206f 7220 4e64 6172 7261 7920 6973 2070   or Ndarray is p
-0000f220: 726f 7669 6465 642c 2074 6865 2064 6174  rovided, the dat
-0000f230: 6120 6973 2077 7269 7474 656e 2074 6f20  a is written to 
-0000f240: 7468 650a 2020 2020 2020 2020 6f6e 6c69  the.        onli
-0000f250: 6e65 2f6f 6666 6c69 6e65 2066 6561 7475  ne/offline featu
-0000f260: 7265 2073 746f 7265 2061 7320 7370 6563  re store as spec
-0000f270: 6966 6965 642e 0a20 2020 2020 2020 2042  ified..        B
-0000f280: 7920 6465 6661 756c 742c 2074 6869 7320  y default, this 
-0000f290: 7772 6974 6573 2074 6865 2066 6561 7475  writes the featu
-0000f2a0: 7265 2067 726f 7570 2074 6f20 7468 6520  re group to the 
-0000f2b0: 6f66 666c 696e 6520 7374 6f72 6167 652c  offline storage,
-0000f2c0: 2061 6e64 2069 660a 2020 2020 2020 2020   and if.        
-0000f2d0: 606f 6e6c 696e 655f 656e 6162 6c65 6460  `online_enabled`
-0000f2e0: 2066 6f72 2074 6865 2066 6561 7475 7265   for the feature
-0000f2f0: 2067 726f 7570 2c20 616c 736f 2074 6f20   group, also to 
-0000f300: 7468 6520 6f6e 6c69 6e65 2066 6561 7475  the online featu
-0000f310: 7265 2073 746f 7265 2e0a 2020 2020 2020  re store..      
-0000f320: 2020 5468 6520 6066 6561 7475 7265 7360    The `features`
-0000f330: 2064 6174 6166 7261 6d65 2063 616e 2062   dataframe can b
-0000f340: 6520 6120 5370 6172 6b20 4461 7461 4672  e a Spark DataFr
-0000f350: 616d 6520 6f72 2052 4444 2c20 6120 5061  ame or RDD, a Pa
-0000f360: 6e64 6173 2044 6174 6146 7261 6d65 2c0a  ndas DataFrame,.
-0000f370: 2020 2020 2020 2020 6f72 2061 2074 776f          or a two
-0000f380: 2d64 696d 656e 7369 6f6e 616c 204e 756d  -dimensional Num
-0000f390: 7079 2061 7272 6179 206f 7220 6120 7477  py array or a tw
-0000f3a0: 6f2d 6469 6d65 6e73 696f 6e61 6c20 5079  o-dimensional Py
-0000f3b0: 7468 6f6e 206e 6573 7465 6420 6c69 7374  thon nested list
-0000f3c0: 2e0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
-0000f3d0: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
-0000f3e0: 2020 6665 6174 7572 6573 3a20 4461 7461    features: Data
-0000f3f0: 4672 616d 652c 2052 4444 2c20 4e64 6172  Frame, RDD, Ndar
-0000f400: 7261 7920 6f72 2061 206c 6973 7420 6f66  ray or a list of
-0000f410: 2066 6561 7475 7265 732e 2046 6561 7475   features. Featu
-0000f420: 7265 7320 746f 2062 6520 7361 7665 642e  res to be saved.
-0000f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f440: 2054 6869 7320 6172 6775 6d65 6e74 2069   This argument i
-0000f450: 7320 6f70 7469 6f6e 616c 2069 6620 7468  s optional if th
-0000f460: 6520 6665 6174 7572 6520 6c69 7374 2069  e feature list i
-0000f470: 7320 7072 6f76 6964 6564 2069 6e20 7468  s provided in th
-0000f480: 6520 6372 6561 7465 5f66 6561 7475 7265  e create_feature
-0000f490: 5f67 726f 7570 206f 720a 2020 2020 2020  _group or.      
-0000f4a0: 2020 2020 2020 2020 2020 696e 2074 6865            in the
-0000f4b0: 2067 6574 5f6f 725f 6372 6561 7465 5f66   get_or_create_f
-0000f4c0: 6561 7475 7265 5f67 726f 7570 206d 6574  eature_group met
-0000f4d0: 686f 6420 696e 766f 6b61 7469 6f6e 2e0a  hod invokation..
-0000f4e0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-0000f4f0: 655f 6f70 7469 6f6e 733a 2041 6464 6974  e_options: Addit
-0000f500: 696f 6e61 6c20 7772 6974 6520 6f70 7469  ional write opti
-0000f510: 6f6e 7320 6173 206b 6579 2d76 616c 7565  ons as key-value
-0000f520: 2070 6169 7273 2c20 6465 6661 756c 7473   pairs, defaults
-0000f530: 2074 6f20 607b 7d60 2e0a 2020 2020 2020   to `{}`..      
-0000f540: 2020 2020 2020 2020 2020 5768 656e 2075            When u
-0000f550: 7369 6e67 2074 6865 2060 7079 7468 6f6e  sing the `python
-0000f560: 6020 656e 6769 6e65 2c20 7772 6974 655f  ` engine, write_
-0000f570: 6f70 7469 6f6e 7320 6361 6e20 636f 6e74  options can cont
-0000f580: 6169 6e20 7468 650a 2020 2020 2020 2020  ain the.        
-0000f590: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-0000f5a0: 6720 656e 7472 6965 733a 0a20 2020 2020  g entries:.     
-0000f5b0: 2020 2020 2020 2020 2020 202a 206b 6579             * key
-0000f5c0: 2060 7370 6172 6b60 2061 6e64 2076 616c   `spark` and val
-0000f5d0: 7565 2061 6e20 6f62 6a65 6374 206f 6620  ue an object of 
-0000f5e0: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
-0000f5f0: 2020 2020 205b 6873 6673 2e63 6f72 652e       [hsfs.core.
-0000f600: 6a6f 625f 636f 6e66 6967 7572 6174 696f  job_configuratio
-0000f610: 6e2e 4a6f 6243 6f6e 6669 6775 7261 7469  n.JobConfigurati
-0000f620: 6f6e 5d28 2e2e 2f6a 6f62 5f63 6f6e 6669  on](../job_confi
-0000f630: 6775 7261 7469 6f6e 290a 2020 2020 2020  guration).      
-0000f640: 2020 2020 2020 2020 2020 2020 746f 2063              to c
-0000f650: 6f6e 6669 6775 7265 2074 6865 2048 6f70  onfigure the Hop
-0000f660: 7377 6f72 6b73 204a 6f62 2075 7365 6420  sworks Job used 
-0000f670: 746f 2077 7269 7465 2064 6174 6120 696e  to write data in
-0000f680: 746f 2074 6865 0a20 2020 2020 2020 2020  to the.         
-0000f690: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-0000f6a0: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
-0000f6b0: 2020 2020 2020 2020 2a20 6b65 7920 6077          * key `w
-0000f6c0: 6169 745f 666f 725f 6a6f 6260 2061 6e64  ait_for_job` and
-0000f6d0: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
-0000f6e0: 2060 4661 6c73 6560 2074 6f20 636f 6e66   `False` to conf
-0000f6f0: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
-0000f700: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
-0000f710: 6f72 206e 6f74 2074 6f20 7468 6520 7361  or not to the sa
-0000f720: 7665 2063 616c 6c20 7368 6f75 6c64 2072  ve call should r
-0000f730: 6574 7572 6e20 6f6e 6c79 0a20 2020 2020  eturn only.     
-0000f740: 2020 2020 2020 2020 2020 2020 2061 6674               aft
-0000f750: 6572 2074 6865 2048 6f70 7377 6f72 6b73  er the Hopsworks
-0000f760: 204a 6f62 2068 6173 2066 696e 6973 6865   Job has finishe
-0000f770: 642e 2042 7920 6465 6661 756c 7420 6974  d. By default it
-0000f780: 2064 6f65 7320 6e6f 7420 7761 6974 2e0a   does not wait..
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2a20 6b65 7920 6073 7461 7274 5f6f 6666  * key `start_off
-0000f7b0: 6c69 6e65 5f62 6163 6b66 696c 6c60 2061  line_backfill` a
-0000f7c0: 6e64 2076 616c 7565 2060 5472 7565 6020  nd value `True` 
-0000f7d0: 6f72 2060 4661 6c73 6560 2074 6f20 636f  or `False` to co
-0000f7e0: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
-0000f7f0: 2020 2020 2020 2020 2020 7768 6574 6865            whethe
-0000f800: 7220 6f72 206e 6f74 2074 6f20 7374 6172  r or not to star
-0000f810: 7420 7468 6520 6261 636b 6669 6c6c 206a  t the backfill j
-0000f820: 6f62 2074 6f20 7772 6974 6520 6461 7461  ob to write data
-0000f830: 2074 6f20 7468 6520 6f66 666c 696e 650a   to the offline.
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 2020 7374 6f72 6167 652e 2042 7920 6465    storage. By de
-0000f860: 6661 756c 7420 7468 6520 6261 636b 6669  fault the backfi
-0000f870: 6c6c 206a 6f62 2067 6574 7320 7374 6172  ll job gets star
-0000f880: 7465 6420 696d 6d65 6469 6174 656c 792e  ted immediately.
-0000f890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f8a0: 202a 206b 6579 2060 696e 7465 726e 616c   * key `internal
-0000f8b0: 5f6b 6166 6b61 6020 616e 6420 7661 6c75  _kafka` and valu
-0000f8c0: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
-0000f8d0: 7365 6020 696e 2063 6173 6520 796f 7520  se` in case you 
-0000f8e0: 6573 7461 626c 6973 6865 640a 2020 2020  established.    
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f900: 6e6e 6563 7469 7669 7479 2066 726f 6d20  nnectivity from 
-0000f910: 796f 7520 5079 7468 6f6e 2065 6e76 6972  you Python envir
-0000f920: 6f6e 6d65 6e74 2074 6f20 7468 6520 696e  onment to the in
-0000f930: 7465 726e 616c 2061 6476 6572 7469 7365  ternal advertise
-0000f940: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000f950: 2020 2020 6c69 7374 656e 6572 7320 6f66      listeners of
-0000f960: 2074 6865 2048 6f70 7377 6f72 6b73 204b   the Hopsworks K
-0000f970: 6166 6b61 2043 6c75 7374 6572 2e20 4465  afka Cluster. De
-0000f980: 6661 756c 7473 2074 6f20 6046 616c 7365  faults to `False
-0000f990: 6020 616e 640a 2020 2020 2020 2020 2020  ` and.          
-0000f9a0: 2020 2020 2020 2020 7769 6c6c 2075 7365          will use
-0000f9b0: 2065 7874 6572 6e61 6c20 6c69 7374 656e   external listen
-0000f9c0: 6572 7320 7768 656e 2063 6f6e 6e65 6374  ers when connect
-0000f9d0: 696e 6720 6672 6f6d 206f 7574 7369 6465  ing from outside
-0000f9e0: 206f 6620 486f 7073 776f 726b 732e 0a20   of Hopsworks.. 
-0000f9f0: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-0000fa00: 6174 696f 6e5f 6f70 7469 6f6e 733a 2041  ation_options: A
-0000fa10: 6464 6974 696f 6e61 6c20 7661 6c69 6461  dditional valida
-0000fa20: 7469 6f6e 206f 7074 696f 6e73 2061 7320  tion options as 
-0000fa30: 6b65 792d 7661 6c75 6520 7061 6972 732c  key-value pairs,
-0000fa40: 2064 6566 6175 6c74 7320 746f 2060 7b7d   defaults to `{}
-0000fa50: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
-0000fa60: 2020 202a 206b 6579 2060 7275 6e5f 7661     * key `run_va
-0000fa70: 6c69 6461 7469 6f6e 6020 626f 6f6c 6561  lidation` boolea
-0000fa80: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
-0000fa90: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
-0000faa0: 7661 6c69 6461 7469 6f6e 2074 656d 706f  validation tempo
-0000fab0: 7261 7269 6c79 206f 6e20 696e 6765 7374  rarily on ingest
-0000fac0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-0000fad0: 2020 2020 202a 206b 6579 2060 7361 7665       * key `save
-0000fae0: 5f72 6570 6f72 7460 2062 6f6f 6c65 616e  _report` boolean
-0000faf0: 2076 616c 7565 2c20 7365 7420 746f 2060   value, set to `
-0000fb00: 4661 6c73 6560 2074 6f20 736b 6970 2075  False` to skip u
-0000fb10: 706c 6f61 6420 6f66 2074 6865 2076 616c  pload of the val
-0000fb20: 6964 6174 696f 6e20 7265 706f 7274 2074  idation report t
-0000fb30: 6f20 486f 7073 776f 726b 732e 0a20 2020  o Hopsworks..   
-0000fb40: 2020 2020 2020 2020 2020 2020 202a 206b               * k
-0000fb50: 6579 2060 6765 5f76 616c 6964 6174 655f  ey `ge_validate_
-0000fb60: 6b77 6172 6773 6020 6120 6469 6374 696f  kwargs` a dictio
-0000fb70: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-0000fb80: 6b77 6172 6773 2066 6f72 2074 6865 2076  kwargs for the v
-0000fb90: 616c 6964 6174 6520 6d65 7468 6f64 206f  alidate method o
-0000fba0: 6620 4772 6561 7420 4578 7065 6374 6174  f Great Expectat
-0000fbb0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000fbc0: 2020 7761 6974 3a20 5761 6974 2066 6f72    wait: Wait for
-0000fbd0: 206a 6f62 2074 6f20 6669 6e69 7368 2062   job to finish b
-0000fbe0: 6566 6f72 6520 7265 7475 726e 696e 672c  efore returning,
-0000fbf0: 2064 6566 6175 6c74 7320 746f 2060 4661   defaults to `Fa
-0000fc00: 6c73 6560 2e0a 2020 2020 2020 2020 2020  lse`..          
-0000fc10: 2020 2020 2020 5368 6f72 7463 7574 2066        Shortcut f
-0000fc20: 6f72 2072 6561 645f 6f70 7469 6f6e 7320  or read_options 
-0000fc30: 607b 2277 6169 745f 666f 725f 6a6f 6222  `{"wait_for_job"
-0000fc40: 3a20 4661 6c73 657d 602e 0a0a 2020 2020  : False}`...    
-0000fc50: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
-0000fc60: 2020 2020 2020 2020 2020 604a 6f62 603a            `Job`:
-0000fc70: 2057 6865 6e20 7573 696e 6720 7468 6520   When using the 
-0000fc80: 6070 7974 686f 6e60 2065 6e67 696e 652c  `python` engine,
-0000fc90: 2069 7420 7265 7475 726e 7320 7468 6520   it returns the 
-0000fca0: 486f 7073 776f 726b 7320 4a6f 620a 2020  Hopsworks Job.  
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0000fcc0: 6174 2077 6173 206c 6175 6e63 6865 6420  at was launched 
-0000fcd0: 746f 2069 6e67 6573 7420 7468 6520 6665  to ingest the fe
-0000fce0: 6174 7572 6520 6772 6f75 7020 6461 7461  ature group data
-0000fcf0: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
-0000fd00: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-0000fd10: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
-0000fd20: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
-0000fd30: 7272 6f72 602e 2055 6e61 626c 6520 746f  rror`. Unable to
-0000fd40: 2063 7265 6174 6520 6665 6174 7572 6520   create feature 
-0000fd50: 6772 6f75 702e 0a20 2020 2020 2020 2022  group..        "
-0000fd60: 2222 0a20 2020 2020 2020 2069 6620 2866  "".        if (f
-0000fd70: 6561 7475 7265 7320 6973 204e 6f6e 6520  eatures is None 
-0000fd80: 616e 6420 6c65 6e28 7365 6c66 2e5f 6665  and len(self._fe
-0000fd90: 6174 7572 6573 2920 3e20 3029 206f 7220  atures) > 0) or 
-0000fda0: 280a 2020 2020 2020 2020 2020 2020 6973  (.            is
-0000fdb0: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
-0000fdc0: 732c 204c 6973 7429 0a20 2020 2020 2020  s, List).       
-0000fdd0: 2020 2020 2061 6e64 206c 656e 2866 6561       and len(fea
-0000fde0: 7475 7265 7329 203e 2030 0a20 2020 2020  tures) > 0.     
-0000fdf0: 2020 2020 2020 2061 6e64 2061 6c6c 285b         and all([
-0000fe00: 6973 696e 7374 616e 6365 2866 2c20 6665  isinstance(f, fe
-0000fe10: 6174 7572 652e 4665 6174 7572 6529 2066  ature.Feature) f
-0000fe20: 6f72 2066 2069 6e20 6665 6174 7572 6573  or f in features
-0000fe30: 5d29 0a20 2020 2020 2020 2029 3a0a 2020  ]).        ):.  
-0000fe40: 2020 2020 2020 2020 2020 2320 5468 6973            # This
-0000fe50: 2069 7320 646f 6e65 2066 6f72 2063 6f6d   is done for com
-0000fe60: 7061 7469 6269 6c69 7479 2e20 5573 6572  patibility. User
-0000fe70: 7320 6361 6e20 7370 6563 6966 7920 7468  s can specify th
-0000fe80: 6520 6665 6174 7572 6520 6c69 7374 2069  e feature list i
-0000fe90: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
-0000fea0: 2020 2320 2867 6574 5f6f 725f 2963 7265    # (get_or_)cre
-0000feb0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
-0000fec0: 702e 2055 7365 7273 2063 616e 2061 6c73  p. Users can als
-0000fed0: 6f20 7072 6f76 6964 6520 7468 6520 6665  o provide the fe
-0000fee0: 6174 7572 6520 6c69 7374 2069 6e20 7468  ature list in th
-0000fef0: 6520 7361 7665 2829 2e0a 2020 2020 2020  e save()..      
-0000ff00: 2020 2020 2020 2320 5468 6f75 6768 2069        # Though i
-0000ff10: 7427 7320 616e 206f 7074 696f 6e61 6c20  t's an optional 
-0000ff20: 7061 7261 6d65 7465 722e 0a20 2020 2020  parameter..     
-0000ff30: 2020 2020 2020 2023 2046 6f72 2063 6f6e         # For con
-0000ff40: 7369 7374 656e 6379 2072 6561 736f 6e73  sistency reasons
-0000ff50: 2069 6620 7468 6520 7573 6572 2073 7065   if the user spe
-0000ff60: 6369 6679 2062 6f74 6820 7468 6520 6665  cify both the fe
-0000ff70: 6174 7572 6520 6c69 7374 2069 6e20 7468  ature list in th
-0000ff80: 6520 2867 6574 5f6f 725f 2963 7265 6174  e (get_or_)creat
-0000ff90: 655f 6665 6174 7572 655f 6772 6f75 700a  e_feature_group.
-0000ffa0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
-0000ffb0: 6420 696e 2074 6865 2060 7361 7665 2829  d in the `save()
-0000ffc0: 6020 6361 6c6c 2c20 7468 656e 2074 6865  ` call, then the
-0000ffd0: 2028 6765 745f 6f72 5f29 6372 6561 7465   (get_or_)create
-0000ffe0: 5f66 6561 7475 7265 5f67 726f 7570 2077  _feature_group w
-0000fff0: 696e 732e 0a20 2020 2020 2020 2020 2020  ins..           
-00010000: 2023 2054 6869 7320 6973 2063 6f6e 7369   # This is consi
-00010010: 7374 656e 7420 7769 7468 2074 6865 2062  stent with the b
-00010020: 6568 6176 696f 7220 6f66 2074 6865 2069  ehavior of the i
-00010030: 6e73 6572 7420 6d65 7468 6f64 2077 6865  nsert method whe
-00010040: 7265 2074 6865 2066 6561 7475 7265 206c  re the feature l
-00010050: 6973 7420 7769 6e73 206f 7665 7220 7468  ist wins over th
-00010060: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-00010070: 6461 7461 6672 616d 6520 7374 7275 6374  dataframe struct
-00010080: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
-00010090: 7365 6c66 2e5f 6665 6174 7572 6573 203d  self._features =
-000100a0: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
-000100b0: 6966 206c 656e 2873 656c 662e 5f66 6561  if len(self._fea
-000100c0: 7475 7265 7329 203e 2030 2065 6c73 6520  tures) > 0 else 
-000100d0: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
-000100e0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-000100f0: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
-00010100: 7361 7665 5f66 6561 7475 7265 5f67 726f  save_feature_gro
-00010110: 7570 5f6d 6574 6164 6174 6128 0a20 2020  up_metadata(.   
-00010120: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010130: 662c 204e 6f6e 652c 2077 7269 7465 5f6f  f, None, write_o
-00010140: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
-00010150: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00010160: 2020 7265 7475 726e 204e 6f6e 652c 204e    return None, N
-00010170: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-00010180: 6665 6174 7572 6573 2069 7320 4e6f 6e65  features is None
-00010190: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000101a0: 6973 6520 4665 6174 7572 6553 746f 7265  ise FeatureStore
-000101b0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-000101c0: 2020 2020 2020 2020 2020 2022 4665 6174             "Feat
-000101d0: 7572 6520 6c69 7374 206e 6f74 2070 726f  ure list not pro
-000101e0: 7669 6465 6420 696e 2074 6865 2063 7265  vided in the cre
-000101f0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
-00010200: 7020 6f72 2067 6574 5f6f 725f 6372 6561  p or get_or_crea
-00010210: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
-00010220: 2069 6e76 6f6b 6174 696f 6e73 2e22 0a20   invokations.". 
-00010230: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00010240: 2022 2050 6c65 6173 6520 7072 6f76 6964   " Please provid
-00010250: 6520 6120 6c69 7374 206f 6620 6665 6174  e a list of feat
-00010260: 7572 6573 206f 7220 6120 4461 7461 6672  ures or a Datafr
-00010270: 616d 6522 0a20 2020 2020 2020 2020 2020  ame".           
-00010280: 2029 0a0a 2020 2020 2020 2020 6665 6174   )..        feat
-00010290: 7572 655f 6461 7461 6672 616d 6520 3d20  ure_dataframe = 
-000102a0: 656e 6769 6e65 2e67 6574 5f69 6e73 7461  engine.get_insta
-000102b0: 6e63 6528 292e 636f 6e76 6572 745f 746f  nce().convert_to
-000102c0: 5f64 6566 6175 6c74 5f64 6174 6166 7261  _default_datafra
-000102d0: 6d65 2866 6561 7475 7265 7329 0a0a 2020  me(features)..  
-000102e0: 2020 2020 2020 7573 6572 5f76 6572 7369        user_versi
-000102f0: 6f6e 203d 2073 656c 662e 5f76 6572 7369  on = self._versi
-00010300: 6f6e 0a0a 2020 2020 2020 2020 6966 2077  on..        if w
-00010310: 7269 7465 5f6f 7074 696f 6e73 2069 7320  rite_options is 
-00010320: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010330: 2020 7772 6974 655f 6f70 7469 6f6e 7320    write_options 
-00010340: 3d20 7b7d 0a20 2020 2020 2020 2069 6620  = {}.        if 
-00010350: 2277 6169 745f 666f 725f 6a6f 6222 206e  "wait_for_job" n
-00010360: 6f74 2069 6e20 7772 6974 655f 6f70 7469  ot in write_opti
-00010370: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00010380: 2077 7269 7465 5f6f 7074 696f 6e73 5b22   write_options["
-00010390: 7761 6974 5f66 6f72 5f6a 6f62 225d 203d  wait_for_job"] =
-000103a0: 2077 6169 740a 0a20 2020 2020 2020 2023   wait..        #
-000103b0: 2066 675f 6a6f 6220 6973 2075 7365 6420   fg_job is used 
-000103c0: 6f6e 6c79 2069 6620 7468 6520 7079 7468  only if the pyth
-000103d0: 6f6e 2065 6e67 696e 6520 6973 2075 7365  on engine is use
-000103e0: 640a 2020 2020 2020 2020 6667 5f6a 6f62  d.        fg_job
-000103f0: 2c20 6765 5f72 6570 6f72 7420 3d20 7365  , ge_report = se
-00010400: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-00010410: 705f 656e 6769 6e65 2e73 6176 6528 0a20  p_engine.save(. 
-00010420: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00010430: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
-00010440: 6d65 2c20 7772 6974 655f 6f70 7469 6f6e  me, write_option
-00010450: 732c 2076 616c 6964 6174 696f 6e5f 6f70  s, validation_op
-00010460: 7469 6f6e 730a 2020 2020 2020 2020 290a  tions.        ).
-00010470: 2020 2020 2020 2020 6966 2067 655f 7265          if ge_re
-00010480: 706f 7274 2069 7320 4e6f 6e65 206f 7220  port is None or 
-00010490: 6765 5f72 6570 6f72 742e 696e 6765 7374  ge_report.ingest
-000104a0: 696f 6e5f 7265 7375 6c74 203d 3d20 2249  ion_result == "I
-000104b0: 4e47 4553 5445 4422 3a0a 2020 2020 2020  NGESTED":.      
-000104c0: 2020 2020 2020 7365 6c66 2e5f 636f 6465        self._code
-000104d0: 5f65 6e67 696e 652e 7361 7665 5f63 6f64  _engine.save_cod
-000104e0: 6528 7365 6c66 290a 0a20 2020 2020 2020  e(self)..       
-000104f0: 2069 6620 7365 6c66 2e73 7461 7469 7374   if self.statist
-00010500: 6963 735f 636f 6e66 6967 2e65 6e61 626c  ics_config.enabl
-00010510: 6564 2061 6e64 2065 6e67 696e 652e 6765  ed and engine.ge
-00010520: 745f 7479 7065 2829 203d 3d20 2273 7061  t_type() == "spa
-00010530: 726b 223a 0a20 2020 2020 2020 2020 2020  rk":.           
-00010540: 2023 204f 6e6c 7920 636f 6d70 7574 6520   # Only compute 
-00010550: 7374 6174 6973 7469 6373 2069 6620 7468  statistics if th
-00010560: 6520 656e 6769 6e65 2069 7320 5370 6172  e engine is Spar
-00010570: 6b2e 0a20 2020 2020 2020 2020 2020 2023  k..            #
-00010580: 2046 6f72 2050 7974 686f 6e20 656e 6769   For Python engi
-00010590: 6e65 2c20 7468 6520 636f 6d70 7574 6174  ne, the computat
-000105a0: 696f 6e20 6861 7070 656e 7320 696e 2074  ion happens in t
-000105b0: 6865 2048 6f70 7377 6f72 6b73 2061 7070  he Hopsworks app
-000105c0: 6c69 6361 7469 6f6e 0a20 2020 2020 2020  lication.       
-000105d0: 2020 2020 2073 656c 662e 5f73 7461 7469       self._stati
-000105e0: 7374 6963 735f 656e 6769 6e65 2e63 6f6d  stics_engine.com
-000105f0: 7075 7465 5f73 7461 7469 7374 6963 7328  pute_statistics(
-00010600: 7365 6c66 2c20 6665 6174 7572 655f 6461  self, feature_da
-00010610: 7461 6672 616d 6529 0a20 2020 2020 2020  taframe).       
-00010620: 2069 6620 7573 6572 5f76 6572 7369 6f6e   if user_version
-00010630: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00010640: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00010650: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00010660: 2020 2020 2022 4e6f 2076 6572 7369 6f6e       "No version
-00010670: 2070 726f 7669 6465 6420 666f 7220 6372   provided for cr
-00010680: 6561 7469 6e67 2066 6561 7475 7265 2067  eating feature g
-00010690: 726f 7570 2060 7b7d 602c 2069 6e63 7265  roup `{}`, incre
-000106a0: 6d65 6e74 6564 2076 6572 7369 6f6e 2074  mented version t
-000106b0: 6f20 607b 7d60 2e22 2e66 6f72 6d61 7428  o `{}`.".format(
-000106c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106d0: 2020 2020 2073 656c 662e 5f6e 616d 652c       self._name,
-000106e0: 2073 656c 662e 5f76 6572 7369 6f6e 0a20   self._version. 
-000106f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010710: 2020 7574 696c 2e56 6572 7369 6f6e 5761    util.VersionWa
-00010720: 726e 696e 672c 0a20 2020 2020 2020 2020  rning,.         
-00010730: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00010740: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
-00010750: 2020 6667 5f6a 6f62 2c0a 2020 2020 2020    fg_job,.      
-00010760: 2020 2020 2020 6765 5f72 6570 6f72 742e        ge_report.
-00010770: 746f 5f67 655f 7479 7065 2829 2069 6620  to_ge_type() if 
-00010780: 6765 5f72 6570 6f72 7420 6973 206e 6f74  ge_report is not
-00010790: 204e 6f6e 6520 656c 7365 204e 6f6e 652c   None else None,
-000107a0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000107b0: 6465 6620 696e 7365 7274 280a 2020 2020  def insert(.    
-000107c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000107d0: 2020 6665 6174 7572 6573 3a20 556e 696f    features: Unio
-000107e0: 6e5b 0a20 2020 2020 2020 2020 2020 2070  n[.            p
-000107f0: 642e 4461 7461 4672 616d 652c 0a20 2020  d.DataFrame,.   
-00010800: 2020 2020 2020 2020 2054 7970 6556 6172           TypeVar
-00010810: 2822 7079 7370 6172 6b2e 7371 6c2e 4461  ("pyspark.sql.Da
-00010820: 7461 4672 616d 6522 292c 2020 2320 6e6f  taFrame"),  # no
-00010830: 7161 3a20 4638 3231 0a20 2020 2020 2020  qa: F821.       
-00010840: 2020 2020 2054 7970 6556 6172 2822 7079       TypeVar("py
-00010850: 7370 6172 6b2e 5244 4422 292c 2020 2320  spark.RDD"),  # 
-00010860: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-00010870: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
-00010880: 792c 0a20 2020 2020 2020 2020 2020 204c  y,.            L
-00010890: 6973 745b 6c69 7374 5d2c 0a20 2020 2020  ist[list],.     
-000108a0: 2020 205d 2c0a 2020 2020 2020 2020 6f76     ],.        ov
-000108b0: 6572 7772 6974 653a 204f 7074 696f 6e61  erwrite: Optiona
-000108c0: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-000108d0: 0a20 2020 2020 2020 206f 7065 7261 7469  .        operati
-000108e0: 6f6e 3a20 4f70 7469 6f6e 616c 5b73 7472  on: Optional[str
-000108f0: 5d20 3d20 2275 7073 6572 7422 2c0a 2020  ] = "upsert",.  
-00010900: 2020 2020 2020 7374 6f72 6167 653a 204f        storage: O
-00010910: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00010920: 6f6e 652c 0a20 2020 2020 2020 2077 7269  one,.        wri
-00010930: 7465 5f6f 7074 696f 6e73 3a20 4f70 7469  te_options: Opti
-00010940: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
-00010950: 6e79 5d5d 203d 207b 7d2c 0a20 2020 2020  ny]] = {},.     
-00010960: 2020 2076 616c 6964 6174 696f 6e5f 6f70     validation_op
-00010970: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00010980: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-00010990: 3d20 7b7d 2c0a 2020 2020 2020 2020 7361  = {},.        sa
-000109a0: 7665 5f63 6f64 653a 204f 7074 696f 6e61  ve_code: Optiona
-000109b0: 6c5b 626f 6f6c 5d20 3d20 5472 7565 2c0a  l[bool] = True,.
-000109c0: 2020 2020 2020 2020 7761 6974 3a20 626f          wait: bo
-000109d0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-000109e0: 2920 2d3e 2054 7570 6c65 5b4f 7074 696f  ) -> Tuple[Optio
-000109f0: 6e61 6c5b 4a6f 625d 2c20 4f70 7469 6f6e  nal[Job], Option
-00010a00: 616c 5b56 616c 6964 6174 696f 6e52 6570  al[ValidationRep
-00010a10: 6f72 745d 5d3a 0a20 2020 2020 2020 2022  ort]]:.        "
-00010a20: 2222 5065 7273 6973 7420 7468 6520 6d65  ""Persist the me
-00010a30: 7461 6461 7461 2061 6e64 206d 6174 6572  tadata and mater
-00010a40: 6961 6c69 7a65 2074 6865 2066 6561 7475  ialize the featu
-00010a50: 7265 2067 726f 7570 2074 6f20 7468 6520  re group to the 
-00010a60: 6665 6174 7572 6520 7374 6f72 650a 2020  feature store.  
-00010a70: 2020 2020 2020 6f72 2069 6e73 6572 7420        or insert 
-00010a80: 6461 7461 2066 726f 6d20 6120 6461 7461  data from a data
-00010a90: 6672 616d 6520 696e 746f 2074 6865 2065  frame into the e
-00010aa0: 7869 7374 696e 6720 6665 6174 7572 6520  xisting feature 
-00010ab0: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
-00010ac0: 496e 6372 656d 656e 7461 6c6c 7920 696e  Incrementally in
-00010ad0: 7365 7274 2064 6174 6120 746f 2061 2066  sert data to a f
-00010ae0: 6561 7475 7265 2067 726f 7570 206f 7220  eature group or 
-00010af0: 6f76 6572 7772 6974 6520 616c 6c20 2064  overwrite all  d
-00010b00: 6174 6120 636f 6e74 6169 6e65 6420 696e  ata contained in
-00010b10: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00010b20: 7570 2e20 4279 0a20 2020 2020 2020 2064  up. By.        d
-00010b30: 6566 6175 6c74 2c20 7468 6520 6461 7461  efault, the data
-00010b40: 2069 7320 696e 7365 7274 6564 2069 6e74   is inserted int
-00010b50: 6f20 7468 6520 6f66 666c 696e 6520 7374  o the offline st
-00010b60: 6f72 6167 6520 6173 2077 656c 6c20 6173  orage as well as
-00010b70: 2074 6865 206f 6e6c 696e 6520 7374 6f72   the online stor
-00010b80: 6167 6520 6966 2074 6865 2066 6561 7475  age if the featu
-00010b90: 7265 2067 726f 7570 2069 730a 2020 2020  re group is.    
-00010ba0: 2020 2020 606f 6e6c 696e 655f 656e 6162      `online_enab
-00010bb0: 6c65 643d 5472 7565 602e 2054 6f20 696e  led=True`. To in
-00010bc0: 7365 7274 206f 6e6c 7920 696e 746f 2074  sert only into t
-00010bd0: 6865 206f 6e6c 696e 6520 6f72 206f 6666  he online or off
-00010be0: 6c69 6e65 2073 746f 7261 6765 2073 6574  line storage set
-00010bf0: 2060 7374 6f72 6167 653d 226f 6e6c 696e   `storage="onlin
-00010c00: 6522 6020 6f72 0a20 2020 2020 2020 2060  e"` or.        `
-00010c10: 7374 6f72 6167 653d 226f 6666 6c69 6e65  storage="offline
-00010c20: 2260 2072 6573 7065 6374 6976 656c 792e  "` respectively.
-00010c30: 0a0a 2020 2020 2020 2020 5468 6520 6066  ..        The `f
-00010c40: 6561 7475 7265 7360 2064 6174 6166 7261  eatures` datafra
-00010c50: 6d65 2063 616e 2062 6520 6120 5370 6172  me can be a Spar
-00010c60: 6b20 4461 7461 4672 616d 6520 6f72 2052  k DataFrame or R
-00010c70: 4444 2c20 6120 5061 6e64 6173 2044 6174  DD, a Pandas Dat
-00010c80: 6146 7261 6d65 2c0a 2020 2020 2020 2020  aFrame,.        
-00010c90: 6f72 2061 2074 776f 2d64 696d 656e 7369  or a two-dimensi
-00010ca0: 6f6e 616c 204e 756d 7079 2061 7272 6179  onal Numpy array
-00010cb0: 206f 7220 6120 7477 6f2d 6469 6d65 6e73   or a two-dimens
-00010cc0: 696f 6e61 6c20 5079 7468 6f6e 206e 6573  ional Python nes
-00010cd0: 7465 6420 6c69 7374 2e0a 2020 2020 2020  ted list..      
-00010ce0: 2020 4966 2073 7461 7469 7374 6963 7320    If statistics 
-00010cf0: 6172 6520 656e 6162 6c65 642c 2073 7461  are enabled, sta
-00010d00: 7469 7374 6963 7320 6172 6520 7265 636f  tistics are reco
-00010d10: 6d70 7574 6564 2066 6f72 2074 6865 2065  mputed for the e
-00010d20: 6e74 6972 6520 6665 6174 7572 650a 2020  ntire feature.  
-00010d30: 2020 2020 2020 6772 6f75 702e 0a20 2020        group..   
-00010d40: 2020 2020 2049 6620 6665 6174 7572 6520       If feature 
-00010d50: 6772 6f75 7027 7320 7469 6d65 2074 7261  group's time tra
-00010d60: 7665 6c20 666f 726d 6174 2069 7320 6048  vel format is `H
-00010d70: 5544 4960 2074 6865 6e20 606f 7065 7261  UDI` then `opera
-00010d80: 7469 6f6e 6020 6172 6775 6d65 6e74 2063  tion` argument c
-00010d90: 616e 2062 650a 2020 2020 2020 2020 6569  an be.        ei
-00010da0: 7468 6572 2060 696e 7365 7274 6020 6f72  ther `insert` or
-00010db0: 2060 7570 7365 7274 602e 0a0a 2020 2020   `upsert`...    
-00010dc0: 2020 2020 4966 2066 6561 7475 7265 2067      If feature g
-00010dd0: 726f 7570 2064 6f65 736e 2774 2065 7869  roup doesn't exi
-00010de0: 7374 7320 2074 6865 2069 6e73 6572 7420  sts  the insert 
-00010df0: 6d65 7468 6f64 2077 696c 6c20 6372 6561  method will crea
-00010e00: 7465 2074 6865 206e 6563 6573 7361 7279  te the necessary
-00010e10: 206d 6574 6164 6174 6120 7468 6520 6669   metadata the fi
-00010e20: 7273 7420 7469 6d65 2069 7420 6973 0a20  rst time it is. 
-00010e30: 2020 2020 2020 2069 6e76 6f6b 6564 2061         invoked a
-00010e40: 6e64 2077 7269 7465 7320 7468 6520 7370  nd writes the sp
-00010e50: 6563 6966 6965 6420 6066 6561 7475 7265  ecified `feature
-00010e60: 7360 2064 6174 6166 7261 6d65 2061 7320  s` dataframe as 
-00010e70: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
-00010e80: 2074 6865 206f 6e6c 696e 652f 6f66 666c   the online/offl
-00010e90: 696e 6520 6665 6174 7572 6520 7374 6f72  ine feature stor
-00010ea0: 652e 0a0a 2020 2020 2020 2020 2121 2120  e...        !!! 
-00010eb0: 7761 726e 696e 6720 2243 6861 6e67 6564  warning "Changed
-00010ec0: 2069 6e20 332e 332e 3022 0a20 2020 2020   in 3.3.0".     
-00010ed0: 2020 2020 2020 2060 696e 7365 7274 6020         `insert` 
-00010ee0: 616e 6420 6073 6176 6560 206d 6574 686f  and `save` metho
-00010ef0: 6473 2061 7265 206e 6f77 2061 7379 6e63  ds are now async
-00010f00: 2062 7920 6465 6661 756c 7420 696e 206e   by default in n
-00010f10: 6f6e 2d73 7061 726b 2063 6c69 656e 7473  on-spark clients
-00010f20: 2e0a 2020 2020 2020 2020 2020 2020 546f  ..            To
-00010f30: 2061 6368 6965 7665 2074 6865 206f 6c64   achieve the old
-00010f40: 2062 6568 6176 696f 7572 2c20 7365 7420   behaviour, set 
-00010f50: 6077 6169 7460 2061 7267 756d 656e 7420  `wait` argument 
-00010f60: 746f 2060 5472 7565 602e 0a0a 2020 2020  to `True`...    
-00010f70: 2020 2020 2121 2120 6578 616d 706c 6520      !!! example 
-00010f80: 2255 7073 6572 7420 6e65 7720 6665 6174  "Upsert new feat
-00010f90: 7572 6520 6461 7461 2077 6974 6820 7469  ure data with ti
-00010fa0: 6d65 2074 7261 7665 6c20 666f 726d 6174  me travel format
-00010fb0: 2060 4855 4449 6022 0a20 2020 2020 2020   `HUDI`".       
-00010fc0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00010fd0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00010fe0: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
-00010ff0: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
-00011000: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
-00011010: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00011020: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00011030: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00011040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011050: 206e 616d 653d 2762 6974 636f 696e 5f70   name='bitcoin_p
-00011060: 7269 6365 272c 0a20 2020 2020 2020 2020  rice',.         
-00011070: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00011080: 6f6e 3d27 4269 7463 6f69 6e20 7072 6963  on='Bitcoin pric
-00011090: 6520 6167 6772 6567 6174 6564 2066 6f72  e aggregated for
-000110a0: 2064 6179 7327 2c0a 2020 2020 2020 2020   days',.        
-000110b0: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
-000110c0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000110d0: 2020 2070 7269 6d61 7279 5f6b 6579 3d5b     primary_key=[
-000110e0: 2775 6e69 7827 5d2c 0a20 2020 2020 2020  'unix'],.       
-000110f0: 2020 2020 2020 2020 206f 6e6c 696e 655f           online_
-00011100: 656e 6162 6c65 643d 5472 7565 2c0a 2020  enabled=True,.  
-00011110: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-00011120: 656e 745f 7469 6d65 3d27 756e 6978 270a  ent_time='unix'.
-00011130: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00011140: 2020 2020 2020 2020 2020 2066 672e 696e             fg.in
-00011150: 7365 7274 2864 665f 6269 7463 6f69 6e5f  sert(df_bitcoin_
-00011160: 7072 6f63 6573 7365 6429 0a20 2020 2020  processed).     
-00011170: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-00011180: 2020 2020 2121 2120 6578 616d 706c 6520      !!! example 
-00011190: 2241 7379 6e63 2069 6e73 6572 7422 0a20  "Async insert". 
-000111a0: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
-000111b0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
-000111c0: 2023 2063 6f6e 6e65 6374 2074 6f20 7468   # connect to th
-000111d0: 6520 4665 6174 7572 6520 5374 6f72 650a  e Feature Store.
-000111e0: 2020 2020 2020 2020 2020 2020 6673 203d              fs =
-000111f0: 202e 2e2e 0a0a 2020 2020 2020 2020 2020   .....          
-00011200: 2020 6667 3120 3d20 6673 2e67 6574 5f6f    fg1 = fs.get_o
-00011210: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
-00011220: 5f67 726f 7570 280a 2020 2020 2020 2020  _group(.        
-00011230: 2020 2020 2020 2020 6e61 6d65 3d27 6665          name='fe
-00011240: 6174 7572 655f 6772 6f75 705f 6e61 6d65  ature_group_name
-00011250: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
-00011260: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00011270: 2744 6573 6372 6970 7469 6f6e 206f 6620  'Description of 
-00011280: 7468 6520 6669 7273 7420 4647 272c 0a20  the first FG',. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000112a0: 6572 7369 6f6e 3d31 2c0a 2020 2020 2020  ersion=1,.      
-000112b0: 2020 2020 2020 2020 2020 7072 696d 6172            primar
-000112c0: 795f 6b65 793d 5b27 756e 6978 275d 2c0a  y_key=['unix'],.
-000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112e0: 6f6e 6c69 6e65 5f65 6e61 626c 6564 3d54  online_enabled=T
-000112f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00011300: 2020 2020 2065 7665 6e74 5f74 696d 653d       event_time=
-00011310: 2775 6e69 7827 0a20 2020 2020 2020 2020  'unix'.         
-00011320: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00011330: 2023 2061 7379 6e63 2069 6e73 6572 7469   # async inserti
-00011340: 6f6e 2069 6e20 6f72 6465 7220 6e6f 7420  on in order not 
-00011350: 746f 2077 6169 7420 7469 6c6c 2066 696e  to wait till fin
-00011360: 6973 6820 6f66 2074 6865 206a 6f62 0a20  ish of the job. 
-00011370: 2020 2020 2020 2020 2020 2066 672e 696e             fg.in
-00011380: 7365 7274 2864 665f 666f 725f 6667 312c  sert(df_for_fg1,
-00011390: 2077 7269 7465 5f6f 7074 696f 6e73 3d7b   write_options={
-000113a0: 2277 6169 745f 666f 725f 6a6f 6222 203a  "wait_for_job" :
-000113b0: 2046 616c 7365 7d29 0a0a 2020 2020 2020   False})..      
-000113c0: 2020 2020 2020 6667 3220 3d20 6673 2e67        fg2 = fs.g
-000113d0: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-000113e0: 7475 7265 5f67 726f 7570 280a 2020 2020  ture_group(.    
-000113f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00011400: 3d27 6665 6174 7572 655f 6772 6f75 705f  ='feature_group_
-00011410: 6e61 6d65 3227 2c0a 2020 2020 2020 2020  name2',.        
-00011420: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00011430: 696f 6e3d 2744 6573 6372 6970 7469 6f6e  ion='Description
-00011440: 206f 6620 7468 6520 7365 636f 6e64 2046   of the second F
-00011450: 4727 2c0a 2020 2020 2020 2020 2020 2020  G',.            
-00011460: 2020 2020 7665 7273 696f 6e3d 312c 0a20      version=1,. 
-00011470: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011480: 7269 6d61 7279 5f6b 6579 3d5b 2775 6e69  rimary_key=['uni
-00011490: 7827 5d2c 0a20 2020 2020 2020 2020 2020  x'],.           
-000114a0: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
-000114b0: 6c65 643d 5472 7565 2c0a 2020 2020 2020  led=True,.      
-000114c0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
-000114d0: 7469 6d65 3d27 756e 6978 270a 2020 2020  time='unix'.    
-000114e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000114f0: 2020 2020 2020 6667 2e69 6e73 6572 7428        fg.insert(
-00011500: 6466 5f66 6f72 5f66 6732 290a 2020 2020  df_for_fg2).    
-00011510: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-00011520: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00011530: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00011540: 7475 7265 733a 2044 6174 6146 7261 6d65  tures: DataFrame
-00011550: 2c20 5244 442c 204e 6461 7272 6179 2c20  , RDD, Ndarray, 
-00011560: 6c69 7374 2e20 4665 6174 7572 6573 2074  list. Features t
-00011570: 6f20 6265 2073 6176 6564 2e0a 2020 2020  o be saved..    
-00011580: 2020 2020 2020 2020 6f76 6572 7772 6974          overwrit
-00011590: 653a 2044 726f 7020 616c 6c20 6461 7461  e: Drop all data
-000115a0: 2069 6e20 7468 6520 6665 6174 7572 6520   in the feature 
-000115b0: 6772 6f75 7020 6265 666f 7265 0a20 2020  group before.   
-000115c0: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
-000115d0: 6572 7469 6e67 206e 6577 2064 6174 612e  erting new data.
-000115e0: 2054 6869 7320 646f 6573 206e 6f74 2061   This does not a
-000115f0: 6666 6563 7420 6d65 7461 6461 7461 2c20  ffect metadata, 
-00011600: 6465 6661 756c 7473 2074 6f20 4661 6c73  defaults to Fals
-00011610: 652e 0a20 2020 2020 2020 2020 2020 206f  e..            o
-00011620: 7065 7261 7469 6f6e 3a20 4170 6163 6865  peration: Apache
-00011630: 2048 7564 6920 6f70 6572 6174 696f 6e20   Hudi operation 
-00011640: 7479 7065 2060 2269 6e73 6572 7422 6020  type `"insert"` 
-00011650: 6f72 2060 2275 7073 6572 7422 602e 0a20  or `"upsert"`.. 
-00011660: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00011670: 6566 6175 6c74 7320 746f 2060 2275 7073  efaults to `"ups
-00011680: 6572 7422 602e 0a20 2020 2020 2020 2020  ert"`..         
-00011690: 2020 2073 746f 7261 6765 3a20 4f76 6572     storage: Over
-000116a0: 7772 6974 6520 6465 6661 756c 7420 6265  write default be
-000116b0: 6861 7669 6f75 722c 2077 7269 7465 2074  haviour, write t
-000116c0: 6f20 6f66 666c 696e 650a 2020 2020 2020  o offline.      
-000116d0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-000116e0: 6520 6f6e 6c79 2077 6974 6820 6022 6f66  e only with `"of
-000116f0: 666c 696e 6522 6020 6f72 206f 6e6c 696e  fline"` or onlin
-00011700: 6520 6f6e 6c79 2077 6974 6820 6022 6f6e  e only with `"on
-00011710: 6c69 6e65 2260 2c20 6465 6661 756c 7473  line"`, defaults
-00011720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011730: 2074 6f20 604e 6f6e 6560 2e0a 2020 2020   to `None`..    
-00011740: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-00011750: 7469 6f6e 733a 2041 6464 6974 696f 6e61  tions: Additiona
-00011760: 6c20 7772 6974 6520 6f70 7469 6f6e 7320  l write options 
-00011770: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-00011780: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-00011790: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-000117a0: 2020 2020 2020 5768 656e 2075 7369 6e67        When using
-000117b0: 2074 6865 2060 7079 7468 6f6e 6020 656e   the `python` en
-000117c0: 6769 6e65 2c20 7772 6974 655f 6f70 7469  gine, write_opti
-000117d0: 6f6e 7320 6361 6e20 636f 6e74 6169 6e20  ons can contain 
-000117e0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-000117f0: 2020 2020 666f 6c6c 6f77 696e 6720 656e      following en
-00011800: 7472 6965 733a 0a20 2020 2020 2020 2020  tries:.         
-00011810: 2020 2020 2020 202a 206b 6579 2060 7370         * key `sp
-00011820: 6172 6b60 2061 6e64 2076 616c 7565 2061  ark` and value a
-00011830: 6e20 6f62 6a65 6374 206f 6620 7479 7065  n object of type
-00011840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011850: 205b 6873 6673 2e63 6f72 652e 6a6f 625f   [hsfs.core.job_
-00011860: 636f 6e66 6967 7572 6174 696f 6e2e 4a6f  configuration.Jo
-00011870: 6243 6f6e 6669 6775 7261 7469 6f6e 5d28  bConfiguration](
-00011880: 2e2e 2f6a 6f62 5f63 6f6e 6669 6775 7261  ../job_configura
-00011890: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-000118a0: 2020 2020 2020 2020 746f 2063 6f6e 6669          to confi
-000118b0: 6775 7265 2074 6865 2048 6f70 7377 6f72  gure the Hopswor
-000118c0: 6b73 204a 6f62 2075 7365 6420 746f 2077  ks Job used to w
-000118d0: 7269 7465 2064 6174 6120 696e 746f 2074  rite data into t
-000118e0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-000118f0: 2020 2020 2066 6561 7475 7265 2067 726f       feature gro
-00011900: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
-00011910: 2020 2020 2a20 6b65 7920 6077 6169 745f      * key `wait_
-00011920: 666f 725f 6a6f 6260 2061 6e64 2076 616c  for_job` and val
-00011930: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
-00011940: 6c73 6560 2074 6f20 636f 6e66 6967 7572  lse` to configur
-00011950: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00011960: 2020 2020 7768 6574 6865 7220 6f72 206e      whether or n
-00011970: 6f74 2074 6f20 7468 6520 696e 7365 7274  ot to the insert
-00011980: 2063 616c 6c20 7368 6f75 6c64 2072 6574   call should ret
-00011990: 7572 6e20 6f6e 6c79 0a20 2020 2020 2020  urn only.       
-000119a0: 2020 2020 2020 2020 2020 2061 6674 6572             after
-000119b0: 2074 6865 2048 6f70 7377 6f72 6b73 204a   the Hopsworks J
-000119c0: 6f62 2068 6173 2066 696e 6973 6865 642e  ob has finished.
-000119d0: 2042 7920 6465 6661 756c 7420 6974 2077   By default it w
-000119e0: 6169 7473 2e0a 2020 2020 2020 2020 2020  aits..          
-000119f0: 2020 2020 2020 2a20 6b65 7920 6073 7461        * key `sta
-00011a00: 7274 5f6f 6666 6c69 6e65 5f62 6163 6b66  rt_offline_backf
-00011a10: 696c 6c60 2061 6e64 2076 616c 7565 2060  ill` and value `
-00011a20: 5472 7565 6020 6f72 2060 4661 6c73 6560  True` or `False`
-00011a30: 2074 6f20 636f 6e66 6967 7572 650a 2020   to configure.  
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-00011a60: 6f20 7374 6172 7420 7468 6520 6261 636b  o start the back
-00011a70: 6669 6c6c 206a 6f62 2074 6f20 7772 6974  fill job to writ
-00011a80: 6520 6461 7461 2074 6f20 7468 6520 6f66  e data to the of
-00011a90: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
-00011aa0: 2020 2020 2020 2020 7374 6f72 6167 652e          storage.
-00011ab0: 2042 7920 6465 6661 756c 7420 7468 6520   By default the 
-00011ac0: 6261 636b 6669 6c6c 206a 6f62 2067 6574  backfill job get
-00011ad0: 7320 7374 6172 7465 6420 696d 6d65 6469  s started immedi
-00011ae0: 6174 656c 792e 0a20 2020 2020 2020 2020  ately..         
-00011af0: 2020 2020 2020 202a 206b 6579 2060 696e         * key `in
-00011b00: 7465 726e 616c 5f6b 6166 6b61 6020 616e  ternal_kafka` an
-00011b10: 6420 7661 6c75 6520 6054 7275 6560 206f  d value `True` o
-00011b20: 7220 6046 616c 7365 6020 696e 2063 6173  r `False` in cas
-00011b30: 6520 796f 7520 6573 7461 626c 6973 6865  e you establishe
-00011b40: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00011b50: 2020 2020 636f 6e6e 6563 7469 7669 7479      connectivity
-00011b60: 2066 726f 6d20 796f 7520 5079 7468 6f6e   from you Python
-00011b70: 2065 6e76 6972 6f6e 6d65 6e74 2074 6f20   environment to 
-00011b80: 7468 6520 696e 7465 726e 616c 2061 6476  the internal adv
-00011b90: 6572 7469 7365 640a 2020 2020 2020 2020  ertised.        
-00011ba0: 2020 2020 2020 2020 2020 6c69 7374 656e            listen
-00011bb0: 6572 7320 6f66 2074 6865 2048 6f70 7377  ers of the Hopsw
-00011bc0: 6f72 6b73 204b 6166 6b61 2043 6c75 7374  orks Kafka Clust
-00011bd0: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
-00011be0: 6046 616c 7365 6020 616e 640a 2020 2020  `False` and.    
-00011bf0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00011c00: 6c6c 2075 7365 2065 7874 6572 6e61 6c20  ll use external 
-00011c10: 6c69 7374 656e 6572 7320 7768 656e 2063  listeners when c
-00011c20: 6f6e 6e65 6374 696e 6720 6672 6f6d 206f  onnecting from o
-00011c30: 7574 7369 6465 206f 6620 486f 7073 776f  utside of Hopswo
-00011c40: 726b 732e 0a20 2020 2020 2020 2020 2020  rks..           
-00011c50: 2076 616c 6964 6174 696f 6e5f 6f70 7469   validation_opti
-00011c60: 6f6e 733a 2041 6464 6974 696f 6e61 6c20  ons: Additional 
-00011c70: 7661 6c69 6461 7469 6f6e 206f 7074 696f  validation optio
-00011c80: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
-00011c90: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
-00011ca0: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
-00011cb0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-00011cc0: 7275 6e5f 7661 6c69 6461 7469 6f6e 6020  run_validation` 
-00011cd0: 626f 6f6c 6561 6e20 7661 6c75 652c 2073  boolean value, s
-00011ce0: 6574 2074 6f20 6046 616c 7365 6020 746f  et to `False` to
-00011cf0: 2073 6b69 7020 7661 6c69 6461 7469 6f6e   skip validation
-00011d00: 2074 656d 706f 7261 7269 6c79 206f 6e20   temporarily on 
-00011d10: 696e 6765 7374 696f 6e2e 0a20 2020 2020  ingestion..     
-00011d20: 2020 2020 2020 2020 2020 202a 206b 6579             * key
-00011d30: 2060 7361 7665 5f72 6570 6f72 7460 2062   `save_report` b
-00011d40: 6f6f 6c65 616e 2076 616c 7565 2c20 7365  oolean value, se
-00011d50: 7420 746f 2060 4661 6c73 6560 2074 6f20  t to `False` to 
-00011d60: 736b 6970 2075 706c 6f61 6420 6f66 2074  skip upload of t
-00011d70: 6865 2076 616c 6964 6174 696f 6e20 7265  he validation re
-00011d80: 706f 7274 2074 6f20 486f 7073 776f 726b  port to Hopswork
-00011d90: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00011da0: 2020 202a 206b 6579 2060 6765 5f76 616c     * key `ge_val
-00011db0: 6964 6174 655f 6b77 6172 6773 6020 6120  idate_kwargs` a 
-00011dc0: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-00011dd0: 696e 696e 6720 6b77 6172 6773 2066 6f72  ining kwargs for
-00011de0: 2074 6865 2076 616c 6964 6174 6520 6d65   the validate me
-00011df0: 7468 6f64 206f 6620 4772 6561 7420 4578  thod of Great Ex
-00011e00: 7065 6374 6174 696f 6e73 2e0a 2020 2020  pectations..    
-00011e10: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
-00011e20: 7920 6066 6574 6368 5f65 7870 6563 7461  y `fetch_expecta
-00011e30: 7469 6f6e 5f73 7569 7465 6020 6120 626f  tion_suite` a bo
-00011e40: 6f6c 6561 6e20 7661 6c75 652c 2062 7920  olean value, by 
-00011e50: 6465 6661 756c 7420 6054 7275 6560 2c20  default `True`, 
-00011e60: 746f 2063 6f6e 7472 6f6c 2077 6865 7468  to control wheth
-00011e70: 6572 2074 6865 2065 7870 6563 7461 7469  er the expectati
-00011e80: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00011e90: 2020 2020 2020 7375 6974 6520 6f66 2074        suite of t
-00011ea0: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00011eb0: 2073 686f 756c 6420 6265 2066 6574 6368   should be fetch
-00011ec0: 6564 2062 6566 6f72 6520 6576 6572 7920  ed before every 
-00011ed0: 696e 7365 7274 2e0a 2020 2020 2020 2020  insert..        
-00011ee0: 2020 2020 7361 7665 5f63 6f64 653a 2057      save_code: W
-00011ef0: 6865 6e20 7275 6e6e 696e 6720 4853 4653  hen running HSFS
-00011f00: 206f 6e20 486f 7073 776f 726b 7320 6f72   on Hopsworks or
-00011f10: 2044 6174 6162 7269 636b 732c 2048 5346   Databricks, HSF
-00011f20: 5320 6361 6e20 7361 7665 2074 6865 2063  S can save the c
-00011f30: 6f64 652f 6e6f 7465 626f 6f6b 2075 7365  ode/notebook use
-00011f40: 6420 746f 2063 7265 6174 650a 2020 2020  d to create.    
-00011f50: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00011f60: 6665 6174 7572 6520 6772 6f75 7020 6f72  feature group or
-00011f70: 2075 7365 6420 746f 2069 6e73 6572 7420   used to insert 
-00011f80: 6461 7461 2074 6f20 6974 2e20 5768 656e  data to it. When
-00011f90: 2063 616c 6c69 6e67 2074 6865 2060 696e   calling the `in
-00011fa0: 7365 7274 6020 6d65 7468 6f64 2072 6570  sert` method rep
-00011fb0: 6561 7465 646c 790a 2020 2020 2020 2020  eatedly.        
-00011fc0: 2020 2020 2020 2020 7769 7468 2073 6d61          with sma
-00011fd0: 6c6c 2062 6174 6368 6573 206f 6620 6461  ll batches of da
-00011fe0: 7461 2c20 7468 6973 2063 616e 2073 6c6f  ta, this can slo
-00011ff0: 7720 646f 776e 2074 6865 2077 7269 7465  w down the write
-00012000: 732e 2055 7365 2074 6869 7320 6f70 7469  s. Use this opti
-00012010: 6f6e 2074 6f20 7475 726e 206f 6666 2073  on to turn off s
-00012020: 6176 696e 670a 2020 2020 2020 2020 2020  aving.          
-00012030: 2020 2020 2020 636f 6465 2e20 4465 6661        code. Defa
-00012040: 756c 7473 2074 6f20 6054 7275 6560 2e0a  ults to `True`..
-00012050: 2020 2020 2020 2020 2020 2020 7761 6974              wait
-00012060: 3a20 5761 6974 2066 6f72 206a 6f62 2074  : Wait for job t
-00012070: 6f20 6669 6e69 7368 2062 6566 6f72 6520  o finish before 
-00012080: 7265 7475 726e 696e 672c 2064 6566 6175  returning, defau
-00012090: 6c74 7320 746f 2060 4661 6c73 6560 2e0a  lts to `False`..
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 5368 6f72 7463 7574 2066 6f72 2072 6561  Shortcut for rea
-000120c0: 645f 6f70 7469 6f6e 7320 607b 2277 6169  d_options `{"wai
-000120d0: 745f 666f 725f 6a6f 6222 3a20 4661 6c73  t_for_job": Fals
-000120e0: 657d 602e 0a0a 2020 2020 2020 2020 2320  e}`...        # 
-000120f0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00012100: 2020 2020 2860 4a6f 6260 2c20 6056 616c      (`Job`, `Val
-00012110: 6964 6174 696f 6e52 6570 6f72 7460 2920  idationReport`) 
-00012120: 4120 7475 706c 6520 7769 7468 206a 6f62  A tuple with job
-00012130: 2069 6e66 6f72 6d61 7469 6f6e 2069 6620   information if 
-00012140: 7079 7468 6f6e 2065 6e67 696e 6520 6973  python engine is
-00012150: 2075 7365 6420 616e 6420 7468 6520 7661   used and the va
-00012160: 6c69 6461 7469 6f6e 2072 6570 6f72 7420  lidation report 
-00012170: 6966 2076 616c 6964 6174 696f 6e20 6973  if validation is
-00012180: 2065 6e61 626c 6564 2e0a 2020 2020 2020   enabled..      
-00012190: 2020 2222 220a 2020 2020 2020 2020 6665    """.        fe
-000121a0: 6174 7572 655f 6461 7461 6672 616d 6520  ature_dataframe 
-000121b0: 3d20 656e 6769 6e65 2e67 6574 5f69 6e73  = engine.get_ins
-000121c0: 7461 6e63 6528 292e 636f 6e76 6572 745f  tance().convert_
-000121d0: 746f 5f64 6566 6175 6c74 5f64 6174 6166  to_default_dataf
-000121e0: 7261 6d65 2866 6561 7475 7265 7329 0a0a  rame(features)..
-000121f0: 2020 2020 2020 2020 6966 2077 7269 7465          if write
-00012200: 5f6f 7074 696f 6e73 2069 7320 4e6f 6e65  _options is None
-00012210: 3a0a 2020 2020 2020 2020 2020 2020 7772  :.            wr
-00012220: 6974 655f 6f70 7469 6f6e 7320 3d20 7b7d  ite_options = {}
-00012230: 0a20 2020 2020 2020 2069 6620 2277 6169  .        if "wai
-00012240: 745f 666f 725f 6a6f 6222 206e 6f74 2069  t_for_job" not i
-00012250: 6e20 7772 6974 655f 6f70 7469 6f6e 733a  n write_options:
-00012260: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00012270: 7465 5f6f 7074 696f 6e73 5b22 7761 6974  te_options["wait
-00012280: 5f66 6f72 5f6a 6f62 225d 203d 2077 6169  _for_job"] = wai
-00012290: 740a 0a20 2020 2020 2020 206a 6f62 2c20  t..        job, 
-000122a0: 6765 5f72 6570 6f72 7420 3d20 7365 6c66  ge_report = self
-000122b0: 2e5f 6665 6174 7572 655f 6772 6f75 705f  ._feature_group_
-000122c0: 656e 6769 6e65 2e69 6e73 6572 7428 0a20  engine.insert(. 
-000122d0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-000122e0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-000122f0: 7475 7265 5f64 6174 6166 7261 6d65 3d66  ture_dataframe=f
-00012300: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
-00012310: 2c0a 2020 2020 2020 2020 2020 2020 6f76  ,.            ov
-00012320: 6572 7772 6974 653d 6f76 6572 7772 6974  erwrite=overwrit
-00012330: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
-00012340: 7065 7261 7469 6f6e 3d6f 7065 7261 7469  peration=operati
-00012350: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00012360: 7374 6f72 6167 653d 7374 6f72 6167 652e  storage=storage.
-00012370: 6c6f 7765 7228 2920 6966 2073 746f 7261  lower() if stora
-00012380: 6765 2069 7320 6e6f 7420 4e6f 6e65 2065  ge is not None e
-00012390: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
-000123a0: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
-000123b0: 6f6e 733d 7772 6974 655f 6f70 7469 6f6e  ons=write_option
-000123c0: 732c 0a20 2020 2020 2020 2020 2020 2076  s,.            v
-000123d0: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
-000123e0: 733d 7b22 7361 7665 5f72 6570 6f72 7422  s={"save_report"
-000123f0: 3a20 5472 7565 2c20 2a2a 7661 6c69 6461  : True, **valida
-00012400: 7469 6f6e 5f6f 7074 696f 6e73 7d2c 0a20  tion_options},. 
-00012410: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00012420: 2069 6620 7361 7665 5f63 6f64 6520 616e   if save_code an
-00012430: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
-00012440: 6765 5f72 6570 6f72 7420 6973 204e 6f6e  ge_report is Non
-00012450: 6520 6f72 2067 655f 7265 706f 7274 2e69  e or ge_report.i
-00012460: 6e67 6573 7469 6f6e 5f72 6573 756c 7420  ngestion_result 
-00012470: 3d3d 2022 494e 4745 5354 4544 220a 2020  == "INGESTED".  
-00012480: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00012490: 2020 2020 2073 656c 662e 5f63 6f64 655f       self._code_
-000124a0: 656e 6769 6e65 2e73 6176 655f 636f 6465  engine.save_code
-000124b0: 2873 656c 6629 0a0a 2020 2020 2020 2020  (self)..        
-000124c0: 6966 2065 6e67 696e 652e 6765 745f 7479  if engine.get_ty
-000124d0: 7065 2829 203d 3d20 2273 7061 726b 223a  pe() == "spark":
-000124e0: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
-000124f0: 6e6c 7920 636f 6d70 7574 6520 7374 6174  nly compute stat
-00012500: 6973 7469 6373 2069 6620 7468 6520 656e  istics if the en
-00012510: 6769 6e65 2069 7320 5370 6172 6b2c 0a20  gine is Spark,. 
-00012520: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00012530: 5079 7468 6f6e 2c20 7468 6520 7374 6174  Python, the stat
-00012540: 6973 7469 6373 2061 7265 2063 6f6d 7075  istics are compu
-00012550: 7465 6420 6279 2074 6865 2061 7070 6c69  ted by the appli
-00012560: 6361 7469 6f6e 2064 6f69 6e67 2074 6865  cation doing the
-00012570: 2069 6e73 6572 740a 2020 2020 2020 2020   insert.        
-00012580: 2020 2020 7365 6c66 2e63 6f6d 7075 7465      self.compute
-00012590: 5f73 7461 7469 7374 6963 7328 290a 0a20  _statistics().. 
-000125a0: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
-000125b0: 2020 2020 2020 2020 2020 2020 6a6f 622c              job,
-000125c0: 0a20 2020 2020 2020 2020 2020 2067 655f  .            ge_
-000125d0: 7265 706f 7274 2e74 6f5f 6765 5f74 7970  report.to_ge_typ
-000125e0: 6528 2920 6966 2067 655f 7265 706f 7274  e() if ge_report
-000125f0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00012600: 6520 4e6f 6e65 2c0a 2020 2020 2020 2020  e None,.        
-00012610: 290a 0a20 2020 2064 6566 206d 756c 7469  )..    def multi
-00012620: 5f70 6172 745f 696e 7365 7274 280a 2020  _part_insert(.  
-00012630: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00012640: 2020 2020 6665 6174 7572 6573 3a20 556e      features: Un
-00012650: 696f 6e5b 0a20 2020 2020 2020 2020 2020  ion[.           
-00012660: 2070 642e 4461 7461 4672 616d 652c 0a20   pd.DataFrame,. 
-00012670: 2020 2020 2020 2020 2020 2054 7970 6556             TypeV
-00012680: 6172 2822 7079 7370 6172 6b2e 7371 6c2e  ar("pyspark.sql.
-00012690: 4461 7461 4672 616d 6522 292c 2020 2320  DataFrame"),  # 
-000126a0: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-000126b0: 2020 2020 2020 2054 7970 6556 6172 2822         TypeVar("
-000126c0: 7079 7370 6172 6b2e 5244 4422 292c 2020  pyspark.RDD"),  
-000126d0: 2320 6e6f 7161 3a20 4638 3231 0a20 2020  # noqa: F821.   
-000126e0: 2020 2020 2020 2020 206e 702e 6e64 6172           np.ndar
-000126f0: 7261 792c 0a20 2020 2020 2020 2020 2020  ray,.           
-00012700: 204c 6973 745b 6c69 7374 5d2c 0a20 2020   List[list],.   
-00012710: 2020 2020 205d 203d 204e 6f6e 652c 0a20       ] = None,. 
-00012720: 2020 2020 2020 206f 7665 7277 7269 7465         overwrite
-00012730: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00012740: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00012750: 2020 6f70 6572 6174 696f 6e3a 204f 7074    operation: Opt
-00012760: 696f 6e61 6c5b 7374 725d 203d 2022 7570  ional[str] = "up
-00012770: 7365 7274 222c 0a20 2020 2020 2020 2073  sert",.        s
-00012780: 746f 7261 6765 3a20 4f70 7469 6f6e 616c  torage: Optional
-00012790: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-000127a0: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
-000127b0: 6f6e 733a 204f 7074 696f 6e61 6c5b 4469  ons: Optional[Di
-000127c0: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
-000127d0: 7b7d 2c0a 2020 2020 2020 2020 7661 6c69  {},.        vali
-000127e0: 6461 7469 6f6e 5f6f 7074 696f 6e73 3a20  dation_options: 
-000127f0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00012800: 722c 2041 6e79 5d5d 203d 207b 7d2c 0a20  r, Any]] = {},. 
-00012810: 2020 2029 202d 3e20 556e 696f 6e5b 0a20     ) -> Union[. 
-00012820: 2020 2020 2020 2054 7570 6c65 5b4f 7074         Tuple[Opt
-00012830: 696f 6e61 6c5b 4a6f 625d 2c20 4f70 7469  ional[Job], Opti
-00012840: 6f6e 616c 5b56 616c 6964 6174 696f 6e52  onal[ValidationR
-00012850: 6570 6f72 745d 5d2c 0a20 2020 2020 2020  eport]],.       
-00012860: 2066 6561 7475 7265 5f67 726f 7570 5f77   feature_group_w
-00012870: 7269 7465 722e 4665 6174 7572 6547 726f  riter.FeatureGro
-00012880: 7570 5772 6974 6572 2c0a 2020 2020 5d3a  upWriter,.    ]:
-00012890: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-000128a0: 4665 6174 7572 6547 726f 7570 5772 6974  FeatureGroupWrit
-000128b0: 6572 2066 6f72 206f 7074 696d 697a 6564  er for optimized
-000128c0: 206d 756c 7469 2070 6172 7420 696e 7365   multi part inse
-000128d0: 7274 7320 6f72 2063 616c 6c20 7468 6973  rts or call this
-000128e0: 206d 6574 686f 640a 2020 2020 2020 2020   method.        
-000128f0: 746f 2073 7461 7274 206d 616e 7561 6c20  to start manual 
-00012900: 6d75 6c74 6920 7061 7274 206f 7074 696d  multi part optim
-00012910: 697a 6564 2069 6e73 6572 7473 2e0a 0a20  ized inserts... 
-00012920: 2020 2020 2020 2049 6e20 7573 6520 6361         In use ca
-00012930: 7365 7320 7768 6572 6520 7665 7279 2073  ses where very s
-00012940: 6d61 6c6c 2062 6174 6368 6573 2028 3120  mall batches (1 
-00012950: 746f 2031 3030 3029 2072 6f77 7320 7065  to 1000) rows pe
-00012960: 7220 4461 7461 6672 616d 6520 6e65 6564  r Dataframe need
-00012970: 0a20 2020 2020 2020 2074 6f20 6265 2077  .        to be w
-00012980: 7269 7474 656e 2074 6f20 7468 6520 6665  ritten to the fe
-00012990: 6174 7572 6520 7374 6f72 6520 7265 7065  ature store repe
-000129a0: 6174 6564 6c79 2c20 6974 206d 6967 6874  atedly, it might
-000129b0: 2062 6520 696e 6566 6669 6369 656e 7420   be inefficient 
-000129c0: 746f 2075 7365 0a20 2020 2020 2020 2074  to use.        t
-000129d0: 6865 2073 7461 6e64 6172 6420 6066 6561  he standard `fea
-000129e0: 7475 7265 5f67 726f 7570 2e69 6e73 6572  ture_group.inser
-000129f0: 7428 2960 206d 6574 686f 6420 6173 2069  t()` method as i
-00012a00: 7420 7065 7266 6f72 6d73 2073 6f6d 6520  t performs some 
-00012a10: 6261 636b 6772 6f75 6e64 0a20 2020 2020  background.     
-00012a20: 2020 2061 6374 696f 6e73 2074 6f20 7570     actions to up
-00012a30: 6461 7465 2074 6865 206d 6574 6164 6174  date the metadat
-00012a40: 6120 6f66 2074 6865 2066 6561 7475 7265  a of the feature
-00012a50: 2067 726f 7570 206f 626a 6563 7420 6669   group object fi
-00012a60: 7273 742e 0a0a 2020 2020 2020 2020 466f  rst...        Fo
-00012a70: 7220 7468 6573 6520 6361 7365 732c 2074  r these cases, t
-00012a80: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00012a90: 2070 726f 7669 6465 7320 7468 6520 606d   provides the `m
-00012aa0: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
-00012ab0: 6020 4150 492c 0a20 2020 2020 2020 2077  ` API,.        w
-00012ac0: 6869 6368 2069 7320 6f70 7469 6d69 7a65  hich is optimize
-00012ad0: 6420 666f 7220 7772 6974 696e 6720 6d61  d for writing ma
-00012ae0: 6e79 2073 6d61 6c6c 2044 6174 6166 7261  ny small Datafra
-00012af0: 6d65 7320 6166 7465 7220 616e 6f74 6865  mes after anothe
-00012b00: 722e 0a0a 2020 2020 2020 2020 5468 6572  r...        Ther
-00012b10: 6520 6172 6520 7477 6f20 7761 7973 2074  e are two ways t
-00012b20: 6f20 7573 6520 7468 6973 2041 5049 3a0a  o use this API:.
-00012b30: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-00012b40: 706c 6520 2250 7974 686f 6e20 436f 6e74  ple "Python Cont
-00012b50: 6578 7420 4d61 6e61 6765 7222 0a20 2020  ext Manager".   
-00012b60: 2020 2020 2020 2020 2055 7369 6e67 2074           Using t
-00012b70: 6865 2050 7974 686f 6e20 6077 6974 6860  he Python `with`
-00012b80: 2073 796e 7461 7820 796f 7520 6361 6e20   syntax you can 
-00012b90: 6163 7175 6972 6520 6120 4665 6174 7572  acquire a Featur
-00012ba0: 6547 726f 7570 5772 6974 6572 0a20 2020  eGroupWriter.   
-00012bb0: 2020 2020 2020 2020 206f 626a 6563 7420           object 
-00012bc0: 7468 6174 2069 6d70 6c65 6d65 6e74 7320  that implements 
-00012bd0: 7468 6520 7361 6d65 2060 6d75 6c74 695f  the same `multi_
-00012be0: 7061 7274 5f69 6e73 6572 7460 2041 5049  part_insert` API
-00012bf0: 2e0a 2020 2020 2020 2020 2020 2020 6060  ..            ``
-00012c00: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00012c10: 2020 2020 6665 6174 7572 655f 6772 6f75      feature_grou
-00012c20: 7020 3d20 6673 2e67 6574 5f6f 725f 6372  p = fs.get_or_cr
-00012c30: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00012c40: 7570 2822 6667 5f6e 616d 6522 2c20 7665  up("fg_name", ve
-00012c50: 7273 696f 6e3d 3129 0a0a 2020 2020 2020  rsion=1)..      
-00012c60: 2020 2020 2020 7769 7468 2066 6561 7475        with featu
-00012c70: 7265 5f67 726f 7570 2e6d 756c 7469 5f70  re_group.multi_p
-00012c80: 6172 745f 696e 7365 7274 2829 2061 7320  art_insert() as 
-00012c90: 7772 6974 6572 3a0a 2020 2020 2020 2020  writer:.        
-00012ca0: 2020 2020 2020 2020 2320 7275 6e20 696e          # run in
-00012cb0: 7365 7274 7320 696e 2061 206c 6f6f 703a  serts in a loop:
-00012cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012cd0: 2077 6869 6c65 206c 6f6f 703a 0a20 2020   while loop:.   
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2073 6d61 6c6c 5f62 6174 6368 5f64 6620   small_batch_df 
-00012d00: 3d20 2e2e 2e0a 2020 2020 2020 2020 2020  = ....          
-00012d10: 2020 2020 2020 2020 2020 7772 6974 6572            writer
-00012d20: 2e69 6e73 6572 7428 736d 616c 6c5f 6261  .insert(small_ba
-00012d30: 7463 685f 6466 290a 2020 2020 2020 2020  tch_df).        
-00012d40: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00012d50: 2020 2020 5468 6520 7772 6974 6572 2062      The writer b
-00012d60: 6174 6368 6573 2074 6865 2073 6d61 6c6c  atches the small
-00012d70: 2044 6174 6166 7261 6d65 7320 616e 6420   Dataframes and 
-00012d80: 7472 616e 736d 6974 7320 7468 656d 2074  transmits them t
-00012d90: 6f20 486f 7073 776f 726b 730a 2020 2020  o Hopsworks.    
-00012da0: 2020 2020 2020 2020 6566 6669 6369 656e          efficien
-00012db0: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
-00012dc0: 2057 6865 6e20 6578 6974 696e 6720 7468   When exiting th
-00012dd0: 6520 636f 6e74 6578 742c 2074 6865 2066  e context, the f
-00012de0: 6561 7475 7265 2067 726f 7570 2077 7269  eature group wri
-00012df0: 7465 7220 6973 2073 7572 6520 746f 2065  ter is sure to e
-00012e00: 7869 740a 2020 2020 2020 2020 2020 2020  xit.            
-00012e10: 6f6e 6c79 206f 6e63 6520 616c 6c20 7468  only once all th
-00012e20: 6520 726f 7773 2068 6176 6520 6265 656e  e rows have been
-00012e30: 2074 7261 6e73 6d69 7474 6564 2e0a 0a20   transmitted... 
-00012e40: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-00012e50: 6c65 2022 4d75 6c74 6920 7061 7274 2069  le "Multi part i
-00012e60: 6e73 6572 7420 7769 7468 206d 616e 7561  nsert with manua
-00012e70: 6c20 636f 6e74 6578 7420 6d61 6e61 6765  l context manage
-00012e80: 6d65 6e74 220a 2020 2020 2020 2020 2020  ment".          
-00012e90: 2020 496e 7374 6561 6420 6f66 206c 6574    Instead of let
-00012ea0: 7469 6e67 2050 7974 686f 6e20 6861 6e64  ting Python hand
-00012eb0: 6c65 2074 6865 2065 6e74 6572 696e 6720  le the entering 
-00012ec0: 616e 6420 6578 6974 696e 6720 6f66 2074  and exiting of t
-00012ed0: 6865 0a20 2020 2020 2020 2020 2020 206d  he.            m
-00012ee0: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
-00012ef0: 2063 6f6e 7465 7874 2c20 796f 7520 6361   context, you ca
-00012f00: 6e20 7374 6172 7420 616e 6420 6669 6e61  n start and fina
-00012f10: 6c69 7a65 2074 6865 2063 6f6e 7465 7874  lize the context
-00012f20: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
-00012f30: 7561 6c6c 792e 0a20 2020 2020 2020 2020  ually..         
-00012f40: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00012f50: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-00012f60: 5f67 726f 7570 203d 2066 732e 6765 745f  _group = fs.get_
-00012f70: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
-00012f80: 655f 6772 6f75 7028 2266 675f 6e61 6d65  e_group("fg_name
-00012f90: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
-00012fa0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00012fb0: 206c 6f6f 703a 0a20 2020 2020 2020 2020   loop:.         
-00012fc0: 2020 2020 2020 2073 6d61 6c6c 5f62 6174         small_bat
-00012fd0: 6368 5f64 6620 3d20 2e2e 2e0a 2020 2020  ch_df = ....    
-00012fe0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00012ff0: 7572 655f 6772 6f75 702e 6d75 6c74 695f  ure_group.multi_
-00013000: 7061 7274 5f69 6e73 6572 7428 736d 616c  part_insert(smal
-00013010: 6c5f 6261 7463 685f 6466 290a 0a20 2020  l_batch_df)..   
-00013020: 2020 2020 2020 2020 2023 2049 4d50 4f52           # IMPOR
-00013030: 5441 4e54 3a20 6669 6e61 6c69 7a65 2074  TANT: finalize t
-00013040: 6865 206d 756c 7469 2070 6172 7420 696e  he multi part in
-00013050: 7365 7274 2074 6f20 6d61 6b65 2073 7572  sert to make sur
-00013060: 6520 616c 6c20 726f 7773 0a20 2020 2020  e all rows.     
-00013070: 2020 2020 2020 2023 2068 6176 6520 6265         # have be
-00013080: 656e 2074 7261 6e73 6d69 7474 6564 0a20  en transmitted. 
-00013090: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-000130a0: 7265 5f67 726f 7570 2e66 696e 616c 697a  re_group.finaliz
-000130b0: 655f 6d75 6c74 695f 7061 7274 5f69 6e73  e_multi_part_ins
-000130c0: 6572 7428 290a 2020 2020 2020 2020 2020  ert().          
-000130d0: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
-000130e0: 2020 4e6f 7465 2074 6861 7420 7468 6520    Note that the 
-000130f0: 6669 7273 7420 6361 6c6c 2074 6f20 606d  first call to `m
-00013100: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
-00013110: 6020 696e 6974 6961 7465 7320 7468 6520  ` initiates the 
-00013120: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
-00013130: 2020 2020 616e 6420 6265 2073 7572 6520      and be sure 
-00013140: 746f 2066 696e 616c 697a 6520 6974 2e20  to finalize it. 
-00013150: 5468 6520 6066 696e 616c 697a 655f 6d75  The `finalize_mu
-00013160: 6c74 695f 7061 7274 5f69 6e73 6572 7460  lti_part_insert`
-00013170: 2069 7320 610a 2020 2020 2020 2020 2020   is a.          
-00013180: 2020 626c 6f63 6b69 6e67 2063 616c 6c20    blocking call 
-00013190: 7468 6174 2072 6574 7572 6e73 206f 6e63  that returns onc
-000131a0: 6520 616c 6c20 726f 7773 2068 6176 6520  e all rows have 
-000131b0: 6265 656e 2074 7261 6e73 6d69 7474 6564  been transmitted
-000131c0: 2e0a 0a20 2020 2020 2020 2020 2020 204f  ...            O
-000131d0: 6e63 6520 796f 7520 6172 6520 646f 6e65  nce you are done
-000131e0: 2077 6974 6820 7468 6520 6d75 6c74 6920   with the multi 
-000131f0: 7061 7274 2069 6e73 6572 742c 2069 7420  part insert, it 
-00013200: 6973 2067 6f6f 6420 7072 6163 7469 6365  is good practice
-00013210: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00013220: 7374 6172 7420 7468 6520 6261 636b 6669  start the backfi
-00013230: 6c6c 206a 6f62 2069 6e20 6f72 6465 7220  ll job in order 
-00013240: 746f 2077 7269 7465 2074 6865 2064 6174  to write the dat
-00013250: 6120 746f 2074 6865 206f 6666 6c69 6e65  a to the offline
-00013260: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
-00013270: 7261 6765 3a0a 2020 2020 2020 2020 2020  rage:.          
-00013280: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00013290: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
-000132a0: 6772 6f75 702e 6261 636b 6669 6c6c 5f6a  group.backfill_j
-000132b0: 6f62 2e72 756e 2861 7761 6974 5f74 6572  ob.run(await_ter
-000132c0: 6d69 6e61 7469 6f6e 3d54 7275 6529 0a20  mination=True). 
-000132d0: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-000132e0: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-000132f0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00013300: 6665 6174 7572 6573 3a20 4461 7461 4672  features: DataFr
-00013310: 616d 652c 2052 4444 2c20 4e64 6172 7261  ame, RDD, Ndarra
-00013320: 792c 206c 6973 742e 2046 6561 7475 7265  y, list. Feature
-00013330: 7320 746f 2062 6520 7361 7665 642e 0a20  s to be saved.. 
-00013340: 2020 2020 2020 2020 2020 206f 7665 7277             overw
-00013350: 7269 7465 3a20 4472 6f70 2061 6c6c 2064  rite: Drop all d
-00013360: 6174 6120 696e 2074 6865 2066 6561 7475  ata in the featu
-00013370: 7265 2067 726f 7570 2062 6566 6f72 650a  re group before.
-00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013390: 696e 7365 7274 696e 6720 6e65 7720 6461  inserting new da
-000133a0: 7461 2e20 5468 6973 2064 6f65 7320 6e6f  ta. This does no
-000133b0: 7420 6166 6665 6374 206d 6574 6164 6174  t affect metadat
-000133c0: 612c 2064 6566 6175 6c74 7320 746f 2046  a, defaults to F
-000133d0: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-000133e0: 2020 6f70 6572 6174 696f 6e3a 2041 7061    operation: Apa
-000133f0: 6368 6520 4875 6469 206f 7065 7261 7469  che Hudi operati
-00013400: 6f6e 2074 7970 6520 6022 696e 7365 7274  on type `"insert
-00013410: 2260 206f 7220 6022 7570 7365 7274 2260  "` or `"upsert"`
-00013420: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013430: 2020 4465 6661 756c 7473 2074 6f20 6022    Defaults to `"
-00013440: 7570 7365 7274 2260 2e0a 2020 2020 2020  upsert"`..      
-00013450: 2020 2020 2020 7374 6f72 6167 653a 204f        storage: O
-00013460: 7665 7277 7269 7465 2064 6566 6175 6c74  verwrite default
-00013470: 2062 6568 6176 696f 7572 2c20 7772 6974   behaviour, writ
-00013480: 6520 746f 206f 6666 6c69 6e65 0a20 2020  e to offline.   
-00013490: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-000134a0: 7261 6765 206f 6e6c 7920 7769 7468 2060  rage only with `
-000134b0: 226f 6666 6c69 6e65 2260 206f 7220 6f6e  "offline"` or on
-000134c0: 6c69 6e65 206f 6e6c 7920 7769 7468 2060  line only with `
-000134d0: 226f 6e6c 696e 6522 602c 2064 6566 6175  "online"`, defau
-000134e0: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
-000134f0: 2020 2020 746f 2060 4e6f 6e65 602e 0a20      to `None`.. 
-00013500: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00013510: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-00013520: 6f6e 616c 2077 7269 7465 206f 7074 696f  onal write optio
-00013530: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
-00013540: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
-00013550: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
-00013560: 2020 2020 2020 2020 2057 6865 6e20 7573           When us
-00013570: 696e 6720 7468 6520 6070 7974 686f 6e60  ing the `python`
-00013580: 2065 6e67 696e 652c 2077 7269 7465 5f6f   engine, write_o
-00013590: 7074 696f 6e73 2063 616e 2063 6f6e 7461  ptions can conta
-000135a0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
-000135b0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
-000135c0: 2065 6e74 7269 6573 3a0a 2020 2020 2020   entries:.      
-000135d0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
-000135e0: 6073 7061 726b 6020 616e 6420 7661 6c75  `spark` and valu
-000135f0: 6520 616e 206f 626a 6563 7420 6f66 2074  e an object of t
-00013600: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-00013610: 2020 2020 5b68 7366 732e 636f 7265 2e6a      [hsfs.core.j
-00013620: 6f62 5f63 6f6e 6669 6775 7261 7469 6f6e  ob_configuration
-00013630: 2e4a 6f62 436f 6e66 6967 7572 6174 696f  .JobConfiguratio
-00013640: 6e5d 282e 2e2f 6a6f 625f 636f 6e66 6967  n](../job_config
-00013650: 7572 6174 696f 6e29 0a20 2020 2020 2020  uration).       
-00013660: 2020 2020 2020 2020 2020 2074 6f20 636f             to co
-00013670: 6e66 6967 7572 6520 7468 6520 486f 7073  nfigure the Hops
-00013680: 776f 726b 7320 4a6f 6220 7573 6564 2074  works Job used t
-00013690: 6f20 7772 6974 6520 6461 7461 2069 6e74  o write data int
-000136a0: 6f20 7468 650a 2020 2020 2020 2020 2020  o the.          
-000136b0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
-000136c0: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
-000136d0: 2020 2020 2020 202a 206b 6579 2060 7761         * key `wa
-000136e0: 6974 5f66 6f72 5f6a 6f62 6020 616e 6420  it_for_job` and 
-000136f0: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
-00013700: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
-00013710: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
-00013720: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
-00013730: 7220 6e6f 7420 746f 2074 6865 2069 6e73  r not to the ins
-00013740: 6572 7420 6361 6c6c 2073 686f 756c 6420  ert call should 
-00013750: 7265 7475 726e 206f 6e6c 790a 2020 2020  return only.    
-00013760: 2020 2020 2020 2020 2020 2020 2020 6166                af
-00013770: 7465 7220 7468 6520 486f 7073 776f 726b  ter the Hopswork
-00013780: 7320 4a6f 6220 6861 7320 6669 6e69 7368  s Job has finish
-00013790: 6564 2e20 4279 2064 6566 6175 6c74 2069  ed. By default i
-000137a0: 7420 7761 6974 732e 0a20 2020 2020 2020  t waits..       
-000137b0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-000137c0: 7374 6172 745f 6f66 666c 696e 655f 6261  start_offline_ba
-000137d0: 636b 6669 6c6c 6020 616e 6420 7661 6c75  ckfill` and valu
-000137e0: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
-000137f0: 7365 6020 746f 2063 6f6e 6669 6775 7265  se` to configure
-00013800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013810: 2020 2077 6865 7468 6572 206f 7220 6e6f     whether or no
-00013820: 7420 746f 2073 7461 7274 2074 6865 2062  t to start the b
-00013830: 6163 6b66 696c 6c20 6a6f 6220 746f 2077  ackfill job to w
-00013840: 7269 7465 2064 6174 6120 746f 2074 6865  rite data to the
-00013850: 206f 6666 6c69 6e65 0a20 2020 2020 2020   offline.       
-00013860: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-00013870: 6765 2e20 4279 2064 6566 6175 6c74 2074  ge. By default t
-00013880: 6865 2062 6163 6b66 696c 6c20 6a6f 6220  he backfill job 
-00013890: 646f 6573 206e 6f74 2067 6574 2073 7461  does not get sta
-000138a0: 7274 6564 2061 7574 6f6d 6174 6963 616c  rted automatical
-000138b0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-000138c0: 2020 2020 2066 6f72 206d 756c 7469 2070       for multi p
-000138d0: 6172 7420 696e 7365 7274 732e 0a20 2020  art inserts..   
-000138e0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
-000138f0: 6579 2060 696e 7465 726e 616c 5f6b 6166  ey `internal_kaf
-00013900: 6b61 6020 616e 6420 7661 6c75 6520 6054  ka` and value `T
-00013910: 7275 6560 206f 7220 6046 616c 7365 6020  rue` or `False` 
-00013920: 696e 2063 6173 6520 796f 7520 6573 7461  in case you esta
-00013930: 626c 6973 6865 640a 2020 2020 2020 2020  blished.        
-00013940: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
-00013950: 7469 7669 7479 2066 726f 6d20 796f 7520  tivity from you 
-00013960: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
-00013970: 6e74 2074 6f20 7468 6520 696e 7465 726e  nt to the intern
-00013980: 616c 2061 6476 6572 7469 7365 640a 2020  al advertised.  
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 6c69 7374 656e 6572 7320 6f66 2074 6865  listeners of the
-000139b0: 2048 6f70 7377 6f72 6b73 204b 6166 6b61   Hopsworks Kafka
-000139c0: 2043 6c75 7374 6572 2e20 4465 6661 756c   Cluster. Defaul
-000139d0: 7473 2074 6f20 6046 616c 7365 6020 616e  ts to `False` an
-000139e0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000139f0: 2020 2020 7769 6c6c 2075 7365 2065 7874      will use ext
-00013a00: 6572 6e61 6c20 6c69 7374 656e 6572 7320  ernal listeners 
-00013a10: 7768 656e 2063 6f6e 6e65 6374 696e 6720  when connecting 
-00013a20: 6672 6f6d 206f 7574 7369 6465 206f 6620  from outside of 
-00013a30: 486f 7073 776f 726b 732e 0a20 2020 2020  Hopsworks..     
-00013a40: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00013a50: 6e5f 6f70 7469 6f6e 733a 2041 6464 6974  n_options: Addit
-00013a60: 696f 6e61 6c20 7661 6c69 6461 7469 6f6e  ional validation
-00013a70: 206f 7074 696f 6e73 2061 7320 6b65 792d   options as key-
-00013a80: 7661 6c75 6520 7061 6972 732c 2064 6566  value pairs, def
-00013a90: 6175 6c74 7320 746f 2060 7b7d 602e 0a20  aults to `{}`.. 
-00013aa0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00013ab0: 206b 6579 2060 7275 6e5f 7661 6c69 6461   key `run_valida
-00013ac0: 7469 6f6e 6020 626f 6f6c 6561 6e20 7661  tion` boolean va
-00013ad0: 6c75 652c 2073 6574 2074 6f20 6046 616c  lue, set to `Fal
-00013ae0: 7365 6020 746f 2073 6b69 7020 7661 6c69  se` to skip vali
-00013af0: 6461 7469 6f6e 2074 656d 706f 7261 7269  dation temporari
-00013b00: 6c79 206f 6e20 696e 6765 7374 696f 6e2e  ly on ingestion.
-00013b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b20: 202a 206b 6579 2060 7361 7665 5f72 6570   * key `save_rep
-00013b30: 6f72 7460 2062 6f6f 6c65 616e 2076 616c  ort` boolean val
-00013b40: 7565 2c20 7365 7420 746f 2060 4661 6c73  ue, set to `Fals
-00013b50: 6560 2074 6f20 736b 6970 2075 706c 6f61  e` to skip uploa
-00013b60: 6420 6f66 2074 6865 2076 616c 6964 6174  d of the validat
-00013b70: 696f 6e20 7265 706f 7274 2074 6f20 486f  ion report to Ho
-00013b80: 7073 776f 726b 732e 0a20 2020 2020 2020  psworks..       
-00013b90: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-00013ba0: 6765 5f76 616c 6964 6174 655f 6b77 6172  ge_validate_kwar
-00013bb0: 6773 6020 6120 6469 6374 696f 6e61 7279  gs` a dictionary
-00013bc0: 2063 6f6e 7461 696e 696e 6720 6b77 6172   containing kwar
-00013bd0: 6773 2066 6f72 2074 6865 2076 616c 6964  gs for the valid
-00013be0: 6174 6520 6d65 7468 6f64 206f 6620 4772  ate method of Gr
-00013bf0: 6561 7420 4578 7065 6374 6174 696f 6e73  eat Expectations
-00013c00: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013c10: 2020 2a20 6b65 7920 6066 6574 6368 5f65    * key `fetch_e
-00013c20: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00013c30: 6020 6120 626f 6f6c 6561 6e20 7661 6c75  ` a boolean valu
-00013c40: 652c 2062 7920 6465 6661 756c 7420 6046  e, by default `F
-00013c50: 616c 7365 6020 666f 7220 6d75 6c74 6920  alse` for multi 
-00013c60: 7061 7274 2069 6e73 6572 7473 2c0a 2020  part inserts,.  
-00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c80: 2074 6f20 636f 6e74 726f 6c20 7768 6574   to control whet
-00013c90: 6865 7220 7468 6520 6578 7065 6374 6174  her the expectat
-00013ca0: 696f 6e20 7375 6974 6520 6f66 2074 6865  ion suite of the
-00013cb0: 2066 6561 7475 7265 2067 726f 7570 2073   feature group s
-00013cc0: 686f 756c 6420 6265 2066 6574 6368 6564  hould be fetched
-00013cd0: 2062 6566 6f72 6520 6576 6572 7920 696e   before every in
-00013ce0: 7365 7274 2e0a 0a20 2020 2020 2020 2023  sert...        #
-00013cf0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00013d00: 2020 2020 2028 604a 6f62 602c 2060 5661       (`Job`, `Va
-00013d10: 6c69 6461 7469 6f6e 5265 706f 7274 6029  lidationReport`)
-00013d20: 2041 2074 7570 6c65 2077 6974 6820 6a6f   A tuple with jo
-00013d30: 6220 696e 666f 726d 6174 696f 6e20 6966  b information if
-00013d40: 2070 7974 686f 6e20 656e 6769 6e65 2069   python engine i
-00013d50: 7320 7573 6564 2061 6e64 2074 6865 2076  s used and the v
-00013d60: 616c 6964 6174 696f 6e20 7265 706f 7274  alidation report
-00013d70: 2069 6620 7661 6c69 6461 7469 6f6e 2069   if validation i
-00013d80: 7320 656e 6162 6c65 642e 0a20 2020 2020  s enabled..     
-00013d90: 2020 2020 2020 2060 4665 6174 7572 6547         `FeatureG
-00013da0: 726f 7570 5772 6974 6572 6020 5768 656e  roupWriter` When
-00013db0: 2075 7365 6420 6173 2061 2063 6f6e 7465   used as a conte
-00013dc0: 7874 206d 616e 6167 6572 2077 6974 6820  xt manager with 
-00013dd0: 5079 7468 6f6e 2060 7769 7468 6020 7374  Python `with` st
-00013de0: 6174 656d 656e 742e 0a20 2020 2020 2020  atement..       
-00013df0: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-00013e00: 662e 5f6d 756c 7469 5f70 6172 745f 696e  f._multi_part_in
-00013e10: 7365 7274 203d 2054 7275 650a 2020 2020  sert = True.    
-00013e20: 2020 2020 6d75 6c74 695f 7061 7274 5f77      multi_part_w
-00013e30: 7269 7465 7220 3d20 6665 6174 7572 655f  riter = feature_
-00013e40: 6772 6f75 705f 7772 6974 6572 2e46 6561  group_writer.Fea
-00013e50: 7475 7265 4772 6f75 7057 7269 7465 7228  tureGroupWriter(
-00013e60: 7365 6c66 290a 2020 2020 2020 2020 6966  self).        if
-00013e70: 2066 6561 7475 7265 7320 6973 204e 6f6e   features is Non
-00013e80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013e90: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
-00013ea0: 5f77 7269 7465 720a 2020 2020 2020 2020  _writer.        
-00013eb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00013ec0: 2020 2320 676f 2074 6872 6f75 6768 2077    # go through w
-00013ed0: 7269 7465 7220 746f 2061 766f 6964 2073  riter to avoid s
-00013ee0: 6574 7469 6e67 206d 756c 7469 2069 6e73  etting multi ins
-00013ef0: 6572 7420 6465 6661 756c 7473 2061 6761  ert defaults aga
-00013f00: 696e 0a20 2020 2020 2020 2020 2020 2072  in.            r
-00013f10: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
-00013f20: 5f77 7269 7465 722e 696e 7365 7274 280a  _writer.insert(.
-00013f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f40: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-00013f50: 2020 2020 2020 2020 2020 6f76 6572 7772            overwr
-00013f60: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-00013f70: 2020 2020 206f 7065 7261 7469 6f6e 2c0a       operation,.
-00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f90: 7374 6f72 6167 652c 0a20 2020 2020 2020  storage,.       
-00013fa0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-00013fb0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
-00013fc0: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
-00013fd0: 6f6e 5f6f 7074 696f 6e73 2c0a 2020 2020  on_options,.    
-00013fe0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00013ff0: 6566 2066 696e 616c 697a 655f 6d75 6c74  ef finalize_mult
-00014000: 695f 7061 7274 5f69 6e73 6572 7428 7365  i_part_insert(se
-00014010: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00014020: 4669 6e61 6c69 7a65 7320 616e 6420 6578  Finalizes and ex
-00014030: 6974 7320 7468 6520 6d75 6c74 6920 7061  its the multi pa
-00014040: 7274 2069 6e73 6572 7420 636f 6e74 6578  rt insert contex
-00014050: 7420 6f70 656e 6564 2062 7920 606d 756c  t opened by `mul
-00014060: 7469 5f70 6172 745f 696e 7365 7274 600a  ti_part_insert`.
-00014070: 2020 2020 2020 2020 696e 2061 2062 6c6f          in a blo
-00014080: 636b 696e 6720 6661 7368 696f 6e20 6f6e  cking fashion on
-00014090: 6365 2061 6c6c 2072 6f77 7320 6861 7665  ce all rows have
-000140a0: 2062 6565 6e20 7472 616e 736d 6974 7465   been transmitte
-000140b0: 642e 0a0a 2020 2020 2020 2020 2121 2120  d...        !!! 
-000140c0: 6578 616d 706c 6520 224d 756c 7469 2070  example "Multi p
-000140d0: 6172 7420 696e 7365 7274 2077 6974 6820  art insert with 
-000140e0: 6d61 6e75 616c 2063 6f6e 7465 7874 206d  manual context m
-000140f0: 616e 6167 656d 656e 7422 0a20 2020 2020  anagement".     
-00014100: 2020 2020 2020 2049 6e73 7465 6164 206f         Instead o
-00014110: 6620 6c65 7474 696e 6720 5079 7468 6f6e  f letting Python
-00014120: 2068 616e 646c 6520 7468 6520 656e 7465   handle the ente
-00014130: 7269 6e67 2061 6e64 2065 7869 7469 6e67  ring and exiting
-00014140: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00014150: 2020 2020 6d75 6c74 6920 7061 7274 2069      multi part i
-00014160: 6e73 6572 7420 636f 6e74 6578 742c 2079  nsert context, y
-00014170: 6f75 2063 616e 2073 7461 7274 2061 6e64  ou can start and
-00014180: 2066 696e 616c 697a 6520 7468 6520 636f   finalize the co
-00014190: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
-000141a0: 2020 6d61 6e75 616c 6c79 2e0a 2020 2020    manually..    
-000141b0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000141c0: 6e0a 2020 2020 2020 2020 2020 2020 6665  n.            fe
-000141d0: 6174 7572 655f 6772 6f75 7020 3d20 6673  ature_group = fs
-000141e0: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-000141f0: 6561 7475 7265 5f67 726f 7570 2822 6667  eature_group("fg
-00014200: 5f6e 616d 6522 2c20 7665 7273 696f 6e3d  _name", version=
-00014210: 3129 0a0a 2020 2020 2020 2020 2020 2020  1)..            
-00014220: 7768 696c 6520 6c6f 6f70 3a0a 2020 2020  while loop:.    
-00014230: 2020 2020 2020 2020 2020 2020 736d 616c              smal
-00014240: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
-00014250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014260: 2066 6561 7475 7265 5f67 726f 7570 2e6d   feature_group.m
-00014270: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
-00014280: 2873 6d61 6c6c 5f62 6174 6368 5f64 6629  (small_batch_df)
-00014290: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000142a0: 494d 504f 5254 414e 543a 2066 696e 616c  IMPORTANT: final
-000142b0: 697a 6520 7468 6520 6d75 6c74 6920 7061  ize the multi pa
-000142c0: 7274 2069 6e73 6572 7420 746f 206d 616b  rt insert to mak
-000142d0: 6520 7375 7265 2061 6c6c 2072 6f77 730a  e sure all rows.
-000142e0: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
-000142f0: 7665 2062 6565 6e20 7472 616e 736d 6974  ve been transmit
-00014300: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00014310: 6665 6174 7572 655f 6772 6f75 702e 6669  feature_group.fi
-00014320: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
-00014330: 745f 696e 7365 7274 2829 0a20 2020 2020  t_insert().     
-00014340: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00014350: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00014360: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
-00014370: 746f 2060 6d75 6c74 695f 7061 7274 5f69  to `multi_part_i
-00014380: 6e73 6572 7460 2069 6e69 7469 6174 6573  nsert` initiates
-00014390: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
-000143a0: 2020 2020 2020 2020 2061 6e64 2062 6520           and be 
-000143b0: 7375 7265 2074 6f20 6669 6e61 6c69 7a65  sure to finalize
-000143c0: 2069 742e 2054 6865 2060 6669 6e61 6c69   it. The `finali
-000143d0: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
-000143e0: 7365 7274 6020 6973 2061 0a20 2020 2020  sert` is a.     
-000143f0: 2020 2020 2020 2062 6c6f 636b 696e 6720         blocking 
-00014400: 6361 6c6c 2074 6861 7420 7265 7475 726e  call that return
-00014410: 7320 6f6e 6365 2061 6c6c 2072 6f77 7320  s once all rows 
-00014420: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
-00014430: 6974 7465 642e 0a20 2020 2020 2020 2022  itted..        "
-00014440: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00014450: 6c66 2e5f 6b61 666b 615f 7072 6f64 7563  lf._kafka_produc
-00014460: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00014470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014480: 2e5f 6b61 666b 615f 7072 6f64 7563 6572  ._kafka_producer
-00014490: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
-000144a0: 2020 2020 2073 656c 662e 5f6b 6166 6b61       self._kafka
-000144b0: 5f70 726f 6475 6365 7220 3d20 4e6f 6e65  _producer = None
-000144c0: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-000144d0: 6561 7475 7265 5f77 7269 7465 7273 203d  eature_writers =
-000144e0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-000144f0: 6c66 2e5f 7772 6974 6572 203d 204e 6f6e  lf._writer = Non
-00014500: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00014510: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
-00014520: 7420 3d20 4661 6c73 650a 0a20 2020 2064  t = False..    d
-00014530: 6566 2069 6e73 6572 745f 7374 7265 616d  ef insert_stream
-00014540: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00014550: 2020 2020 2020 2020 6665 6174 7572 6573          features
-00014560: 3a20 5479 7065 5661 7228 2270 7973 7061  : TypeVar("pyspa
-00014570: 726b 2e73 716c 2e44 6174 6146 7261 6d65  rk.sql.DataFrame
-00014580: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
-00014590: 310a 2020 2020 2020 2020 7175 6572 795f  1.        query_
-000145a0: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
-000145b0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000145c0: 2020 2020 6f75 7470 7574 5f6d 6f64 653a      output_mode:
-000145d0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-000145e0: 2022 6170 7065 6e64 222c 0a20 2020 2020   "append",.     
-000145f0: 2020 2061 7761 6974 5f74 6572 6d69 6e61     await_termina
-00014600: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b62  tion: Optional[b
-00014610: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-00014620: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
-00014630: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00014640: 6f6e 652c 0a20 2020 2020 2020 2063 6865  one,.        che
-00014650: 636b 706f 696e 745f 6469 723a 204f 7074  ckpoint_dir: Opt
-00014660: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00014670: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
-00014680: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-00014690: 616c 5b44 6963 745b 416e 792c 2041 6e79  al[Dict[Any, Any
-000146a0: 5d5d 203d 207b 7d2c 0a20 2020 2029 3a0a  ]] = {},.    ):.
-000146b0: 2020 2020 2020 2020 2222 2249 6e67 6573          """Inges
-000146c0: 7420 6120 5370 6172 6b20 5374 7275 6374  t a Spark Struct
-000146d0: 7572 6564 2053 7472 6561 6d69 6e67 2044  ured Streaming D
-000146e0: 6174 6166 7261 6d65 2074 6f20 7468 6520  ataframe to the 
-000146f0: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-00014700: 746f 7265 2e0a 0a20 2020 2020 2020 2054  tore...        T
-00014710: 6869 7320 6d65 7468 6f64 2063 7265 6174  his method creat
-00014720: 6573 2061 206c 6f6e 6720 7275 6e6e 696e  es a long runnin
-00014730: 6720 5370 6172 6b20 5374 7265 616d 696e  g Spark Streamin
-00014740: 6720 5175 6572 792c 2079 6f75 2063 616e  g Query, you can
-00014750: 2063 6f6e 7472 6f6c 2074 6865 0a20 2020   control the.   
-00014760: 2020 2020 2074 6572 6d69 6e61 7469 6f6e       termination
-00014770: 206f 6620 7468 6520 7175 6572 7920 7468   of the query th
-00014780: 726f 7567 6820 7468 6520 6172 6775 6d65  rough the argume
-00014790: 6e74 732e 0a0a 2020 2020 2020 2020 4974  nts...        It
-000147a0: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
-000147b0: 7374 6f70 2074 6865 2072 6574 7572 6e65  stop the returne
-000147c0: 6420 7175 6572 7920 7769 7468 2074 6865  d query with the
-000147d0: 2060 2e73 746f 7028 2960 2061 6e64 2063   `.stop()` and c
-000147e0: 6865 636b 2069 7473 0a20 2020 2020 2020  heck its.       
-000147f0: 2073 7461 7475 7320 7769 7468 2060 2e69   status with `.i
-00014800: 7341 6374 6976 6560 2e0a 0a20 2020 2020  sActive`...     
-00014810: 2020 2054 6f20 6765 7420 6120 6c69 7374     To get a list
-00014820: 206f 6620 616c 6c20 6163 7469 7665 2071   of all active q
-00014830: 7565 7269 6573 2c20 7573 653a 0a0a 2020  ueries, use:..  
-00014840: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00014850: 2020 2020 2020 2020 7371 6d20 3d20 7370          sqm = sp
-00014860: 6172 6b2e 7374 7265 616d 730a 0a20 2020  ark.streams..   
-00014870: 2020 2020 2023 2067 6574 2074 6865 206c       # get the l
-00014880: 6973 7420 6f66 2061 6374 6976 6520 7374  ist of active st
-00014890: 7265 616d 696e 6720 7175 6572 6965 730a  reaming queries.
-000148a0: 2020 2020 2020 2020 5b71 2e6e 616d 6520          [q.name 
-000148b0: 666f 7220 7120 696e 2073 716d 2e61 6374  for q in sqm.act
-000148c0: 6976 655d 0a20 2020 2020 2020 2060 6060  ive].        ```
-000148d0: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
-000148e0: 726e 696e 6720 2245 6e67 696e 6520 5375  rning "Engine Su
-000148f0: 7070 6f72 7422 0a20 2020 2020 2020 2020  pport".         
-00014900: 2020 202a 2a53 7061 726b 206f 6e6c 792a     **Spark only*
-00014910: 2a0a 0a20 2020 2020 2020 2020 2020 2053  *..            S
-00014920: 7472 6561 6d20 696e 6765 7374 696f 6e20  tream ingestion 
-00014930: 7573 696e 6720 5061 6e64 6173 2f50 7974  using Pandas/Pyt
-00014940: 686f 6e20 6173 2065 6e67 696e 6520 6973  hon as engine is
-00014950: 2063 7572 7265 6e74 6c79 206e 6f74 2073   currently not s
-00014960: 7570 706f 7274 6564 2e0a 2020 2020 2020  upported..      
-00014970: 2020 2020 2020 5079 7468 6f6e 2f50 616e        Python/Pan
-00014980: 6461 7320 6861 7320 6e6f 206e 6f74 696f  das has no notio
-00014990: 6e20 6f66 2073 7472 6561 6d69 6e67 2e0a  n of streaming..
-000149a0: 0a20 2020 2020 2020 2021 2121 2077 6172  .        !!! war
-000149b0: 6e69 6e67 2022 4461 7461 2056 616c 6964  ning "Data Valid
-000149c0: 6174 696f 6e20 5375 7070 6f72 7422 0a20  ation Support". 
-000149d0: 2020 2020 2020 2020 2020 2060 696e 7365             `inse
-000149e0: 7274 5f73 7472 6561 6d60 2064 6f65 7320  rt_stream` does 
-000149f0: 6e6f 7420 7065 7266 6f72 6d20 616e 7920  not perform any 
-00014a00: 6461 7461 2076 616c 6964 6174 696f 6e20  data validation 
-00014a10: 7573 696e 6720 4772 6561 7420 4578 7065  using Great Expe
-00014a20: 6374 6174 696f 6e73 0a20 2020 2020 2020  ctations.       
-00014a30: 2020 2020 2065 7665 6e20 7768 656e 2061       even when a
-00014a40: 2065 7870 6563 7461 7469 6f6e 2073 7569   expectation sui
-00014a50: 7465 2069 7320 6174 7461 6368 6564 2e0a  te is attached..
-00014a60: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-00014a70: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00014a80: 2066 6561 7475 7265 733a 2046 6561 7475   features: Featu
-00014a90: 7265 7320 696e 2053 7472 6561 6d69 6e67  res in Streaming
-00014aa0: 2044 6174 6166 7261 6d65 2074 6f20 6265   Dataframe to be
-00014ab0: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
-00014ac0: 2020 2020 7175 6572 795f 6e61 6d65 3a20      query_name: 
-00014ad0: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-00014ae0: 6f20 6f70 7469 6f6e 616c 6c79 2073 7065  o optionally spe
-00014af0: 6369 6679 2061 206e 616d 6520 666f 7220  cify a name for 
-00014b00: 7468 6520 7175 6572 7920 746f 0a20 2020  the query to.   
-00014b10: 2020 2020 2020 2020 2020 2020 206d 616b               mak
-00014b20: 6520 6974 2065 6173 6965 7220 746f 2072  e it easier to r
-00014b30: 6563 6f67 6e69 7365 2069 6e20 7468 6520  ecognise in the 
-00014b40: 5370 6172 6b20 5549 2e20 4465 6661 756c  Spark UI. Defaul
-00014b50: 7473 2074 6f20 604e 6f6e 6560 2e0a 2020  ts to `None`..  
-00014b60: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00014b70: 5f6d 6f64 653a 2053 7065 6369 6669 6573  _mode: Specifies
-00014b80: 2068 6f77 2064 6174 6120 6f66 2061 2073   how data of a s
-00014b90: 7472 6561 6d69 6e67 2044 6174 6146 7261  treaming DataFra
-00014ba0: 6d65 2f44 6174 6173 6574 2069 730a 2020  me/Dataset is.  
-00014bb0: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-00014bc0: 6974 7465 6e20 746f 2061 2073 7472 6561  itten to a strea
-00014bd0: 6d69 6e67 2073 696e 6b2e 2028 3129 2060  ming sink. (1) `
-00014be0: 2261 7070 656e 6422 603a 204f 6e6c 7920  "append"`: Only 
-00014bf0: 7468 6520 6e65 7720 726f 7773 2069 6e20  the new rows in 
-00014c00: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00014c10: 2020 2020 7374 7265 616d 696e 6720 4461      streaming Da
-00014c20: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
-00014c30: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-00014c40: 746f 2074 6865 2073 696e 6b2e 2028 3229  to the sink. (2)
-00014c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c60: 2060 2263 6f6d 706c 6574 6522 603a 2041   `"complete"`: A
-00014c70: 6c6c 2074 6865 2072 6f77 7320 696e 2074  ll the rows in t
-00014c80: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
-00014c90: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
-00014ca0: 696c 6c20 6265 0a20 2020 2020 2020 2020  ill be.         
-00014cb0: 2020 2020 2020 2077 7269 7474 656e 2074         written t
-00014cc0: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
-00014cd0: 2074 696d 6520 7468 6572 6520 6973 2073   time there is s
-00014ce0: 6f6d 6520 7570 6461 7465 2e20 2833 2920  ome update. (3) 
-00014cf0: 6022 7570 6461 7465 2260 3a0a 2020 2020  `"update"`:.    
-00014d00: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
-00014d10: 2074 6865 2072 6f77 7320 7468 6174 2077   the rows that w
-00014d20: 6572 6520 7570 6461 7465 6420 696e 2074  ere updated in t
-00014d30: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
-00014d40: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
-00014d50: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
-00014d60: 2020 2020 6265 2077 7269 7474 656e 2074      be written t
-00014d70: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
-00014d80: 2074 696d 6520 7468 6572 6520 6172 6520   time there are 
-00014d90: 736f 6d65 2075 7064 6174 6573 2e0a 2020  some updates..  
-00014da0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-00014db0: 2074 6865 2071 7565 7279 2064 6f65 736e   the query doesn
-00014dc0: e280 9974 2063 6f6e 7461 696e 2061 6767  ...t contain agg
-00014dd0: 7265 6761 7469 6f6e 732c 2069 7420 7769  regations, it wi
-00014de0: 6c6c 2062 6520 6571 7569 7661 6c65 6e74  ll be equivalent
-00014df0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00014e00: 2020 2020 6170 7065 6e64 206d 6f64 652e      append mode.
-00014e10: 2044 6566 6175 6c74 7320 746f 2060 2261   Defaults to `"a
-00014e20: 7070 656e 6422 602e 0a20 2020 2020 2020  ppend"`..       
-00014e30: 2020 2020 2061 7761 6974 5f74 6572 6d69       await_termi
-00014e40: 6e61 7469 6f6e 3a20 5761 6974 7320 666f  nation: Waits fo
-00014e50: 7220 7468 6520 7465 726d 696e 6174 696f  r the terminatio
-00014e60: 6e20 6f66 2074 6869 7320 7175 6572 792c  n of this query,
-00014e70: 2065 6974 6865 7220 6279 0a20 2020 2020   either by.     
-00014e80: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00014e90: 2e73 746f 7028 2920 6f72 2062 7920 616e  .stop() or by an
-00014ea0: 2065 7863 6570 7469 6f6e 2e20 4966 2074   exception. If t
-00014eb0: 6865 2071 7565 7279 2068 6173 2074 6572  he query has ter
-00014ec0: 6d69 6e61 7465 6420 7769 7468 2061 6e0a  minated with an.
-00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ee0: 6578 6365 7074 696f 6e2c 2074 6865 6e20  exception, then 
-00014ef0: 7468 6520 6578 6365 7074 696f 6e20 7769  the exception wi
-00014f00: 6c6c 2062 6520 7468 726f 776e 2e20 4966  ll be thrown. If
-00014f10: 2074 696d 656f 7574 2069 7320 7365 742c   timeout is set,
-00014f20: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
-00014f30: 2020 2020 7265 7475 726e 7320 7768 6574      returns whet
-00014f40: 6865 7220 7468 6520 7175 6572 7920 6861  her the query ha
-00014f50: 7320 7465 726d 696e 6174 6564 206f 7220  s terminated or 
-00014f60: 6e6f 7420 7769 7468 696e 2074 6865 2074  not within the t
-00014f70: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-00014f80: 2020 2020 2020 2073 6563 6f6e 6473 2e20         seconds. 
-00014f90: 4465 6661 756c 7473 2074 6f20 6046 616c  Defaults to `Fal
-00014fa0: 7365 602e 0a20 2020 2020 2020 2020 2020  se`..           
-00014fb0: 2074 696d 656f 7574 3a20 4f6e 6c79 2072   timeout: Only r
-00014fc0: 656c 6576 616e 7420 696e 2063 6f6d 6269  elevant in combi
-00014fd0: 6e61 7469 6f6e 2077 6974 6820 6061 7761  nation with `awa
-00014fe0: 6974 5f74 6572 6d69 6e61 7469 6f6e 3d54  it_termination=T
-00014ff0: 7275 6560 2e0a 2020 2020 2020 2020 2020  rue`..          
-00015000: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00015010: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
-00015020: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
-00015030: 5f64 6972 3a20 4368 6563 6b70 6f69 6e74  _dir: Checkpoint
-00015040: 2064 6972 6563 746f 7279 206c 6f63 6174   directory locat
-00015050: 696f 6e2e 2054 6869 7320 7769 6c6c 2062  ion. This will b
-00015060: 6520 7573 6564 2074 6f20 6173 2061 2072  e used to as a r
-00015070: 6566 6572 656e 6365 2074 6f0a 2020 2020  eference to.    
-00015080: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00015090: 2077 6865 7265 2074 6f20 7265 7375 6d65   where to resume
-000150a0: 2074 6865 2073 7472 6561 6d69 6e67 206a   the streaming j
-000150b0: 6f62 2e20 4966 2060 4e6f 6e65 6020 7468  ob. If `None` th
-000150c0: 656e 2068 7366 7320 7769 6c6c 2063 6f6e  en hsfs will con
-000150d0: 7374 7275 6374 2061 730a 2020 2020 2020  struct as.      
-000150e0: 2020 2020 2020 2020 2020 2269 6e73 6572            "inser
-000150f0: 745f 7374 7265 616d 5f22 202b 206f 6e6c  t_stream_" + onl
-00015100: 696e 655f 746f 7069 635f 6e61 6d65 2e20  ine_topic_name. 
-00015110: 4465 6661 756c 7473 2074 6f20 604e 6f6e  Defaults to `Non
-00015120: 6560 2e0a 2020 2020 2020 2020 2020 2020  e`..            
-00015130: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
-00015140: 733a 2041 6464 6974 696f 6e61 6c20 7772  s: Additional wr
-00015150: 6974 6520 6f70 7469 6f6e 7320 666f 7220  ite options for 
-00015160: 5370 6172 6b20 6173 206b 6579 2d76 616c  Spark as key-val
-00015170: 7565 2070 6169 7273 2e0a 2020 2020 2020  ue pairs..      
-00015180: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00015190: 7473 2074 6f20 607b 7d60 2e0a 0a20 2020  ts to `{}`...   
-000151a0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
-000151b0: 2020 2020 2020 2020 2020 2060 5374 7265             `Stre
-000151c0: 616d 696e 6751 7565 7279 603a 2053 7061  amingQuery`: Spa
-000151d0: 726b 2053 7472 7563 7475 7265 6420 5374  rk Structured St
-000151e0: 7265 616d 696e 6720 5175 6572 7920 6f62  reaming Query ob
-000151f0: 6a65 6374 2e0a 2020 2020 2020 2020 2222  ject..        ""
-00015200: 220a 2020 2020 2020 2020 6966 2028 0a20  ".        if (. 
-00015210: 2020 2020 2020 2020 2020 206e 6f74 2065             not e
-00015220: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
-00015230: 6365 2829 2e69 735f 7370 6172 6b5f 6461  ce().is_spark_da
-00015240: 7461 6672 616d 6528 6665 6174 7572 6573  taframe(features
-00015250: 290a 2020 2020 2020 2020 2020 2020 6f72  ).            or
-00015260: 206e 6f74 2066 6561 7475 7265 732e 6973   not features.is
-00015270: 5374 7265 616d 696e 670a 2020 2020 2020  Streaming.      
-00015280: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00015290: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000152a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000152b0: 2020 2246 6561 7475 7265 7320 6861 7665    "Features have
-000152c0: 2074 6f20 6265 2061 2073 7472 6561 6d69   to be a streami
-000152d0: 6e67 2074 7970 6520 7370 6172 6b20 6461  ng type spark da
-000152e0: 7461 6672 616d 652e 2055 7365 2060 696e  taframe. Use `in
-000152f0: 7365 7274 2829 6020 6d65 7468 6f64 2069  sert()` method i
-00015300: 6e73 7465 6164 2e22 0a20 2020 2020 2020  nstead.".       
-00015310: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00015320: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015330: 2023 206c 6f77 6572 2063 6173 696e 6720   # lower casing 
-00015340: 6665 6174 7572 6520 6e61 6d65 730a 2020  feature names.  
-00015350: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00015360: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
-00015370: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
-00015380: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
-00015390: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
-000153a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000153b0: 2020 6665 6174 7572 6573 0a20 2020 2020    features.     
-000153c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000153d0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-000153e0: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
-000153f0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00015400: 2020 2020 2020 2020 2020 2253 7472 6561            "Strea
-00015410: 6d20 696e 6765 7374 696f 6e20 666f 7220  m ingestion for 
-00015420: 6665 6174 7572 6520 6772 6f75 7020 607b  feature group `{
-00015430: 7d60 2c20 7769 7468 2076 6572 7369 6f6e  }`, with version
-00015440: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00015450: 2020 2020 2020 2220 607b 7d60 2077 696c        " `{}` wil
-00015460: 6c20 6e6f 7420 636f 6d70 7574 6520 7374  l not compute st
-00015470: 6174 6973 7469 6373 2e22 0a20 2020 2020  atistics.".     
-00015480: 2020 2020 2020 2020 2020 2029 2e66 6f72             ).for
-00015490: 6d61 7428 7365 6c66 2e5f 6e61 6d65 2c20  mat(self._name, 
-000154a0: 7365 6c66 2e5f 7665 7273 696f 6e29 2c0a  self._version),.
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154c0: 7574 696c 2e53 7461 7469 7374 6963 7357  util.StatisticsW
-000154d0: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-000154e0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-000154f0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00015500: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-00015510: 6769 6e65 2e69 6e73 6572 745f 7374 7265  gine.insert_stre
-00015520: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-00015530: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00015540: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00015550: 655f 6461 7461 6672 616d 652c 0a20 2020  e_dataframe,.   
-00015560: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00015570: 7279 5f6e 616d 652c 0a20 2020 2020 2020  ry_name,.       
-00015580: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00015590: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
-000155a0: 2020 2020 2020 6177 6169 745f 7465 726d        await_term
-000155b0: 696e 6174 696f 6e2c 0a20 2020 2020 2020  ination,.       
-000155c0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-000155d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000155e0: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
-000155f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015600: 2020 7772 6974 655f 6f70 7469 6f6e 732c    write_options,
-00015610: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00015620: 2020 2020 6465 6620 636f 6d6d 6974 5f64      def commit_d
-00015630: 6574 6169 6c73 280a 2020 2020 2020 2020  etails(.        
-00015640: 7365 6c66 2c0a 2020 2020 2020 2020 7761  self,.        wa
-00015650: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
-00015660: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-00015670: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
-00015680: 2064 6174 655d 5d20 3d20 4e6f 6e65 2c0a   date]] = None,.
-00015690: 2020 2020 2020 2020 6c69 6d69 743a 204f          limit: O
-000156a0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000156b0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000156c0: 2020 2020 2222 2252 6574 7269 6576 6573      """Retrieves
-000156d0: 2063 6f6d 6d69 7420 7469 6d65 6c69 6e65   commit timeline
-000156e0: 2066 6f72 2074 6869 7320 6665 6174 7572   for this featur
-000156f0: 6520 6772 6f75 702e 2054 6869 7320 6d65  e group. This me
-00015700: 7468 6f64 2063 616e 206f 6e6c 7920 6265  thod can only be
-00015710: 2075 7365 640a 2020 2020 2020 2020 6f6e   used.        on
-00015720: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
-00015730: 626c 6564 2066 6561 7475 7265 2067 726f  bled feature gro
-00015740: 7570 730a 0a20 2020 2020 2020 2021 2121  ups..        !!!
-00015750: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-00015760: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00015770: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00015780: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
-00015790: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
-000157a0: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
-000157b0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-000157c0: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
-000157d0: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
-000157e0: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
-000157f0: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-00015800: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
-00015810: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
-00015820: 6f6d 6d69 745f 6465 7461 696c 7320 3d20  ommit_details = 
-00015830: 6667 2e63 6f6d 6d69 745f 6465 7461 696c  fg.commit_detail
-00015840: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00015850: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
-00015860: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-00015870: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
-00015880: 696d 653a 2043 6f6d 6d69 7420 6465 7461  ime: Commit deta
-00015890: 696c 7320 6173 206f 6620 7370 6563 6966  ils as of specif
-000158a0: 6963 2070 6f69 6e74 2069 6e20 7469 6d65  ic point in time
-000158b0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
-000158c0: 6f6e 6560 2e0a 2020 2020 2020 2020 2020  one`..          
-000158d0: 2020 2020 2020 2053 7472 696e 6773 2073         Strings s
-000158e0: 686f 756c 6420 6265 2066 6f72 6d61 7474  hould be formatt
-000158f0: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-00015900: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-00015910: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-00015920: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-00015930: 592d 256d 2d25 6420 2548 3a25 4d60 2c0a  Y-%m-%d %H:%M`,.
-00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015950: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-00015960: 2553 602c 206f 7220 6025 592d 256d 2d25  %S`, or `%Y-%m-%
-00015970: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-00015980: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00015990: 743a 204e 756d 6265 7220 6f66 2063 6f6d  t: Number of com
-000159a0: 6d69 7473 2074 6f20 7265 7472 6965 7665  mits to retrieve
-000159b0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
-000159c0: 6f6e 6560 2e0a 0a20 2020 2020 2020 2023  one`...        #
-000159d0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-000159e0: 2020 2020 2060 4469 6374 5b73 7472 2c20       `Dict[str, 
-000159f0: 4469 6374 5b73 7472 2c20 7374 725d 5d60  Dict[str, str]]`
-00015a00: 2e20 4469 6374 696f 6e61 7279 206f 626a  . Dictionary obj
-00015a10: 6563 7420 6f66 2063 6f6d 6d69 7420 6d65  ect of commit me
-00015a20: 7461 6461 7461 2074 696d 656c 696e 652c  tadata timeline,
-00015a30: 2077 6865 7265 204b 6579 2069 7320 636f   where Key is co
-00015a40: 6d6d 6974 2069 6420 616e 6420 7661 6c75  mmit id and valu
-00015a50: 650a 2020 2020 2020 2020 2020 2020 6973  e.            is
-00015a60: 2060 4469 6374 5b73 7472 2c20 7374 725d   `Dict[str, str]
-00015a70: 6020 7769 7468 206b 6579 2076 616c 7565  ` with key value
-00015a80: 2070 6169 7273 206f 6620 6461 7465 2063   pairs of date c
-00015a90: 6f6d 6d69 7474 6564 206f 6e2c 206e 756d  ommitted on, num
-00015aa0: 6265 7220 6f66 2072 6f77 7320 7570 6461  ber of rows upda
-00015ab0: 7465 642c 2069 6e73 6572 7465 6420 616e  ted, inserted an
-00015ac0: 6420 6465 6c65 7465 642e 0a0a 2020 2020  d deleted...    
-00015ad0: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-00015ae0: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-00015af0: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-00015b00: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
-00015b10: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
-00015b20: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
-00015b30: 6f6e 732e 4665 6174 7572 6553 746f 7265  ons.FeatureStore
-00015b40: 4578 6365 7074 696f 6e60 2e20 4966 2074  Exception`. If t
-00015b50: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00015b60: 2064 6f65 7320 6e6f 7420 6861 7665 2060   does not have `
-00015b70: 4855 4449 6020 7469 6d65 2074 7261 7665  HUDI` time trave
-00015b80: 6c20 666f 726d 6174 0a20 2020 2020 2020  l format.       
-00015b90: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00015ba0: 7572 6e20 7365 6c66 2e5f 6665 6174 7572  urn self._featur
-00015bb0: 655f 6772 6f75 705f 656e 6769 6e65 2e63  e_group_engine.c
-00015bc0: 6f6d 6d69 745f 6465 7461 696c 7328 7365  ommit_details(se
-00015bd0: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
-00015be0: 6d65 2c20 6c69 6d69 7429 0a0a 2020 2020  me, limit)..    
-00015bf0: 6465 6620 636f 6d6d 6974 5f64 656c 6574  def commit_delet
-00015c00: 655f 7265 636f 7264 280a 2020 2020 2020  e_record(.      
-00015c10: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00015c20: 6465 6c65 7465 5f64 663a 2054 7970 6556  delete_df: TypeV
-00015c30: 6172 2822 7079 7370 6172 6b2e 7371 6c2e  ar("pyspark.sql.
-00015c40: 4461 7461 4672 616d 6522 292c 2020 2320  DataFrame"),  # 
-00015c50: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-00015c60: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
-00015c70: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00015c80: 416e 792c 2041 6e79 5d5d 203d 207b 7d2c  Any, Any]] = {},
-00015c90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00015ca0: 2222 2244 726f 7073 2072 6563 6f72 6473  """Drops records
-00015cb0: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
-00015cc0: 7072 6f76 6964 6564 2044 6174 6146 7261  provided DataFra
-00015cd0: 6d65 2061 6e64 2063 6f6d 6d69 7473 2069  me and commits i
-00015ce0: 7420 6173 2075 7064 6174 6520 746f 2074  t as update to t
-00015cf0: 6869 730a 2020 2020 2020 2020 4665 6174  his.        Feat
-00015d00: 7572 6520 6772 6f75 702e 2054 6869 7320  ure group. This 
-00015d10: 6d65 7468 6f64 2063 616e 206f 6e6c 7920  method can only 
-00015d20: 6265 2075 7365 6420 6f6e 2074 696d 6520  be used on time 
-00015d30: 7472 6176 656c 2065 6e61 626c 6564 2066  travel enabled f
-00015d40: 6561 7475 7265 2067 726f 7570 732e 0a0a  eature groups...
-00015d50: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-00015d60: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00015d70: 6465 6c65 7465 5f64 663a 2064 6174 6146  delete_df: dataF
-00015d80: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
-00015d90: 7265 636f 7264 7320 746f 2062 6520 6465  records to be de
-00015da0: 6c65 7465 642e 0a20 2020 2020 2020 2020  leted..         
-00015db0: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
-00015dc0: 3a20 5573 6572 2070 726f 7669 6465 6420  : User provided 
-00015dd0: 7772 6974 6520 6f70 7469 6f6e 732e 2044  write options. D
-00015de0: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
-00015df0: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
-00015e00: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
-00015e10: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
-00015e20: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
-00015e30: 726f 7260 2e0a 2020 2020 2020 2020 2222  ror`..        ""
-00015e40: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
-00015e50: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-00015e60: 6769 6e65 2e63 6f6d 6d69 745f 6465 6c65  gine.commit_dele
-00015e70: 7465 2873 656c 662c 2064 656c 6574 655f  te(self, delete_
-00015e80: 6466 2c20 7772 6974 655f 6f70 7469 6f6e  df, write_option
-00015e90: 7329 0a0a 2020 2020 6465 6620 6173 5f6f  s)..    def as_o
-00015ea0: 6628 0a20 2020 2020 2020 2073 656c 662c  f(.        self,
-00015eb0: 0a20 2020 2020 2020 2077 616c 6c63 6c6f  .        wallclo
-00015ec0: 636b 5f74 696d 653a 204f 7074 696f 6e61  ck_time: Optiona
-00015ed0: 6c5b 556e 696f 6e5b 7374 722c 2069 6e74  l[Union[str, int
-00015ee0: 2c20 6461 7465 7469 6d65 2c20 6461 7465  , datetime, date
-00015ef0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00015f00: 2020 2065 7863 6c75 6465 5f75 6e74 696c     exclude_until
-00015f10: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-00015f20: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
-00015f30: 696d 652c 2064 6174 655d 5d20 3d20 4e6f  ime, date]] = No
-00015f40: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00015f50: 2020 2022 2222 4765 7420 5175 6572 7920     """Get Query 
-00015f60: 6f62 6a65 6374 2074 6f20 7265 7472 6965  object to retrie
-00015f70: 7665 2061 6c6c 2066 6561 7475 7265 7320  ve all features 
-00015f80: 6f66 2074 6865 2067 726f 7570 2061 7420  of the group at 
-00015f90: 6120 706f 696e 7420 696e 2074 6865 2070  a point in the p
-00015fa0: 6173 742e 0a0a 2020 2020 2020 2020 5468  ast...        Th
-00015fb0: 6973 206d 6574 686f 6420 7365 6c65 6374  is method select
-00015fc0: 7320 616c 6c20 6665 6174 7572 6573 2069  s all features i
-00015fd0: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
-00015fe0: 6f75 7020 616e 6420 7265 7475 726e 7320  oup and returns 
-00015ff0: 6120 5175 6572 7920 6f62 6a65 6374 0a20  a Query object. 
-00016000: 2020 2020 2020 2061 7420 7468 6520 7370         at the sp
-00016010: 6563 6966 6965 6420 706f 696e 7420 696e  ecified point in
-00016020: 2074 696d 652e 204f 7074 696f 6e61 6c6c   time. Optionall
-00016030: 792c 2063 6f6d 6d69 7473 2062 6566 6f72  y, commits befor
-00016040: 6520 6120 7370 6563 6966 6965 6420 706f  e a specified po
-00016050: 696e 7420 696e 2074 696d 6520 6361 6e20  int in time can 
-00016060: 6265 0a20 2020 2020 2020 2065 7863 6c75  be.        exclu
-00016070: 6465 6420 6672 6f6d 2074 6865 2071 7565  ded from the que
-00016080: 7279 2e20 5468 6520 5175 6572 7920 6361  ry. The Query ca
-00016090: 6e20 7468 656e 2065 6974 6865 7220 6265  n then either be
-000160a0: 2072 6561 6420 696e 746f 2061 2044 6174   read into a Dat
-000160b0: 6166 7261 6d65 0a20 2020 2020 2020 206f  aframe.        o
-000160c0: 7220 7573 6564 2066 7572 7468 6572 2074  r used further t
-000160d0: 6f20 7065 7266 6f72 6d20 6a6f 696e 7320  o perform joins 
-000160e0: 6f72 2063 6f6e 7374 7275 6374 2061 2074  or construct a t
-000160f0: 7261 696e 696e 6720 6461 7461 7365 742e  raining dataset.
-00016100: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
-00016110: 616d 706c 6520 2252 6561 6469 6e67 2066  ample "Reading f
-00016120: 6561 7475 7265 7320 6174 2061 2073 7065  eatures at a spe
-00016130: 6369 6669 6320 706f 696e 7420 696e 2074  cific point in t
-00016140: 696d 653a 220a 2020 2020 2020 2020 2020  ime:".          
-00016150: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00016160: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
-00016170: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
-00016180: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
-00016190: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
-000161a0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-000161b0: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-000161c0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
-000161d0: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
-000161e0: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-000161f0: 7572 655f 6772 6f75 7028 2e2e 2e29 0a0a  ure_group(...)..
-00016200: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00016210: 7420 6461 7461 2061 7420 6120 7370 6563  t data at a spec
-00016220: 6966 6963 2070 6f69 6e74 2069 6e20 7469  ific point in ti
-00016230: 6d65 2061 6e64 2073 686f 7720 6974 0a20  me and show it. 
-00016240: 2020 2020 2020 2020 2020 2066 672e 6173             fg.as
-00016250: 5f6f 6628 2232 3032 302d 3130 2d32 3020  _of("2020-10-20 
-00016260: 3037 3a33 343a 3131 2229 2e72 6561 6428  07:34:11").read(
-00016270: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
-00016280: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00016290: 2020 2121 2120 6578 616d 706c 6520 2252    !!! example "R
-000162a0: 6561 6469 6e67 2063 6f6d 6d69 7473 2069  eading commits i
-000162b0: 6e63 7265 6d65 6e74 616c 6c79 2062 6574  ncrementally bet
-000162c0: 7765 656e 2073 7065 6369 6669 6564 2070  ween specified p
-000162d0: 6f69 6e74 7320 696e 2074 696d 653a 220a  oints in time:".
-000162e0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-000162f0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-00016300: 2020 6667 2e61 735f 6f66 2822 3230 3230    fg.as_of("2020
-00016310: 2d31 302d 3230 2030 373a 3334 3a31 3122  -10-20 07:34:11"
-00016320: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
-00016330: 2232 3032 302d 3130 2d31 3920 3037 3a33  "2020-10-19 07:3
-00016340: 343a 3131 2229 2e72 6561 6428 292e 7368  4:11").read().sh
-00016350: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
-00016360: 2060 6060 0a0a 2020 2020 2020 2020 5468   ```..        Th
-00016370: 6520 6669 7273 7420 7061 7261 6d65 7465  e first paramete
-00016380: 7220 6973 2069 6e63 6c75 7369 7665 2077  r is inclusive w
-00016390: 6869 6c65 2074 6865 206c 6174 7465 7220  hile the latter 
-000163a0: 6973 2065 7863 6c75 7369 7665 2e0a 2020  is exclusive..  
-000163b0: 2020 2020 2020 5468 6174 206d 6561 6e73        That means
-000163c0: 2c20 696e 206f 7264 6572 2074 6f20 7175  , in order to qu
-000163d0: 6572 7920 6120 7369 6e67 6c65 2063 6f6d  ery a single com
-000163e0: 6d69 742c 2079 6f75 206e 6565 6420 746f  mit, you need to
-000163f0: 2071 7565 7279 2074 6861 7420 636f 6d6d   query that comm
-00016400: 6974 2074 696d 650a 2020 2020 2020 2020  it time.        
-00016410: 616e 6420 6578 636c 7564 6520 6576 6572  and exclude ever
-00016420: 7974 6869 6e67 206a 7573 7420 6265 666f  ything just befo
-00016430: 7265 2074 6865 2063 6f6d 6d69 742e 0a0a  re the commit...
-00016440: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-00016450: 706c 6520 2252 6561 6469 6e67 206f 6e6c  ple "Reading onl
-00016460: 7920 7468 6520 6368 616e 6765 7320 6672  y the changes fr
-00016470: 6f6d 2061 2073 696e 676c 6520 636f 6d6d  om a single comm
-00016480: 6974 220a 2020 2020 2020 2020 2020 2020  it".            
-00016490: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000164a0: 2020 2020 2020 6667 2e61 735f 6f66 2822        fg.as_of("
-000164b0: 3230 3230 2d31 302d 3230 2030 373a 3331  2020-10-20 07:31
-000164c0: 3a33 3822 2c20 6578 636c 7564 655f 756e  :38", exclude_un
-000164d0: 7469 6c3d 2232 3032 302d 3130 2d32 3020  til="2020-10-20 
-000164e0: 3037 3a33 313a 3337 2229 2e72 6561 6428  07:31:37").read(
-000164f0: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
-00016500: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00016510: 2020 5768 656e 206e 6f20 7761 6c6c 636c    When no wallcl
-00016520: 6f63 6b5f 7469 6d65 2069 7320 6769 7665  ock_time is give
-00016530: 6e2c 2074 6865 206c 6174 6573 7420 7374  n, the latest st
-00016540: 6174 6520 6f66 2066 6561 7475 7265 7320  ate of features 
-00016550: 6973 2072 6574 7572 6e65 642e 204f 7074  is returned. Opt
-00016560: 696f 6e61 6c6c 792c 2063 6f6d 6d69 7473  ionally, commits
-00016570: 2062 6566 6f72 650a 2020 2020 2020 2020   before.        
-00016580: 6120 7370 6563 6966 6965 6420 706f 696e  a specified poin
-00016590: 7420 696e 2074 696d 6520 6361 6e20 7374  t in time can st
-000165a0: 696c 6c20 6265 2065 7863 6c75 6465 642e  ill be excluded.
-000165b0: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
-000165c0: 616d 706c 6520 2252 6561 6469 6e67 2074  ample "Reading t
-000165d0: 6865 206c 6174 6573 7420 7374 6174 6520  he latest state 
-000165e0: 6f66 2066 6561 7475 7265 732c 2065 7863  of features, exc
-000165f0: 6c75 6469 6e67 2063 6f6d 6d69 7473 2062  luding commits b
-00016600: 6566 6f72 6520 6120 7370 6563 6966 6965  efore a specifie
-00016610: 6420 706f 696e 7420 696e 2074 696d 653a  d point in time:
-00016620: 220a 2020 2020 2020 2020 2020 2020 6060  ".            ``
-00016630: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00016640: 2020 2020 6667 2e61 735f 6f66 284e 6f6e      fg.as_of(Non
-00016650: 652c 2065 7863 6c75 6465 5f75 6e74 696c  e, exclude_until
-00016660: 3d22 3230 3230 2d31 302d 3230 2030 373a  ="2020-10-20 07:
-00016670: 3331 3a33 3822 292e 7265 6164 2829 2e73  31:38").read().s
-00016680: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
-00016690: 2020 6060 600a 0a20 2020 2020 2020 204e    ```..        N
-000166a0: 6f74 6520 7468 6174 2074 6865 2069 6e74  ote that the int
-000166b0: 6572 7661 6c20 7769 6c6c 2062 6520 6170  erval will be ap
-000166c0: 706c 6965 6420 746f 2061 6c6c 206a 6f69  plied to all joi
-000166d0: 6e73 2069 6e20 7468 6520 7175 6572 792e  ns in the query.
-000166e0: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
-000166f0: 7761 6e74 2074 6f20 7175 6572 7920 6469  want to query di
-00016700: 6666 6572 656e 7420 696e 7465 7276 616c  fferent interval
-00016710: 7320 666f 7220 6469 6666 6572 656e 7420  s for different 
-00016720: 6665 6174 7572 6520 6772 6f75 7073 2069  feature groups i
-00016730: 6e0a 2020 2020 2020 2020 7468 6520 7175  n.        the qu
-00016740: 6572 792c 2079 6f75 2068 6176 6520 746f  ery, you have to
-00016750: 2061 7070 6c79 2074 6865 6d20 696e 2061   apply them in a
-00016760: 206e 6573 7465 6420 6661 7368 696f 6e3a   nested fashion:
-00016770: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00016780: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00016790: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-000167a0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-000167b0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-000167c0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-000167d0: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-000167e0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-000167f0: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-00016800: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00016810: 2020 2020 2066 6731 203d 2066 732e 6765       fg1 = fs.ge
-00016820: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-00016830: 7572 655f 6772 6f75 7028 2e2e 2e29 0a20  ure_group(...). 
-00016840: 2020 2020 2020 2020 2020 2066 6732 203d             fg2 =
-00016850: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00016860: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00016870: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00016880: 2020 6667 312e 7365 6c65 6374 5f61 6c6c    fg1.select_all
-00016890: 2829 2e61 735f 6f66 2822 3230 3230 2d31  ().as_of("2020-1
-000168a0: 302d 3230 222c 2065 7863 6c75 6465 5f75  0-20", exclude_u
-000168b0: 6e74 696c 3d22 3230 3230 2d31 302d 3139  ntil="2020-10-19
-000168c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000168d0: 2020 202e 6a6f 696e 2866 6732 2e73 656c     .join(fg2.sel
-000168e0: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
-000168f0: 2232 3032 302d 3130 2d32 3022 2c20 6578  "2020-10-20", ex
-00016900: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
-00016910: 302d 3130 2d31 3922 2929 0a20 2020 2020  0-10-19")).     
-00016920: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-00016930: 2020 2020 4966 2069 6e73 7465 6164 2079      If instead y
-00016940: 6f75 2061 7070 6c79 2061 6e6f 7468 6572  ou apply another
-00016950: 2060 6173 5f6f 6660 2073 656c 6563 7469   `as_of` selecti
-00016960: 6f6e 2061 6674 6572 2074 6865 206a 6f69  on after the joi
-00016970: 6e2c 2061 6c6c 0a20 2020 2020 2020 206a  n, all.        j
-00016980: 6f69 6e65 6420 6665 6174 7572 6520 6772  oined feature gr
-00016990: 6f75 7073 2077 696c 6c20 6265 2071 7565  oups will be que
-000169a0: 7269 6564 2077 6974 6820 7468 6973 2069  ried with this i
-000169b0: 6e74 6572 7661 6c3a 0a20 2020 2020 2020  nterval:.       
-000169c0: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
-000169d0: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
-000169e0: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
-000169f0: 6731 2e73 656c 6563 745f 616c 6c28 292e  g1.select_all().
-00016a00: 6173 5f6f 6628 2232 3032 302d 3130 2d32  as_of("2020-10-2
-00016a10: 3022 2c20 6578 636c 7564 655f 756e 7469  0", exclude_unti
-00016a20: 6c3d 2232 3032 302d 3130 2d31 3922 2920  l="2020-10-19") 
-00016a30: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
-00016a40: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
-00016a50: 2020 2020 2020 2020 2e6a 6f69 6e28 6667          .join(fg
-00016a60: 322e 7365 6c65 6374 5f61 6c6c 2829 2e61  2.select_all().a
-00016a70: 735f 6f66 2822 3230 3230 2d31 302d 3230  s_of("2020-10-20
-00016a80: 222c 2065 7863 6c75 6465 5f75 6e74 696c  ", exclude_until
-00016a90: 3d22 3230 3230 2d31 302d 3135 2229 2920  ="2020-10-15")) 
-00016aa0: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
-00016ab0: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
-00016ac0: 2020 2020 2020 2020 2e61 735f 6f66 2822          .as_of("
-00016ad0: 3230 3230 2d31 302d 3230 222c 2065 7863  2020-10-20", exc
-00016ae0: 6c75 6465 5f75 6e74 696c 3d22 3230 3230  lude_until="2020
-00016af0: 2d31 302d 3139 2229 0a20 2020 2020 2020  -10-19").       
-00016b00: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00016b10: 2020 2121 2120 7761 726e 696e 670a 2020    !!! warning.  
-00016b20: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00016b30: 756e 6374 696f 6e20 6f6e 6c79 2077 6f72  unction only wor
-00016b40: 6b73 2066 6f72 2066 6561 7475 7265 2067  ks for feature g
-00016b50: 726f 7570 7320 7769 7468 2074 696d 655f  roups with time_
-00016b60: 7472 6176 656c 5f66 6f72 6d61 743d 2748  travel_format='H
-00016b70: 5544 4927 2e0a 0a20 2020 2020 2020 2021  UDI'...        !
-00016b80: 2121 2077 6172 6e69 6e67 0a20 2020 2020  !! warning.     
-00016b90: 2020 2020 2020 2045 7863 6c75 6469 6e67         Excluding
-00016ba0: 2063 6f6d 6d69 7473 2076 6961 2065 7863   commits via exc
-00016bb0: 6c75 6465 5f75 6e74 696c 2069 7320 6f6e  lude_until is on
-00016bc0: 6c79 2070 6f73 7369 626c 6520 7769 7468  ly possible with
-00016bd0: 696e 2074 6865 2072 616e 6765 206f 6620  in the range of 
-00016be0: 7468 6520 4875 6469 2061 6374 6976 6520  the Hudi active 
-00016bf0: 7469 6d65 6c69 6e65 2e0a 2020 2020 2020  timeline..      
-00016c00: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
-00016c10: 2c20 4875 6469 206b 6565 7073 2074 6865  , Hudi keeps the
-00016c20: 206c 6173 7420 3230 2074 6f20 3330 2063   last 20 to 30 c
-00016c30: 6f6d 6d69 7473 2069 6e20 7468 6520 6163  ommits in the ac
-00016c40: 7469 7665 2074 696d 656c 696e 652e 0a20  tive timeline.. 
-00016c50: 2020 2020 2020 2020 2020 2049 6620 796f             If yo
-00016c60: 7520 6e65 6564 2074 6f20 6b65 6570 2061  u need to keep a
-00016c70: 206c 6f6e 6765 7220 6163 7469 7665 2074   longer active t
-00016c80: 696d 656c 696e 652c 2079 6f75 2063 616e  imeline, you can
-00016c90: 206f 7665 7277 7269 7465 2074 6865 206f   overwrite the o
-00016ca0: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-00016cb0: 2020 2020 6068 6f6f 6469 652e 6b65 6570      `hoodie.keep
-00016cc0: 2e6d 696e 2e63 6f6d 6d69 7473 6020 616e  .min.commits` an
-00016cd0: 6420 6068 6f6f 6469 652e 6b65 6570 2e6d  d `hoodie.keep.m
-00016ce0: 6178 2e63 6f6d 6d69 7473 600a 2020 2020  ax.commits`.    
-00016cf0: 2020 2020 2020 2020 7768 656e 2063 616c          when cal
-00016d00: 6c69 6e67 2074 6865 2060 696e 7365 7274  ling the `insert
-00016d10: 2829 6020 6d65 7468 6f64 2e0a 0a20 2020  ()` method...   
-00016d20: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00016d30: 0a20 2020 2020 2020 2020 2020 2077 616c  .            wal
-00016d40: 6c63 6c6f 636b 5f74 696d 653a 2052 6561  lclock_time: Rea
-00016d50: 6420 6461 7461 2061 7320 6f66 2074 6869  d data as of thi
-00016d60: 7320 706f 696e 7420 696e 2074 696d 652e  s point in time.
-00016d70: 2053 7472 696e 6773 2073 686f 756c 6420   Strings should 
-00016d80: 6265 2066 6f72 6d61 7474 6564 2069 6e20  be formatted in 
-00016d90: 6f6e 6520 6f66 2074 6865 0a20 2020 2020  one of the.     
-00016da0: 2020 2020 2020 2020 2020 2066 6f6c 6c6f             follo
-00016db0: 7769 6e67 2066 6f72 6d61 7473 2060 2559  wing formats `%Y
-00016dc0: 2d25 6d2d 2564 602c 2060 2559 2d25 6d2d  -%m-%d`, `%Y-%m-
-00016dd0: 2564 2025 4860 2c20 6025 592d 256d 2d25  %d %H`, `%Y-%m-%
-00016de0: 6420 2548 3a25 4d60 2c20 6f72 2060 2559  d %H:%M`, or `%Y
-00016df0: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
-00016e00: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00016e10: 636c 7564 655f 756e 7469 6c3a 2045 7863  clude_until: Exc
-00016e20: 6c75 6465 2063 6f6d 6d69 7473 2075 6e74  lude commits unt
-00016e30: 696c 2074 6869 7320 706f 696e 7420 696e  il this point in
-00016e40: 2074 696d 652e 2053 7472 696e 6720 7368   time. String sh
-00016e50: 6f75 6c64 2062 6520 666f 726d 6174 7465  ould be formatte
-00016e60: 6420 696e 206f 6e65 206f 6620 7468 650a  d in one of the.
-00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e80: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
-00016e90: 7320 6025 592d 256d 2d25 6460 2c20 6025  s `%Y-%m-%d`, `%
-00016ea0: 592d 256d 2d25 6420 2548 602c 2060 2559  Y-%m-%d %H`, `%Y
-00016eb0: 2d25 6d2d 2564 2025 483a 254d 602c 206f  -%m-%d %H:%M`, o
-00016ec0: 7220 6025 592d 256d 2d25 6420 2548 3a25  r `%Y-%m-%d %H:%
-00016ed0: 4d3a 2553 602e 0a0a 2020 2020 2020 2020  M:%S`...        
-00016ee0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-00016ef0: 2020 2020 2020 6051 7565 7279 602e 2054        `Query`. T
-00016f00: 6865 2071 7565 7279 206f 626a 6563 7420  he query object 
-00016f10: 7769 7468 2074 6865 2061 7070 6c69 6564  with the applied
-00016f20: 2074 696d 6520 7472 6176 656c 2063 6f6e   time travel con
-00016f30: 6469 7469 6f6e 2e0a 2020 2020 2020 2020  dition..        
-00016f40: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00016f50: 726e 2073 656c 662e 7365 6c65 6374 5f61  rn self.select_a
-00016f60: 6c6c 2829 2e61 735f 6f66 2877 616c 6c63  ll().as_of(wallc
-00016f70: 6c6f 636b 5f74 696d 652c 2065 7863 6c75  lock_time, exclu
-00016f80: 6465 5f75 6e74 696c 290a 0a20 2020 2064  de_until)..    d
-00016f90: 6566 2063 6f6d 7075 7465 5f73 7461 7469  ef compute_stati
-00016fa0: 7374 6963 7328 0a20 2020 2020 2020 2073  stics(.        s
-00016fb0: 656c 662c 2077 616c 6c63 6c6f 636b 5f74  elf, wallclock_t
-00016fc0: 696d 653a 204f 7074 696f 6e61 6c5b 556e  ime: Optional[Un
-00016fd0: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
-00016fe0: 7465 7469 6d65 2c20 6461 7465 5d5d 203d  tetime, date]] =
-00016ff0: 204e 6f6e 650a 2020 2020 293a 0a20 2020   None.    ):.   
-00017000: 2020 2020 2022 2222 5265 636f 6d70 7574       """Recomput
-00017010: 6520 7468 6520 7374 6174 6973 7469 6373  e the statistics
-00017020: 2066 6f72 2074 6865 2066 6561 7475 7265   for the feature
-00017030: 2067 726f 7570 2061 6e64 2073 6176 6520   group and save 
-00017040: 7468 656d 2074 6f20 7468 650a 2020 2020  them to the.    
-00017050: 2020 2020 6665 6174 7572 6520 7374 6f72      feature stor
-00017060: 652e 0a0a 2020 2020 2020 2020 5374 6174  e...        Stat
-00017070: 6973 7469 6373 2061 7265 206f 6e6c 7920  istics are only 
-00017080: 636f 6d70 7574 6564 2066 6f72 2064 6174  computed for dat
-00017090: 6120 696e 2074 6865 206f 6666 6c69 6e65  a in the offline
-000170a0: 2073 746f 7261 6765 206f 6620 7468 6520   storage of the 
-000170b0: 6665 6174 7572 650a 2020 2020 2020 2020  feature.        
-000170c0: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
-000170d0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-000170e0: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
-000170f0: 6b5f 7469 6d65 3a20 4966 2073 7065 6369  k_time: If speci
-00017100: 6669 6564 2077 696c 6c20 7265 636f 6d70  fied will recomp
-00017110: 7574 6520 7374 6174 6973 7469 6373 206f  ute statistics o
-00017120: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00017130: 2020 6665 6174 7572 6520 6772 6f75 7020    feature group 
-00017140: 6173 206f 6620 7370 6563 6966 6963 2070  as of specific p
-00017150: 6f69 6e74 2069 6e20 7469 6d65 2e20 4966  oint in time. If
-00017160: 206e 6f74 2073 7065 6369 6669 6564 2074   not specified t
-00017170: 6865 6e20 7769 6c6c 2063 6f6d 7075 7465  hen will compute
-00017180: 2073 7461 7469 7374 6963 730a 2020 2020   statistics.    
-00017190: 2020 2020 2020 2020 2020 2020 6173 206f              as o
-000171a0: 6620 6d6f 7374 2072 6563 656e 7420 7469  f most recent ti
-000171b0: 6d65 206f 6620 7468 6973 2066 6561 7475  me of this featu
-000171c0: 7265 2067 726f 7570 2e20 4465 6661 756c  re group. Defaul
-000171d0: 7473 2074 6f20 604e 6f6e 6560 2e20 5374  ts to `None`. St
-000171e0: 7269 6e67 7320 7368 6f75 6c64 0a20 2020  rings should.   
-000171f0: 2020 2020 2020 2020 2020 2020 2062 6520               be 
-00017200: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
-00017210: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00017220: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
-00017230: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
-00017240: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
-00017250: 483a 254d 602c 2060 2559 2d25 6d2d 2564  H:%M`, `%Y-%m-%d
-00017260: 2025 483a 254d 3a25 5360 2c0a 2020 2020   %H:%M:%S`,.    
-00017270: 2020 2020 2020 2020 2020 2020 6f72 2060              or `
-00017280: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-00017290: 532e 2566 602e 0a0a 2020 2020 2020 2020  S.%f`...        
-000172a0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-000172b0: 2020 2020 2020 6053 7461 7469 7374 6963        `Statistic
-000172c0: 7360 2e20 5468 6520 7374 6174 6973 7469  s`. The statisti
-000172d0: 6373 206d 6574 6164 6174 6120 6f62 6a65  cs metadata obje
-000172e0: 6374 2e0a 0a20 2020 2020 2020 2023 2052  ct...        # R
-000172f0: 6169 7365 730a 2020 2020 2020 2020 2020  aises.          
-00017300: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
-00017310: 7863 6570 7469 6f6e 732e 5265 7374 4150  xceptions.RestAP
-00017320: 4945 7272 6f72 602e 2055 6e61 626c 6520  IError`. Unable 
-00017330: 746f 2070 6572 7369 7374 2074 6865 2073  to persist the s
-00017340: 7461 7469 7374 6963 732e 0a20 2020 2020  tatistics..     
-00017350: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00017360: 6620 7365 6c66 2e73 7461 7469 7374 6963  f self.statistic
-00017370: 735f 636f 6e66 6967 2e65 6e61 626c 6564  s_config.enabled
-00017380: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00017390: 446f 6e27 7420 7265 6164 2074 6865 2064  Don't read the d
-000173a0: 6174 6166 7261 6d65 2068 6572 652c 2074  ataframe here, t
-000173b0: 6f20 6176 6f69 6420 7472 6967 6765 7269  o avoid triggeri
-000173c0: 6e67 2061 2072 6561 6420 6f70 6572 6174  ng a read operat
-000173d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000173e0: 2320 666f 7220 7468 6520 5079 7468 6f6e  # for the Python
-000173f0: 2065 6e67 696e 652e 2054 6865 2050 7974   engine. The Pyt
-00017400: 686f 6e20 656e 6769 6e65 2069 7320 676f  hon engine is go
-00017410: 696e 6720 746f 2073 6574 7570 2061 2053  ing to setup a S
-00017420: 7061 726b 204a 6f62 0a20 2020 2020 2020  park Job.       
-00017430: 2020 2020 2023 2074 6f20 7570 6461 7465       # to update
-00017440: 2074 6865 2073 7461 7469 7374 6963 732e   the statistics.
-00017450: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
-00017460: 5f63 6f6d 6d69 745f 6964 203d 204e 6f6e  _commit_id = Non
-00017470: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-00017480: 2077 616c 6c63 6c6f 636b 5f74 696d 6520   wallclock_time 
-00017490: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000174a0: 2020 2020 2020 2020 2020 2020 2023 2052               # R
-000174b0: 6574 7269 6576 6520 6667 2063 6f6d 6d69  etrieve fg commi
-000174c0: 7420 6964 2072 656c 6174 6564 2074 6f20  t id related to 
-000174d0: 7468 6973 2077 616c 6c20 636c 6f63 6b20  this wall clock 
-000174e0: 7469 6d65 2061 6e64 2072 6563 6f6d 7075  time and recompu
-000174f0: 7465 2073 7461 7469 7374 6963 732e 2049  te statistics. I
-00017500: 7420 7769 6c6c 2074 6872 6f77 0a20 2020  t will throw.   
-00017510: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-00017520: 7863 6570 7469 6f6e 2069 6620 6974 7320  xception if its 
-00017530: 6e6f 7420 7469 6d65 2074 7261 7665 6c20  not time travel 
-00017540: 656e 6162 6c65 6420 6665 6174 7572 6520  enabled feature 
-00017550: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
-00017560: 2020 2020 2020 2066 675f 636f 6d6d 6974         fg_commit
-00017570: 5f69 6420 3d20 5b0a 2020 2020 2020 2020  _id = [.        
-00017580: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-00017590: 6974 5f69 640a 2020 2020 2020 2020 2020  it_id.          
-000175a0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000175b0: 6d6d 6974 5f69 6420 696e 2073 656c 662e  mmit_id in self.
-000175c0: 5f66 6561 7475 7265 5f67 726f 7570 5f65  _feature_group_e
-000175d0: 6e67 696e 652e 636f 6d6d 6974 5f64 6574  ngine.commit_det
-000175e0: 6169 6c73 280a 2020 2020 2020 2020 2020  ails(.          
-000175f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017600: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
-00017610: 6d65 2c20 310a 2020 2020 2020 2020 2020  me, 1.          
-00017620: 2020 2020 2020 2020 2020 292e 6b65 7973            ).keys
-00017630: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00017640: 2020 205d 5b30 5d0a 0a20 2020 2020 2020     ][0]..       
-00017650: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00017660: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
-00017670: 696e 652e 636f 6d70 7574 655f 7374 6174  ine.compute_stat
-00017680: 6973 7469 6373 280a 2020 2020 2020 2020  istics(.        
-00017690: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000176a0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
-000176b0: 6174 7572 655f 6772 6f75 705f 636f 6d6d  ature_group_comm
-000176c0: 6974 5f69 643d 6667 5f63 6f6d 6d69 745f  it_id=fg_commit_
-000176d0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-000176e0: 2020 2069 6620 6667 5f63 6f6d 6d69 745f     if fg_commit_
-000176f0: 6964 2069 7320 6e6f 7420 4e6f 6e65 0a20  id is not None. 
-00017700: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00017710: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
-00017720: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00017730: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00017740: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00017750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017760: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00017770: 2020 2020 2020 2022 5468 6520 7374 6174         "The stat
-00017780: 6973 7469 6373 2061 7265 206e 6f74 2065  istics are not e
-00017790: 6e61 626c 6564 206f 6620 6665 6174 7572  nabled of featur
-000177a0: 6520 6772 6f75 7020 607b 7d60 2c20 7769  e group `{}`, wi
-000177b0: 7468 2076 6572 7369 6f6e 220a 2020 2020  th version".    
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 2220 607b 7d60 2e20 4e6f 2073 7461 7469  " `{}`. No stati
-000177e0: 7374 6963 7320 636f 6d70 7574 6564 2e22  stics computed."
-000177f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017800: 2029 2e66 6f72 6d61 7428 7365 6c66 2e5f   ).format(self._
-00017810: 6e61 6d65 2c20 7365 6c66 2e5f 7665 7273  name, self._vers
-00017820: 696f 6e29 2c0a 2020 2020 2020 2020 2020  ion),.          
-00017830: 2020 2020 2020 7574 696c 2e53 746f 7261        util.Stora
-00017840: 6765 5761 726e 696e 672c 0a20 2020 2020  geWarning,.     
-00017850: 2020 2020 2020 2029 0a0a 2020 2020 4063         )..    @c
-00017860: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00017870: 6566 2066 726f 6d5f 7265 7370 6f6e 7365  ef from_response
-00017880: 5f6a 736f 6e28 636c 732c 206a 736f 6e5f  _json(cls, json_
-00017890: 6469 6374 293a 0a20 2020 2020 2020 206a  dict):.        j
-000178a0: 736f 6e5f 6465 6361 6d65 6c69 7a65 6420  son_decamelized 
-000178b0: 3d20 6875 6d70 732e 6465 6361 6d65 6c69  = humps.decameli
-000178c0: 7a65 286a 736f 6e5f 6469 6374 290a 2020  ze(json_dict).  
-000178d0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000178e0: 6e63 6528 6a73 6f6e 5f64 6563 616d 656c  nce(json_decamel
-000178f0: 697a 6564 2c20 6469 6374 293a 0a20 2020  ized, dict):.   
-00017900: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
-00017910: 6522 2069 6e20 6a73 6f6e 5f64 6563 616d  e" in json_decam
-00017920: 656c 697a 6564 3a0a 2020 2020 2020 2020  elized:.        
-00017930: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
-00017940: 616d 656c 697a 6564 5b22 7374 7265 616d  amelized["stream
-00017950: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00017960: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00017970: 6465 6361 6d65 6c69 7a65 645b 2274 7970  decamelized["typ
-00017980: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
-00017990: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000179b0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
-000179c0: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-000179d0: 642e 706f 7028 2274 7970 6522 2c20 4e6f  d.pop("type", No
-000179e0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-000179f0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00017a00: 2e70 6f70 2822 7661 6c69 6461 7469 6f6e  .pop("validation
-00017a10: 5f74 7970 6522 2c20 4e6f 6e65 290a 2020  _type", None).  
-00017a20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017a30: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
-00017a40: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
-00017a50: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
-00017a60: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
-00017a70: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
-00017a80: 6522 2069 6e20 6667 3a0a 2020 2020 2020  e" in fg:.      
-00017a90: 2020 2020 2020 2020 2020 6667 5b22 7374            fg["st
-00017aa0: 7265 616d 225d 203d 2066 675b 2274 7970  ream"] = fg["typ
-00017ab0: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
-00017ac0: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
-00017ad0: 2020 2020 2020 2020 2020 205f 203d 2066             _ = f
-00017ae0: 672e 706f 7028 2274 7970 6522 2c20 4e6f  g.pop("type", No
-00017af0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00017b00: 6667 2e70 6f70 2822 7661 6c69 6461 7469  fg.pop("validati
-00017b10: 6f6e 5f74 7970 6522 2c20 4e6f 6e65 290a  on_type", None).
-00017b20: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00017b30: 636c 7328 2a2a 6667 2920 666f 7220 6667  cls(**fg) for fg
-00017b40: 2069 6e20 6a73 6f6e 5f64 6563 616d 656c   in json_decamel
-00017b50: 697a 6564 5d0a 0a20 2020 2064 6566 2075  ized]..    def u
-00017b60: 7064 6174 655f 6672 6f6d 5f72 6573 706f  pdate_from_respo
-00017b70: 6e73 655f 6a73 6f6e 2873 656c 662c 206a  nse_json(self, j
-00017b80: 736f 6e5f 6469 6374 293a 0a20 2020 2020  son_dict):.     
-00017b90: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
-00017ba0: 7a65 6420 3d20 6875 6d70 732e 6465 6361  zed = humps.deca
-00017bb0: 6d65 6c69 7a65 286a 736f 6e5f 6469 6374  melize(json_dict
-00017bc0: 290a 2020 2020 2020 2020 6a73 6f6e 5f64  ).        json_d
-00017bd0: 6563 616d 656c 697a 6564 5b22 7374 7265  ecamelized["stre
-00017be0: 616d 225d 203d 206a 736f 6e5f 6465 6361  am"] = json_deca
-00017bf0: 6d65 6c69 7a65 645b 2274 7970 6522 5d20  melized["type"] 
-00017c00: 3d3d 2022 7374 7265 616d 4665 6174 7572  == "streamFeatur
-00017c10: 6547 726f 7570 4454 4f22 0a20 2020 2020  eGroupDTO".     
-00017c20: 2020 205f 203d 206a 736f 6e5f 6465 6361     _ = json_deca
-00017c30: 6d65 6c69 7a65 642e 706f 7028 2274 7970  melized.pop("typ
-00017c40: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
-00017c50: 2e5f 5f69 6e69 745f 5f28 2a2a 6a73 6f6e  .__init__(**json
-00017c60: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
-00017c70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00017c80: 660a 0a20 2020 2064 6566 206a 736f 6e28  f..    def json(
-00017c90: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00017ca0: 2222 4765 7420 7370 6563 6966 6963 2046  ""Get specific F
-00017cb0: 6561 7475 7265 2047 726f 7570 206d 6574  eature Group met
-00017cc0: 6164 6174 6120 696e 206a 736f 6e20 666f  adata in json fo
-00017cd0: 726d 6174 2e0a 0a20 2020 2020 2020 2021  rmat...        !
-00017ce0: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
-00017cf0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00017d00: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-00017d10: 6a73 6f6e 2829 0a20 2020 2020 2020 2020  json().         
-00017d20: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
-00017d30: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00017d40: 6e20 6a73 6f6e 2e64 756d 7073 2873 656c  n json.dumps(sel
-00017d50: 662c 2063 6c73 3d75 7469 6c2e 4665 6174  f, cls=util.Feat
-00017d60: 7572 6553 746f 7265 456e 636f 6465 7229  ureStoreEncoder)
-00017d70: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
-00017d80: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00017d90: 2022 2222 4765 7420 7374 7275 6374 7572   """Get structur
-00017da0: 6564 2069 6e66 6f20 6162 6f75 7420 7370  ed info about sp
-00017db0: 6563 6966 6963 2046 6561 7475 7265 2047  ecific Feature G
-00017dc0: 726f 7570 2069 6e20 7079 7468 6f6e 2064  roup in python d
-00017dd0: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
-00017de0: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-00017df0: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-00017e00: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00017e10: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-00017e20: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-00017e30: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-00017e40: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
-00017e50: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-00017e60: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
-00017e70: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
-00017e80: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
-00017e90: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-00017ea0: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-00017eb0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-00017ec0: 746f 5f64 6963 7428 290a 2020 2020 2020  to_dict().      
-00017ed0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00017ee0: 2020 2222 220a 2020 2020 2020 2020 6667    """.        fg
-00017ef0: 5f6d 6574 615f 6469 6374 203d 207b 0a20  _meta_dict = {. 
-00017f00: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00017f10: 2073 656c 662e 5f69 642c 0a20 2020 2020   self._id,.     
-00017f20: 2020 2020 2020 2022 6e61 6d65 223a 2073         "name": s
-00017f30: 656c 662e 5f6e 616d 652c 0a20 2020 2020  elf._name,.     
-00017f40: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00017f50: 3a20 7365 6c66 2e5f 7665 7273 696f 6e2c  : self._version,
-00017f60: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00017f70: 7363 7269 7074 696f 6e22 3a20 7365 6c66  scription": self
-00017f80: 2e5f 6465 7363 7269 7074 696f 6e2c 0a20  ._description,. 
-00017f90: 2020 2020 2020 2020 2020 2022 6f6e 6c69             "onli
-00017fa0: 6e65 456e 6162 6c65 6422 3a20 7365 6c66  neEnabled": self
-00017fb0: 2e5f 6f6e 6c69 6e65 5f65 6e61 626c 6564  ._online_enabled
-00017fc0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-00017fd0: 696d 6554 7261 7665 6c46 6f72 6d61 7422  imeTravelFormat"
-00017fe0: 3a20 7365 6c66 2e5f 7469 6d65 5f74 7261  : self._time_tra
-00017ff0: 7665 6c5f 666f 726d 6174 2c0a 2020 2020  vel_format,.    
-00018000: 2020 2020 2020 2020 2266 6561 7475 7265          "feature
-00018010: 7322 3a20 7365 6c66 2e5f 6665 6174 7572  s": self._featur
-00018020: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00018030: 2266 6561 7475 7265 7374 6f72 6549 6422  "featurestoreId"
-00018040: 3a20 7365 6c66 2e5f 6665 6174 7572 655f  : self._feature_
-00018050: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
-00018060: 2020 2020 2020 2274 7970 6522 3a20 2263        "type": "c
-00018070: 6163 6865 6446 6561 7475 7265 6772 6f75  achedFeaturegrou
-00018080: 7044 544f 220a 2020 2020 2020 2020 2020  pDTO".          
-00018090: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
-000180a0: 7472 6561 6d0a 2020 2020 2020 2020 2020  tream.          
-000180b0: 2020 656c 7365 2022 7374 7265 616d 4665    else "streamFe
-000180c0: 6174 7572 6547 726f 7570 4454 4f22 2c0a  atureGroupDTO",.
-000180d0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-000180e0: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
-000180f0: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
-00018100: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
-00018110: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
-00018120: 3a20 7365 6c66 2e65 7665 6e74 5f74 696d  : self.event_tim
-00018130: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
-00018140: 6578 7065 6374 6174 696f 6e53 7569 7465  expectationSuite
-00018150: 223a 2073 656c 662e 5f65 7870 6563 7461  ": self._expecta
-00018160: 7469 6f6e 5f73 7569 7465 2c0a 2020 2020  tion_suite,.    
-00018170: 2020 2020 2020 2020 2270 6172 656e 7473          "parents
-00018180: 223a 2073 656c 662e 5f70 6172 656e 7473  ": self._parents
-00018190: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-000181a0: 2020 2020 6966 2073 656c 662e 5f73 7472      if self._str
-000181b0: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-000181c0: 2066 675f 6d65 7461 5f64 6963 745b 2264   fg_meta_dict["d
-000181d0: 656c 7461 5374 7265 616d 6572 4a6f 6243  eltaStreamerJobC
-000181e0: 6f6e 6622 5d20 3d20 7365 6c66 2e5f 6465  onf"] = self._de
-000181f0: 6c74 6173 7472 6561 6d65 725f 6a6f 6263  ltastreamer_jobc
-00018200: 6f6e 660a 2020 2020 2020 2020 7265 7475  onf.        retu
-00018210: 726e 2066 675f 6d65 7461 5f64 6963 740a  rn fg_meta_dict.
-00018220: 0a20 2020 2064 6566 205f 6765 745f 7461  .    def _get_ta
-00018230: 626c 655f 6e61 6d65 2873 656c 6629 3a0a  ble_name(self):.
-00018240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00018250: 656c 662e 6665 6174 7572 655f 7374 6f72  elf.feature_stor
-00018260: 655f 6e61 6d65 202b 2022 2e22 202b 2073  e_name + "." + s
-00018270: 656c 662e 6e61 6d65 202b 2022 5f22 202b  elf.name + "_" +
-00018280: 2073 7472 2873 656c 662e 7665 7273 696f   str(self.versio
-00018290: 6e29 0a0a 2020 2020 6465 6620 5f67 6574  n)..    def _get
-000182a0: 5f6f 6e6c 696e 655f 7461 626c 655f 6e61  _online_table_na
-000182b0: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
-000182c0: 2020 7265 7475 726e 2073 656c 662e 6e61    return self.na
-000182d0: 6d65 202b 2022 5f22 202b 2073 7472 2873  me + "_" + str(s
-000182e0: 656c 662e 7665 7273 696f 6e29 0a0a 2020  elf.version)..  
-000182f0: 2020 6465 6620 5f67 6574 5f70 726f 6a65    def _get_proje
-00018300: 6374 5f6e 616d 6528 7365 6c66 293a 0a20  ct_name(self):. 
-00018310: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-00018320: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
-00018330: 652e 656e 6473 7769 7468 2822 5f66 6561  e.endswith("_fea
-00018340: 7475 7265 7374 6f72 6522 293a 0a20 2020  turestore"):.   
-00018350: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00018360: 7365 6c66 2e66 6561 7475 7265 5f73 746f  self.feature_sto
-00018370: 7265 5f6e 616d 655b 3a2d 3133 5d0a 2020  re_name[:-13].  
-00018380: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00018390: 662e 6665 6174 7572 655f 7374 6f72 655f  f.feature_store_
-000183a0: 6e61 6d65 0a0a 2020 2020 4070 726f 7065  name..    @prope
-000183b0: 7274 790a 2020 2020 6465 6620 6964 2873  rty.    def id(s
-000183c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000183d0: 2246 6561 7475 7265 2067 726f 7570 2069  "Feature group i
-000183e0: 642e 2222 220a 2020 2020 2020 2020 7265  d.""".        re
-000183f0: 7475 726e 2073 656c 662e 5f69 640a 0a20  turn self._id.. 
-00018400: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00018410: 2064 6566 206e 616d 6528 7365 6c66 293a   def name(self):
-00018420: 0a20 2020 2020 2020 2022 2222 4e61 6d65  .        """Name
-00018430: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
-00018440: 6772 6f75 702e 2222 220a 2020 2020 2020  group.""".      
-00018450: 2020 7265 7475 726e 2073 656c 662e 5f6e    return self._n
-00018460: 616d 650a 0a20 2020 2040 7072 6f70 6572  ame..    @proper
-00018470: 7479 0a20 2020 2064 6566 2076 6572 7369  ty.    def versi
-00018480: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
-00018490: 2020 2222 2256 6572 7369 6f6e 206e 756d    """Version num
-000184a0: 6265 7220 6f66 2074 6865 2066 6561 7475  ber of the featu
-000184b0: 7265 2067 726f 7570 2e22 2222 0a20 2020  re group.""".   
-000184c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000184d0: 2e5f 7665 7273 696f 6e0a 0a20 2020 2040  ._version..    @
-000184e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000184f0: 2064 6573 6372 6970 7469 6f6e 2873 656c   description(sel
-00018500: 6629 3a0a 2020 2020 2020 2020 2222 2244  f):.        """D
-00018510: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
-00018520: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-00018530: 636f 6e74 656e 7473 2e22 2222 0a20 2020  contents.""".   
-00018540: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00018550: 2e5f 6465 7363 7269 7074 696f 6e0a 0a20  ._description.. 
-00018560: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00018570: 2064 6566 2074 696d 655f 7472 6176 656c   def time_travel
-00018580: 5f66 6f72 6d61 7428 7365 6c66 293a 0a20  _format(self):. 
-00018590: 2020 2020 2020 2022 2222 5365 7474 696e         """Settin
-000185a0: 6720 6f66 2074 6865 2066 6561 7475 7265  g of the feature
-000185b0: 2067 726f 7570 2074 696d 6520 7472 6176   group time trav
-000185c0: 656c 2066 6f72 6d61 742e 2222 220a 2020  el format.""".  
-000185d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000185e0: 662e 5f74 696d 655f 7472 6176 656c 5f66  f._time_travel_f
-000185f0: 6f72 6d61 740a 0a20 2020 2040 7072 6f70  ormat..    @prop
-00018600: 6572 7479 0a20 2020 2064 6566 2070 6172  erty.    def par
-00018610: 7469 7469 6f6e 5f6b 6579 2873 656c 6629  tition_key(self)
-00018620: 3a0a 2020 2020 2020 2020 2222 224c 6973  :.        """Lis
-00018630: 7420 6f66 2066 6561 7475 7265 7320 6275  t of features bu
-00018640: 696c 6469 6e67 2074 6865 2070 6172 7469  ilding the parti
-00018650: 7469 6f6e 206b 6579 2e22 2222 0a20 2020  tion key.""".   
-00018660: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00018670: 2e5f 7061 7274 6974 696f 6e5f 6b65 790a  ._partition_key.
-00018680: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00018690: 2020 2064 6566 2068 7564 695f 7072 6563     def hudi_prec
-000186a0: 6f6d 6269 6e65 5f6b 6579 2873 656c 6629  ombine_key(self)
-000186b0: 3a0a 2020 2020 2020 2020 2222 2246 6561  :.        """Fea
-000186c0: 7475 7265 206e 616d 6520 7468 6174 2069  ture name that i
-000186d0: 7320 7468 6520 6875 6469 2070 7265 636f  s the hudi preco
-000186e0: 6d62 696e 6520 6b65 792e 2222 220a 2020  mbine key.""".  
-000186f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00018700: 662e 5f68 7564 695f 7072 6563 6f6d 6269  f._hudi_precombi
-00018710: 6e65 5f6b 6579 0a0a 2020 2020 4070 726f  ne_key..    @pro
-00018720: 7065 7274 790a 2020 2020 6465 6620 6665  perty.    def fe
-00018730: 6174 7572 655f 7374 6f72 655f 6964 2873  ature_store_id(s
-00018740: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00018750: 7475 726e 2073 656c 662e 5f66 6561 7475  turn self._featu
-00018760: 7265 5f73 746f 7265 5f69 640a 0a20 2020  re_store_id..   
-00018770: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00018780: 6566 2066 6561 7475 7265 5f73 746f 7265  ef feature_store
-00018790: 5f6e 616d 6528 7365 6c66 293a 0a20 2020  _name(self):.   
-000187a0: 2020 2020 2022 2222 4e61 6d65 206f 6620       """Name of 
-000187b0: 7468 6520 6665 6174 7572 6520 7374 6f72  the feature stor
-000187c0: 6520 696e 2077 6869 6368 2074 6865 2066  e in which the f
-000187d0: 6561 7475 7265 2067 726f 7570 2069 7320  eature group is 
-000187e0: 6c6f 6361 7465 642e 2222 220a 2020 2020  located.""".    
-000187f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00018800: 5f66 6561 7475 7265 5f73 746f 7265 5f6e  _feature_store_n
-00018810: 616d 650a 0a20 2020 2040 7072 6f70 6572  ame..    @proper
-00018820: 7479 0a20 2020 2064 6566 2063 7265 6174  ty.    def creat
-00018830: 6f72 2873 656c 6629 3a0a 2020 2020 2020  or(self):.      
-00018840: 2020 2222 2255 7365 726e 616d 6520 6f66    """Username of
-00018850: 2074 6865 2063 7265 6174 6f72 2e22 2222   the creator."""
-00018860: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018870: 7365 6c66 2e5f 6372 6561 746f 720a 0a20  self._creator.. 
-00018880: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00018890: 2064 6566 2063 7265 6174 6564 2873 656c   def created(sel
-000188a0: 6629 3a0a 2020 2020 2020 2020 2222 2254  f):.        """T
-000188b0: 696d 6573 7461 6d70 2077 6865 6e20 7468  imestamp when th
-000188c0: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-000188d0: 7761 7320 6372 6561 7465 642e 2222 220a  was created.""".
-000188e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000188f0: 656c 662e 5f63 7265 6174 6564 0a0a 2020  elf._created..  
-00018900: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00018910: 6465 6620 7374 7265 616d 2873 656c 6629  def stream(self)
-00018920: 3a0a 2020 2020 2020 2020 2222 2257 6865  :.        """Whe
-00018930: 7468 6572 2074 6f20 656e 6162 6c65 2072  ther to enable r
-00018940: 6561 6c20 7469 6d65 2073 7472 6561 6d20  eal time stream 
-00018950: 7772 6974 696e 6720 6361 7061 6269 6c69  writing capabili
-00018960: 7469 6573 2e22 2222 0a20 2020 2020 2020  ties.""".       
-00018970: 2072 6574 7572 6e20 7365 6c66 2e5f 7374   return self._st
-00018980: 7265 616d 0a0a 2020 2020 4070 726f 7065  ream..    @prope
-00018990: 7274 790a 2020 2020 6465 6620 7061 7265  rty.    def pare
-000189a0: 6e74 7328 7365 6c66 293a 0a20 2020 2020  nts(self):.     
-000189b0: 2020 2022 2222 5061 7265 6e74 2066 6561     """Parent fea
-000189c0: 7475 7265 2067 726f 7570 7320 6173 206f  ture groups as o
-000189d0: 7269 6769 6e20 6f66 2074 6865 2064 6174  rigin of the dat
-000189e0: 6120 696e 2074 6865 2063 7572 7265 6e74  a in the current
-000189f0: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-00018a00: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-00018a10: 7061 7274 206f 6620 6578 706c 6963 6974  part of explicit
-00018a20: 2070 726f 7665 6e61 6e63 6522 2222 0a20   provenance""". 
-00018a30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00018a40: 6c66 2e5f 7061 7265 6e74 730a 0a20 2020  lf._parents..   
-00018a50: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00018a60: 6566 2062 6163 6b66 696c 6c5f 6a6f 6228  ef backfill_job(
-00018a70: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00018a80: 2222 4765 7420 7468 6520 4a6f 6220 6f62  ""Get the Job ob
-00018a90: 6a65 6374 2072 6566 6572 656e 6365 2066  ject reference f
-00018aa0: 6f72 2074 6865 2062 6163 6b66 696c 6c20  or the backfill 
-00018ab0: 6a6f 6220 666f 7220 7468 6973 0a20 2020  job for this.   
-00018ac0: 2020 2020 2046 6561 7475 7265 2047 726f       Feature Gro
-00018ad0: 7570 2e22 2222 0a20 2020 2020 2020 2069  up.""".        i
-00018ae0: 6620 7365 6c66 2e5f 6261 636b 6669 6c6c  f self._backfill
-00018af0: 5f6a 6f62 2069 7320 4e6f 6e65 3a0a 2020  _job is None:.  
-00018b00: 2020 2020 2020 2020 2020 6a6f 625f 6e61            job_na
-00018b10: 6d65 203d 2022 7b66 675f 6e61 6d65 7d5f  me = "{fg_name}_
-00018b20: 7b76 6572 7369 6f6e 7d5f 6f66 666c 696e  {version}_offlin
-00018b30: 655f 6667 5f62 6163 6b66 696c 6c22 2e66  e_fg_backfill".f
-00018b40: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00018b50: 2020 2020 2020 2066 675f 6e61 6d65 3d73         fg_name=s
-00018b60: 656c 662e 5f6e 616d 652c 2076 6572 7369  elf._name, versi
-00018b70: 6f6e 3d73 656c 662e 5f76 6572 7369 6f6e  on=self._version
-00018b80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00018b90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018ba0: 5f62 6163 6b66 696c 6c5f 6a6f 6220 3d20  _backfill_job = 
-00018bb0: 6a6f 625f 6170 692e 4a6f 6241 7069 2829  job_api.JobApi()
-00018bc0: 2e67 6574 286a 6f62 5f6e 616d 6529 0a20  .get(job_name). 
-00018bd0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00018be0: 6c66 2e5f 6261 636b 6669 6c6c 5f6a 6f62  lf._backfill_job
-00018bf0: 0a0a 2020 2020 4076 6572 7369 6f6e 2e73  ..    @version.s
-00018c00: 6574 7465 720a 2020 2020 6465 6620 7665  etter.    def ve
-00018c10: 7273 696f 6e28 7365 6c66 2c20 7665 7273  rsion(self, vers
-00018c20: 696f 6e29 3a0a 2020 2020 2020 2020 7365  ion):.        se
-00018c30: 6c66 2e5f 7665 7273 696f 6e20 3d20 7665  lf._version = ve
-00018c40: 7273 696f 6e0a 0a20 2020 2040 6465 7363  rsion..    @desc
-00018c50: 7269 7074 696f 6e2e 7365 7474 6572 0a20  ription.setter. 
-00018c60: 2020 2064 6566 2064 6573 6372 6970 7469     def descripti
-00018c70: 6f6e 2873 656c 662c 206e 6577 5f64 6573  on(self, new_des
-00018c80: 6372 6970 7469 6f6e 293a 0a20 2020 2020  cription):.     
-00018c90: 2020 2073 656c 662e 5f64 6573 6372 6970     self._descrip
-00018ca0: 7469 6f6e 203d 206e 6577 5f64 6573 6372  tion = new_descr
-00018cb0: 6970 7469 6f6e 0a0a 2020 2020 4074 696d  iption..    @tim
-00018cc0: 655f 7472 6176 656c 5f66 6f72 6d61 742e  e_travel_format.
-00018cd0: 7365 7474 6572 0a20 2020 2064 6566 2074  setter.    def t
-00018ce0: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
-00018cf0: 7428 7365 6c66 2c20 6e65 775f 7469 6d65  t(self, new_time
-00018d00: 5f74 7261 7665 6c5f 666f 726d 6174 293a  _travel_format):
-00018d10: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00018d20: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
-00018d30: 7420 3d20 6e65 775f 7469 6d65 5f74 7261  t = new_time_tra
-00018d40: 7665 6c5f 666f 726d 6174 0a0a 2020 2020  vel_format..    
-00018d50: 4070 6172 7469 7469 6f6e 5f6b 6579 2e73  @partition_key.s
-00018d60: 6574 7465 720a 2020 2020 6465 6620 7061  etter.    def pa
-00018d70: 7274 6974 696f 6e5f 6b65 7928 7365 6c66  rtition_key(self
-00018d80: 2c20 6e65 775f 7061 7274 6974 696f 6e5f  , new_partition_
-00018d90: 6b65 7929 3a0a 2020 2020 2020 2020 7365  key):.        se
-00018da0: 6c66 2e5f 7061 7274 6974 696f 6e5f 6b65  lf._partition_ke
-00018db0: 7920 3d20 5b70 6b2e 6c6f 7765 7228 2920  y = [pk.lower() 
-00018dc0: 666f 7220 706b 2069 6e20 6e65 775f 7061  for pk in new_pa
-00018dd0: 7274 6974 696f 6e5f 6b65 795d 0a0a 2020  rtition_key]..  
-00018de0: 2020 4068 7564 695f 7072 6563 6f6d 6269    @hudi_precombi
-00018df0: 6e65 5f6b 6579 2e73 6574 7465 720a 2020  ne_key.setter.  
-00018e00: 2020 6465 6620 6875 6469 5f70 7265 636f    def hudi_preco
-00018e10: 6d62 696e 655f 6b65 7928 7365 6c66 2c20  mbine_key(self, 
-00018e20: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
-00018e30: 6b65 7929 3a0a 2020 2020 2020 2020 7365  key):.        se
-00018e40: 6c66 2e5f 6875 6469 5f70 7265 636f 6d62  lf._hudi_precomb
-00018e50: 696e 655f 6b65 7920 3d20 6875 6469 5f70  ine_key = hudi_p
-00018e60: 7265 636f 6d62 696e 655f 6b65 792e 6c6f  recombine_key.lo
-00018e70: 7765 7228 290a 0a20 2020 2040 7374 7265  wer()..    @stre
-00018e80: 616d 2e73 6574 7465 720a 2020 2020 6465  am.setter.    de
-00018e90: 6620 7374 7265 616d 2873 656c 662c 2073  f stream(self, s
-00018ea0: 7472 6561 6d29 3a0a 2020 2020 2020 2020  tream):.        
-00018eb0: 7365 6c66 2e5f 7374 7265 616d 203d 2073  self._stream = s
-00018ec0: 7472 6561 6d0a 0a20 2020 2040 7061 7265  tream..    @pare
-00018ed0: 6e74 732e 7365 7474 6572 0a20 2020 2064  nts.setter.    d
-00018ee0: 6566 2070 6172 656e 7473 2873 656c 662c  ef parents(self,
-00018ef0: 206e 6577 5f70 6172 656e 7473 293a 0a20   new_parents):. 
-00018f00: 2020 2020 2020 2073 656c 662e 5f70 6172         self._par
-00018f10: 656e 7473 203d 206e 6577 5f70 6172 656e  ents = new_paren
-00018f20: 7473 0a0a 0a63 6c61 7373 2045 7874 6572  ts...class Exter
-00018f30: 6e61 6c46 6561 7475 7265 4772 6f75 7028  nalFeatureGroup(
-00018f40: 4665 6174 7572 6547 726f 7570 4261 7365  FeatureGroupBase
-00018f50: 293a 0a20 2020 2045 5854 4552 4e41 4c5f  ):.    EXTERNAL_
-00018f60: 4645 4154 5552 455f 4752 4f55 5020 3d20  FEATURE_GROUP = 
-00018f70: 224f 4e5f 4445 4d41 4e44 5f46 4541 5455  "ON_DEMAND_FEATU
-00018f80: 5245 5f47 524f 5550 220a 2020 2020 454e  RE_GROUP".    EN
-00018f90: 5449 5459 5f54 5950 4520 3d20 2266 6561  TITY_TYPE = "fea
-00018fa0: 7475 7265 6772 6f75 7073 220a 0a20 2020  turegroups"..   
-00018fb0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00018fc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00018fd0: 2020 2020 2073 746f 7261 6765 5f63 6f6e       storage_con
-00018fe0: 6e65 6374 6f72 2c0a 2020 2020 2020 2020  nector,.        
-00018ff0: 7175 6572 793d 4e6f 6e65 2c0a 2020 2020  query=None,.    
-00019000: 2020 2020 6461 7461 5f66 6f72 6d61 743d      data_format=
-00019010: 4e6f 6e65 2c0a 2020 2020 2020 2020 7061  None,.        pa
-00019020: 7468 3d4e 6f6e 652c 0a20 2020 2020 2020  th=None,.       
-00019030: 206f 7074 696f 6e73 3d7b 7d2c 0a20 2020   options={},.   
-00019040: 2020 2020 206e 616d 653d 4e6f 6e65 2c0a       name=None,.
-00019050: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
-00019060: 4e6f 6e65 2c0a 2020 2020 2020 2020 6465  None,.        de
-00019070: 7363 7269 7074 696f 6e3d 4e6f 6e65 2c0a  scription=None,.
-00019080: 2020 2020 2020 2020 7072 696d 6172 795f          primary_
-00019090: 6b65 793d 4e6f 6e65 2c0a 2020 2020 2020  key=None,.      
-000190a0: 2020 6665 6174 7572 6573 746f 7265 5f69    featurestore_i
-000190b0: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
-000190c0: 6665 6174 7572 6573 746f 7265 5f6e 616d  featurestore_nam
-000190d0: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
-000190e0: 6372 6561 7465 643d 4e6f 6e65 2c0a 2020  created=None,.  
-000190f0: 2020 2020 2020 6372 6561 746f 723d 4e6f        creator=No
-00019100: 6e65 2c0a 2020 2020 2020 2020 6964 3d4e  ne,.        id=N
-00019110: 6f6e 652c 0a20 2020 2020 2020 2066 6561  one,.        fea
-00019120: 7475 7265 733d 4e6f 6e65 2c0a 2020 2020  tures=None,.    
-00019130: 2020 2020 6c6f 6361 7469 6f6e 3d4e 6f6e      location=Non
-00019140: 652c 0a20 2020 2020 2020 2073 7461 7469  e,.        stati
-00019150: 7374 6963 735f 636f 6e66 6967 3d4e 6f6e  stics_config=Non
-00019160: 652c 0a20 2020 2020 2020 2065 7665 6e74  e,.        event
-00019170: 5f74 696d 653d 4e6f 6e65 2c0a 2020 2020  _time=None,.    
-00019180: 2020 2020 6578 7065 6374 6174 696f 6e5f      expectation_
-00019190: 7375 6974 653d 4e6f 6e65 2c0a 2020 2020  suite=None,.    
-000191a0: 2020 2020 6f6e 6c69 6e65 5f65 6e61 626c      online_enabl
-000191b0: 6564 3d46 616c 7365 2c0a 2020 2020 2020  ed=False,.      
-000191c0: 2020 6872 6566 3d4e 6f6e 652c 0a20 2020    href=None,.   
-000191d0: 2020 2020 206f 6e6c 696e 655f 746f 7069       online_topi
-000191e0: 635f 6e61 6d65 3d4e 6f6e 652c 0a20 2020  c_name=None,.   
-000191f0: 2020 2020 2073 7069 6e65 3d46 616c 7365       spine=False
-00019200: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00019210: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00019220: 5f28 0a20 2020 2020 2020 2020 2020 2066  _(.            f
-00019230: 6561 7475 7265 7374 6f72 655f 6964 2c0a  eaturestore_id,.
-00019240: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00019250: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00019260: 2020 6576 656e 745f 7469 6d65 3d65 7665    event_time=eve
-00019270: 6e74 5f74 696d 652c 0a20 2020 2020 2020  nt_time,.       
-00019280: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
-00019290: 6c65 643d 6f6e 6c69 6e65 5f65 6e61 626c  led=online_enabl
-000192a0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-000192b0: 6964 3d69 642c 0a20 2020 2020 2020 2020  id=id,.         
-000192c0: 2020 2065 7870 6563 7461 7469 6f6e 5f73     expectation_s
-000192d0: 7569 7465 3d65 7870 6563 7461 7469 6f6e  uite=expectation
-000192e0: 5f73 7569 7465 2c0a 2020 2020 2020 2020  _suite,.        
-000192f0: 2020 2020 6f6e 6c69 6e65 5f74 6f70 6963      online_topic
-00019300: 5f6e 616d 653d 6f6e 6c69 6e65 5f74 6f70  _name=online_top
-00019310: 6963 5f6e 616d 652c 0a20 2020 2020 2020  ic_name,.       
-00019320: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
-00019330: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
-00019340: 6e61 6d65 203d 2066 6561 7475 7265 7374  name = featurest
-00019350: 6f72 655f 6e61 6d65 0a20 2020 2020 2020  ore_name.       
-00019360: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
-00019370: 6f6e 203d 2064 6573 6372 6970 7469 6f6e  on = description
-00019380: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00019390: 7265 6174 6564 203d 2063 7265 6174 6564  reated = created
-000193a0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-000193b0: 7265 6174 6f72 203d 2075 7365 722e 5573  reator = user.Us
-000193c0: 6572 2e66 726f 6d5f 7265 7370 6f6e 7365  er.from_response
-000193d0: 5f6a 736f 6e28 6372 6561 746f 7229 0a20  _json(creator). 
-000193e0: 2020 2020 2020 2073 656c 662e 5f76 6572         self._ver
-000193f0: 7369 6f6e 203d 2076 6572 7369 6f6e 0a20  sion = version. 
-00019400: 2020 2020 2020 2073 656c 662e 5f6e 616d         self._nam
-00019410: 6520 3d20 6e61 6d65 0a20 2020 2020 2020  e = name.       
-00019420: 2073 656c 662e 5f71 7565 7279 203d 2071   self._query = q
-00019430: 7565 7279 0a20 2020 2020 2020 2073 656c  uery.        sel
-00019440: 662e 5f64 6174 615f 666f 726d 6174 203d  f._data_format =
-00019450: 2064 6174 615f 666f 726d 6174 2e75 7070   data_format.upp
-00019460: 6572 2829 2069 6620 6461 7461 5f66 6f72  er() if data_for
-00019470: 6d61 7420 656c 7365 204e 6f6e 650a 2020  mat else None.  
-00019480: 2020 2020 2020 7365 6c66 2e5f 7061 7468        self._path
-00019490: 203d 2070 6174 680a 0a20 2020 2020 2020   = path..       
-000194a0: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
-000194b0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-000194c0: 6665 6174 7572 652e 4665 6174 7572 652e  feature.Feature.
-000194d0: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
-000194e0: 6f6e 2866 6561 7429 2069 6620 6973 696e  on(feat) if isin
-000194f0: 7374 616e 6365 2866 6561 742c 2064 6963  stance(feat, dic
-00019500: 7429 2065 6c73 6520 6665 6174 0a20 2020  t) else feat.   
-00019510: 2020 2020 2020 2020 2066 6f72 2066 6561           for fea
-00019520: 7420 696e 2028 6665 6174 7572 6573 206f  t in (features o
-00019530: 7220 5b5d 290a 2020 2020 2020 2020 5d0a  r []).        ].
-00019540: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-00019550: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
-00019560: 696e 6520 3d20 280a 2020 2020 2020 2020  ine = (.        
-00019570: 2020 2020 6578 7465 726e 616c 5f66 6561      external_fea
-00019580: 7475 7265 5f67 726f 7570 5f65 6e67 696e  ture_group_engin
-00019590: 652e 4578 7465 726e 616c 4665 6174 7572  e.ExternalFeatur
-000195a0: 6547 726f 7570 456e 6769 6e65 2866 6561  eGroupEngine(fea
-000195b0: 7475 7265 7374 6f72 655f 6964 290a 2020  turestore_id).  
-000195c0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000195d0: 2069 6620 7365 6c66 2e5f 6964 3a0a 2020   if self._id:.  
-000195e0: 2020 2020 2020 2020 2020 2320 476f 7420            # Got 
-000195f0: 6672 6f6d 2048 6f70 7377 6f72 6b73 2c20  from Hopsworks, 
-00019600: 6465 7365 7269 616c 697a 6520 6665 6174  deserialize feat
-00019610: 7572 6573 2061 6e64 2073 746f 7261 6765  ures and storage
-00019620: 2063 6f6e 6e65 6374 6f72 0a20 2020 2020   connector.     
-00019630: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
-00019640: 7475 7265 7320 3d20 280a 2020 2020 2020  tures = (.      
-00019650: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
-00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019670: 6665 6174 7572 652e 4665 6174 7572 652e  feature.Feature.
-00019680: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
-00019690: 6f6e 2866 6561 7429 0a20 2020 2020 2020  on(feat).       
-000196a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000196b0: 6973 696e 7374 616e 6365 2866 6561 742c  isinstance(feat,
-000196c0: 2064 6963 7429 0a20 2020 2020 2020 2020   dict).         
-000196d0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-000196e0: 6665 6174 0a20 2020 2020 2020 2020 2020  feat.           
-000196f0: 2020 2020 2020 2020 2066 6f72 2066 6561           for fea
-00019700: 7420 696e 2066 6561 7475 7265 730a 2020  t in features.  
-00019710: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019730: 6966 2066 6561 7475 7265 730a 2020 2020  if features.    
-00019740: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00019750: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00019760: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00019770: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
-00019780: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00019790: 2020 2020 205b 6665 6174 2e6e 616d 6520       [feat.name 
-000197a0: 666f 7220 6665 6174 2069 6e20 7365 6c66  for feat in self
-000197b0: 2e5f 6665 6174 7572 6573 2069 6620 6665  ._features if fe
-000197c0: 6174 2e70 7269 6d61 7279 2069 7320 5472  at.primary is Tr
-000197d0: 7565 5d0a 2020 2020 2020 2020 2020 2020  ue].            
-000197e0: 2020 2020 6966 2073 656c 662e 5f66 6561      if self._fea
-000197f0: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
-00019800: 2020 2020 2020 656c 7365 205b 5d0a 2020        else [].  
-00019810: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00019820: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00019830: 7469 7374 6963 735f 636f 6e66 6967 203d  tistics_config =
-00019840: 2073 7461 7469 7374 6963 735f 636f 6e66   statistics_conf
-00019850: 6967 0a0a 2020 2020 2020 2020 2020 2020  ig..            
-00019860: 7365 6c66 2e5f 6f70 7469 6f6e 7320 3d20  self._options = 
-00019870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019880: 2020 7b6f 7074 696f 6e5b 226e 616d 6522    {option["name"
-00019890: 5d3a 206f 7074 696f 6e5b 2276 616c 7565  ]: option["value
-000198a0: 225d 2066 6f72 206f 7074 696f 6e20 696e  "] for option in
-000198b0: 206f 7074 696f 6e73 7d0a 2020 2020 2020   options}.      
-000198c0: 2020 2020 2020 2020 2020 6966 206f 7074            if opt
-000198d0: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
-000198e0: 2020 2020 2065 6c73 6520 4e6f 6e65 0a20       else None. 
-000198f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00019900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00019910: 2020 2020 2020 2073 656c 662e 7072 696d         self.prim
-00019920: 6172 795f 6b65 7920 3d20 7072 696d 6172  ary_key = primar
-00019930: 795f 6b65 790a 2020 2020 2020 2020 2020  y_key.          
-00019940: 2020 7365 6c66 2e73 7461 7469 7374 6963    self.statistic
-00019950: 735f 636f 6e66 6967 203d 2073 7461 7469  s_config = stati
-00019960: 7374 6963 735f 636f 6e66 6967 0a20 2020  stics_config.   
-00019970: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
-00019980: 6561 7475 7265 7320 3d20 6665 6174 7572  eatures = featur
-00019990: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
-000199a0: 656c 662e 5f6f 7074 696f 6e73 203d 206f  elf._options = o
-000199b0: 7074 696f 6e73 0a0a 2020 2020 2020 2020  ptions..        
-000199c0: 6966 2073 746f 7261 6765 5f63 6f6e 6e65  if storage_conne
-000199d0: 6374 6f72 2069 7320 6e6f 7420 4e6f 6e65  ctor is not None
-000199e0: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
-000199f0: 7374 6f72 6167 655f 636f 6e6e 6563 746f  storage_connecto
-00019a00: 722c 2064 6963 7429 3a0a 2020 2020 2020  r, dict):.      
-00019a10: 2020 2020 2020 7365 6c66 2e5f 7374 6f72        self._stor
-00019a20: 6167 655f 636f 6e6e 6563 746f 7220 3d20  age_connector = 
-00019a30: 7363 2e53 746f 7261 6765 436f 6e6e 6563  sc.StorageConnec
-00019a40: 746f 722e 6672 6f6d 5f72 6573 706f 6e73  tor.from_respons
-00019a50: 655f 6a73 6f6e 280a 2020 2020 2020 2020  e_json(.        
-00019a60: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-00019a70: 636f 6e6e 6563 746f 720a 2020 2020 2020  connector.      
-00019a80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00019a90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00019aa0: 2020 7365 6c66 2e5f 7374 6f72 6167 655f    self._storage_
-00019ab0: 636f 6e6e 6563 746f 7220 3d20 7374 6f72  connector = stor
-00019ac0: 6167 655f 636f 6e6e 6563 746f 720a 0a20  age_connector.. 
-00019ad0: 2020 2020 2020 2073 656c 662e 5f68 7265         self._hre
-00019ae0: 6620 3d20 6872 6566 0a0a 2020 2020 6465  f = href..    de
-00019af0: 6620 7361 7665 2873 656c 6629 3a0a 2020  f save(self):.  
-00019b00: 2020 2020 2020 2222 2250 6572 7369 7374        """Persist
-00019b10: 2074 6865 206d 6574 6164 6174 6120 666f   the metadata fo
-00019b20: 7220 7468 6973 2065 7874 6572 6e61 6c20  r this external 
-00019b30: 6665 6174 7572 6520 6772 6f75 702e 0a0a  feature group...
-00019b40: 2020 2020 2020 2020 5769 7468 6f75 7420          Without 
-00019b50: 6361 6c6c 696e 6720 7468 6973 206d 6574  calling this met
-00019b60: 686f 642c 2079 6f75 7220 6665 6174 7572  hod, your featur
-00019b70: 6520 6772 6f75 7020 7769 6c6c 206f 6e6c  e group will onl
-00019b80: 7920 6578 6973 740a 2020 2020 2020 2020  y exist.        
-00019b90: 696e 2079 6f75 7220 5079 7468 6f6e 204b  in your Python K
-00019ba0: 6572 6e65 6c2c 2062 7574 206e 6f74 2069  ernel, but not i
-00019bb0: 6e20 486f 7073 776f 726b 732e 0a0a 2020  n Hopsworks...  
-00019bc0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00019bd0: 2020 2020 2020 2020 7175 6572 7920 3d20          query = 
-00019be0: 2253 454c 4543 5420 2a20 4652 4f4d 2073  "SELECT * FROM s
-00019bf0: 616c 6573 220a 0a20 2020 2020 2020 2066  ales"..        f
-00019c00: 6720 3d20 6665 6174 7572 655f 7374 6f72  g = feature_stor
-00019c10: 652e 6372 6561 7465 5f65 7874 6572 6e61  e.create_externa
-00019c20: 6c5f 6665 6174 7572 655f 6772 6f75 7028  l_feature_group(
-00019c30: 6e61 6d65 3d22 7361 6c65 7322 2c0a 2020  name="sales",.  
-00019c40: 2020 2020 2020 2020 2020 7665 7273 696f            versio
-00019c50: 6e3d 312c 0a20 2020 2020 2020 2020 2020  n=1,.           
-00019c60: 2064 6573 6372 6970 7469 6f6e 3d22 5068   description="Ph
-00019c70: 7973 6963 616c 2073 686f 7020 7361 6c65  ysical shop sale
-00019c80: 7320 6665 6174 7572 6573 222c 0a20 2020  s features",.   
-00019c90: 2020 2020 2020 2020 2071 7565 7279 3d71           query=q
-00019ca0: 7565 7279 2c0a 2020 2020 2020 2020 2020  uery,.          
-00019cb0: 2020 7374 6f72 6167 655f 636f 6e6e 6563    storage_connec
-00019cc0: 746f 723d 636f 6e6e 6563 746f 722c 0a20  tor=connector,. 
-00019cd0: 2020 2020 2020 2020 2020 2070 7269 6d61             prima
-00019ce0: 7279 5f6b 6579 3d5b 2773 735f 7374 6f72  ry_key=['ss_stor
-00019cf0: 655f 736b 275d 2c0a 2020 2020 2020 2020  e_sk'],.        
-00019d00: 2020 2020 6576 656e 745f 7469 6d65 3d27      event_time='
-00019d10: 7361 6c65 5f64 6174 6527 0a20 2020 2020  sale_date'.     
-00019d20: 2020 2029 0a0a 2020 2020 2020 2020 6667     )..        fg
-00019d30: 2e73 6176 6528 290a 2020 2020 2020 2020  .save().        
-00019d40: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00019d50: 2e5f 6665 6174 7572 655f 6772 6f75 705f  ._feature_group_
-00019d60: 656e 6769 6e65 2e73 6176 6528 7365 6c66  engine.save(self
-00019d70: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00019d80: 636f 6465 5f65 6e67 696e 652e 7361 7665  code_engine.save
-00019d90: 5f63 6f64 6528 7365 6c66 290a 0a20 2020  _code(self)..   
-00019da0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00019db0: 7469 7374 6963 735f 636f 6e66 6967 2e65  tistics_config.e
-00019dc0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-00019dd0: 2020 2020 7365 6c66 2e5f 7374 6174 6973      self._statis
-00019de0: 7469 6373 5f65 6e67 696e 652e 636f 6d70  tics_engine.comp
-00019df0: 7574 655f 7374 6174 6973 7469 6373 2873  ute_statistics(s
-00019e00: 656c 6629 0a0a 2020 2020 6465 6620 696e  elf)..    def in
-00019e10: 7365 7274 280a 2020 2020 2020 2020 7365  sert(.        se
-00019e20: 6c66 2c0a 2020 2020 2020 2020 6665 6174  lf,.        feat
-00019e30: 7572 6573 3a20 556e 696f 6e5b 0a20 2020  ures: Union[.   
-00019e40: 2020 2020 2020 2020 2070 642e 4461 7461           pd.Data
-00019e50: 4672 616d 652c 0a20 2020 2020 2020 2020  Frame,.         
-00019e60: 2020 2054 7970 6556 6172 2822 7079 7370     TypeVar("pysp
-00019e70: 6172 6b2e 7371 6c2e 4461 7461 4672 616d  ark.sql.DataFram
-00019e80: 6522 292c 2020 2320 6e6f 7161 3a20 4638  e"),  # noqa: F8
-00019e90: 3231 0a20 2020 2020 2020 2020 2020 2054  21.            T
-00019ea0: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
-00019eb0: 5244 4422 292c 2020 2320 6e6f 7161 3a20  RDD"),  # noqa: 
-00019ec0: 4638 3231 0a20 2020 2020 2020 2020 2020  F821.           
-00019ed0: 206e 702e 6e64 6172 7261 792c 0a20 2020   np.ndarray,.   
-00019ee0: 2020 2020 2020 2020 204c 6973 745b 6c69           List[li
-00019ef0: 7374 5d2c 0a20 2020 2020 2020 205d 2c0a  st],.        ],.
-00019f00: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-00019f10: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00019f20: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-00019f30: 3d20 7b7d 2c0a 2020 2020 2020 2020 7661  = {},.        va
-00019f40: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-00019f50: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00019f60: 7374 722c 2041 6e79 5d5d 203d 207b 7d2c  str, Any]] = {},
-00019f70: 0a20 2020 2020 2020 2073 6176 655f 636f  .        save_co
-00019f80: 6465 3a20 4f70 7469 6f6e 616c 5b62 6f6f  de: Optional[boo
-00019f90: 6c5d 203d 2054 7275 652c 0a20 2020 2020  l] = True,.     
-00019fa0: 2020 2077 6169 743a 2062 6f6f 6c20 3d20     wait: bool = 
-00019fb0: 4661 6c73 652c 0a20 2020 2029 202d 3e20  False,.    ) -> 
-00019fc0: 5475 706c 655b 4f70 7469 6f6e 616c 5b4a  Tuple[Optional[J
-00019fd0: 6f62 5d2c 204f 7074 696f 6e61 6c5b 5661  ob], Optional[Va
-00019fe0: 6c69 6461 7469 6f6e 5265 706f 7274 5d5d  lidationReport]]
-00019ff0: 3a0a 2020 2020 2020 2020 6665 6174 7572  :.        featur
-0001a000: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
-0001a010: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
-0001a020: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
-0001a030: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
-0001a040: 2866 6561 7475 7265 7329 0a0a 2020 2020  (features)..    
-0001a050: 2020 2020 6966 2077 7269 7465 5f6f 7074      if write_opt
-0001a060: 696f 6e73 2069 7320 4e6f 6e65 3a0a 2020  ions is None:.  
-0001a070: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-0001a080: 6f70 7469 6f6e 7320 3d20 7b7d 0a20 2020  options = {}.   
-0001a090: 2020 2020 2069 6620 2277 6169 745f 666f       if "wait_fo
-0001a0a0: 725f 6a6f 6222 206e 6f74 2069 6e20 7772  r_job" not in wr
-0001a0b0: 6974 655f 6f70 7469 6f6e 733a 0a20 2020  ite_options:.   
-0001a0c0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-0001a0d0: 7074 696f 6e73 5b22 7761 6974 5f66 6f72  ptions["wait_for
-0001a0e0: 5f6a 6f62 225d 203d 2077 6169 740a 0a20  _job"] = wait.. 
-0001a0f0: 2020 2020 2020 206a 6f62 2c20 6765 5f72         job, ge_r
-0001a100: 6570 6f72 7420 3d20 7365 6c66 2e5f 6665  eport = self._fe
-0001a110: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-0001a120: 6e65 2e69 6e73 6572 7428 0a20 2020 2020  ne.insert(.     
-0001a130: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0001a140: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-0001a150: 5f64 6174 6166 7261 6d65 3d66 6561 7475  _dataframe=featu
-0001a160: 7265 5f64 6174 6166 7261 6d65 2c0a 2020  re_dataframe,.  
-0001a170: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-0001a180: 6f70 7469 6f6e 733d 7772 6974 655f 6f70  options=write_op
-0001a190: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-0001a1a0: 2020 2076 616c 6964 6174 696f 6e5f 6f70     validation_op
-0001a1b0: 7469 6f6e 733d 7b22 7361 7665 5f72 6570  tions={"save_rep
-0001a1c0: 6f72 7422 3a20 5472 7565 2c20 2a2a 7661  ort": True, **va
-0001a1d0: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-0001a1e0: 7d2c 0a20 2020 2020 2020 2029 0a0a 2020  },.        )..  
-0001a1f0: 2020 2020 2020 6966 2073 6176 655f 636f        if save_co
-0001a200: 6465 2061 6e64 2028 0a20 2020 2020 2020  de and (.       
-0001a210: 2020 2020 2067 655f 7265 706f 7274 2069       ge_report i
-0001a220: 7320 4e6f 6e65 206f 7220 6765 5f72 6570  s None or ge_rep
-0001a230: 6f72 742e 696e 6765 7374 696f 6e5f 7265  ort.ingestion_re
-0001a240: 7375 6c74 203d 3d20 2249 4e47 4553 5445  sult == "INGESTE
-0001a250: 4422 0a20 2020 2020 2020 2029 3a0a 2020  D".        ):.  
-0001a260: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001a270: 636f 6465 5f65 6e67 696e 652e 7361 7665  code_engine.save
-0001a280: 5f63 6f64 6528 7365 6c66 290a 0a20 2020  _code(self)..   
-0001a290: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0001a2a0: 7469 7374 6963 735f 636f 6e66 6967 2e65  tistics_config.e
-0001a2b0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-0001a2c0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-0001a2d0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-0001a2e0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-0001a2f0: 2020 2020 2020 2020 2022 5374 6174 6973           "Statis
-0001a300: 7469 6373 2061 7265 206e 6f74 2063 6f6d  tics are not com
-0001a310: 7075 7465 6420 666f 7220 696e 7365 7274  puted for insert
-0001a320: 696f 6e20 746f 206f 6e6c 696e 6520 656e  ion to online en
-0001a330: 6162 6c65 6420 6578 7465 726e 616c 2066  abled external f
-0001a340: 6561 7475 7265 2067 726f 7570 2060 7b7d  eature group `{}
-0001a350: 602c 2077 6974 6820 7665 7273 696f 6e22  `, with version"
-0001a360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a370: 2020 2020 2022 2060 7b7d 602e 2043 616c       " `{}`. Cal
-0001a380: 6c20 6063 6f6d 7075 7465 5f73 7461 7469  l `compute_stati
-0001a390: 7374 6963 7360 2065 7870 6c69 6369 746c  stics` explicitl
-0001a3a0: 7920 746f 2063 6f6d 7075 7465 2073 7461  y to compute sta
-0001a3b0: 7469 7374 6963 7320 6f76 6572 2074 6865  tistics over the
-0001a3c0: 2064 6174 6120 696e 2074 6865 2065 7874   data in the ext
-0001a3d0: 6572 6e61 6c20 7374 6f72 6167 6520 7379  ernal storage sy
-0001a3e0: 7374 656d 2e22 0a20 2020 2020 2020 2020  stem.".         
-0001a3f0: 2020 2020 2020 2029 2e66 6f72 6d61 7428         ).format(
-0001a400: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
-0001a410: 2e5f 7665 7273 696f 6e29 2c0a 2020 2020  ._version),.    
-0001a420: 2020 2020 2020 2020 2020 2020 7574 696c              util
-0001a430: 2e53 746f 7261 6765 5761 726e 696e 672c  .StorageWarning,
-0001a440: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0001a450: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0001a460: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0001a470: 2c0a 2020 2020 2020 2020 2020 2020 6765  ,.            ge
-0001a480: 5f72 6570 6f72 742e 746f 5f67 655f 7479  _report.to_ge_ty
-0001a490: 7065 2829 2069 6620 6765 5f72 6570 6f72  pe() if ge_repor
-0001a4a0: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
-0001a4b0: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
-0001a4c0: 2029 0a0a 2020 2020 6465 6620 7265 6164   )..    def read
-0001a4d0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0001a4e0: 6461 7461 6672 616d 655f 7479 7065 3a20  dataframe_type: 
-0001a4f0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0001a500: 2264 6566 6175 6c74 222c 206f 6e6c 696e  "default", onlin
-0001a510: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
-0001a520: 5d20 3d20 4661 6c73 650a 2020 2020 293a  ] = False.    ):
-0001a530: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0001a540: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-0001a550: 7020 6173 2061 2044 6174 6146 7261 6d65  p as a DataFrame
-0001a560: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-0001a570: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-0001a580: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-0001a590: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-0001a5a0: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-0001a5b0: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-0001a5c0: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
-0001a5d0: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-0001a5e0: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
-0001a5f0: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
-0001a600: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
-0001a610: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-0001a620: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-0001a630: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
-0001a640: 3d20 6667 2e72 6561 6428 290a 2020 2020  = fg.read().    
-0001a650: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-0001a660: 2020 2020 2021 2121 2077 6172 6e69 6e67       !!! warning
-0001a670: 2022 456e 6769 6e65 2053 7570 706f 7274   "Engine Support
-0001a680: 220a 2020 2020 2020 2020 2020 2020 2a2a  ".            **
-0001a690: 5370 6172 6b20 6f6e 6c79 2a2a 0a0a 2020  Spark only**..  
-0001a6a0: 2020 2020 2020 2020 2020 5265 6164 696e            Readin
-0001a6b0: 6720 616e 2045 7874 6572 6e61 6c20 4665  g an External Fe
-0001a6c0: 6174 7572 6520 4772 6f75 7020 6469 7265  ature Group dire
-0001a6d0: 6374 6c79 2069 6e74 6f20 6120 5061 6e64  ctly into a Pand
-0001a6e0: 6173 2044 6174 6166 7261 6d65 2075 7369  as Dataframe usi
-0001a6f0: 6e67 0a20 2020 2020 2020 2020 2020 2050  ng.            P
-0001a700: 7974 686f 6e2f 5061 6e64 6173 2061 7320  ython/Pandas as 
-0001a710: 456e 6769 6e65 2069 7320 6e6f 7420 7375  Engine is not su
-0001a720: 7070 6f72 7465 642c 2068 6f77 6576 6572  pported, however
-0001a730: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
-0001a740: 650a 2020 2020 2020 2020 2020 2020 5175  e.            Qu
-0001a750: 6572 7920 4150 4920 746f 2063 7265 6174  ery API to creat
-0001a760: 6520 4665 6174 7572 6520 5669 6577 732f  e Feature Views/
-0001a770: 5472 6169 6e69 6e67 2044 6174 6120 636f  Training Data co
-0001a780: 6e74 6169 6e69 6e67 2045 7874 6572 6e61  ntaining Externa
-0001a790: 6c0a 2020 2020 2020 2020 2020 2020 4665  l.            Fe
-0001a7a0: 6174 7572 6520 4772 6f75 7073 2e0a 0a20  ature Groups... 
-0001a7b0: 2020 2020 2020 2023 2041 7267 756d 656e         # Argumen
-0001a7c0: 7473 0a20 2020 2020 2020 2020 2020 2064  ts.            d
-0001a7d0: 6174 6166 7261 6d65 5f74 7970 653a 2073  ataframe_type: s
-0001a7e0: 7472 2c20 6f70 7469 6f6e 616c 2e20 506f  tr, optional. Po
-0001a7f0: 7373 6962 6c65 2076 616c 7565 7320 6172  ssible values ar
-0001a800: 6520 6022 6465 6661 756c 7422 602c 2060  e `"default"`, `
-0001a810: 2273 7061 726b 2260 2c0a 2020 2020 2020  "spark"`,.      
-0001a820: 2020 2020 2020 2020 2020 6022 7061 6e64            `"pand
-0001a830: 6173 2260 2c20 6022 6e75 6d70 7922 6020  as"`, `"numpy"` 
-0001a840: 6f72 2060 2270 7974 686f 6e22 602c 2064  or `"python"`, d
-0001a850: 6566 6175 6c74 7320 746f 2060 2264 6566  efaults to `"def
-0001a860: 6175 6c74 2260 2e0a 2020 2020 2020 2020  ault"`..        
-0001a870: 2020 2020 6f6e 6c69 6e65 3a20 626f 6f6c      online: bool
-0001a880: 2c20 6f70 7469 6f6e 616c 2e20 4966 2060  , optional. If `
-0001a890: 5472 7565 6020 7265 6164 2066 726f 6d20  True` read from 
-0001a8a0: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-0001a8b0: 746f 7265 2c20 6465 6661 756c 7473 0a20  tore, defaults. 
-0001a8c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001a8d0: 6f20 6046 616c 7365 602e 0a0a 2020 2020  o `False`...    
-0001a8e0: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
-0001a8f0: 2020 2020 2020 2020 2020 6044 6174 6146            `DataF
-0001a900: 7261 6d65 603a 2054 6865 2073 7061 726b  rame`: The spark
-0001a910: 2064 6174 6166 7261 6d65 2063 6f6e 7461   dataframe conta
-0001a920: 696e 696e 6720 7468 6520 6665 6174 7572  ining the featur
-0001a930: 6520 6461 7461 2e0a 2020 2020 2020 2020  e data..        
-0001a940: 2020 2020 6070 7973 7061 726b 2e44 6174      `pyspark.Dat
-0001a950: 6146 7261 6d65 602e 2041 2053 7061 726b  aFrame`. A Spark
-0001a960: 2044 6174 6146 7261 6d65 2e0a 2020 2020   DataFrame..    
-0001a970: 2020 2020 2020 2020 6070 616e 6461 732e          `pandas.
-0001a980: 4461 7461 4672 616d 6560 2e20 4120 5061  DataFrame`. A Pa
-0001a990: 6e64 6173 2044 6174 6146 7261 6d65 2e0a  ndas DataFrame..
-0001a9a0: 2020 2020 2020 2020 2020 2020 606e 756d              `num
-0001a9b0: 7079 2e6e 6461 7272 6179 602e 2041 2074  py.ndarray`. A t
-0001a9c0: 776f 2d64 696d 656e 7369 6f6e 616c 204e  wo-dimensional N
-0001a9d0: 756d 7079 2061 7272 6179 2e0a 2020 2020  umpy array..    
-0001a9e0: 2020 2020 2020 2020 606c 6973 7460 2e20          `list`. 
-0001a9f0: 4120 7477 6f2d 6469 6d65 6e73 696f 6e61  A two-dimensiona
-0001aa00: 6c20 5079 7468 6f6e 206c 6973 742e 0a0a  l Python list...
-0001aa10: 2020 2020 2020 2020 2320 5261 6973 6573          # Raises
-0001aa20: 0a20 2020 2020 2020 2020 2020 2060 6873  .            `hs
-0001aa30: 6673 2e63 6c69 656e 742e 6578 6365 7074  fs.client.except
-0001aa40: 696f 6e73 2e52 6573 7441 5049 4572 726f  ions.RestAPIErro
-0001aa50: 7260 2e0a 2020 2020 2020 2020 2222 220a  r`..        """.
-0001aa60: 2020 2020 2020 2020 6966 2065 6e67 696e          if engin
-0001aa70: 652e 6765 745f 7479 7065 2829 203d 3d20  e.get_type() == 
-0001aa80: 2270 7974 686f 6e22 2061 6e64 206e 6f74  "python" and not
-0001aa90: 206f 6e6c 696e 653a 0a20 2020 2020 2020   online:.       
-0001aaa0: 2020 2020 2072 6169 7365 2046 6561 7475       raise Featu
-0001aab0: 7265 5374 6f72 6545 7863 6570 7469 6f6e  reStoreException
-0001aac0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001aad0: 2020 2252 6561 6469 6e67 2061 6e20 4578    "Reading an Ex
-0001aae0: 7465 726e 616c 2046 6561 7475 7265 2047  ternal Feature G
-0001aaf0: 726f 7570 2064 6972 6563 746c 7920 696e  roup directly in
-0001ab00: 746f 2061 2050 616e 6461 7320 4461 7461  to a Pandas Data
-0001ab10: 6672 616d 6520 7573 696e 6720 220a 2020  frame using ".  
-0001ab20: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001ab30: 2250 7974 686f 6e2f 5061 6e64 6173 2061  "Python/Pandas a
-0001ab40: 7320 456e 6769 6e65 2066 726f 6d20 7468  s Engine from th
-0001ab50: 6520 6578 7465 726e 616c 2073 746f 7261  e external stora
-0001ab60: 6765 2073 7973 7465 6d20 220a 2020 2020  ge system ".    
-0001ab70: 2020 2020 2020 2020 2020 2020 2b20 2269              + "i
-0001ab80: 7320 6e6f 7420 7375 7070 6f72 7465 642c  s not supported,
-0001ab90: 2068 6f77 6576 6572 2c20 6966 2074 6865   however, if the
-0001aba0: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-0001abb0: 7320 6f6e 6c69 6e65 2065 6e61 626c 6564  s online enabled
-0001abc0: 2c20 796f 7520 6361 6e20 7265 6164 2022  , you can read "
-0001abd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001abe0: 202b 2022 6672 6f6d 206f 6e6c 696e 6520   + "from online 
-0001abf0: 7374 6f72 6167 6520 6f72 2079 6f75 2063  storage or you c
-0001ac00: 616e 2075 7365 2074 6865 2022 0a20 2020  an use the ".   
-0001ac10: 2020 2020 2020 2020 2020 2020 202b 2022               + "
-0001ac20: 5175 6572 7920 4150 4920 746f 2063 7265  Query API to cre
-0001ac30: 6174 6520 4665 6174 7572 6520 5669 6577  ate Feature View
-0001ac40: 732f 5472 6169 6e69 6e67 2044 6174 6120  s/Training Data 
-0001ac50: 636f 6e74 6169 6e69 6e67 2045 7874 6572  containing Exter
-0001ac60: 6e61 6c20 220a 2020 2020 2020 2020 2020  nal ".          
-0001ac70: 2020 2020 2020 2b20 2246 6561 7475 7265        + "Feature
-0001ac80: 2047 726f 7570 732e 220a 2020 2020 2020   Groups.".      
-0001ac90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001aca0: 656e 6769 6e65 2e67 6574 5f69 6e73 7461  engine.get_insta
-0001acb0: 6e63 6528 292e 7365 745f 6a6f 625f 6772  nce().set_job_gr
-0001acc0: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
-0001acd0: 2022 4665 7463 6869 6e67 2046 6561 7475   "Fetching Featu
-0001ace0: 7265 2067 726f 7570 222c 0a20 2020 2020  re group",.     
-0001acf0: 2020 2020 2020 2022 4765 7474 696e 6720         "Getting 
-0001ad00: 6665 6174 7572 6520 6772 6f75 703a 207b  feature group: {
-0001ad10: 7d20 6672 6f6d 2074 6865 2066 6561 7475  } from the featu
-0001ad20: 7265 7374 6f72 6520 7b7d 222e 666f 726d  restore {}".form
-0001ad30: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-0001ad40: 2020 2020 7365 6c66 2e5f 6e61 6d65 2c20      self._name, 
-0001ad50: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
-0001ad60: 6f72 655f 6e61 6d65 0a20 2020 2020 2020  ore_name.       
-0001ad70: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-0001ad80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001ad90: 2073 656c 662e 7365 6c65 6374 5f61 6c6c   self.select_all
-0001ada0: 2829 2e72 6561 6428 6461 7461 6672 616d  ().read(datafram
-0001adb0: 655f 7479 7065 3d64 6174 6166 7261 6d65  e_type=dataframe
-0001adc0: 5f74 7970 652c 206f 6e6c 696e 653d 6f6e  _type, online=on
-0001add0: 6c69 6e65 290a 0a20 2020 2064 6566 2073  line)..    def s
-0001ade0: 686f 7728 7365 6c66 2c20 6e29 3a0a 2020  how(self, n):.  
-0001adf0: 2020 2020 2020 2222 2253 686f 7720 7468        """Show th
-0001ae00: 6520 6669 7273 7420 6e20 726f 7773 206f  e first n rows o
-0001ae10: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-0001ae20: 6f75 702e 0a0a 2020 2020 2020 2020 2121  oup...        !!
-0001ae30: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
-0001ae40: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-0001ae50: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-0001ae60: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-0001ae70: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-0001ae80: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-0001ae90: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-0001aea0: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
-0001aeb0: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-0001aec0: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-0001aed0: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-0001aee0: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-0001aef0: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
-0001af00: 6667 2e73 686f 7728 3529 0a20 2020 2020  fg.show(5).     
-0001af10: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-0001af20: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
-0001af30: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
-0001af40: 6365 2829 2e73 6574 5f6a 6f62 5f67 726f  ce().set_job_gro
-0001af50: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
-0001af60: 2246 6574 6368 696e 6720 4665 6174 7572  "Fetching Featur
-0001af70: 6520 6772 6f75 7022 2c0a 2020 2020 2020  e group",.      
-0001af80: 2020 2020 2020 2247 6574 7469 6e67 2066        "Getting f
-0001af90: 6561 7475 7265 2067 726f 7570 3a20 7b7d  eature group: {}
-0001afa0: 2066 726f 6d20 7468 6520 6665 6174 7572   from the featur
-0001afb0: 6573 746f 7265 207b 7d22 2e66 6f72 6d61  estore {}".forma
-0001afc0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0001afd0: 2020 2073 656c 662e 5f6e 616d 652c 2073     self._name, s
-0001afe0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
-0001aff0: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
-0001b000: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
-0001b010: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001b020: 7365 6c66 2e73 656c 6563 745f 616c 6c28  self.select_all(
-0001b030: 292e 7368 6f77 286e 290a 0a20 2020 2040  ).show(n)..    @
-0001b040: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-0001b050: 6465 6620 6672 6f6d 5f72 6573 706f 6e73  def from_respons
-0001b060: 655f 6a73 6f6e 2863 6c73 2c20 6a73 6f6e  e_json(cls, json
-0001b070: 5f64 6963 7429 3a0a 2020 2020 2020 2020  _dict):.        
-0001b080: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-0001b090: 203d 2068 756d 7073 2e64 6563 616d 656c   = humps.decamel
-0001b0a0: 697a 6528 6a73 6f6e 5f64 6963 7429 0a20  ize(json_dict). 
-0001b0b0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0001b0c0: 616e 6365 286a 736f 6e5f 6465 6361 6d65  ance(json_decame
-0001b0d0: 6c69 7a65 642c 2064 6963 7429 3a0a 2020  lized, dict):.  
-0001b0e0: 2020 2020 2020 2020 2020 5f20 3d20 6a73            _ = js
-0001b0f0: 6f6e 5f64 6563 616d 656c 697a 6564 2e70  on_decamelized.p
-0001b100: 6f70 2822 7479 7065 222c 204e 6f6e 6529  op("type", None)
-0001b110: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001b120: 7572 6e20 636c 7328 2a2a 6a73 6f6e 5f64  urn cls(**json_d
-0001b130: 6563 616d 656c 697a 6564 290a 2020 2020  ecamelized).    
-0001b140: 2020 2020 666f 7220 6667 2069 6e20 6a73      for fg in js
-0001b150: 6f6e 5f64 6563 616d 656c 697a 6564 3a0a  on_decamelized:.
-0001b160: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
-0001b170: 6667 2e70 6f70 2822 7479 7065 222c 204e  fg.pop("type", N
-0001b180: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
-0001b190: 7572 6e20 5b63 6c73 282a 2a66 6729 2066  urn [cls(**fg) f
-0001b1a0: 6f72 2066 6720 696e 206a 736f 6e5f 6465  or fg in json_de
-0001b1b0: 6361 6d65 6c69 7a65 645d 0a0a 2020 2020  camelized]..    
-0001b1c0: 6465 6620 7570 6461 7465 5f66 726f 6d5f  def update_from_
-0001b1d0: 7265 7370 6f6e 7365 5f6a 736f 6e28 7365  response_json(se
-0001b1e0: 6c66 2c20 6a73 6f6e 5f64 6963 7429 3a0a  lf, json_dict):.
-0001b1f0: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
-0001b200: 616d 656c 697a 6564 203d 2068 756d 7073  amelized = humps
-0001b210: 2e64 6563 616d 656c 697a 6528 6a73 6f6e  .decamelize(json
-0001b220: 5f64 6963 7429 0a20 2020 2020 2020 2069  _dict).        i
-0001b230: 6620 2274 7970 6522 2069 6e20 6a73 6f6e  f "type" in json
-0001b240: 5f64 6563 616d 656c 697a 6564 3a0a 2020  _decamelized:.  
-0001b250: 2020 2020 2020 2020 2020 5f20 3d20 6a73            _ = js
-0001b260: 6f6e 5f64 6563 616d 656c 697a 6564 2e70  on_decamelized.p
-0001b270: 6f70 2822 7479 7065 2229 0a20 2020 2020  op("type").     
-0001b280: 2020 2073 656c 662e 5f5f 696e 6974 5f5f     self.__init__
-0001b290: 282a 2a6a 736f 6e5f 6465 6361 6d65 6c69  (**json_decameli
-0001b2a0: 7a65 6429 0a20 2020 2020 2020 2072 6574  zed).        ret
-0001b2b0: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-0001b2c0: 6620 6a73 6f6e 2873 656c 6629 3a0a 2020  f json(self):.  
-0001b2d0: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
-0001b2e0: 6e2e 6475 6d70 7328 7365 6c66 2c20 636c  n.dumps(self, cl
-0001b2f0: 733d 7574 696c 2e46 6561 7475 7265 5374  s=util.FeatureSt
-0001b300: 6f72 6545 6e63 6f64 6572 290a 0a20 2020  oreEncoder)..   
-0001b310: 2064 6566 2074 6f5f 6469 6374 2873 656c   def to_dict(sel
-0001b320: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-0001b330: 726e 207b 0a20 2020 2020 2020 2020 2020  rn {.           
-0001b340: 2022 6964 223a 2073 656c 662e 5f69 642c   "id": self._id,
-0001b350: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
-0001b360: 6d65 223a 2073 656c 662e 5f6e 616d 652c  me": self._name,
-0001b370: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-0001b380: 7363 7269 7074 696f 6e22 3a20 7365 6c66  scription": self
-0001b390: 2e5f 6465 7363 7269 7074 696f 6e2c 0a20  ._description,. 
-0001b3a0: 2020 2020 2020 2020 2020 2022 7665 7273             "vers
-0001b3b0: 696f 6e22 3a20 7365 6c66 2e5f 7665 7273  ion": self._vers
-0001b3c0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-0001b3d0: 2022 6665 6174 7572 6573 223a 2073 656c   "features": sel
-0001b3e0: 662e 5f66 6561 7475 7265 732c 0a20 2020  f._features,.   
-0001b3f0: 2020 2020 2020 2020 2022 6665 6174 7572           "featur
-0001b400: 6573 746f 7265 4964 223a 2073 656c 662e  estoreId": self.
-0001b410: 5f66 6561 7475 7265 5f73 746f 7265 5f69  _feature_store_i
-0001b420: 642c 0a20 2020 2020 2020 2020 2020 2022  d,.            "
-0001b430: 7175 6572 7922 3a20 7365 6c66 2e5f 7175  query": self._qu
-0001b440: 6572 792c 0a20 2020 2020 2020 2020 2020  ery,.           
-0001b450: 2022 6461 7461 466f 726d 6174 223a 2073   "dataFormat": s
-0001b460: 656c 662e 5f64 6174 615f 666f 726d 6174  elf._data_format
-0001b470: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
-0001b480: 6174 6822 3a20 7365 6c66 2e5f 7061 7468  ath": self._path
-0001b490: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
-0001b4a0: 7074 696f 6e73 223a 205b 7b22 6e61 6d65  ptions": [{"name
-0001b4b0: 223a 206b 2c20 2276 616c 7565 223a 2076  ": k, "value": v
-0001b4c0: 7d20 666f 7220 6b2c 2076 2069 6e20 7365  } for k, v in se
-0001b4d0: 6c66 2e5f 6f70 7469 6f6e 732e 6974 656d  lf._options.item
-0001b4e0: 7328 295d 0a20 2020 2020 2020 2020 2020  s()].           
-0001b4f0: 2069 6620 7365 6c66 2e5f 6f70 7469 6f6e   if self._option
-0001b500: 730a 2020 2020 2020 2020 2020 2020 656c  s.            el
-0001b510: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
-0001b520: 2020 2020 2022 7374 6f72 6167 6543 6f6e       "storageCon
-0001b530: 6e65 6374 6f72 223a 2073 656c 662e 5f73  nector": self._s
-0001b540: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
-0001b550: 2e74 6f5f 6469 6374 2829 2c0a 2020 2020  .to_dict(),.    
-0001b560: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-0001b570: 226f 6e44 656d 616e 6446 6561 7475 7265  "onDemandFeature
-0001b580: 6772 6f75 7044 544f 222c 0a20 2020 2020  groupDTO",.     
-0001b590: 2020 2020 2020 2022 7374 6174 6973 7469         "statisti
-0001b5a0: 6373 436f 6e66 6967 223a 2073 656c 662e  csConfig": self.
-0001b5b0: 5f73 7461 7469 7374 6963 735f 636f 6e66  _statistics_conf
-0001b5c0: 6967 2c0a 2020 2020 2020 2020 2020 2020  ig,.            
-0001b5d0: 2265 7665 6e74 5469 6d65 223a 2073 656c  "eventTime": sel
-0001b5e0: 662e 5f65 7665 6e74 5f74 696d 652c 0a20  f._event_time,. 
-0001b5f0: 2020 2020 2020 2020 2020 2022 6578 7065             "expe
-0001b600: 6374 6174 696f 6e53 7569 7465 223a 2073  ctationSuite": s
-0001b610: 656c 662e 5f65 7870 6563 7461 7469 6f6e  elf._expectation
-0001b620: 5f73 7569 7465 2c0a 2020 2020 2020 2020  _suite,.        
-0001b630: 2020 2020 226f 6e6c 696e 6545 6e61 626c      "onlineEnabl
-0001b640: 6564 223a 2073 656c 662e 5f6f 6e6c 696e  ed": self._onlin
-0001b650: 655f 656e 6162 6c65 642c 0a20 2020 2020  e_enabled,.     
-0001b660: 2020 2020 2020 2022 7370 696e 6522 3a20         "spine": 
-0001b670: 4661 6c73 652c 0a20 2020 2020 2020 207d  False,.        }
-0001b680: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0001b690: 2020 2020 6465 6620 6964 2873 656c 6629      def id(self)
-0001b6a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001b6b0: 2073 656c 662e 5f69 640a 0a20 2020 2040   self._id..    @
-0001b6c0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0001b6d0: 206e 616d 6528 7365 6c66 293a 0a20 2020   name(self):.   
-0001b6e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001b6f0: 2e5f 6e61 6d65 0a0a 2020 2020 4070 726f  ._name..    @pro
-0001b700: 7065 7274 790a 2020 2020 6465 6620 7665  perty.    def ve
-0001b710: 7273 696f 6e28 7365 6c66 293a 0a20 2020  rsion(self):.   
-0001b720: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001b730: 2e5f 7665 7273 696f 6e0a 0a20 2020 2040  ._version..    @
-0001b740: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0001b750: 2064 6573 6372 6970 7469 6f6e 2873 656c   description(sel
-0001b760: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-0001b770: 726e 2073 656c 662e 5f64 6573 6372 6970  rn self._descrip
-0001b780: 7469 6f6e 0a0a 2020 2020 4070 726f 7065  tion..    @prope
-0001b790: 7274 790a 2020 2020 6465 6620 7175 6572  rty.    def quer
-0001b7a0: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
-0001b7b0: 2072 6574 7572 6e20 7365 6c66 2e5f 7175   return self._qu
-0001b7c0: 6572 790a 0a20 2020 2040 7072 6f70 6572  ery..    @proper
-0001b7d0: 7479 0a20 2020 2064 6566 2064 6174 615f  ty.    def data_
-0001b7e0: 666f 726d 6174 2873 656c 6629 3a0a 2020  format(self):.  
-0001b7f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001b800: 662e 5f64 6174 615f 666f 726d 6174 0a0a  f._data_format..
-0001b810: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0001b820: 2020 6465 6620 7061 7468 2873 656c 6629    def path(self)
-0001b830: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001b840: 2073 656c 662e 5f70 6174 680a 0a20 2020   self._path..   
-0001b850: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0001b860: 6566 206f 7074 696f 6e73 2873 656c 6629  ef options(self)
-0001b870: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001b880: 2073 656c 662e 5f6f 7074 696f 6e73 0a0a   self._options..
-0001b890: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0001b8a0: 2020 6465 6620 7374 6f72 6167 655f 636f    def storage_co
-0001b8b0: 6e6e 6563 746f 7228 7365 6c66 293a 0a20  nnector(self):. 
-0001b8c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001b8d0: 6c66 2e5f 7374 6f72 6167 655f 636f 6e6e  lf._storage_conn
-0001b8e0: 6563 746f 720a 0a20 2020 2040 7072 6f70  ector..    @prop
-0001b8f0: 6572 7479 0a20 2020 2064 6566 2063 7265  erty.    def cre
-0001b900: 6174 6f72 2873 656c 6629 3a0a 2020 2020  ator(self):.    
-0001b910: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001b920: 5f63 7265 6174 6f72 0a0a 2020 2020 4070  _creator..    @p
-0001b930: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0001b940: 6372 6561 7465 6428 7365 6c66 293a 0a20  created(self):. 
-0001b950: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001b960: 6c66 2e5f 6372 6561 7465 640a 0a20 2020  lf._created..   
-0001b970: 2040 7665 7273 696f 6e2e 7365 7474 6572   @version.setter
-0001b980: 0a20 2020 2064 6566 2076 6572 7369 6f6e  .    def version
-0001b990: 2873 656c 662c 2076 6572 7369 6f6e 293a  (self, version):
-0001b9a0: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
-0001b9b0: 6572 7369 6f6e 203d 2076 6572 7369 6f6e  ersion = version
-0001b9c0: 0a0a 2020 2020 4064 6573 6372 6970 7469  ..    @descripti
-0001b9d0: 6f6e 2e73 6574 7465 720a 2020 2020 6465  on.setter.    de
-0001b9e0: 6620 6465 7363 7269 7074 696f 6e28 7365  f description(se
-0001b9f0: 6c66 2c20 6e65 775f 6465 7363 7269 7074  lf, new_descript
-0001ba00: 696f 6e29 3a0a 2020 2020 2020 2020 7365  ion):.        se
-0001ba10: 6c66 2e5f 6465 7363 7269 7074 696f 6e20  lf._description 
-0001ba20: 3d20 6e65 775f 6465 7363 7269 7074 696f  = new_descriptio
-0001ba30: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
-0001ba40: 0a20 2020 2064 6566 2066 6561 7475 7265  .    def feature
-0001ba50: 5f73 746f 7265 5f6e 616d 6528 7365 6c66  _store_name(self
-0001ba60: 293a 0a20 2020 2020 2020 2022 2222 4e61  ):.        """Na
-0001ba70: 6d65 206f 6620 7468 6520 6665 6174 7572  me of the featur
-0001ba80: 6520 7374 6f72 6520 696e 2077 6869 6368  e store in which
-0001ba90: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-0001baa0: 7570 2069 7320 6c6f 6361 7465 642e 2222  up is located.""
-0001bab0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0001bac0: 2073 656c 662e 5f66 6561 7475 7265 5f73   self._feature_s
-0001bad0: 746f 7265 5f6e 616d 650a 0a20 2020 2040  tore_name..    @
-0001bae0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0001baf0: 2066 6561 7475 7265 5f73 746f 7265 5f69   feature_store_i
-0001bb00: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-0001bb10: 2022 2222 4964 206f 6620 7468 6520 6665   """Id of the fe
-0001bb20: 6174 7572 6520 7374 6f72 6520 696e 2077  ature store in w
-0001bb30: 6869 6368 2074 6865 2066 6561 7475 7265  hich the feature
-0001bb40: 2067 726f 7570 2069 7320 6c6f 6361 7465   group is locate
-0001bb50: 642e 2222 220a 2020 2020 2020 2020 7265  d.""".        re
-0001bb60: 7475 726e 2073 656c 662e 5f66 6561 7475  turn self._featu
-0001bb70: 7265 5f73 746f 7265 5f69 640a 0a0a 636c  re_store_id...cl
-0001bb80: 6173 7320 5370 696e 6547 726f 7570 2846  ass SpineGroup(F
-0001bb90: 6561 7475 7265 4772 6f75 7042 6173 6529  eatureGroupBase)
-0001bba0: 3a0a 2020 2020 5350 494e 455f 4752 4f55  :.    SPINE_GROU
-0001bbb0: 5020 3d20 224f 4e5f 4445 4d41 4e44 5f46  P = "ON_DEMAND_F
-0001bbc0: 4541 5455 5245 5f47 524f 5550 220a 2020  EATURE_GROUP".  
-0001bbd0: 2020 454e 5449 5459 5f54 5950 4520 3d20    ENTITY_TYPE = 
-0001bbe0: 2266 6561 7475 7265 6772 6f75 7073 220a  "featuregroups".
-0001bbf0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0001bc00: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0001bc10: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
-0001bc20: 5f63 6f6e 6e65 6374 6f72 3d4e 6f6e 652c  _connector=None,
-0001bc30: 0a20 2020 2020 2020 2071 7565 7279 3d4e  .        query=N
-0001bc40: 6f6e 652c 0a20 2020 2020 2020 2064 6174  one,.        dat
-0001bc50: 615f 666f 726d 6174 3d4e 6f6e 652c 0a20  a_format=None,. 
-0001bc60: 2020 2020 2020 2070 6174 683d 4e6f 6e65         path=None
-0001bc70: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0001bc80: 733d 7b7d 2c0a 2020 2020 2020 2020 6e61  s={},.        na
-0001bc90: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
-0001bca0: 2076 6572 7369 6f6e 3d4e 6f6e 652c 0a20   version=None,. 
-0001bcb0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0001bcc0: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
-0001bcd0: 2070 7269 6d61 7279 5f6b 6579 3d4e 6f6e   primary_key=Non
-0001bce0: 652c 0a20 2020 2020 2020 2066 6561 7475  e,.        featu
-0001bcf0: 7265 7374 6f72 655f 6964 3d4e 6f6e 652c  restore_id=None,
-0001bd00: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
-0001bd10: 7374 6f72 655f 6e61 6d65 3d4e 6f6e 652c  store_name=None,
-0001bd20: 0a20 2020 2020 2020 2063 7265 6174 6564  .        created
-0001bd30: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
-0001bd40: 7265 6174 6f72 3d4e 6f6e 652c 0a20 2020  reator=None,.   
-0001bd50: 2020 2020 2069 643d 4e6f 6e65 2c0a 2020       id=None,.  
-0001bd60: 2020 2020 2020 6665 6174 7572 6573 3d4e        features=N
-0001bd70: 6f6e 652c 0a20 2020 2020 2020 206c 6f63  one,.        loc
-0001bd80: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
-0001bd90: 2020 2020 7374 6174 6973 7469 6373 5f63      statistics_c
-0001bda0: 6f6e 6669 673d 4e6f 6e65 2c0a 2020 2020  onfig=None,.    
-0001bdb0: 2020 2020 6576 656e 745f 7469 6d65 3d4e      event_time=N
-0001bdc0: 6f6e 652c 0a20 2020 2020 2020 2065 7870  one,.        exp
-0001bdd0: 6563 7461 7469 6f6e 5f73 7569 7465 3d4e  ectation_suite=N
-0001bde0: 6f6e 652c 0a20 2020 2020 2020 206f 6e6c  one,.        onl
-0001bdf0: 696e 655f 656e 6162 6c65 643d 4661 6c73  ine_enabled=Fals
-0001be00: 652c 0a20 2020 2020 2020 2068 7265 663d  e,.        href=
-0001be10: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f6e  None,.        on
-0001be20: 6c69 6e65 5f74 6f70 6963 5f6e 616d 653d  line_topic_name=
-0001be30: 4e6f 6e65 2c0a 2020 2020 2020 2020 7370  None,.        sp
-0001be40: 696e 653d 5472 7565 2c0a 2020 2020 2020  ine=True,.      
-0001be50: 2020 6461 7461 6672 616d 653d 2273 7069    dataframe="spi
-0001be60: 6e65 222c 0a20 2020 2029 3a0a 2020 2020  ne",.    ):.    
-0001be70: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0001be80: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
-0001be90: 2020 6665 6174 7572 6573 746f 7265 5f69    featurestore_i
-0001bea0: 642c 0a20 2020 2020 2020 2020 2020 206c  d,.            l
-0001beb0: 6f63 6174 696f 6e2c 0a20 2020 2020 2020  ocation,.       
-0001bec0: 2020 2020 2065 7665 6e74 5f74 696d 653d       event_time=
-0001bed0: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
-0001bee0: 2020 2020 2020 2020 6f6e 6c69 6e65 5f65          online_e
-0001bef0: 6e61 626c 6564 3d6f 6e6c 696e 655f 656e  nabled=online_en
-0001bf00: 6162 6c65 642c 0a20 2020 2020 2020 2020  abled,.         
-0001bf10: 2020 2069 643d 6964 2c0a 2020 2020 2020     id=id,.      
-0001bf20: 2020 2020 2020 6578 7065 6374 6174 696f        expectatio
-0001bf30: 6e5f 7375 6974 653d 6578 7065 6374 6174  n_suite=expectat
-0001bf40: 696f 6e5f 7375 6974 652c 0a20 2020 2020  ion_suite,.     
-0001bf50: 2020 2020 2020 206f 6e6c 696e 655f 746f         online_to
-0001bf60: 7069 635f 6e61 6d65 3d6f 6e6c 696e 655f  pic_name=online_
-0001bf70: 746f 7069 635f 6e61 6d65 2c0a 2020 2020  topic_name,.    
-0001bf80: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
-0001bf90: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
-0001bfa0: 7265 5f6e 616d 6520 3d20 6665 6174 7572  re_name = featur
-0001bfb0: 6573 746f 7265 5f6e 616d 650a 2020 2020  estore_name.    
-0001bfc0: 2020 2020 7365 6c66 2e5f 6465 7363 7269      self._descri
-0001bfd0: 7074 696f 6e20 3d20 6465 7363 7269 7074  ption = descript
-0001bfe0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
-0001bff0: 2e5f 6372 6561 7465 6420 3d20 6372 6561  ._created = crea
-0001c000: 7465 640a 2020 2020 2020 2020 7365 6c66  ted.        self
-0001c010: 2e5f 6372 6561 746f 7220 3d20 7573 6572  ._creator = user
-0001c020: 2e55 7365 722e 6672 6f6d 5f72 6573 706f  .User.from_respo
-0001c030: 6e73 655f 6a73 6f6e 2863 7265 6174 6f72  nse_json(creator
-0001c040: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0001c050: 7665 7273 696f 6e20 3d20 7665 7273 696f  version = versio
-0001c060: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
-0001c070: 6e61 6d65 203d 206e 616d 650a 0a20 2020  name = name..   
-0001c080: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-0001c090: 7265 7320 3d20 5b0a 2020 2020 2020 2020  res = [.        
-0001c0a0: 2020 2020 6665 6174 7572 652e 4665 6174      feature.Feat
-0001c0b0: 7572 652e 6672 6f6d 5f72 6573 706f 6e73  ure.from_respons
-0001c0c0: 655f 6a73 6f6e 2866 6561 7429 2069 6620  e_json(feat) if 
-0001c0d0: 6973 696e 7374 616e 6365 2866 6561 742c  isinstance(feat,
-0001c0e0: 2064 6963 7429 2065 6c73 6520 6665 6174   dict) else feat
-0001c0f0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0001c100: 2066 6561 7420 696e 2028 6665 6174 7572   feat in (featur
-0001c110: 6573 206f 7220 5b5d 290a 2020 2020 2020  es or []).      
-0001c120: 2020 5d0a 0a20 2020 2020 2020 2073 656c    ]..        sel
-0001c130: 662e 5f66 6561 7475 7265 5f67 726f 7570  f._feature_group
-0001c140: 5f65 6e67 696e 6520 3d20 7370 696e 655f  _engine = spine_
-0001c150: 6772 6f75 705f 656e 6769 6e65 2e53 7069  group_engine.Spi
-0001c160: 6e65 4772 6f75 7045 6e67 696e 6528 0a20  neGroupEngine(. 
-0001c170: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-0001c180: 7265 7374 6f72 655f 6964 0a20 2020 2020  restore_id.     
-0001c190: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-0001c1a0: 2073 656c 662e 5f69 643a 0a20 2020 2020   self._id:.     
-0001c1b0: 2020 2020 2020 2023 2047 6f74 2066 726f         # Got fro
-0001c1c0: 6d20 486f 7073 776f 726b 732c 2064 6573  m Hopsworks, des
-0001c1d0: 6572 6961 6c69 7a65 2066 6561 7475 7265  erialize feature
-0001c1e0: 7320 616e 6420 7374 6f72 6167 6520 636f  s and storage co
-0001c1f0: 6e6e 6563 746f 720a 2020 2020 2020 2020  nnector.        
-0001c200: 2020 2020 7365 6c66 2e5f 6665 6174 7572      self._featur
-0001c210: 6573 203d 2028 0a20 2020 2020 2020 2020  es = (.         
-0001c220: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0001c230: 2020 2020 2020 2020 2020 2020 2066 6561               fea
-0001c240: 7475 7265 2e46 6561 7475 7265 2e66 726f  ture.Feature.fro
-0001c250: 6d5f 7265 7370 6f6e 7365 5f6a 736f 6e28  m_response_json(
-0001c260: 6665 6174 290a 2020 2020 2020 2020 2020  feat).          
-0001c270: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0001c280: 6e73 7461 6e63 6528 6665 6174 2c20 6469  nstance(feat, di
-0001c290: 6374 290a 2020 2020 2020 2020 2020 2020  ct).            
-0001c2a0: 2020 2020 2020 2020 656c 7365 2066 6561          else fea
-0001c2b0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0001c2c0: 2020 2020 2020 666f 7220 6665 6174 2069        for feat i
-0001c2d0: 6e20 6665 6174 7572 6573 0a20 2020 2020  n features.     
-0001c2e0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0001c2f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001c300: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
-0001c310: 2020 2020 2020 2020 2065 6c73 6520 4e6f           else No
-0001c320: 6e65 0a20 2020 2020 2020 2020 2020 2029  ne.            )
-0001c330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001c340: 662e 7072 696d 6172 795f 6b65 7920 3d20  f.primary_key = 
-0001c350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001c360: 2020 5b66 6561 742e 6e61 6d65 2066 6f72    [feat.name for
-0001c370: 2066 6561 7420 696e 2073 656c 662e 5f66   feat in self._f
-0001c380: 6561 7475 7265 7320 6966 2066 6561 742e  eatures if feat.
-0001c390: 7072 696d 6172 7920 6973 2054 7275 655d  primary is True]
-0001c3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c3b0: 2069 6620 7365 6c66 2e5f 6665 6174 7572   if self._featur
-0001c3c0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-0001c3d0: 2020 2065 6c73 6520 5b5d 0a20 2020 2020     else [].     
-0001c3e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001c3f0: 2020 2020 2073 656c 662e 7374 6174 6973       self.statis
-0001c400: 7469 6373 5f63 6f6e 6669 6720 3d20 7374  tics_config = st
-0001c410: 6174 6973 7469 6373 5f63 6f6e 6669 670a  atistics_config.
-0001c420: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001c430: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0001c440: 7269 6d61 7279 5f6b 6579 203d 2070 7269  rimary_key = pri
-0001c450: 6d61 7279 5f6b 6579 0a20 2020 2020 2020  mary_key.       
-0001c460: 2020 2020 2073 656c 662e 7374 6174 6973       self.statis
-0001c470: 7469 6373 5f63 6f6e 6669 6720 3d20 7374  tics_config = st
-0001c480: 6174 6973 7469 6373 5f63 6f6e 6669 670a  atistics_config.
-0001c490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001c4a0: 2e5f 6665 6174 7572 6573 203d 2066 6561  ._features = fea
-0001c4b0: 7475 7265 730a 0a20 2020 2020 2020 2073  tures..        s
-0001c4c0: 656c 662e 5f68 7265 6620 3d20 6872 6566  elf._href = href
-0001c4d0: 0a0a 2020 2020 2020 2020 2320 6861 7320  ..        # has 
-0001c4e0: 746f 2068 6170 7065 6e20 6c61 7374 202d  to happen last -
-0001c4f0: 3e20 6665 6174 7572 6573 2061 6e64 2069  > features and i
-0001c500: 6420 6172 6520 6e65 6564 6564 2066 6f72  d are needed for
-0001c510: 2073 6368 656d 6120 7665 7269 6669 6361   schema verifica
-0001c520: 7469 6f6e 0a20 2020 2020 2020 2023 2075  tion.        # u
-0001c530: 7365 2073 6574 7465 7220 746f 2063 6f6e  se setter to con
-0001c540: 7665 7274 2074 6f20 6465 6661 756c 7420  vert to default 
-0001c550: 6461 7461 6672 616d 6520 7479 7065 2066  dataframe type f
-0001c560: 6f72 2065 6e67 696e 650a 2020 2020 2020  or engine.      
-0001c570: 2020 7365 6c66 2e64 6174 6166 7261 6d65    self.dataframe
-0001c580: 203d 2064 6174 6166 7261 6d65 0a0a 2020   = dataframe..  
-0001c590: 2020 6465 6620 5f73 6176 6528 7365 6c66    def _save(self
-0001c5a0: 293a 0a20 2020 2020 2020 2022 2222 5065  ):.        """Pe
-0001c5b0: 7273 6973 7420 7468 6520 6d65 7461 6461  rsist the metada
-0001c5c0: 7461 2066 6f72 2074 6869 7320 7370 696e  ta for this spin
-0001c5d0: 6520 6772 6f75 702e 0a0a 2020 2020 2020  e group...      
-0001c5e0: 2020 5769 7468 6f75 7420 6361 6c6c 696e    Without callin
-0001c5f0: 6720 7468 6973 206d 6574 686f 642c 2079  g this method, y
-0001c600: 6f75 7220 6665 6174 7572 6520 6772 6f75  our feature grou
-0001c610: 7020 7769 6c6c 206f 6e6c 7920 6578 6973  p will only exis
-0001c620: 740a 2020 2020 2020 2020 696e 2079 6f75  t.        in you
-0001c630: 7220 5079 7468 6f6e 204b 6572 6e65 6c2c  r Python Kernel,
-0001c640: 2062 7574 206e 6f74 2069 6e20 486f 7073   but not in Hops
-0001c650: 776f 726b 732e 0a0a 2020 2020 2020 2020  works...        
-0001c660: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-0001c670: 2020 7175 6572 7920 3d20 2253 454c 4543    query = "SELEC
-0001c680: 5420 2a20 4652 4f4d 2073 616c 6573 220a  T * FROM sales".
-0001c690: 0a20 2020 2020 2020 2066 6720 3d20 6665  .        fg = fe
-0001c6a0: 6174 7572 655f 7374 6f72 652e 6372 6561  ature_store.crea
-0001c6b0: 7465 5f73 7069 6e65 5f67 726f 7570 286e  te_spine_group(n
-0001c6c0: 616d 653d 2273 616c 6573 222c 0a20 2020  ame="sales",.   
-0001c6d0: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
-0001c6e0: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
-0001c6f0: 6465 7363 7269 7074 696f 6e3d 2250 6879  description="Phy
-0001c700: 7369 6361 6c20 7368 6f70 2073 616c 6573  sical shop sales
-0001c710: 2066 6561 7475 7265 7322 2c0a 2020 2020   features",.    
-0001c720: 2020 2020 2020 2020 7072 696d 6172 795f          primary_
-0001c730: 6b65 793d 5b27 7373 5f73 746f 7265 5f73  key=['ss_store_s
-0001c740: 6b27 5d2c 0a20 2020 2020 2020 2020 2020  k'],.           
-0001c750: 2065 7665 6e74 5f74 696d 653d 2773 616c   event_time='sal
-0001c760: 655f 6461 7465 272c 0a20 2020 2020 2020  e_date',.       
-0001c770: 2020 2020 2064 6174 6166 7261 6d65 3d64       dataframe=d
-0001c780: 662c 0a20 2020 2020 2020 2029 0a0a 2020  f,.        )..  
-0001c790: 2020 2020 2020 6667 2e5f 7361 7665 2829        fg._save()
-0001c7a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001c7b0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-0001c7c0: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
-0001c7d0: 7361 7665 2873 656c 6629 0a20 2020 2020  save(self).     
-0001c7e0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0001c7f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0001c800: 2020 6465 6620 6461 7461 6672 616d 6528    def dataframe(
-0001c810: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0001c820: 2222 5370 696e 6520 6461 7461 6672 616d  ""Spine datafram
-0001c830: 6520 7769 7468 2070 7269 6d61 7279 206b  e with primary k
-0001c840: 6579 2c20 6576 656e 7420 7469 6d65 2061  ey, event time a
-0001c850: 6e64 0a20 2020 2020 2020 206c 6162 656c  nd.        label
-0001c860: 2063 6f6c 756d 6e20 746f 2075 7365 2066   column to use f
-0001c870: 6f72 2070 6f69 6e74 2069 6e20 7469 6d65  or point in time
-0001c880: 206a 6f69 6e20 7768 656e 2066 6574 6368   join when fetch
-0001c890: 696e 6720 6665 6174 7572 6573 2e0a 2020  ing features..  
-0001c8a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001c8b0: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
-0001c8c0: 6174 6166 7261 6d65 0a0a 2020 2020 4064  ataframe..    @d
-0001c8d0: 6174 6166 7261 6d65 2e73 6574 7465 720a  ataframe.setter.
-0001c8e0: 2020 2020 6465 6620 6461 7461 6672 616d      def datafram
-0001c8f0: 6528 7365 6c66 2c20 6461 7461 6672 616d  e(self, datafram
-0001c900: 6529 3a0a 2020 2020 2020 2020 2222 2255  e):.        """U
-0001c910: 7064 6174 6520 7468 6520 7370 696e 6520  pdate the spine 
-0001c920: 6461 7461 6672 616d 6520 636f 6e74 6169  dataframe contai
-0001c930: 6e65 6420 696e 2074 6865 2073 7069 6e65  ned in the spine
-0001c940: 2067 726f 7570 2e22 2222 0a20 2020 2020   group.""".     
-0001c950: 2020 2073 656c 662e 5f64 6174 6166 7261     self._datafra
-0001c960: 6d65 203d 2065 6e67 696e 652e 6765 745f  me = engine.get_
-0001c970: 696e 7374 616e 6365 2829 2e63 6f6e 7665  instance().conve
-0001c980: 7274 5f74 6f5f 6465 6661 756c 745f 6461  rt_to_default_da
-0001c990: 7461 6672 616d 6528 6461 7461 6672 616d  taframe(datafram
-0001c9a0: 6529 0a0a 2020 2020 2020 2020 2320 696e  e)..        # in
-0001c9b0: 2066 7320 7175 6572 7920 7468 6520 6665   fs query the fe
-0001c9c0: 6174 7572 6573 2061 7265 206e 6f74 2073  atures are not s
-0001c9d0: 656e 742c 2073 6f20 7468 656e 2064 6f6e  ent, so then don
-0001c9e0: 2774 2064 6f20 7661 6c69 6461 7469 6f6e  't do validation
-0001c9f0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-0001ca00: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001ca10: 6964 2069 7320 6e6f 7420 4e6f 6e65 0a20  id is not None. 
-0001ca20: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
-0001ca30: 656c 662e 5f64 6174 6166 7261 6d65 2069  elf._dataframe i
-0001ca40: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0001ca50: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-0001ca60: 5f66 6561 7475 7265 7320 6973 206e 6f74  _features is not
-0001ca70: 204e 6f6e 650a 2020 2020 2020 2020 293a   None.        ):
-0001ca80: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0001ca90: 6166 7261 6d65 5f66 6561 7475 7265 7320  aframe_features 
-0001caa0: 3d20 656e 6769 6e65 2e67 6574 5f69 6e73  = engine.get_ins
-0001cab0: 7461 6e63 6528 292e 7061 7273 655f 7363  tance().parse_sc
-0001cac0: 6865 6d61 5f66 6561 7475 7265 5f67 726f  hema_feature_gro
-0001cad0: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
-0001cae0: 2020 2020 7365 6c66 2e5f 6461 7461 6672      self._datafr
-0001caf0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0001cb00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001cb10: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-0001cb20: 705f 656e 6769 6e65 2e5f 7665 7269 6679  p_engine._verify
-0001cb30: 5f73 6368 656d 615f 636f 6d70 6174 6962  _schema_compatib
-0001cb40: 696c 6974 7928 0a20 2020 2020 2020 2020  ility(.         
-0001cb50: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
-0001cb60: 7475 7265 732c 2064 6174 6166 7261 6d65  tures, dataframe
-0001cb70: 5f66 6561 7475 7265 730a 2020 2020 2020  _features.      
-0001cb80: 2020 2020 2020 290a 0a20 2020 2040 636c        )..    @cl
-0001cb90: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-0001cba0: 6620 6672 6f6d 5f72 6573 706f 6e73 655f  f from_response_
-0001cbb0: 6a73 6f6e 2863 6c73 2c20 6a73 6f6e 5f64  json(cls, json_d
-0001cbc0: 6963 7429 3a0a 2020 2020 2020 2020 6a73  ict):.        js
-0001cbd0: 6f6e 5f64 6563 616d 656c 697a 6564 203d  on_decamelized =
-0001cbe0: 2068 756d 7073 2e64 6563 616d 656c 697a   humps.decameliz
-0001cbf0: 6528 6a73 6f6e 5f64 6963 7429 0a20 2020  e(json_dict).   
-0001cc00: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0001cc10: 6365 286a 736f 6e5f 6465 6361 6d65 6c69  ce(json_decameli
-0001cc20: 7a65 642c 2064 6963 7429 3a0a 2020 2020  zed, dict):.    
-0001cc30: 2020 2020 2020 2020 5f20 3d20 6a73 6f6e          _ = json
-0001cc40: 5f64 6563 616d 656c 697a 6564 2e70 6f70  _decamelized.pop
-0001cc50: 2822 7479 7065 222c 204e 6f6e 6529 0a20  ("type", None). 
-0001cc60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001cc70: 6e20 636c 7328 2a2a 6a73 6f6e 5f64 6563  n cls(**json_dec
-0001cc80: 616d 656c 697a 6564 290a 2020 2020 2020  amelized).      
-0001cc90: 2020 666f 7220 6667 2069 6e20 6a73 6f6e    for fg in json
-0001cca0: 5f64 6563 616d 656c 697a 6564 3a0a 2020  _decamelized:.  
-0001ccb0: 2020 2020 2020 2020 2020 5f20 3d20 6667            _ = fg
-0001ccc0: 2e70 6f70 2822 7479 7065 222c 204e 6f6e  .pop("type", Non
-0001ccd0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-0001cce0: 6e20 5b63 6c73 282a 2a66 6729 2066 6f72  n [cls(**fg) for
-0001ccf0: 2066 6720 696e 206a 736f 6e5f 6465 6361   fg in json_deca
-0001cd00: 6d65 6c69 7a65 645d 0a0a 2020 2020 6465  melized]..    de
-0001cd10: 6620 7570 6461 7465 5f66 726f 6d5f 7265  f update_from_re
-0001cd20: 7370 6f6e 7365 5f6a 736f 6e28 7365 6c66  sponse_json(self
-0001cd30: 2c20 6a73 6f6e 5f64 6963 7429 3a0a 2020  , json_dict):.  
-0001cd40: 2020 2020 2020 6a73 6f6e 5f64 6563 616d        json_decam
-0001cd50: 656c 697a 6564 203d 2068 756d 7073 2e64  elized = humps.d
-0001cd60: 6563 616d 656c 697a 6528 6a73 6f6e 5f64  ecamelize(json_d
-0001cd70: 6963 7429 0a20 2020 2020 2020 2069 6620  ict).        if 
-0001cd80: 2274 7970 6522 2069 6e20 6a73 6f6e 5f64  "type" in json_d
-0001cd90: 6563 616d 656c 697a 6564 3a0a 2020 2020  ecamelized:.    
-0001cda0: 2020 2020 2020 2020 5f20 3d20 6a73 6f6e          _ = json
-0001cdb0: 5f64 6563 616d 656c 697a 6564 2e70 6f70  _decamelized.pop
-0001cdc0: 2822 7479 7065 2229 0a20 2020 2020 2020  ("type").       
-0001cdd0: 2073 656c 662e 5f5f 696e 6974 5f5f 282a   self.__init__(*
-0001cde0: 2a6a 736f 6e5f 6465 6361 6d65 6c69 7a65  *json_decamelize
-0001cdf0: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
-0001ce00: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
-0001ce10: 6a73 6f6e 2873 656c 6629 3a0a 2020 2020  json(self):.    
-0001ce20: 2020 2020 7265 7475 726e 206a 736f 6e2e      return json.
-0001ce30: 6475 6d70 7328 7365 6c66 2c20 636c 733d  dumps(self, cls=
-0001ce40: 7574 696c 2e46 6561 7475 7265 5374 6f72  util.FeatureStor
-0001ce50: 6545 6e63 6f64 6572 290a 0a20 2020 2064  eEncoder)..    d
-0001ce60: 6566 2074 6f5f 6469 6374 2873 656c 6629  ef to_dict(self)
-0001ce70: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001ce80: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-0001ce90: 6964 223a 2073 656c 662e 5f69 642c 0a20  id": self._id,. 
-0001cea0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0001ceb0: 223a 2073 656c 662e 5f6e 616d 652c 0a20  ": self._name,. 
-0001cec0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-0001ced0: 7269 7074 696f 6e22 3a20 7365 6c66 2e5f  ription": self._
-0001cee0: 6465 7363 7269 7074 696f 6e2c 0a20 2020  description,.   
-0001cef0: 2020 2020 2020 2020 2022 7665 7273 696f           "versio
-0001cf00: 6e22 3a20 7365 6c66 2e5f 7665 7273 696f  n": self._versio
-0001cf10: 6e2c 0a20 2020 2020 2020 2020 2020 2022  n,.            "
-0001cf20: 6665 6174 7572 6573 223a 2073 656c 662e  features": self.
-0001cf30: 5f66 6561 7475 7265 732c 0a20 2020 2020  _features,.     
-0001cf40: 2020 2020 2020 2022 6665 6174 7572 6573         "features
-0001cf50: 746f 7265 4964 223a 2073 656c 662e 5f66  toreId": self._f
-0001cf60: 6561 7475 7265 5f73 746f 7265 5f69 642c  eature_store_id,
-0001cf70: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-0001cf80: 7065 223a 2022 6f6e 4465 6d61 6e64 4665  pe": "onDemandFe
-0001cf90: 6174 7572 6567 726f 7570 4454 4f22 2c0a  aturegroupDTO",.
-0001cfa0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-0001cfb0: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
-0001cfc0: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
-0001cfd0: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
-0001cfe0: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
-0001cff0: 3a20 7365 6c66 2e5f 6576 656e 745f 7469  : self._event_ti
-0001d000: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001d010: 2273 7069 6e65 223a 2054 7275 652c 0a20  "spine": True,. 
-0001d020: 2020 2020 2020 207d 0a                          }.
+0000b7c0: 746f 5f6a 736f 6e5f 6469 6374 2864 6563  to_json_dict(dec
+0000b7d0: 616d 656c 697a 653d 5472 7565 290a 2020  amelize=True).  
+0000b7e0: 2020 2020 2020 2020 2020 746d 705f 6578            tmp_ex
+0000b7f0: 7065 6374 6174 696f 6e5f 7375 6974 655b  pectation_suite[
+0000b800: 2266 6561 7475 7265 5f67 726f 7570 5f69  "feature_group_i
+0000b810: 6422 5d20 3d20 7365 6c66 2e5f 6964 0a20  d"] = self._id. 
+0000b820: 2020 2020 2020 2020 2020 2074 6d70 5f65             tmp_e
+0000b830: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+0000b840: 5b22 6665 6174 7572 655f 7374 6f72 655f  ["feature_store_
+0000b850: 6964 225d 203d 2073 656c 662e 5f66 6561  id"] = self._fea
+0000b860: 7475 7265 5f73 746f 7265 5f69 640a 2020  ture_store_id.  
+0000b870: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000b880: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000b890: 6520 3d20 4578 7065 6374 6174 696f 6e53  e = ExpectationS
+0000b8a0: 7569 7465 282a 2a74 6d70 5f65 7870 6563  uite(**tmp_expec
+0000b8b0: 7461 7469 6f6e 5f73 7569 7465 290a 2020  tation_suite).  
+0000b8c0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+0000b8d0: 7461 6e63 6528 6578 7065 6374 6174 696f  tance(expectatio
+0000b8e0: 6e5f 7375 6974 652c 2067 652e 636f 7265  n_suite, ge.core
+0000b8f0: 2e65 7870 6563 7461 7469 6f6e 5f73 7569  .expectation_sui
+0000b900: 7465 2e45 7870 6563 7461 7469 6f6e 5375  te.ExpectationSu
+0000b910: 6974 6529 3a0a 2020 2020 2020 2020 2020  ite):.          
+0000b920: 2020 7365 6c66 2e5f 6578 7065 6374 6174    self._expectat
+0000b930: 696f 6e5f 7375 6974 6520 3d20 4578 7065  ion_suite = Expe
+0000b940: 6374 6174 696f 6e53 7569 7465 280a 2020  ctationSuite(.  
+0000b950: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+0000b960: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000b970: 652e 746f 5f6a 736f 6e5f 6469 6374 2829  e.to_json_dict()
+0000b980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b990: 2020 6665 6174 7572 655f 7374 6f72 655f    feature_store_
+0000b9a0: 6964 3d73 656c 662e 5f66 6561 7475 7265  id=self._feature
+0000b9b0: 5f73 746f 7265 5f69 642c 0a20 2020 2020  _store_id,.     
+0000b9c0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+0000b9d0: 7265 5f67 726f 7570 5f69 643d 7365 6c66  re_group_id=self
+0000b9e0: 2e5f 6964 2c0a 2020 2020 2020 2020 2020  ._id,.          
+0000b9f0: 2020 290a 2020 2020 2020 2020 656c 6966    ).        elif
+0000ba00: 2069 7369 6e73 7461 6e63 6528 6578 7065   isinstance(expe
+0000ba10: 6374 6174 696f 6e5f 7375 6974 652c 2064  ctation_suite, d
+0000ba20: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
+0000ba30: 2020 746d 705f 6578 7065 6374 6174 696f    tmp_expectatio
+0000ba40: 6e5f 7375 6974 6520 3d20 6578 7065 6374  n_suite = expect
+0000ba50: 6174 696f 6e5f 7375 6974 652e 636f 7079  ation_suite.copy
+0000ba60: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+0000ba70: 6d70 5f65 7870 6563 7461 7469 6f6e 5f73  mp_expectation_s
+0000ba80: 7569 7465 5b22 6665 6174 7572 655f 7374  uite["feature_st
+0000ba90: 6f72 655f 6964 225d 203d 2073 656c 662e  ore_id"] = self.
+0000baa0: 5f66 6561 7475 7265 5f73 746f 7265 5f69  _feature_store_i
+0000bab0: 640a 2020 2020 2020 2020 2020 2020 746d  d.            tm
+0000bac0: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
+0000bad0: 6974 655b 2266 6561 7475 7265 5f67 726f  ite["feature_gro
+0000bae0: 7570 5f69 6422 5d20 3d20 7365 6c66 2e5f  up_id"] = self._
+0000baf0: 6964 0a20 2020 2020 2020 2020 2020 2073  id.            s
+0000bb00: 656c 662e 5f65 7870 6563 7461 7469 6f6e  elf._expectation
+0000bb10: 5f73 7569 7465 203d 2045 7870 6563 7461  _suite = Expecta
+0000bb20: 7469 6f6e 5375 6974 6528 2a2a 746d 705f  tionSuite(**tmp_
+0000bb30: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000bb40: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
+0000bb50: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000bb60: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+0000bb70: 2020 2020 2020 2073 656c 662e 5f65 7870         self._exp
+0000bb80: 6563 7461 7469 6f6e 5f73 7569 7465 203d  ectation_suite =
+0000bb90: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
+0000bba0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bbb0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+0000bbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bbd0: 2022 5468 6520 6172 6775 6d65 6e74 2060   "The argument `
+0000bbe0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000bbf0: 6560 2068 6173 2074 6f20 6265 2060 4e6f  e` has to be `No
+0000bc00: 6e65 6020 6f66 2074 7970 6520 6045 7870  ne` of type `Exp
+0000bc10: 6563 7461 7469 6f6e 5375 6974 6560 206f  ectationSuite` o
+0000bc20: 7220 6064 6963 7460 2c20 6275 7420 6973  r `dict`, but is
+0000bc30: 206f 6620 7479 7065 3a20 607b 7d60 222e   of type: `{}`".
+0000bc40: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+0000bc50: 2020 2020 2020 2020 2020 2020 7479 7065              type
+0000bc60: 2865 7870 6563 7461 7469 6f6e 5f73 7569  (expectation_sui
+0000bc70: 7465 290a 2020 2020 2020 2020 2020 2020  te).            
+0000bc80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000bc90: 2020 290a 0a20 2020 2040 7072 6f70 6572    )..    @proper
+0000bca0: 7479 0a20 2020 2064 6566 206f 6e6c 696e  ty.    def onlin
+0000bcb0: 655f 656e 6162 6c65 6428 7365 6c66 293a  e_enabled(self):
+0000bcc0: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
+0000bcd0: 696e 6720 6966 2074 6865 2066 6561 7475  ing if the featu
+0000bce0: 7265 2067 726f 7570 2069 7320 6176 6169  re group is avai
+0000bcf0: 6c61 626c 6520 696e 206f 6e6c 696e 6520  lable in online 
+0000bd00: 7374 6f72 6167 652e 2222 220a 2020 2020  storage.""".    
+0000bd10: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000bd20: 5f6f 6e6c 696e 655f 656e 6162 6c65 640a  _online_enabled.
+0000bd30: 0a20 2020 2040 6f6e 6c69 6e65 5f65 6e61  .    @online_ena
+0000bd40: 626c 6564 2e73 6574 7465 720a 2020 2020  bled.setter.    
+0000bd50: 6465 6620 6f6e 6c69 6e65 5f65 6e61 626c  def online_enabl
+0000bd60: 6564 2873 656c 662c 206f 6e6c 696e 655f  ed(self, online_
+0000bd70: 656e 6162 6c65 6429 3a0a 2020 2020 2020  enabled):.      
+0000bd80: 2020 7365 6c66 2e5f 6f6e 6c69 6e65 5f65    self._online_e
+0000bd90: 6e61 626c 6564 203d 206f 6e6c 696e 655f  nabled = online_
+0000bda0: 656e 6162 6c65 640a 0a20 2020 2040 7072  enabled..    @pr
+0000bdb0: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
+0000bdc0: 7562 6a65 6374 2873 656c 6629 3a0a 2020  ubject(self):.  
+0000bdd0: 2020 2020 2020 2222 2253 7562 6a65 6374        """Subject
+0000bde0: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+0000bdf0: 6772 6f75 702e 2222 220a 2020 2020 2020  group.""".      
+0000be00: 2020 6966 2073 656c 662e 5f73 7562 6a65    if self._subje
+0000be10: 6374 2069 7320 4e6f 6e65 3a0a 2020 2020  ct is None:.    
+0000be20: 2020 2020 2020 2020 2320 6361 6368 6520          # cache 
+0000be30: 7468 6520 7363 6865 6d61 0a20 2020 2020  the schema.     
+0000be40: 2020 2020 2020 2073 656c 662e 5f73 7562         self._sub
+0000be50: 6a65 6374 203d 2073 656c 662e 5f66 6561  ject = self._fea
+0000be60: 7475 7265 5f67 726f 7570 5f65 6e67 696e  ture_group_engin
+0000be70: 652e 6765 745f 7375 626a 6563 7428 7365  e.get_subject(se
+0000be80: 6c66 290a 2020 2020 2020 2020 7265 7475  lf).        retu
+0000be90: 726e 2073 656c 662e 5f73 7562 6a65 6374  rn self._subject
+0000bea0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000beb0: 2020 2020 6465 6620 6176 726f 5f73 6368      def avro_sch
+0000bec0: 656d 6128 7365 6c66 293a 0a20 2020 2020  ema(self):.     
+0000bed0: 2020 2022 2222 4176 726f 2073 6368 656d     """Avro schem
+0000bee0: 6120 7265 7072 6573 656e 7461 7469 6f6e  a representation
+0000bef0: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+0000bf00: 6772 6f75 702e 2222 220a 2020 2020 2020  group.""".      
+0000bf10: 2020 7265 7475 726e 2073 656c 662e 7375    return self.su
+0000bf20: 626a 6563 745b 2273 6368 656d 6122 5d0a  bject["schema"].
+0000bf30: 0a20 2020 2064 6566 2067 6574 5f63 6f6d  .    def get_com
+0000bf40: 706c 6578 5f66 6561 7475 7265 7328 7365  plex_features(se
+0000bf50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000bf60: 5265 7475 726e 7320 7468 6520 6e61 6d65  Returns the name
+0000bf70: 7320 6f66 2061 6c6c 2066 6561 7475 7265  s of all feature
+0000bf80: 7320 7769 7468 2061 2063 6f6d 706c 6578  s with a complex
+0000bf90: 2064 6174 6120 7479 7065 2069 6e20 7468   data type in th
+0000bfa0: 6973 0a20 2020 2020 2020 2066 6561 7475  is.        featu
+0000bfb0: 7265 2067 726f 7570 2e0a 0a20 2020 2020  re group...     
+0000bfc0: 2020 2021 2121 2065 7861 6d70 6c65 0a20     !!! example. 
+0000bfd0: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
+0000bfe0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
+0000bff0: 2063 6f6d 706c 6578 5f64 7479 7065 5f66   complex_dtype_f
+0000c000: 6561 7475 7265 7320 3d20 6667 2e67 6574  eatures = fg.get
+0000c010: 5f63 6f6d 706c 6578 5f66 6561 7475 7265  _complex_feature
+0000c020: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0000c030: 6060 600a 2020 2020 2020 2020 2222 220a  ```.        """.
+0000c040: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+0000c050: 662e 6e61 6d65 2066 6f72 2066 2069 6e20  f.name for f in 
+0000c060: 7365 6c66 2e66 6561 7475 7265 7320 6966  self.features if
+0000c070: 2066 2e69 735f 636f 6d70 6c65 7828 295d   f.is_complex()]
+0000c080: 0a0a 2020 2020 6465 6620 5f67 6574 5f65  ..    def _get_e
+0000c090: 6e63 6f64 6564 5f61 7672 6f5f 7363 6865  ncoded_avro_sche
+0000c0a0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
+0000c0b0: 2020 636f 6d70 6c65 785f 6665 6174 7572    complex_featur
+0000c0c0: 6573 203d 2073 656c 662e 6765 745f 636f  es = self.get_co
+0000c0d0: 6d70 6c65 785f 6665 6174 7572 6573 2829  mplex_features()
+0000c0e0: 0a20 2020 2020 2020 2073 6368 656d 6120  .        schema 
+0000c0f0: 3d20 6a73 6f6e 2e6c 6f61 6473 2873 656c  = json.loads(sel
+0000c100: 662e 6176 726f 5f73 6368 656d 6129 0a0a  f.avro_schema)..
+0000c110: 2020 2020 2020 2020 666f 7220 6669 656c          for fiel
+0000c120: 6420 696e 2073 6368 656d 615b 2266 6965  d in schema["fie
+0000c130: 6c64 7322 5d3a 0a20 2020 2020 2020 2020  lds"]:.         
+0000c140: 2020 2069 6620 6669 656c 645b 226e 616d     if field["nam
+0000c150: 6522 5d20 696e 2063 6f6d 706c 6578 5f66  e"] in complex_f
+0000c160: 6561 7475 7265 733a 0a20 2020 2020 2020  eatures:.       
+0000c170: 2020 2020 2020 2020 2066 6965 6c64 5b22           field["
+0000c180: 7479 7065 225d 203d 205b 226e 756c 6c22  type"] = ["null"
+0000c190: 2c20 2262 7974 6573 225d 0a0a 2020 2020  , "bytes"]..    
+0000c1a0: 2020 2020 7363 6865 6d61 5f73 203d 206a      schema_s = j
+0000c1b0: 736f 6e2e 6475 6d70 7328 7363 6865 6d61  son.dumps(schema
+0000c1c0: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+0000c1d0: 2020 2020 2020 2020 2020 2061 7672 6f2e             avro.
+0000c1e0: 7363 6865 6d61 2e70 6172 7365 2873 6368  schema.parse(sch
+0000c1f0: 656d 615f 7329 0a20 2020 2020 2020 2065  ema_s).        e
+0000c200: 7863 6570 7420 6176 726f 2e73 6368 656d  xcept avro.schem
+0000c210: 612e 5363 6865 6d61 5061 7273 6545 7863  a.SchemaParseExc
+0000c220: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0000c230: 2020 2020 2020 2020 2072 6169 7365 2046           raise F
+0000c240: 6561 7475 7265 5374 6f72 6545 7863 6570  eatureStoreExcep
+0000c250: 7469 6f6e 2822 4661 696c 6564 2074 6f20  tion("Failed to 
+0000c260: 636f 6e73 7472 7563 7420 4176 726f 2053  construct Avro S
+0000c270: 6368 656d 613a 207b 7d22 2e66 6f72 6d61  chema: {}".forma
+0000c280: 7428 6529 290a 2020 2020 2020 2020 7265  t(e)).        re
+0000c290: 7475 726e 2073 6368 656d 615f 730a 0a20  turn schema_s.. 
+0000c2a0: 2020 2064 6566 205f 6765 745f 6665 6174     def _get_feat
+0000c2b0: 7572 655f 6176 726f 5f73 6368 656d 6128  ure_avro_schema(
+0000c2c0: 7365 6c66 2c20 6665 6174 7572 655f 6e61  self, feature_na
+0000c2d0: 6d65 293a 0a20 2020 2020 2020 2066 6f72  me):.        for
+0000c2e0: 2066 6965 6c64 2069 6e20 6a73 6f6e 2e6c   field in json.l
+0000c2f0: 6f61 6473 2873 656c 662e 6176 726f 5f73  oads(self.avro_s
+0000c300: 6368 656d 6129 5b22 6669 656c 6473 225d  chema)["fields"]
+0000c310: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000c320: 2066 6965 6c64 5b22 6e61 6d65 225d 203d   field["name"] =
+0000c330: 3d20 6665 6174 7572 655f 6e61 6d65 3a0a  = feature_name:.
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+0000c360: 7328 6669 656c 645b 2274 7970 6522 5d29  s(field["type"])
+0000c370: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000c380: 2020 2020 6465 6620 6665 6174 7572 6573      def features
+0000c390: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000c3a0: 2222 2253 6368 656d 6120 696e 666f 726d  """Schema inform
+0000c3b0: 6174 696f 6e2e 2222 220a 2020 2020 2020  ation.""".      
+0000c3c0: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+0000c3d0: 6561 7475 7265 730a 0a20 2020 2040 6665  eatures..    @fe
+0000c3e0: 6174 7572 6573 2e73 6574 7465 720a 2020  atures.setter.  
+0000c3f0: 2020 6465 6620 6665 6174 7572 6573 2873    def features(s
+0000c400: 656c 662c 206e 6577 5f66 6561 7475 7265  elf, new_feature
+0000c410: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+0000c420: 2e5f 6665 6174 7572 6573 203d 206e 6577  ._features = new
+0000c430: 5f66 6561 7475 7265 730a 0a0a 636c 6173  _features...clas
+0000c440: 7320 4665 6174 7572 6547 726f 7570 2846  s FeatureGroup(F
+0000c450: 6561 7475 7265 4772 6f75 7042 6173 6529  eatureGroupBase)
+0000c460: 3a0a 2020 2020 4341 4348 4544 5f46 4541  :.    CACHED_FEA
+0000c470: 5455 5245 5f47 524f 5550 203d 2022 4341  TURE_GROUP = "CA
+0000c480: 4348 4544 5f46 4541 5455 5245 5f47 524f  CHED_FEATURE_GRO
+0000c490: 5550 220a 2020 2020 5354 5245 414d 5f46  UP".    STREAM_F
+0000c4a0: 4541 5455 5245 5f47 524f 5550 203d 2022  EATURE_GROUP = "
+0000c4b0: 5354 5245 414d 5f46 4541 5455 5245 5f47  STREAM_FEATURE_G
+0000c4c0: 524f 5550 220a 2020 2020 454e 5449 5459  ROUP".    ENTITY
+0000c4d0: 5f54 5950 4520 3d20 2266 6561 7475 7265  _TYPE = "feature
+0000c4e0: 6772 6f75 7073 220a 0a20 2020 2064 6566  groups"..    def
+0000c4f0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0000c500: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000c510: 206e 616d 652c 0a20 2020 2020 2020 2076   name,.        v
+0000c520: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
+0000c530: 6665 6174 7572 6573 746f 7265 5f69 642c  featurestore_id,
+0000c540: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+0000c550: 7469 6f6e 3d22 222c 0a20 2020 2020 2020  tion="",.       
+0000c560: 2070 6172 7469 7469 6f6e 5f6b 6579 3d4e   partition_key=N
+0000c570: 6f6e 652c 0a20 2020 2020 2020 2070 7269  one,.        pri
+0000c580: 6d61 7279 5f6b 6579 3d4e 6f6e 652c 0a20  mary_key=None,. 
+0000c590: 2020 2020 2020 2068 7564 695f 7072 6563         hudi_prec
+0000c5a0: 6f6d 6269 6e65 5f6b 6579 3d4e 6f6e 652c  ombine_key=None,
+0000c5b0: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+0000c5c0: 7374 6f72 655f 6e61 6d65 3d4e 6f6e 652c  store_name=None,
+0000c5d0: 0a20 2020 2020 2020 2063 7265 6174 6564  .        created
+0000c5e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
+0000c5f0: 7265 6174 6f72 3d4e 6f6e 652c 0a20 2020  reator=None,.   
+0000c600: 2020 2020 2069 643d 4e6f 6e65 2c0a 2020       id=None,.  
+0000c610: 2020 2020 2020 6665 6174 7572 6573 3d4e        features=N
+0000c620: 6f6e 652c 0a20 2020 2020 2020 206c 6f63  one,.        loc
+0000c630: 6174 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ation=None,.    
+0000c640: 2020 2020 6f6e 6c69 6e65 5f65 6e61 626c      online_enabl
+0000c650: 6564 3d46 616c 7365 2c0a 2020 2020 2020  ed=False,.      
+0000c660: 2020 7469 6d65 5f74 7261 7665 6c5f 666f    time_travel_fo
+0000c670: 726d 6174 3d4e 6f6e 652c 0a20 2020 2020  rmat=None,.     
+0000c680: 2020 2073 7461 7469 7374 6963 735f 636f     statistics_co
+0000c690: 6e66 6967 3d4e 6f6e 652c 0a20 2020 2020  nfig=None,.     
+0000c6a0: 2020 206f 6e6c 696e 655f 746f 7069 635f     online_topic_
+0000c6b0: 6e61 6d65 3d4e 6f6e 652c 0a20 2020 2020  name=None,.     
+0000c6c0: 2020 2065 7665 6e74 5f74 696d 653d 4e6f     event_time=No
+0000c6d0: 6e65 2c0a 2020 2020 2020 2020 7374 7265  ne,.        stre
+0000c6e0: 616d 3d46 616c 7365 2c0a 2020 2020 2020  am=False,.      
+0000c6f0: 2020 6578 7065 6374 6174 696f 6e5f 7375    expectation_su
+0000c700: 6974 653d 4e6f 6e65 2c0a 2020 2020 2020  ite=None,.      
+0000c710: 2020 7061 7265 6e74 733d 4e6f 6e65 2c0a    parents=None,.
+0000c720: 2020 2020 2020 2020 6872 6566 3d4e 6f6e          href=Non
+0000c730: 652c 0a20 2020 2020 2020 2064 656c 7461  e,.        delta
+0000c740: 5f73 7472 6561 6d65 725f 6a6f 625f 636f  _streamer_job_co
+0000c750: 6e66 3d4e 6f6e 652c 0a20 2020 2029 3a0a  nf=None,.    ):.
+0000c760: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+0000c770: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0000c780: 2020 2020 2020 6665 6174 7572 6573 746f        featuresto
+0000c790: 7265 5f69 642c 0a20 2020 2020 2020 2020  re_id,.         
+0000c7a0: 2020 206c 6f63 6174 696f 6e2c 0a20 2020     location,.   
+0000c7b0: 2020 2020 2020 2020 2065 7665 6e74 5f74           event_t
+0000c7c0: 696d 653d 6576 656e 745f 7469 6d65 2c0a  ime=event_time,.
+0000c7d0: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
+0000c7e0: 6e65 5f65 6e61 626c 6564 3d6f 6e6c 696e  ne_enabled=onlin
+0000c7f0: 655f 656e 6162 6c65 642c 0a20 2020 2020  e_enabled,.     
+0000c800: 2020 2020 2020 2069 643d 6964 2c0a 2020         id=id,.  
+0000c810: 2020 2020 2020 2020 2020 6578 7065 6374            expect
+0000c820: 6174 696f 6e5f 7375 6974 653d 6578 7065  ation_suite=expe
+0000c830: 6374 6174 696f 6e5f 7375 6974 652c 0a20  ctation_suite,. 
+0000c840: 2020 2020 2020 2020 2020 206f 6e6c 696e             onlin
+0000c850: 655f 746f 7069 635f 6e61 6d65 3d6f 6e6c  e_topic_name=onl
+0000c860: 696e 655f 746f 7069 635f 6e61 6d65 2c0a  ine_topic_name,.
+0000c870: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000c880: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
+0000c890: 5f73 746f 7265 5f6e 616d 6520 3d20 6665  _store_name = fe
+0000c8a0: 6174 7572 6573 746f 7265 5f6e 616d 650a  aturestore_name.
+0000c8b0: 2020 2020 2020 2020 7365 6c66 2e5f 6465          self._de
+0000c8c0: 7363 7269 7074 696f 6e20 3d20 6465 7363  scription = desc
+0000c8d0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
+0000c8e0: 7365 6c66 2e5f 6372 6561 7465 6420 3d20  self._created = 
+0000c8f0: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
+0000c900: 7365 6c66 2e5f 6372 6561 746f 7220 3d20  self._creator = 
+0000c910: 7573 6572 2e55 7365 722e 6672 6f6d 5f72  user.User.from_r
+0000c920: 6573 706f 6e73 655f 6a73 6f6e 2863 7265  esponse_json(cre
+0000c930: 6174 6f72 290a 2020 2020 2020 2020 7365  ator).        se
+0000c940: 6c66 2e5f 7665 7273 696f 6e20 3d20 7665  lf._version = ve
+0000c950: 7273 696f 6e0a 2020 2020 2020 2020 7365  rsion.        se
+0000c960: 6c66 2e5f 6e61 6d65 203d 206e 616d 650a  lf._name = name.
+0000c970: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+0000c980: 6174 7572 6573 203d 205b 0a20 2020 2020  atures = [.     
+0000c990: 2020 2020 2020 2066 6561 7475 7265 2e46         feature.F
+0000c9a0: 6561 7475 7265 2e66 726f 6d5f 7265 7370  eature.from_resp
+0000c9b0: 6f6e 7365 5f6a 736f 6e28 6665 6174 2920  onse_json(feat) 
+0000c9c0: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
+0000c9d0: 6174 2c20 6469 6374 2920 656c 7365 2066  at, dict) else f
+0000c9e0: 6561 740a 2020 2020 2020 2020 2020 2020  eat.            
+0000c9f0: 666f 7220 6665 6174 2069 6e20 2866 6561  for feat in (fea
+0000ca00: 7475 7265 7320 6f72 205b 5d29 0a20 2020  tures or []).   
+0000ca10: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+0000ca20: 7365 6c66 2e5f 7469 6d65 5f74 7261 7665  self._time_trave
+0000ca30: 6c5f 666f 726d 6174 203d 2028 0a20 2020  l_format = (.   
+0000ca40: 2020 2020 2020 2020 2074 696d 655f 7472           time_tr
+0000ca50: 6176 656c 5f66 6f72 6d61 742e 7570 7065  avel_format.uppe
+0000ca60: 7228 2920 6966 2074 696d 655f 7472 6176  r() if time_trav
+0000ca70: 656c 5f66 6f72 6d61 7420 6973 206e 6f74  el_format is not
+0000ca80: 204e 6f6e 6520 656c 7365 204e 6f6e 650a   None else None.
+0000ca90: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000caa0: 2020 2073 656c 662e 5f73 7472 6561 6d20     self._stream 
+0000cab0: 3d20 7374 7265 616d 0a20 2020 2020 2020  = stream.       
+0000cac0: 2073 656c 662e 5f70 6172 656e 7473 203d   self._parents =
+0000cad0: 2070 6172 656e 7473 0a20 2020 2020 2020   parents.       
+0000cae0: 2073 656c 662e 5f64 656c 7461 7374 7265   self._deltastre
+0000caf0: 616d 6572 5f6a 6f62 636f 6e66 203d 2064  amer_jobconf = d
+0000cb00: 656c 7461 5f73 7472 6561 6d65 725f 6a6f  elta_streamer_jo
+0000cb10: 625f 636f 6e66 0a0a 2020 2020 2020 2020  b_conf..        
+0000cb20: 7365 6c66 2e5f 6261 636b 6669 6c6c 5f6a  self._backfill_j
+0000cb30: 6f62 203d 204e 6f6e 650a 0a20 2020 2020  ob = None..     
+0000cb40: 2020 2069 6620 7365 6c66 2e5f 6964 3a0a     if self._id:.
+0000cb50: 2020 2020 2020 2020 2020 2020 2320 696e              # in
+0000cb60: 6974 6961 6c69 7a65 6420 6279 2062 6163  itialized by bac
+0000cb70: 6b65 6e64 0a20 2020 2020 2020 2020 2020  kend.           
+0000cb80: 2073 656c 662e 7072 696d 6172 795f 6b65   self.primary_ke
+0000cb90: 7920 3d20 5b0a 2020 2020 2020 2020 2020  y = [.          
+0000cba0: 2020 2020 2020 6665 6174 2e6e 616d 6520        feat.name 
+0000cbb0: 666f 7220 6665 6174 2069 6e20 7365 6c66  for feat in self
+0000cbc0: 2e5f 6665 6174 7572 6573 2069 6620 6665  ._features if fe
+0000cbd0: 6174 2e70 7269 6d61 7279 2069 7320 5472  at.primary is Tr
+0000cbe0: 7565 0a20 2020 2020 2020 2020 2020 205d  ue.            ]
+0000cbf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cc00: 662e 5f70 6172 7469 7469 6f6e 5f6b 6579  f._partition_key
+0000cc10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+0000cc20: 2020 2020 2066 6561 742e 6e61 6d65 2066       feat.name f
+0000cc30: 6f72 2066 6561 7420 696e 2073 656c 662e  or feat in self.
+0000cc40: 5f66 6561 7475 7265 7320 6966 2066 6561  _features if fea
+0000cc50: 742e 7061 7274 6974 696f 6e20 6973 2054  t.partition is T
+0000cc60: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000cc70: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+0000cc80: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000cc90: 2020 2074 696d 655f 7472 6176 656c 5f66     time_travel_f
+0000cca0: 6f72 6d61 7420 6973 206e 6f74 204e 6f6e  ormat is not Non
+0000ccb0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000ccc0: 2020 616e 6420 7469 6d65 5f74 7261 7665    and time_trave
+0000ccd0: 6c5f 666f 726d 6174 2e75 7070 6572 2829  l_format.upper()
+0000cce0: 203d 3d20 2248 5544 4922 0a20 2020 2020   == "HUDI".     
+0000ccf0: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
+0000cd00: 656c 662e 5f66 6561 7475 7265 730a 2020  elf._features.  
+0000cd10: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0000cd20: 2020 2020 2020 2020 2020 2020 2023 2068               # h
+0000cd30: 7564 6920 7072 6563 6f6d 6269 6e65 206b  udi precombine k
+0000cd40: 6579 2069 7320 616c 7761 7973 2061 2073  ey is always a s
+0000cd50: 696e 676c 6520 6665 6174 7572 650a 2020  ingle feature.  
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cd70: 6c66 2e5f 6875 6469 5f70 7265 636f 6d62  lf._hudi_precomb
+0000cd80: 696e 655f 6b65 7920 3d20 5b0a 2020 2020  ine_key = [.    
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cda0: 6665 6174 2e6e 616d 650a 2020 2020 2020  feat.name.      
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000cdc0: 7220 6665 6174 2069 6e20 7365 6c66 2e5f  r feat in self._
+0000cdd0: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
+0000cde0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000cdf0: 6665 6174 2e68 7564 695f 7072 6563 6f6d  feat.hudi_precom
+0000ce00: 6269 6e65 5f6b 6579 2069 7320 5472 7565  bine_key is True
+0000ce10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce20: 205d 5b30 5d0a 2020 2020 2020 2020 2020   ][0].          
+0000ce30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ce40: 2020 2020 2020 2020 7365 6c66 2e5f 6875          self._hu
+0000ce50: 6469 5f70 7265 636f 6d62 696e 655f 6b65  di_precombine_ke
+0000ce60: 7920 3d20 4e6f 6e65 0a0a 2020 2020 2020  y = None..      
+0000ce70: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000ce80: 7374 6963 735f 636f 6e66 6967 203d 2073  stics_config = s
+0000ce90: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
+0000cea0: 0a0a 2020 2020 2020 2020 656c 7365 3a0a  ..        else:.
+0000ceb0: 2020 2020 2020 2020 2020 2020 2320 696e              # in
+0000cec0: 6974 6961 6c69 7a65 6420 6279 2075 7365  itialized by use
+0000ced0: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
+0000cee0: 666f 7220 7079 7468 6f6e 2065 6e67 696e  for python engin
+0000cef0: 6520 7765 2061 6c77 6179 7320 7573 6520  e we always use 
+0000cf00: 7374 7265 616d 2066 6561 7475 7265 2067  stream feature g
+0000cf10: 726f 7570 0a20 2020 2020 2020 2020 2020  roup.           
+0000cf20: 2069 6620 656e 6769 6e65 2e67 6574 5f74   if engine.get_t
+0000cf30: 7970 6528 2920 3d3d 2022 7079 7468 6f6e  ype() == "python
+0000cf40: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000cf50: 2020 2073 656c 662e 5f73 7472 6561 6d20     self._stream 
+0000cf60: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+0000cf70: 2020 2023 2066 6f72 2073 7472 6561 6d20     # for stream 
+0000cf80: 6665 6174 7572 6520 6772 6f75 7020 7469  feature group ti
+0000cf90: 6d65 2074 7261 7665 6c20 666f 726d 6174  me travel format
+0000cfa0: 2069 7320 616c 7761 7973 2048 5544 490a   is always HUDI.
+0000cfb0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000cfc0: 656c 662e 5f73 7472 6561 6d3a 0a20 2020  elf._stream:.   
+0000cfd0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0000cfe0: 6563 7465 645f 666f 726d 6174 203d 2022  ected_format = "
+0000cff0: 4855 4449 220a 2020 2020 2020 2020 2020  HUDI".          
+0000d000: 2020 2020 2020 6966 2073 656c 662e 5f74        if self._t
+0000d010: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
+0000d020: 7420 213d 2065 7870 6563 7465 645f 666f  t != expected_fo
+0000d030: 726d 6174 3a0a 2020 2020 2020 2020 2020  rmat:.          
+0000d040: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0000d050: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d070: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000d090: 5468 6520 7072 6f76 6964 6564 2074 696d  The provided tim
+0000d0a0: 6520 7472 6176 656c 2066 6f72 6d61 7420  e travel format 
+0000d0b0: 607b 7d60 2068 6173 2062 6565 6e20 6f76  `{}` has been ov
+0000d0c0: 6572 7772 6974 7465 6e20 220a 2020 2020  erwritten ".    
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2020 2262 6563 6175 7365          "because
+0000d0f0: 2053 7472 6561 6d20 656e 6162 6c65 6420   Stream enabled 
+0000d100: 6665 6174 7572 6520 6772 6f75 7073 206f  feature groups o
+0000d110: 6e6c 7920 7375 7070 6f72 7420 607b 7d60  nly support `{}`
+0000d120: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000d130: 2020 2020 2020 2020 2020 292e 666f 726d            ).form
+0000d140: 6174 2873 656c 662e 5f74 696d 655f 7472  at(self._time_tr
+0000d150: 6176 656c 5f66 6f72 6d61 742c 2065 7870  avel_format, exp
+0000d160: 6563 7465 645f 666f 726d 6174 292c 0a20  ected_format),. 
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 2075 7469 6c2e 4665 6174         util.Feat
+0000d190: 7572 6547 726f 7570 5761 726e 696e 672c  ureGroupWarning,
+0000d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000d1c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d1d0: 5f74 696d 655f 7472 6176 656c 5f66 6f72  _time_travel_for
+0000d1e0: 6d61 7420 3d20 6578 7065 6374 6564 5f66  mat = expected_f
+0000d1f0: 6f72 6d61 740a 0a20 2020 2020 2020 2020  ormat..         
+0000d200: 2020 2073 656c 662e 7072 696d 6172 795f     self.primary_
+0000d210: 6b65 7920 3d20 7072 696d 6172 795f 6b65  key = primary_ke
+0000d220: 790a 2020 2020 2020 2020 2020 2020 7365  y.            se
+0000d230: 6c66 2e70 6172 7469 7469 6f6e 5f6b 6579  lf.partition_key
+0000d240: 203d 2070 6172 7469 7469 6f6e 5f6b 6579   = partition_key
+0000d250: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d260: 662e 5f68 7564 695f 7072 6563 6f6d 6269  f._hudi_precombi
+0000d270: 6e65 5f6b 6579 203d 2028 0a20 2020 2020  ne_key = (.     
+0000d280: 2020 2020 2020 2020 2020 2068 7564 695f             hudi_
+0000d290: 7072 6563 6f6d 6269 6e65 5f6b 6579 2e6c  precombine_key.l
+0000d2a0: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+0000d2b0: 2020 2020 2020 2069 6620 6875 6469 5f70         if hudi_p
+0000d2c0: 7265 636f 6d62 696e 655f 6b65 7920 6973  recombine_key is
+0000d2d0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000d2e0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+0000d2f0: 6c66 2e5f 7469 6d65 5f74 7261 7665 6c5f  lf._time_travel_
+0000d300: 666f 726d 6174 2069 7320 6e6f 7420 4e6f  format is not No
+0000d310: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000d320: 2020 2061 6e64 2073 656c 662e 5f74 696d     and self._tim
+0000d330: 655f 7472 6176 656c 5f66 6f72 6d61 7420  e_travel_format 
+0000d340: 3d3d 2022 4855 4449 220a 2020 2020 2020  == "HUDI".      
+0000d350: 2020 2020 2020 2020 2020 656c 7365 204e            else N
+0000d360: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000d370: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000d380: 6c66 2e73 7461 7469 7374 6963 735f 636f  lf.statistics_co
+0000d390: 6e66 6967 203d 2073 7461 7469 7374 6963  nfig = statistic
+0000d3a0: 735f 636f 6e66 6967 0a0a 2020 2020 2020  s_config..      
+0000d3b0: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
+0000d3c0: 6772 6f75 705f 656e 6769 6e65 203d 2066  group_engine = f
+0000d3d0: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
+0000d3e0: 696e 652e 4665 6174 7572 6547 726f 7570  ine.FeatureGroup
+0000d3f0: 456e 6769 6e65 280a 2020 2020 2020 2020  Engine(.        
+0000d400: 2020 2020 6665 6174 7572 6573 746f 7265      featurestore
+0000d410: 5f69 640a 2020 2020 2020 2020 290a 2020  _id.        ).  
+0000d420: 2020 2020 2020 7365 6c66 2e5f 6872 6566        self._href
+0000d430: 203d 2068 7265 660a 0a20 2020 2020 2020   = href..       
+0000d440: 2023 2063 6163 6865 2066 6f72 206f 7074   # cache for opt
+0000d450: 696d 697a 6564 2077 7269 7465 730a 2020  imized writes.  
+0000d460: 2020 2020 2020 7365 6c66 2e5f 6b61 666b        self._kafk
+0000d470: 615f 7072 6f64 7563 6572 203d 204e 6f6e  a_producer = Non
+0000d480: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000d490: 6665 6174 7572 655f 7772 6974 6572 7320  feature_writers 
+0000d4a0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000d4b0: 656c 662e 5f77 7269 7465 7220 3d20 4e6f  elf._writer = No
+0000d4c0: 6e65 0a0a 2020 2020 6465 6620 7265 6164  ne..    def read
+0000d4d0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000d4e0: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
+0000d4f0: 6b5f 7469 6d65 3a20 4f70 7469 6f6e 616c  k_time: Optional
+0000d500: 5b55 6e69 6f6e 5b73 7472 2c20 696e 742c  [Union[str, int,
+0000d510: 2064 6174 6574 696d 652c 2064 6174 655d   datetime, date]
+0000d520: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000d530: 2020 6f6e 6c69 6e65 3a20 4f70 7469 6f6e    online: Option
+0000d540: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
+0000d550: 2c0a 2020 2020 2020 2020 6461 7461 6672  ,.        datafr
+0000d560: 616d 655f 7479 7065 3a20 4f70 7469 6f6e  ame_type: Option
+0000d570: 616c 5b73 7472 5d20 3d20 2264 6566 6175  al[str] = "defau
+0000d580: 6c74 222c 0a20 2020 2020 2020 2072 6561  lt",.        rea
+0000d590: 645f 6f70 7469 6f6e 733a 204f 7074 696f  d_options: Optio
+0000d5a0: 6e61 6c5b 6469 6374 5d20 3d20 7b7d 2c0a  nal[dict] = {},.
+0000d5b0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+0000d5c0: 2222 0a20 2020 2020 2020 2052 6561 6420  "".        Read 
+0000d5d0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+0000d5e0: 7020 696e 746f 2061 2064 6174 6166 7261  p into a datafra
+0000d5f0: 6d65 2e0a 0a20 2020 2020 2020 2052 6561  me...        Rea
+0000d600: 6473 2074 6865 2066 6561 7475 7265 2067  ds the feature g
+0000d610: 726f 7570 2062 7920 6465 6661 756c 7420  roup by default 
+0000d620: 6672 6f6d 2074 6865 206f 6666 6c69 6e65  from the offline
+0000d630: 2073 746f 7261 6765 2061 7320 5370 6172   storage as Spar
+0000d640: 6b20 4461 7461 4672 616d 650a 2020 2020  k DataFrame.    
+0000d650: 2020 2020 6f6e 2048 6f70 7377 6f72 6b73      on Hopsworks
+0000d660: 2061 6e64 2044 6174 6162 7269 636b 732c   and Databricks,
+0000d670: 2061 6e64 2061 7320 5061 6e64 6173 2064   and as Pandas d
+0000d680: 6174 6166 7261 6d65 206f 6e20 4157 5320  ataframe on AWS 
+0000d690: 5361 6765 6d61 6b65 7220 616e 6420 7075  Sagemaker and pu
+0000d6a0: 7265 0a20 2020 2020 2020 2050 7974 686f  re.        Pytho
+0000d6b0: 6e20 656e 7669 726f 6e6d 656e 7473 2e0a  n environments..
+0000d6c0: 0a20 2020 2020 2020 2053 6574 2060 6f6e  .        Set `on
+0000d6d0: 6c69 6e65 6020 746f 2060 5472 7565 6020  line` to `True` 
+0000d6e0: 746f 2072 6561 6420 6672 6f6d 2074 6865  to read from the
+0000d6f0: 206f 6e6c 696e 6520 7374 6f72 6167 652c   online storage,
+0000d700: 206f 7220 6368 616e 6765 0a20 2020 2020   or change.     
+0000d710: 2020 2060 6461 7461 6672 616d 655f 7479     `dataframe_ty
+0000d720: 7065 6020 746f 2072 6561 6420 6173 2061  pe` to read as a
+0000d730: 2064 6966 6665 7265 6e74 2066 6f72 6d61   different forma
+0000d740: 742e 0a0a 2020 2020 2020 2020 2121 2120  t...        !!! 
+0000d750: 6578 616d 706c 6520 2252 6561 6420 6665  example "Read fe
+0000d760: 6174 7572 6520 6772 6f75 7020 6173 206f  ature group as o
+0000d770: 6620 6c61 7465 7374 2073 7461 7465 3a22  f latest state:"
+0000d780: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+0000d790: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
+0000d7a0: 2020 2023 2063 6f6e 6e65 6374 2074 6f20     # connect to 
+0000d7b0: 7468 6520 4665 6174 7572 6520 5374 6f72  the Feature Stor
+0000d7c0: 650a 2020 2020 2020 2020 2020 2020 6673  e.            fs
+0000d7d0: 203d 202e 2e2e 0a0a 2020 2020 2020 2020   = .....        
+0000d7e0: 2020 2020 2320 6765 7420 7468 6520 4665      # get the Fe
+0000d7f0: 6174 7572 6520 4772 6f75 7020 696e 7374  ature Group inst
+0000d800: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
+0000d810: 2066 6720 3d20 6673 2e67 6574 5f6f 725f   fg = fs.get_or_
+0000d820: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+0000d830: 726f 7570 282e 2e2e 290a 2020 2020 2020  roup(...).      
+0000d840: 2020 2020 2020 6667 2e72 6561 6428 290a        fg.read().
+0000d850: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+0000d860: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+0000d870: 6d70 6c65 2022 5265 6164 2066 6561 7475  mple "Read featu
+0000d880: 7265 2067 726f 7570 2061 7320 6f66 2073  re group as of s
+0000d890: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
+0000d8a0: 2074 696d 653a 220a 2020 2020 2020 2020   time:".        
+0000d8b0: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+0000d8c0: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
+0000d8d0: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
+0000d8e0: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
+0000d8f0: 2e29 0a20 2020 2020 2020 2020 2020 2066  .).            f
+0000d900: 672e 7265 6164 2822 3230 3230 2d31 302d  g.read("2020-10-
+0000d910: 3230 2030 373a 3334 3a31 3122 290a 2020  20 07:34:11").  
+0000d920: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+0000d930: 2020 2020 2020 2023 2041 7267 756d 656e         # Argumen
+0000d940: 7473 0a20 2020 2020 2020 2020 2020 2077  ts.            w
+0000d950: 616c 6c63 6c6f 636b 5f74 696d 653a 2049  allclock_time: I
+0000d960: 6620 7370 6563 6966 6965 6420 7769 6c6c  f specified will
+0000d970: 2072 6574 7269 6576 6520 6665 6174 7572   retrieve featur
+0000d980: 6520 6772 6f75 7020 6173 206f 6620 7370  e group as of sp
+0000d990: 6563 6966 6963 2070 6f69 6e74 2069 6e20  ecific point in 
+0000d9a0: 7469 6d65 2e20 4465 6661 756c 7473 2074  time. Defaults t
+0000d9b0: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
+0000d9c0: 2020 2020 2020 2020 2020 4966 206e 6f74            If not
+0000d9d0: 2073 7065 6369 6669 6564 2c20 7769 6c6c   specified, will
+0000d9e0: 2072 6574 7572 6e20 6173 206f 6620 6d6f   return as of mo
+0000d9f0: 7374 2072 6563 656e 7420 7469 6d65 2e0a  st recent time..
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 5374 7269 6e67 7320 7368 6f75 6c64 2062  Strings should b
+0000da20: 6520 666f 726d 6174 7465 6420 696e 206f  e formatted in o
+0000da30: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
+0000da40: 696e 6720 666f 726d 6174 7320 6025 592d  ing formats `%Y-
+0000da50: 256d 2d25 6460 2c20 6025 592d 256d 2d25  %m-%d`, `%Y-%m-%
+0000da60: 6420 2548 602c 2060 2559 2d25 6d2d 2564  d %H`, `%Y-%m-%d
+0000da70: 2025 483a 254d 602c 2060 2559 2d25 6d2d   %H:%M`, `%Y-%m-
+0000da80: 2564 2025 483a 254d 3a25 5360 2c0a 2020  %d %H:%M:%S`,.  
+0000da90: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+0000daa0: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
+0000dab0: 3a25 532e 2566 602e 0a20 2020 2020 2020  :%S.%f`..       
+0000dac0: 2020 2020 206f 6e6c 696e 653a 2062 6f6f       online: boo
+0000dad0: 6c2c 206f 7074 696f 6e61 6c2e 2049 6620  l, optional. If 
+0000dae0: 6054 7275 6560 2072 6561 6420 6672 6f6d  `True` read from
+0000daf0: 206f 6e6c 696e 6520 6665 6174 7572 6520   online feature 
+0000db00: 7374 6f72 652c 2064 6566 6175 6c74 730a  store, defaults.
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 746f 2060 4661 6c73 6560 2e0a 2020 2020  to `False`..    
+0000db30: 2020 2020 2020 2020 6461 7461 6672 616d          datafram
+0000db40: 655f 7479 7065 3a20 7374 722c 206f 7074  e_type: str, opt
+0000db50: 696f 6e61 6c2e 2050 6f73 7369 626c 6520  ional. Possible 
+0000db60: 7661 6c75 6573 2061 7265 2060 2264 6566  values are `"def
+0000db70: 6175 6c74 2260 2c20 6022 7370 6172 6b22  ault"`, `"spark"
+0000db80: 602c 0a20 2020 2020 2020 2020 2020 2020  `,.             
+0000db90: 2020 2060 2270 616e 6461 7322 602c 2060     `"pandas"`, `
+0000dba0: 226e 756d 7079 2260 206f 7220 6022 7079  "numpy"` or `"py
+0000dbb0: 7468 6f6e 2260 2c20 6465 6661 756c 7473  thon"`, defaults
+0000dbc0: 2074 6f20 6022 6465 6661 756c 7422 602e   to `"default"`.
+0000dbd0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+0000dbe0: 645f 6f70 7469 6f6e 733a 2041 6464 6974  d_options: Addit
+0000dbf0: 696f 6e61 6c20 6f70 7469 6f6e 7320 6173  ional options as
+0000dc00: 206b 6579 2f76 616c 7565 2070 6169 7273   key/value pairs
+0000dc10: 2074 6f20 7061 7373 2074 6f20 7468 6520   to pass to the 
+0000dc20: 6578 6563 7574 696f 6e20 656e 6769 6e65  execution engine
+0000dc30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dc40: 2020 466f 7220 7370 6172 6b20 656e 6769    For spark engi
+0000dc50: 6e65 3a20 4469 6374 696f 6e61 7279 206f  ne: Dictionary o
+0000dc60: 6620 7265 6164 206f 7074 696f 6e73 2066  f read options f
+0000dc70: 6f72 2053 7061 726b 2e0a 2020 2020 2020  or Spark..      
+0000dc80: 2020 2020 2020 2020 2020 466f 7220 7079            For py
+0000dc90: 7468 6f6e 2065 6e67 696e 653a 0a20 2020  thon engine:.   
+0000dca0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000dcb0: 6579 2060 2275 7365 5f68 6976 6522 6020  ey `"use_hive"` 
+0000dcc0: 616e 6420 7661 6c75 6520 6054 7275 6560  and value `True`
+0000dcd0: 2074 6f20 7265 6164 2066 6561 7475 7265   to read feature
+0000dce0: 2067 726f 7570 0a20 2020 2020 2020 2020   group.         
+0000dcf0: 2020 2020 2020 2020 2077 6974 6820 4869           with Hi
+0000dd00: 7665 2069 6e73 7465 6164 206f 6620 5b41  ve instead of [A
+0000dd10: 7272 6f77 466c 6967 6874 2053 6572 7665  rrowFlight Serve
+0000dd20: 725d 2868 7474 7073 3a2f 2f64 6f63 732e  r](https://docs.
+0000dd30: 686f 7073 776f 726b 732e 6169 2f6c 6174  hopsworks.ai/lat
+0000dd40: 6573 742f 7365 7475 705f 696e 7374 616c  est/setup_instal
+0000dd50: 6c61 7469 6f6e 2f63 6f6d 6d6f 6e2f 6172  lation/common/ar
+0000dd60: 726f 775f 666c 6967 6874 5f64 7563 6b64  row_flight_duckd
+0000dd70: 622f 292e 0a20 2020 2020 2020 2020 2020  b/)..           
+0000dd80: 2020 2020 202a 206b 6579 2060 2268 6976       * key `"hiv
+0000dd90: 655f 636f 6e66 6967 2260 2074 6f20 7061  e_config"` to pa
+0000dda0: 7373 2061 2064 6963 7469 6f6e 6172 7920  ss a dictionary 
+0000ddb0: 6f66 2068 6976 6520 6f72 2074 657a 2063  of hive or tez c
+0000ddc0: 6f6e 6669 6775 7261 7469 6f6e 732e 0a20  onfigurations.. 
+0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dde0: 2046 6f72 2065 7861 6d70 6c65 3a20 607b   For example: `{
+0000ddf0: 2268 6976 655f 636f 6e66 6967 223a 207b  "hive_config": {
+0000de00: 2268 6976 652e 7465 7a2e 6370 752e 7663  "hive.tez.cpu.vc
+0000de10: 6f72 6573 223a 2032 2c20 2274 657a 2e67  ores": 2, "tez.g
+0000de20: 726f 7570 696e 672e 7370 6c69 742d 636f  rouping.split-co
+0000de30: 756e 7422 3a20 2233 227d 7d60 0a20 2020  unt": "3"}}`.   
+0000de40: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000de50: 6579 2060 2270 616e 6461 735f 7479 7065  ey `"pandas_type
+0000de60: 7322 6020 616e 6420 7661 6c75 6520 6054  s"` and value `T
+0000de70: 7275 6560 2074 6f20 7265 7472 6965 7665  rue` to retrieve
+0000de80: 2063 6f6c 756d 6e73 2061 730a 2020 2020   columns as.    
+0000de90: 2020 2020 2020 2020 2020 2020 2020 5b50                [P
+0000dea0: 616e 6461 7320 6e75 6c6c 6162 6c65 2074  andas nullable t
+0000deb0: 7970 6573 5d28 6874 7470 733a 2f2f 7061  ypes](https://pa
+0000dec0: 6e64 6173 2e70 7964 6174 612e 6f72 672f  ndas.pydata.org/
+0000ded0: 646f 6373 2f75 7365 725f 6775 6964 652f  docs/user_guide/
+0000dee0: 696e 7465 6765 725f 6e61 2e68 746d 6c29  integer_na.html)
+0000def0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df00: 2020 2072 6174 6865 7220 7468 616e 206e     rather than n
+0000df10: 756d 7079 2f6f 626a 6563 7428 7374 7269  umpy/object(stri
+0000df20: 6e67 2920 7479 7065 7320 2865 7870 6572  ng) types (exper
+0000df30: 696d 656e 7461 6c29 2e0a 2020 2020 2020  imental)..      
+0000df40: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000df50: 7473 2074 6f20 607b 7d60 2e0a 0a20 2020  ts to `{}`...   
+0000df60: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+0000df70: 2020 2020 2020 2020 2020 2060 4461 7461             `Data
+0000df80: 4672 616d 6560 3a20 5468 6520 7370 6172  Frame`: The spar
+0000df90: 6b20 6461 7461 6672 616d 6520 636f 6e74  k dataframe cont
+0000dfa0: 6169 6e69 6e67 2074 6865 2066 6561 7475  aining the featu
+0000dfb0: 7265 2064 6174 612e 0a20 2020 2020 2020  re data..       
+0000dfc0: 2020 2020 2060 7079 7370 6172 6b2e 4461       `pyspark.Da
+0000dfd0: 7461 4672 616d 6560 2e20 4120 5370 6172  taFrame`. A Spar
+0000dfe0: 6b20 4461 7461 4672 616d 652e 0a20 2020  k DataFrame..   
+0000dff0: 2020 2020 2020 2020 2060 7061 6e64 6173           `pandas
+0000e000: 2e44 6174 6146 7261 6d65 602e 2041 2050  .DataFrame`. A P
+0000e010: 616e 6461 7320 4461 7461 4672 616d 652e  andas DataFrame.
+0000e020: 0a20 2020 2020 2020 2020 2020 2060 6e75  .            `nu
+0000e030: 6d70 792e 6e64 6172 7261 7960 2e20 4120  mpy.ndarray`. A 
+0000e040: 7477 6f2d 6469 6d65 6e73 696f 6e61 6c20  two-dimensional 
+0000e050: 4e75 6d70 7920 6172 7261 792e 0a20 2020  Numpy array..   
+0000e060: 2020 2020 2020 2020 2060 6c69 7374 602e           `list`.
+0000e070: 2041 2074 776f 2d64 696d 656e 7369 6f6e   A two-dimension
+0000e080: 616c 2050 7974 686f 6e20 6c69 7374 2e0a  al Python list..
+0000e090: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
+0000e0a0: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
+0000e0b0: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
+0000e0c0: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
+0000e0d0: 6f72 602e 204e 6f20 6461 7461 2069 7320  or`. No data is 
+0000e0e0: 6176 6169 6c61 626c 6520 666f 7220 6665  available for fe
+0000e0f0: 6174 7572 6520 6772 6f75 7020 7769 7468  ature group with
+0000e100: 2074 6869 7320 636f 6d6d 6974 2064 6174   this commit dat
+0000e110: 652c 2049 6620 7469 6d65 2074 7261 7665  e, If time trave
+0000e120: 6c20 656e 6162 6c65 642e 0a20 2020 2020  l enabled..     
+0000e130: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+0000e140: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
+0000e150: 6365 2829 2e73 6574 5f6a 6f62 5f67 726f  ce().set_job_gro
+0000e160: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+0000e170: 2246 6574 6368 696e 6720 4665 6174 7572  "Fetching Featur
+0000e180: 6520 6772 6f75 7022 2c0a 2020 2020 2020  e group",.      
+0000e190: 2020 2020 2020 2247 6574 7469 6e67 2066        "Getting f
+0000e1a0: 6561 7475 7265 2067 726f 7570 3a20 7b7d  eature group: {}
+0000e1b0: 2066 726f 6d20 7468 6520 6665 6174 7572   from the featur
+0000e1c0: 6573 746f 7265 207b 7d22 2e66 6f72 6d61  estore {}".forma
+0000e1d0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000e1e0: 2020 2073 656c 662e 5f6e 616d 652c 2073     self._name, s
+0000e1f0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+0000e200: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
+0000e210: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
+0000e220: 0a20 2020 2020 2020 2069 6620 7761 6c6c  .        if wall
+0000e230: 636c 6f63 6b5f 7469 6d65 3a0a 2020 2020  clock_time:.    
+0000e240: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000e250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e260: 2073 656c 662e 7365 6c65 6374 5f61 6c6c   self.select_all
+0000e270: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e280: 2020 202e 6173 5f6f 6628 7761 6c6c 636c     .as_of(wallcl
+0000e290: 6f63 6b5f 7469 6d65 290a 2020 2020 2020  ock_time).      
+0000e2a0: 2020 2020 2020 2020 2020 2e72 6561 6428            .read(
+0000e2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e2c0: 2020 2020 206f 6e6c 696e 652c 0a20 2020       online,.   
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2e0: 2064 6174 6166 7261 6d65 5f74 7970 652c   dataframe_type,
+0000e2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e300: 2020 2020 2072 6561 645f 6f70 7469 6f6e       read_option
+0000e310: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000e320: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000e330: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+0000e340: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e350: 7572 6e20 7365 6c66 2e73 656c 6563 745f  urn self.select_
+0000e360: 616c 6c28 292e 7265 6164 280a 2020 2020  all().read(.    
+0000e370: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
+0000e380: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000e390: 2020 2020 6461 7461 6672 616d 655f 7479      dataframe_ty
+0000e3a0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0000e3b0: 2020 2020 7265 6164 5f6f 7074 696f 6e73      read_options
+0000e3c0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000e3d0: 0a20 2020 2064 6566 2072 6561 645f 6368  .    def read_ch
+0000e3e0: 616e 6765 7328 0a20 2020 2020 2020 2073  anges(.        s
+0000e3f0: 656c 662c 0a20 2020 2020 2020 2073 7461  elf,.        sta
+0000e400: 7274 5f77 616c 6c63 6c6f 636b 5f74 696d  rt_wallclock_tim
+0000e410: 653a 2055 6e69 6f6e 5b73 7472 2c20 696e  e: Union[str, in
+0000e420: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
+0000e430: 655d 2c0a 2020 2020 2020 2020 656e 645f  e],.        end_
+0000e440: 7761 6c6c 636c 6f63 6b5f 7469 6d65 3a20  wallclock_time: 
+0000e450: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+0000e460: 6461 7465 7469 6d65 2c20 6461 7465 5d2c  datetime, date],
+0000e470: 0a20 2020 2020 2020 2072 6561 645f 6f70  .        read_op
+0000e480: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+0000e490: 6469 6374 5d20 3d20 7b7d 2c0a 2020 2020  dict] = {},.    
+0000e4a0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+0000e4b0: 6164 7320 7570 6461 7465 7320 6f66 2074  ads updates of t
+0000e4c0: 6869 7320 6665 6174 7572 6520 7468 6174  his feature that
+0000e4d0: 206f 6363 7572 7265 6420 6265 7477 6565   occurred betwee
+0000e4e0: 6e20 7370 6563 6966 6965 6420 706f 696e  n specified poin
+0000e4f0: 7473 2069 6e20 7469 6d65 2e0a 0a20 2020  ts in time...   
+0000e500: 2020 2020 2021 2121 2077 6172 6e69 6e67       !!! warning
+0000e510: 2022 4465 7072 6563 6174 6564 220a 2020   "Deprecated".  
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2020 6072 6561 645f 6368 616e 6765 7360    `read_changes`
+0000e540: 206d 6574 686f 6420 6973 2064 6570 7265   method is depre
+0000e550: 6361 7465 642e 2055 7365 0a20 2020 2020  cated. Use.     
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0000e570: 6173 5f6f 6628 656e 645f 7761 6c6c 636c  as_of(end_wallcl
+0000e580: 6f63 6b5f 7469 6d65 2c20 6578 636c 7564  ock_time, exclud
+0000e590: 655f 756e 7469 6c3d 7374 6172 745f 7761  e_until=start_wa
+0000e5a0: 6c6c 636c 6f63 6b5f 7469 6d65 292e 7265  llclock_time).re
+0000e5b0: 6164 2872 6561 645f 6f70 7469 6f6e 733d  ad(read_options=
+0000e5c0: 7265 6164 5f6f 7074 696f 6e73 2960 0a20  read_options)`. 
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2069 6e73 7465 6164 2e0a 0a20 2020     instead...   
+0000e5f0: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+0000e600: 6f6e 206f 6e6c 7920 776f 726b 7320 6f6e  on only works on
+0000e610: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
+0000e620: 7769 7468 2060 4855 4449 6020 7469 6d65  with `HUDI` time
+0000e630: 2074 7261 7665 6c20 666f 726d 6174 2e0a   travel format..
+0000e640: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
+0000e650: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+0000e660: 2073 7461 7274 5f77 616c 6c63 6c6f 636b   start_wallclock
+0000e670: 5f74 696d 653a 2053 7461 7274 2074 696d  _time: Start tim
+0000e680: 6520 6f66 2074 6865 2074 696d 6520 7472  e of the time tr
+0000e690: 6176 656c 2071 7565 7279 2e20 5374 7269  avel query. Stri
+0000e6a0: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
+0000e6b0: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
+0000e6c0: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+0000e6d0: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
+0000e6e0: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
+0000e6f0: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
+0000e700: 254d 602c 0a20 2020 2020 2020 2020 2020  %M`,.           
+0000e710: 2020 2020 2060 2559 2d25 6d2d 2564 2025       `%Y-%m-%d %
+0000e720: 483a 254d 3a25 5360 2c20 6f72 2060 2559  H:%M:%S`, or `%Y
+0000e730: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+0000e740: 2566 602e 0a20 2020 2020 2020 2020 2020  %f`..           
+0000e750: 2065 6e64 5f77 616c 6c63 6c6f 636b 5f74   end_wallclock_t
+0000e760: 696d 653a 2045 6e64 2074 696d 6520 6f66  ime: End time of
+0000e770: 2074 6865 2074 696d 6520 7472 6176 656c   the time travel
+0000e780: 2071 7565 7279 2e20 5374 7269 6e67 7320   query. Strings 
+0000e790: 7368 6f75 6c64 2062 6520 666f 726d 6174  should be format
+0000e7a0: 7465 6420 696e 206f 6e65 206f 6620 7468  ted in one of th
+0000e7b0: 6520 666f 6c6c 6f77 696e 6720 666f 726d  e following form
+0000e7c0: 6174 7320 6025 592d 256d 2d25 6460 2c20  ats `%Y-%m-%d`, 
+0000e7d0: 6025 592d 256d 2d25 6420 2548 602c 2060  `%Y-%m-%d %H`, `
+0000e7e0: 2559 2d25 6d2d 2564 2025 483a 254d 602c  %Y-%m-%d %H:%M`,
+0000e7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e800: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
+0000e810: 3a25 5360 2c20 6f72 2060 2559 2d25 6d2d  :%S`, or `%Y-%m-
+0000e820: 2564 2025 483a 254d 3a25 532e 2566 602e  %d %H:%M:%S.%f`.
+0000e830: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+0000e840: 645f 6f70 7469 6f6e 733a 2041 6464 6974  d_options: Addit
+0000e850: 696f 6e61 6c20 6f70 7469 6f6e 7320 6173  ional options as
+0000e860: 206b 6579 2f76 616c 7565 2070 6169 7273   key/value pairs
+0000e870: 2074 6f20 7061 7373 2074 6f20 7468 6520   to pass to the 
+0000e880: 6578 6563 7574 696f 6e20 656e 6769 6e65  execution engine
+0000e890: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e8a0: 2020 466f 7220 7370 6172 6b20 656e 6769    For spark engi
+0000e8b0: 6e65 3a20 4469 6374 696f 6e61 7279 206f  ne: Dictionary o
+0000e8c0: 6620 7265 6164 206f 7074 696f 6e73 2066  f read options f
+0000e8d0: 6f72 2053 7061 726b 2e0a 2020 2020 2020  or Spark..      
+0000e8e0: 2020 2020 2020 2020 2020 466f 7220 7079            For py
+0000e8f0: 7468 6f6e 2065 6e67 696e 653a 0a20 2020  thon engine:.   
+0000e900: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000e910: 6579 2060 2268 6976 655f 636f 6e66 6967  ey `"hive_config
+0000e920: 2260 2074 6f20 7061 7373 2061 2064 6963  "` to pass a dic
+0000e930: 7469 6f6e 6172 7920 6f66 2068 6976 6520  tionary of hive 
+0000e940: 6f72 2074 657a 2063 6f6e 6669 6775 7261  or tez configura
+0000e950: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+0000e960: 2020 2020 2020 2020 2046 6f72 2065 7861           For exa
+0000e970: 6d70 6c65 3a20 607b 2268 6976 655f 636f  mple: `{"hive_co
+0000e980: 6e66 6967 223a 207b 2268 6976 652e 7465  nfig": {"hive.te
+0000e990: 7a2e 6370 752e 7663 6f72 6573 223a 2032  z.cpu.vcores": 2
+0000e9a0: 2c20 2274 657a 2e67 726f 7570 696e 672e  , "tez.grouping.
+0000e9b0: 7370 6c69 742d 636f 756e 7422 3a20 2233  split-count": "3
+0000e9c0: 227d 7d60 0a20 2020 2020 2020 2020 2020  "}}`.           
+0000e9d0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+0000e9e0: 2060 7b7d 602e 0a0a 2020 2020 2020 2020   `{}`...        
+0000e9f0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+0000ea00: 2020 2020 2020 6044 6174 6146 7261 6d65        `DataFrame
+0000ea10: 602e 2054 6865 2073 7061 726b 2064 6174  `. The spark dat
+0000ea20: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
+0000ea30: 6720 7468 6520 696e 6372 656d 656e 7461  g the incrementa
+0000ea40: 6c20 6368 616e 6765 7320 6f66 0a20 2020  l changes of.   
+0000ea50: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+0000ea60: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+0000ea70: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+0000ea80: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+0000ea90: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+0000eaa0: 7441 5049 4572 726f 7260 2e20 204e 6f20  tAPIError`.  No 
+0000eab0: 6461 7461 2069 7320 6176 6169 6c61 626c  data is availabl
+0000eac0: 6520 666f 7220 6665 6174 7572 6520 6772  e for feature gr
+0000ead0: 6f75 7020 7769 7468 2074 6869 7320 636f  oup with this co
+0000eae0: 6d6d 6974 2064 6174 652e 0a20 2020 2020  mmit date..     
+0000eaf0: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+0000eb00: 656e 742e 6578 6365 7074 696f 6e73 2e46  ent.exceptions.F
+0000eb10: 6561 7475 7265 5374 6f72 6545 7863 6570  eatureStoreExcep
+0000eb20: 7469 6f6e 602e 2049 6620 7468 6520 6665  tion`. If the fe
+0000eb30: 6174 7572 6520 6772 6f75 7020 646f 6573  ature group does
+0000eb40: 206e 6f74 2068 6176 6520 6048 5544 4960   not have `HUDI`
+0000eb50: 2074 696d 6520 7472 6176 656c 2066 6f72   time travel for
+0000eb60: 6d61 740a 2020 2020 2020 2020 2222 220a  mat.        """.
+0000eb70: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000eb80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000eb90: 662e 7365 6c65 6374 5f61 6c6c 2829 0a20  f.select_all(). 
+0000eba0: 2020 2020 2020 2020 2020 202e 7075 6c6c             .pull
+0000ebb0: 5f63 6861 6e67 6573 2873 7461 7274 5f77  _changes(start_w
+0000ebc0: 616c 6c63 6c6f 636b 5f74 696d 652c 2065  allclock_time, e
+0000ebd0: 6e64 5f77 616c 6c63 6c6f 636b 5f74 696d  nd_wallclock_tim
+0000ebe0: 6529 0a20 2020 2020 2020 2020 2020 202e  e).            .
+0000ebf0: 7265 6164 2846 616c 7365 2c20 2264 6566  read(False, "def
+0000ec00: 6175 6c74 222c 2072 6561 645f 6f70 7469  ault", read_opti
+0000ec10: 6f6e 7329 0a20 2020 2020 2020 2029 0a0a  ons).        )..
+0000ec20: 2020 2020 6465 6620 7368 6f77 2873 656c      def show(sel
+0000ec30: 662c 206e 3a20 696e 742c 206f 6e6c 696e  f, n: int, onlin
+0000ec40: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+0000ec50: 5d20 3d20 4661 6c73 6529 3a0a 2020 2020  ] = False):.    
+0000ec60: 2020 2020 2222 2253 686f 7720 7468 6520      """Show the 
+0000ec70: 6669 7273 7420 606e 6020 726f 7773 206f  first `n` rows o
+0000ec80: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+0000ec90: 6f75 702e 0a0a 2020 2020 2020 2020 2121  oup...        !!
+0000eca0: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
+0000ecb0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+0000ecc0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+0000ecd0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
+0000ece0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
+0000ecf0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
+0000ed00: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+0000ed10: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
+0000ed20: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
+0000ed30: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
+0000ed40: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
+0000ed50: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
+0000ed60: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
+0000ed70: 2320 6d61 6b65 2061 2071 7565 7279 2061  # make a query a
+0000ed80: 6e64 2073 686f 7720 746f 7020 3520 726f  nd show top 5 ro
+0000ed90: 7773 0a20 2020 2020 2020 2020 2020 2066  ws.            f
+0000eda0: 672e 7365 6c65 6374 285b 2764 6174 6527  g.select(['date'
+0000edb0: 2c27 7765 656b 6c79 5f73 616c 6573 272c  ,'weekly_sales',
+0000edc0: 2769 735f 686f 6c69 6461 7927 5d29 2e73  'is_holiday']).s
+0000edd0: 686f 7728 3529 0a20 2020 2020 2020 2020  how(5).         
+0000ede0: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
+0000edf0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+0000ee00: 2020 2020 2020 2020 6e3a 2069 6e74 2e20          n: int. 
+0000ee10: 4e75 6d62 6572 206f 6620 726f 7773 2074  Number of rows t
+0000ee20: 6f20 7368 6f77 2e0a 2020 2020 2020 2020  o show..        
+0000ee30: 2020 2020 6f6e 6c69 6e65 3a20 626f 6f6c      online: bool
+0000ee40: 2c20 6f70 7469 6f6e 616c 2e20 4966 2060  , optional. If `
+0000ee50: 5472 7565 6020 7265 6164 2066 726f 6d20  True` read from 
+0000ee60: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
+0000ee70: 746f 7265 2c20 6465 6661 756c 7473 0a20  tore, defaults. 
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000ee90: 6f20 6046 616c 7365 602e 0a20 2020 2020  o `False`..     
+0000eea0: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+0000eeb0: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
+0000eec0: 6365 2829 2e73 6574 5f6a 6f62 5f67 726f  ce().set_job_gro
+0000eed0: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+0000eee0: 2246 6574 6368 696e 6720 4665 6174 7572  "Fetching Featur
+0000eef0: 6520 6772 6f75 7022 2c0a 2020 2020 2020  e group",.      
+0000ef00: 2020 2020 2020 2247 6574 7469 6e67 2066        "Getting f
+0000ef10: 6561 7475 7265 2067 726f 7570 3a20 7b7d  eature group: {}
+0000ef20: 2066 726f 6d20 7468 6520 6665 6174 7572   from the featur
+0000ef30: 6573 746f 7265 207b 7d22 2e66 6f72 6d61  estore {}".forma
+0000ef40: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000ef50: 2020 2073 656c 662e 5f6e 616d 652c 2073     self._name, s
+0000ef60: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+0000ef70: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
+0000ef80: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
+0000ef90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000efa0: 7365 6c66 2e73 656c 6563 745f 616c 6c28  self.select_all(
+0000efb0: 292e 7368 6f77 286e 2c20 6f6e 6c69 6e65  ).show(n, online
+0000efc0: 290a 0a20 2020 2064 6566 2073 6176 6528  )..    def save(
+0000efd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000efe0: 2020 2020 2020 2066 6561 7475 7265 733a         features:
+0000eff0: 2055 6e69 6f6e 5b0a 2020 2020 2020 2020   Union[.        
+0000f000: 2020 2020 7064 2e44 6174 6146 7261 6d65      pd.DataFrame
+0000f010: 2c0a 2020 2020 2020 2020 2020 2020 5479  ,.            Ty
+0000f020: 7065 5661 7228 2270 7973 7061 726b 2e73  peVar("pyspark.s
+0000f030: 716c 2e44 6174 6146 7261 6d65 2229 2c20  ql.DataFrame"), 
+0000f040: 2023 206e 6f71 613a 2046 3832 310a 2020   # noqa: F821.  
+0000f050: 2020 2020 2020 2020 2020 5479 7065 5661            TypeVa
+0000f060: 7228 2270 7973 7061 726b 2e52 4444 2229  r("pyspark.RDD")
+0000f070: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+0000f080: 2020 2020 2020 2020 2020 2020 6e70 2e6e              np.n
+0000f090: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
+0000f0a0: 2020 2020 4c69 7374 5b66 6561 7475 7265      List[feature
+0000f0b0: 2e46 6561 7475 7265 5d2c 0a20 2020 2020  .Feature],.     
+0000f0c0: 2020 205d 203d 204e 6f6e 652c 0a20 2020     ] = None,.   
+0000f0d0: 2020 2020 2077 7269 7465 5f6f 7074 696f       write_optio
+0000f0e0: 6e73 3a20 4f70 7469 6f6e 616c 5b44 6963  ns: Optional[Dic
+0000f0f0: 745b 416e 792c 2041 6e79 5d5d 203d 207b  t[Any, Any]] = {
+0000f100: 7d2c 0a20 2020 2020 2020 2076 616c 6964  },.        valid
+0000f110: 6174 696f 6e5f 6f70 7469 6f6e 733a 204f  ation_options: O
+0000f120: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
+0000f130: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
+0000f140: 2020 2020 2020 7761 6974 3a20 626f 6f6c        wait: bool
+0000f150: 203d 2046 616c 7365 2c0a 2020 2020 293a   = False,.    ):
+0000f160: 0a20 2020 2020 2020 2022 2222 5065 7273  .        """Pers
+0000f170: 6973 7420 7468 6520 6d65 7461 6461 7461  ist the metadata
+0000f180: 2061 6e64 206d 6174 6572 6961 6c69 7a65   and materialize
+0000f190: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+0000f1a0: 7570 2074 6f20 7468 6520 6665 6174 7572  up to the featur
+0000f1b0: 6520 7374 6f72 652e 0a0a 2020 2020 2020  e store...      
+0000f1c0: 2020 2121 2120 7761 726e 696e 6720 2243    !!! warning "C
+0000f1d0: 6861 6e67 6564 2069 6e20 332e 332e 3022  hanged in 3.3.0"
+0000f1e0: 0a20 2020 2020 2020 2020 2020 2060 696e  .            `in
+0000f1f0: 7365 7274 6020 616e 6420 6073 6176 6560  sert` and `save`
+0000f200: 206d 6574 686f 6473 2061 7265 206e 6f77   methods are now
+0000f210: 2061 7379 6e63 2062 7920 6465 6661 756c   async by defaul
+0000f220: 7420 696e 206e 6f6e 2d73 7061 726b 2063  t in non-spark c
+0000f230: 6c69 656e 7473 2e0a 2020 2020 2020 2020  lients..        
+0000f240: 2020 2020 546f 2061 6368 6965 7665 2074      To achieve t
+0000f250: 6865 206f 6c64 2062 6568 6176 696f 7572  he old behaviour
+0000f260: 2c20 7365 7420 6077 6169 7460 2061 7267  , set `wait` arg
+0000f270: 756d 656e 7420 746f 2060 5472 7565 602e  ument to `True`.
+0000f280: 0a0a 2020 2020 2020 2020 4361 6c6c 696e  ..        Callin
+0000f290: 6720 6073 6176 6560 2063 7265 6174 6573  g `save` creates
+0000f2a0: 2074 6865 206d 6574 6164 6174 6120 666f   the metadata fo
+0000f2b0: 7220 7468 6520 6665 6174 7572 6520 6772  r the feature gr
+0000f2c0: 6f75 7020 696e 2074 6865 2066 6561 7475  oup in the featu
+0000f2d0: 7265 2073 746f 7265 2e0a 2020 2020 2020  re store..      
+0000f2e0: 2020 4966 2061 2044 6174 6146 7261 6d65    If a DataFrame
+0000f2f0: 2c20 5244 4420 6f72 204e 6461 7272 6179  , RDD or Ndarray
+0000f300: 2069 7320 7072 6f76 6964 6564 2c20 7468   is provided, th
+0000f310: 6520 6461 7461 2069 7320 7772 6974 7465  e data is writte
+0000f320: 6e20 746f 2074 6865 0a20 2020 2020 2020  n to the.       
+0000f330: 206f 6e6c 696e 652f 6f66 666c 696e 6520   online/offline 
+0000f340: 6665 6174 7572 6520 7374 6f72 6520 6173  feature store as
+0000f350: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
+0000f360: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
+0000f370: 7468 6973 2077 7269 7465 7320 7468 6520  this writes the 
+0000f380: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
+0000f390: 2074 6865 206f 6666 6c69 6e65 2073 746f   the offline sto
+0000f3a0: 7261 6765 2c20 616e 6420 6966 0a20 2020  rage, and if.   
+0000f3b0: 2020 2020 2060 6f6e 6c69 6e65 5f65 6e61       `online_ena
+0000f3c0: 626c 6564 6020 666f 7220 7468 6520 6665  bled` for the fe
+0000f3d0: 6174 7572 6520 6772 6f75 702c 2061 6c73  ature group, als
+0000f3e0: 6f20 746f 2074 6865 206f 6e6c 696e 6520  o to the online 
+0000f3f0: 6665 6174 7572 6520 7374 6f72 652e 0a20  feature store.. 
+0000f400: 2020 2020 2020 2054 6865 2060 6665 6174         The `feat
+0000f410: 7572 6573 6020 6461 7461 6672 616d 6520  ures` dataframe 
+0000f420: 6361 6e20 6265 2061 2053 7061 726b 2044  can be a Spark D
+0000f430: 6174 6146 7261 6d65 206f 7220 5244 442c  ataFrame or RDD,
+0000f440: 2061 2050 616e 6461 7320 4461 7461 4672   a Pandas DataFr
+0000f450: 616d 652c 0a20 2020 2020 2020 206f 7220  ame,.        or 
+0000f460: 6120 7477 6f2d 6469 6d65 6e73 696f 6e61  a two-dimensiona
+0000f470: 6c20 4e75 6d70 7920 6172 7261 7920 6f72  l Numpy array or
+0000f480: 2061 2074 776f 2d64 696d 656e 7369 6f6e   a two-dimension
+0000f490: 616c 2050 7974 686f 6e20 6e65 7374 6564  al Python nested
+0000f4a0: 206c 6973 742e 0a20 2020 2020 2020 2023   list..        #
+0000f4b0: 2041 7267 756d 656e 7473 0a20 2020 2020   Arguments.     
+0000f4c0: 2020 2020 2020 2066 6561 7475 7265 733a         features:
+0000f4d0: 2044 6174 6146 7261 6d65 2c20 5244 442c   DataFrame, RDD,
+0000f4e0: 204e 6461 7272 6179 206f 7220 6120 6c69   Ndarray or a li
+0000f4f0: 7374 206f 6620 6665 6174 7572 6573 2e20  st of features. 
+0000f500: 4665 6174 7572 6573 2074 6f20 6265 2073  Features to be s
+0000f510: 6176 6564 2e0a 2020 2020 2020 2020 2020  aved..          
+0000f520: 2020 2020 2020 5468 6973 2061 7267 756d        This argum
+0000f530: 656e 7420 6973 206f 7074 696f 6e61 6c20  ent is optional 
+0000f540: 6966 2074 6865 2066 6561 7475 7265 206c  if the feature l
+0000f550: 6973 7420 6973 2070 726f 7669 6465 6420  ist is provided 
+0000f560: 696e 2074 6865 2063 7265 6174 655f 6665  in the create_fe
+0000f570: 6174 7572 655f 6772 6f75 7020 6f72 0a20  ature_group or. 
+0000f580: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f590: 6e20 7468 6520 6765 745f 6f72 5f63 7265  n the get_or_cre
+0000f5a0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+0000f5b0: 7020 6d65 7468 6f64 2069 6e76 6f6b 6174  p method invokat
+0000f5c0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+0000f5d0: 2077 7269 7465 5f6f 7074 696f 6e73 3a20   write_options: 
+0000f5e0: 4164 6469 7469 6f6e 616c 2077 7269 7465  Additional write
+0000f5f0: 206f 7074 696f 6e73 2061 7320 6b65 792d   options as key-
+0000f600: 7661 6c75 6520 7061 6972 732c 2064 6566  value pairs, def
+0000f610: 6175 6c74 7320 746f 2060 7b7d 602e 0a20  aults to `{}`.. 
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+0000f630: 6865 6e20 7573 696e 6720 7468 6520 6070  hen using the `p
+0000f640: 7974 686f 6e60 2065 6e67 696e 652c 2077  ython` engine, w
+0000f650: 7269 7465 5f6f 7074 696f 6e73 2063 616e  rite_options can
+0000f660: 2063 6f6e 7461 696e 2074 6865 0a20 2020   contain the.   
+0000f670: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
+0000f680: 6c6f 7769 6e67 2065 6e74 7269 6573 3a0a  lowing entries:.
+0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6a0: 2a20 6b65 7920 6073 7061 726b 6020 616e  * key `spark` an
+0000f6b0: 6420 7661 6c75 6520 616e 206f 626a 6563  d value an objec
+0000f6c0: 7420 6f66 2074 7970 650a 2020 2020 2020  t of type.      
+0000f6d0: 2020 2020 2020 2020 2020 5b68 7366 732e            [hsfs.
+0000f6e0: 636f 7265 2e6a 6f62 5f63 6f6e 6669 6775  core.job_configu
+0000f6f0: 7261 7469 6f6e 2e4a 6f62 436f 6e66 6967  ration.JobConfig
+0000f700: 7572 6174 696f 6e5d 282e 2e2f 6a6f 625f  uration](../job_
+0000f710: 636f 6e66 6967 7572 6174 696f 6e29 0a20  configuration). 
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
+0000f740: 6520 486f 7073 776f 726b 7320 4a6f 6220  e Hopsworks Job 
+0000f750: 7573 6564 2074 6f20 7772 6974 6520 6461  used to write da
+0000f760: 7461 2069 6e74 6f20 7468 650a 2020 2020  ta into the.    
+0000f770: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+0000f780: 6174 7572 6520 6772 6f75 702e 0a20 2020  ature group..   
+0000f790: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000f7a0: 6579 2060 7761 6974 5f66 6f72 5f6a 6f62  ey `wait_for_job
+0000f7b0: 6020 616e 6420 7661 6c75 6520 6054 7275  ` and value `Tru
+0000f7c0: 6560 206f 7220 6046 616c 7365 6020 746f  e` or `False` to
+0000f7d0: 2063 6f6e 6669 6775 7265 0a20 2020 2020   configure.     
+0000f7e0: 2020 2020 2020 2020 2020 2020 2077 6865               whe
+0000f7f0: 7468 6572 206f 7220 6e6f 7420 746f 2074  ther or not to t
+0000f800: 6865 2073 6176 6520 6361 6c6c 2073 686f  he save call sho
+0000f810: 756c 6420 7265 7475 726e 206f 6e6c 790a  uld return only.
+0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f830: 2020 6166 7465 7220 7468 6520 486f 7073    after the Hops
+0000f840: 776f 726b 7320 4a6f 6220 6861 7320 6669  works Job has fi
+0000f850: 6e69 7368 6564 2e20 4279 2064 6566 6175  nished. By defau
+0000f860: 6c74 2069 7420 646f 6573 206e 6f74 2077  lt it does not w
+0000f870: 6169 742e 0a20 2020 2020 2020 2020 2020  ait..           
+0000f880: 2020 2020 202a 206b 6579 2060 7374 6172       * key `star
+0000f890: 745f 6f66 666c 696e 655f 6261 636b 6669  t_offline_backfi
+0000f8a0: 6c6c 6020 616e 6420 7661 6c75 6520 6054  ll` and value `T
+0000f8b0: 7275 6560 206f 7220 6046 616c 7365 6020  rue` or `False` 
+0000f8c0: 746f 2063 6f6e 6669 6775 7265 0a20 2020  to configure.   
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000f8e0: 6865 7468 6572 206f 7220 6e6f 7420 746f  hether or not to
+0000f8f0: 2073 7461 7274 2074 6865 2062 6163 6b66   start the backf
+0000f900: 696c 6c20 6a6f 6220 746f 2077 7269 7465  ill job to write
+0000f910: 2064 6174 6120 746f 2074 6865 206f 6666   data to the off
+0000f920: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
+0000f930: 2020 2020 2020 2073 746f 7261 6765 2e20         storage. 
+0000f940: 4279 2064 6566 6175 6c74 2074 6865 2062  By default the b
+0000f950: 6163 6b66 696c 6c20 6a6f 6220 6765 7473  ackfill job gets
+0000f960: 2073 7461 7274 6564 2069 6d6d 6564 6961   started immedia
+0000f970: 7465 6c79 2e0a 2020 2020 2020 2020 2020  tely..          
+0000f980: 2020 2020 2020 2a20 6b65 7920 6069 6e74        * key `int
+0000f990: 6572 6e61 6c5f 6b61 666b 6160 2061 6e64  ernal_kafka` and
+0000f9a0: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
+0000f9b0: 2060 4661 6c73 6560 2069 6e20 6361 7365   `False` in case
+0000f9c0: 2079 6f75 2065 7374 6162 6c69 7368 6564   you established
+0000f9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f9e0: 2020 2063 6f6e 6e65 6374 6976 6974 7920     connectivity 
+0000f9f0: 6672 6f6d 2079 6f75 2050 7974 686f 6e20  from you Python 
+0000fa00: 656e 7669 726f 6e6d 656e 7420 746f 2074  environment to t
+0000fa10: 6865 2069 6e74 6572 6e61 6c20 6164 7665  he internal adve
+0000fa20: 7274 6973 6564 0a20 2020 2020 2020 2020  rtised.         
+0000fa30: 2020 2020 2020 2020 206c 6973 7465 6e65           listene
+0000fa40: 7273 206f 6620 7468 6520 486f 7073 776f  rs of the Hopswo
+0000fa50: 726b 7320 4b61 666b 6120 436c 7573 7465  rks Kafka Cluste
+0000fa60: 722e 2044 6566 6175 6c74 7320 746f 2060  r. Defaults to `
+0000fa70: 4661 6c73 6560 2061 6e64 0a20 2020 2020  False` and.     
+0000fa80: 2020 2020 2020 2020 2020 2020 2077 696c               wil
+0000fa90: 6c20 7573 6520 6578 7465 726e 616c 206c  l use external l
+0000faa0: 6973 7465 6e65 7273 2077 6865 6e20 636f  isteners when co
+0000fab0: 6e6e 6563 7469 6e67 2066 726f 6d20 6f75  nnecting from ou
+0000fac0: 7473 6964 6520 6f66 2048 6f70 7377 6f72  tside of Hopswor
+0000fad0: 6b73 2e0a 2020 2020 2020 2020 2020 2020  ks..            
+0000fae0: 7661 6c69 6461 7469 6f6e 5f6f 7074 696f  validation_optio
+0000faf0: 6e73 3a20 4164 6469 7469 6f6e 616c 2076  ns: Additional v
+0000fb00: 616c 6964 6174 696f 6e20 6f70 7469 6f6e  alidation option
+0000fb10: 7320 6173 206b 6579 2d76 616c 7565 2070  s as key-value p
+0000fb20: 6169 7273 2c20 6465 6661 756c 7473 2074  airs, defaults t
+0000fb30: 6f20 607b 7d60 2e0a 2020 2020 2020 2020  o `{}`..        
+0000fb40: 2020 2020 2020 2020 2a20 6b65 7920 6072          * key `r
+0000fb50: 756e 5f76 616c 6964 6174 696f 6e60 2062  un_validation` b
+0000fb60: 6f6f 6c65 616e 2076 616c 7565 2c20 7365  oolean value, se
+0000fb70: 7420 746f 2060 4661 6c73 6560 2074 6f20  t to `False` to 
+0000fb80: 736b 6970 2076 616c 6964 6174 696f 6e20  skip validation 
+0000fb90: 7465 6d70 6f72 6172 696c 7920 6f6e 2069  temporarily on i
+0000fba0: 6e67 6573 7469 6f6e 2e0a 2020 2020 2020  ngestion..      
+0000fbb0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+0000fbc0: 6073 6176 655f 7265 706f 7274 6020 626f  `save_report` bo
+0000fbd0: 6f6c 6561 6e20 7661 6c75 652c 2073 6574  olean value, set
+0000fbe0: 2074 6f20 6046 616c 7365 6020 746f 2073   to `False` to s
+0000fbf0: 6b69 7020 7570 6c6f 6164 206f 6620 7468  kip upload of th
+0000fc00: 6520 7661 6c69 6461 7469 6f6e 2072 6570  e validation rep
+0000fc10: 6f72 7420 746f 2048 6f70 7377 6f72 6b73  ort to Hopsworks
+0000fc20: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fc30: 2020 2a20 6b65 7920 6067 655f 7661 6c69    * key `ge_vali
+0000fc40: 6461 7465 5f6b 7761 7267 7360 2061 2064  date_kwargs` a d
+0000fc50: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+0000fc60: 6e69 6e67 206b 7761 7267 7320 666f 7220  ning kwargs for 
+0000fc70: 7468 6520 7661 6c69 6461 7465 206d 6574  the validate met
+0000fc80: 686f 6420 6f66 2047 7265 6174 2045 7870  hod of Great Exp
+0000fc90: 6563 7461 7469 6f6e 732e 0a20 2020 2020  ectations..     
+0000fca0: 2020 2020 2020 2077 6169 743a 2057 6169         wait: Wai
+0000fcb0: 7420 666f 7220 6a6f 6220 746f 2066 696e  t for job to fin
+0000fcc0: 6973 6820 6265 666f 7265 2072 6574 7572  ish before retur
+0000fcd0: 6e69 6e67 2c20 6465 6661 756c 7473 2074  ning, defaults t
+0000fce0: 6f20 6046 616c 7365 602e 0a20 2020 2020  o `False`..     
+0000fcf0: 2020 2020 2020 2020 2020 2053 686f 7274             Short
+0000fd00: 6375 7420 666f 7220 7265 6164 5f6f 7074  cut for read_opt
+0000fd10: 696f 6e73 2060 7b22 7761 6974 5f66 6f72  ions `{"wait_for
+0000fd20: 5f6a 6f62 223a 2046 616c 7365 7d60 2e0a  _job": False}`..
+0000fd30: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+0000fd40: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+0000fd50: 4a6f 6260 3a20 5768 656e 2075 7369 6e67  Job`: When using
+0000fd60: 2074 6865 2060 7079 7468 6f6e 6020 656e   the `python` en
+0000fd70: 6769 6e65 2c20 6974 2072 6574 7572 6e73  gine, it returns
+0000fd80: 2074 6865 2048 6f70 7377 6f72 6b73 204a   the Hopsworks J
+0000fd90: 6f62 0a20 2020 2020 2020 2020 2020 2020  ob.             
+0000fda0: 2020 2074 6861 7420 7761 7320 6c61 756e     that was laun
+0000fdb0: 6368 6564 2074 6f20 696e 6765 7374 2074  ched to ingest t
+0000fdc0: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0000fdd0: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+0000fde0: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+0000fdf0: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+0000fe00: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+0000fe10: 7441 5049 4572 726f 7260 2e20 556e 6162  tAPIError`. Unab
+0000fe20: 6c65 2074 6f20 6372 6561 7465 2066 6561  le to create fea
+0000fe30: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+0000fe40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fe50: 6966 2028 6665 6174 7572 6573 2069 7320  if (features is 
+0000fe60: 4e6f 6e65 2061 6e64 206c 656e 2873 656c  None and len(sel
+0000fe70: 662e 5f66 6561 7475 7265 7329 203e 2030  f._features) > 0
+0000fe80: 2920 6f72 2028 0a20 2020 2020 2020 2020  ) or (.         
+0000fe90: 2020 2069 7369 6e73 7461 6e63 6528 6665     isinstance(fe
+0000fea0: 6174 7572 6573 2c20 4c69 7374 290a 2020  atures, List).  
+0000feb0: 2020 2020 2020 2020 2020 616e 6420 6c65            and le
+0000fec0: 6e28 6665 6174 7572 6573 2920 3e20 300a  n(features) > 0.
+0000fed0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0000fee0: 616c 6c28 5b69 7369 6e73 7461 6e63 6528  all([isinstance(
+0000fef0: 662c 2066 6561 7475 7265 2e46 6561 7475  f, feature.Featu
+0000ff00: 7265 2920 666f 7220 6620 696e 2066 6561  re) for f in fea
+0000ff10: 7475 7265 735d 290a 2020 2020 2020 2020  tures]).        
+0000ff20: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+0000ff30: 2054 6869 7320 6973 2064 6f6e 6520 666f   This is done fo
+0000ff40: 7220 636f 6d70 6174 6962 696c 6974 792e  r compatibility.
+0000ff50: 2055 7365 7273 2063 616e 2073 7065 6369   Users can speci
+0000ff60: 6679 2074 6865 2066 6561 7475 7265 206c  fy the feature l
+0000ff70: 6973 7420 696e 2074 6865 0a20 2020 2020  ist in the.     
+0000ff80: 2020 2020 2020 2023 2028 6765 745f 6f72         # (get_or
+0000ff90: 5f29 6372 6561 7465 5f66 6561 7475 7265  _)create_feature
+0000ffa0: 5f67 726f 7570 2e20 5573 6572 7320 6361  _group. Users ca
+0000ffb0: 6e20 616c 736f 2070 726f 7669 6465 2074  n also provide t
+0000ffc0: 6865 2066 6561 7475 7265 206c 6973 7420  he feature list 
+0000ffd0: 696e 2074 6865 2073 6176 6528 292e 0a20  in the save().. 
+0000ffe0: 2020 2020 2020 2020 2020 2023 2054 686f             # Tho
+0000fff0: 7567 6820 6974 2773 2061 6e20 6f70 7469  ugh it's an opti
+00010000: 6f6e 616c 2070 6172 616d 6574 6572 2e0a  onal parameter..
+00010010: 2020 2020 2020 2020 2020 2020 2320 466f              # Fo
+00010020: 7220 636f 6e73 6973 7465 6e63 7920 7265  r consistency re
+00010030: 6173 6f6e 7320 6966 2074 6865 2075 7365  asons if the use
+00010040: 7220 7370 6563 6966 7920 626f 7468 2074  r specify both t
+00010050: 6865 2066 6561 7475 7265 206c 6973 7420  he feature list 
+00010060: 696e 2074 6865 2028 6765 745f 6f72 5f29  in the (get_or_)
+00010070: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00010080: 726f 7570 0a20 2020 2020 2020 2020 2020  roup.           
+00010090: 2023 2061 6e64 2069 6e20 7468 6520 6073   # and in the `s
+000100a0: 6176 6528 2960 2063 616c 6c2c 2074 6865  ave()` call, the
+000100b0: 6e20 7468 6520 2867 6574 5f6f 725f 2963  n the (get_or_)c
+000100c0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+000100d0: 6f75 7020 7769 6e73 2e0a 2020 2020 2020  oup wins..      
+000100e0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
+000100f0: 636f 6e73 6973 7465 6e74 2077 6974 6820  consistent with 
+00010100: 7468 6520 6265 6861 7669 6f72 206f 6620  the behavior of 
+00010110: 7468 6520 696e 7365 7274 206d 6574 686f  the insert metho
+00010120: 6420 7768 6572 6520 7468 6520 6665 6174  d where the feat
+00010130: 7572 6520 6c69 7374 2077 696e 7320 6f76  ure list wins ov
+00010140: 6572 2074 6865 0a20 2020 2020 2020 2020  er the.         
+00010150: 2020 2023 2064 6174 6166 7261 6d65 2073     # dataframe s
+00010160: 7472 7563 7475 7265 0a20 2020 2020 2020  tructure.       
+00010170: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
+00010180: 7265 7320 3d20 7365 6c66 2e5f 6665 6174  res = self._feat
+00010190: 7572 6573 2069 6620 6c65 6e28 7365 6c66  ures if len(self
+000101a0: 2e5f 6665 6174 7572 6573 2920 3e20 3020  ._features) > 0 
+000101b0: 656c 7365 2066 6561 7475 7265 730a 2020  else features.  
+000101c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000101d0: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+000101e0: 6769 6e65 2e73 6176 655f 6665 6174 7572  gine.save_featur
+000101f0: 655f 6772 6f75 705f 6d65 7461 6461 7461  e_group_metadata
+00010200: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010210: 2020 7365 6c66 2c20 4e6f 6e65 2c20 7772    self, None, wr
+00010220: 6974 655f 6f70 7469 6f6e 730a 2020 2020  ite_options.    
+00010230: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00010240: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00010250: 6e65 2c20 4e6f 6e65 0a0a 2020 2020 2020  ne, None..      
+00010260: 2020 6966 2066 6561 7475 7265 7320 6973    if features is
+00010270: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00010280: 2020 2072 6169 7365 2046 6561 7475 7265     raise Feature
+00010290: 5374 6f72 6545 7863 6570 7469 6f6e 280a  StoreException(.
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2246 6561 7475 7265 206c 6973 7420 6e6f  "Feature list no
+000102c0: 7420 7072 6f76 6964 6564 2069 6e20 7468  t provided in th
+000102d0: 6520 6372 6561 7465 5f66 6561 7475 7265  e create_feature
+000102e0: 5f67 726f 7570 206f 7220 6765 745f 6f72  _group or get_or
+000102f0: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
+00010300: 6772 6f75 7020 696e 766f 6b61 7469 6f6e  group invokation
+00010310: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
+00010320: 2020 2020 2b20 2220 506c 6561 7365 2070      + " Please p
+00010330: 726f 7669 6465 2061 206c 6973 7420 6f66  rovide a list of
+00010340: 2066 6561 7475 7265 7320 6f72 2061 2044   features or a D
+00010350: 6174 6166 7261 6d65 220a 2020 2020 2020  ataframe".      
+00010360: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010370: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
+00010380: 6d65 203d 2065 6e67 696e 652e 6765 745f  me = engine.get_
+00010390: 696e 7374 616e 6365 2829 2e63 6f6e 7665  instance().conve
+000103a0: 7274 5f74 6f5f 6465 6661 756c 745f 6461  rt_to_default_da
+000103b0: 7461 6672 616d 6528 6665 6174 7572 6573  taframe(features
+000103c0: 290a 0a20 2020 2020 2020 2075 7365 725f  )..        user_
+000103d0: 7665 7273 696f 6e20 3d20 7365 6c66 2e5f  version = self._
+000103e0: 7665 7273 696f 6e0a 0a20 2020 2020 2020  version..       
+000103f0: 2069 6620 7772 6974 655f 6f70 7469 6f6e   if write_option
+00010400: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+00010410: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
+00010420: 696f 6e73 203d 207b 7d0a 2020 2020 2020  ions = {}.      
+00010430: 2020 6966 2022 7761 6974 5f66 6f72 5f6a    if "wait_for_j
+00010440: 6f62 2220 6e6f 7420 696e 2077 7269 7465  ob" not in write
+00010450: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
+00010460: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+00010470: 6f6e 735b 2277 6169 745f 666f 725f 6a6f  ons["wait_for_jo
+00010480: 6222 5d20 3d20 7761 6974 0a0a 2020 2020  b"] = wait..    
+00010490: 2020 2020 2320 6667 5f6a 6f62 2069 7320      # fg_job is 
+000104a0: 7573 6564 206f 6e6c 7920 6966 2074 6865  used only if the
+000104b0: 2070 7974 686f 6e20 656e 6769 6e65 2069   python engine i
+000104c0: 7320 7573 6564 0a20 2020 2020 2020 2066  s used.        f
+000104d0: 675f 6a6f 622c 2067 655f 7265 706f 7274  g_job, ge_report
+000104e0: 203d 2073 656c 662e 5f66 6561 7475 7265   = self._feature
+000104f0: 5f67 726f 7570 5f65 6e67 696e 652e 7361  _group_engine.sa
+00010500: 7665 280a 2020 2020 2020 2020 2020 2020  ve(.            
+00010510: 7365 6c66 2c20 6665 6174 7572 655f 6461  self, feature_da
+00010520: 7461 6672 616d 652c 2077 7269 7465 5f6f  taframe, write_o
+00010530: 7074 696f 6e73 2c20 7661 6c69 6461 7469  ptions, validati
+00010540: 6f6e 5f6f 7074 696f 6e73 0a20 2020 2020  on_options.     
+00010550: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00010560: 6765 5f72 6570 6f72 7420 6973 204e 6f6e  ge_report is Non
+00010570: 6520 6f72 2067 655f 7265 706f 7274 2e69  e or ge_report.i
+00010580: 6e67 6573 7469 6f6e 5f72 6573 756c 7420  ngestion_result 
+00010590: 3d3d 2022 494e 4745 5354 4544 223a 0a20  == "INGESTED":. 
+000105a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000105b0: 5f63 6f64 655f 656e 6769 6e65 2e73 6176  _code_engine.sav
+000105c0: 655f 636f 6465 2873 656c 6629 0a0a 2020  e_code(self)..  
+000105d0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000105e0: 6174 6973 7469 6373 5f63 6f6e 6669 672e  atistics_config.
+000105f0: 656e 6162 6c65 6420 616e 6420 656e 6769  enabled and engi
+00010600: 6e65 2e67 6574 5f74 7970 6528 2920 3d3d  ne.get_type() ==
+00010610: 2022 7370 6172 6b22 3a0a 2020 2020 2020   "spark":.      
+00010620: 2020 2020 2020 2320 4f6e 6c79 2063 6f6d        # Only com
+00010630: 7075 7465 2073 7461 7469 7374 6963 7320  pute statistics 
+00010640: 6966 2074 6865 2065 6e67 696e 6520 6973  if the engine is
+00010650: 2053 7061 726b 2e0a 2020 2020 2020 2020   Spark..        
+00010660: 2020 2020 2320 466f 7220 5079 7468 6f6e      # For Python
+00010670: 2065 6e67 696e 652c 2074 6865 2063 6f6d   engine, the com
+00010680: 7075 7461 7469 6f6e 2068 6170 7065 6e73  putation happens
+00010690: 2069 6e20 7468 6520 486f 7073 776f 726b   in the Hopswork
+000106a0: 7320 6170 706c 6963 6174 696f 6e0a 2020  s application.  
+000106b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000106c0: 7374 6174 6973 7469 6373 5f65 6e67 696e  statistics_engin
+000106d0: 652e 636f 6d70 7574 655f 7374 6174 6973  e.compute_statis
+000106e0: 7469 6373 2873 656c 662c 2066 6561 7475  tics(self, featu
+000106f0: 7265 5f64 6174 6166 7261 6d65 290a 2020  re_dataframe).  
+00010700: 2020 2020 2020 6966 2075 7365 725f 7665        if user_ve
+00010710: 7273 696f 6e20 6973 204e 6f6e 653a 0a20  rsion is None:. 
+00010720: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00010730: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
+00010740: 2020 2020 2020 2020 2020 224e 6f20 7665            "No ve
+00010750: 7273 696f 6e20 7072 6f76 6964 6564 2066  rsion provided f
+00010760: 6f72 2063 7265 6174 696e 6720 6665 6174  or creating feat
+00010770: 7572 6520 6772 6f75 7020 607b 7d60 2c20  ure group `{}`, 
+00010780: 696e 6372 656d 656e 7465 6420 7665 7273  incremented vers
+00010790: 696f 6e20 746f 2060 7b7d 602e 222e 666f  ion to `{}`.".fo
+000107a0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+000107b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000107c0: 6e61 6d65 2c20 7365 6c66 2e5f 7665 7273  name, self._vers
+000107d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000107e0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+000107f0: 2020 2020 2020 2075 7469 6c2e 5665 7273         util.Vers
+00010800: 696f 6e57 6172 6e69 6e67 2c0a 2020 2020  ionWarning,.    
+00010810: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010820: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
+00010830: 2020 2020 2020 2066 675f 6a6f 622c 0a20         fg_job,. 
+00010840: 2020 2020 2020 2020 2020 2067 655f 7265             ge_re
+00010850: 706f 7274 2e74 6f5f 6765 5f74 7970 6528  port.to_ge_type(
+00010860: 2920 6966 2067 655f 7265 706f 7274 2069  ) if ge_report i
+00010870: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00010880: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
+00010890: 0a20 2020 2064 6566 2069 6e73 6572 7428  .    def insert(
+000108a0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000108b0: 2020 2020 2020 2066 6561 7475 7265 733a         features:
+000108c0: 2055 6e69 6f6e 5b0a 2020 2020 2020 2020   Union[.        
+000108d0: 2020 2020 7064 2e44 6174 6146 7261 6d65      pd.DataFrame
+000108e0: 2c0a 2020 2020 2020 2020 2020 2020 5479  ,.            Ty
+000108f0: 7065 5661 7228 2270 7973 7061 726b 2e73  peVar("pyspark.s
+00010900: 716c 2e44 6174 6146 7261 6d65 2229 2c20  ql.DataFrame"), 
+00010910: 2023 206e 6f71 613a 2046 3832 310a 2020   # noqa: F821.  
+00010920: 2020 2020 2020 2020 2020 5479 7065 5661            TypeVa
+00010930: 7228 2270 7973 7061 726b 2e52 4444 2229  r("pyspark.RDD")
+00010940: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+00010950: 2020 2020 2020 2020 2020 2020 6e70 2e6e              np.n
+00010960: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
+00010970: 2020 2020 4c69 7374 5b6c 6973 745d 2c0a      List[list],.
+00010980: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00010990: 2020 206f 7665 7277 7269 7465 3a20 4f70     overwrite: Op
+000109a0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
+000109b0: 616c 7365 2c0a 2020 2020 2020 2020 6f70  alse,.        op
+000109c0: 6572 6174 696f 6e3a 204f 7074 696f 6e61  eration: Optiona
+000109d0: 6c5b 7374 725d 203d 2022 7570 7365 7274  l[str] = "upsert
+000109e0: 222c 0a20 2020 2020 2020 2073 746f 7261  ",.        stora
+000109f0: 6765 3a20 4f70 7469 6f6e 616c 5b73 7472  ge: Optional[str
+00010a00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00010a10: 2020 7772 6974 655f 6f70 7469 6f6e 733a    write_options:
+00010a20: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00010a30: 7472 2c20 416e 795d 5d20 3d20 7b7d 2c0a  tr, Any]] = {},.
+00010a40: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+00010a50: 6f6e 5f6f 7074 696f 6e73 3a20 4f70 7469  on_options: Opti
+00010a60: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
+00010a70: 6e79 5d5d 203d 207b 7d2c 0a20 2020 2020  ny]] = {},.     
+00010a80: 2020 2073 6176 655f 636f 6465 3a20 4f70     save_code: Op
+00010a90: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
+00010aa0: 7275 652c 0a20 2020 2020 2020 2077 6169  rue,.        wai
+00010ab0: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
+00010ac0: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
+00010ad0: 4f70 7469 6f6e 616c 5b4a 6f62 5d2c 204f  Optional[Job], O
+00010ae0: 7074 696f 6e61 6c5b 5661 6c69 6461 7469  ptional[Validati
+00010af0: 6f6e 5265 706f 7274 5d5d 3a0a 2020 2020  onReport]]:.    
+00010b00: 2020 2020 2222 2250 6572 7369 7374 2074      """Persist t
+00010b10: 6865 206d 6574 6164 6174 6120 616e 6420  he metadata and 
+00010b20: 6d61 7465 7269 616c 697a 6520 7468 6520  materialize the 
+00010b30: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
+00010b40: 2074 6865 2066 6561 7475 7265 2073 746f   the feature sto
+00010b50: 7265 0a20 2020 2020 2020 206f 7220 696e  re.        or in
+00010b60: 7365 7274 2064 6174 6120 6672 6f6d 2061  sert data from a
+00010b70: 2064 6174 6166 7261 6d65 2069 6e74 6f20   dataframe into 
+00010b80: 7468 6520 6578 6973 7469 6e67 2066 6561  the existing fea
+00010b90: 7475 7265 2067 726f 7570 2e0a 0a20 2020  ture group...   
+00010ba0: 2020 2020 2049 6e63 7265 6d65 6e74 616c       Incremental
+00010bb0: 6c79 2069 6e73 6572 7420 6461 7461 2074  ly insert data t
+00010bc0: 6f20 6120 6665 6174 7572 6520 6772 6f75  o a feature grou
+00010bd0: 7020 6f72 206f 7665 7277 7269 7465 2061  p or overwrite a
+00010be0: 6c6c 2020 6461 7461 2063 6f6e 7461 696e  ll  data contain
+00010bf0: 6564 2069 6e20 7468 6520 6665 6174 7572  ed in the featur
+00010c00: 6520 6772 6f75 702e 2042 790a 2020 2020  e group. By.    
+00010c10: 2020 2020 6465 6661 756c 742c 2074 6865      default, the
+00010c20: 2064 6174 6120 6973 2069 6e73 6572 7465   data is inserte
+00010c30: 6420 696e 746f 2074 6865 206f 6666 6c69  d into the offli
+00010c40: 6e65 2073 746f 7261 6765 2061 7320 7765  ne storage as we
+00010c50: 6c6c 2061 7320 7468 6520 6f6e 6c69 6e65  ll as the online
+00010c60: 2073 746f 7261 6765 2069 6620 7468 6520   storage if the 
+00010c70: 6665 6174 7572 6520 6772 6f75 7020 6973  feature group is
+00010c80: 0a20 2020 2020 2020 2060 6f6e 6c69 6e65  .        `online
+00010c90: 5f65 6e61 626c 6564 3d54 7275 6560 2e20  _enabled=True`. 
+00010ca0: 546f 2069 6e73 6572 7420 6f6e 6c79 2069  To insert only i
+00010cb0: 6e74 6f20 7468 6520 6f6e 6c69 6e65 206f  nto the online o
+00010cc0: 7220 6f66 666c 696e 6520 7374 6f72 6167  r offline storag
+00010cd0: 6520 7365 7420 6073 746f 7261 6765 3d22  e set `storage="
+00010ce0: 6f6e 6c69 6e65 2260 206f 720a 2020 2020  online"` or.    
+00010cf0: 2020 2020 6073 746f 7261 6765 3d22 6f66      `storage="of
+00010d00: 666c 696e 6522 6020 7265 7370 6563 7469  fline"` respecti
+00010d10: 7665 6c79 2e0a 0a20 2020 2020 2020 2054  vely...        T
+00010d20: 6865 2060 6665 6174 7572 6573 6020 6461  he `features` da
+00010d30: 7461 6672 616d 6520 6361 6e20 6265 2061  taframe can be a
+00010d40: 2053 7061 726b 2044 6174 6146 7261 6d65   Spark DataFrame
+00010d50: 206f 7220 5244 442c 2061 2050 616e 6461   or RDD, a Panda
+00010d60: 7320 4461 7461 4672 616d 652c 0a20 2020  s DataFrame,.   
+00010d70: 2020 2020 206f 7220 6120 7477 6f2d 6469       or a two-di
+00010d80: 6d65 6e73 696f 6e61 6c20 4e75 6d70 7920  mensional Numpy 
+00010d90: 6172 7261 7920 6f72 2061 2074 776f 2d64  array or a two-d
+00010da0: 696d 656e 7369 6f6e 616c 2050 7974 686f  imensional Pytho
+00010db0: 6e20 6e65 7374 6564 206c 6973 742e 0a20  n nested list.. 
+00010dc0: 2020 2020 2020 2049 6620 7374 6174 6973         If statis
+00010dd0: 7469 6373 2061 7265 2065 6e61 626c 6564  tics are enabled
+00010de0: 2c20 7374 6174 6973 7469 6373 2061 7265  , statistics are
+00010df0: 2072 6563 6f6d 7075 7465 6420 666f 7220   recomputed for 
+00010e00: 7468 6520 656e 7469 7265 2066 6561 7475  the entire featu
+00010e10: 7265 0a20 2020 2020 2020 2067 726f 7570  re.        group
+00010e20: 2e0a 2020 2020 2020 2020 4966 2066 6561  ..        If fea
+00010e30: 7475 7265 2067 726f 7570 2773 2074 696d  ture group's tim
+00010e40: 6520 7472 6176 656c 2066 6f72 6d61 7420  e travel format 
+00010e50: 6973 2060 4855 4449 6020 7468 656e 2060  is `HUDI` then `
+00010e60: 6f70 6572 6174 696f 6e60 2061 7267 756d  operation` argum
+00010e70: 656e 7420 6361 6e20 6265 0a20 2020 2020  ent can be.     
+00010e80: 2020 2065 6974 6865 7220 6069 6e73 6572     either `inser
+00010e90: 7460 206f 7220 6075 7073 6572 7460 2e0a  t` or `upsert`..
+00010ea0: 0a20 2020 2020 2020 2049 6620 6665 6174  .        If feat
+00010eb0: 7572 6520 6772 6f75 7020 646f 6573 6e27  ure group doesn'
+00010ec0: 7420 6578 6973 7473 2020 7468 6520 696e  t exists  the in
+00010ed0: 7365 7274 206d 6574 686f 6420 7769 6c6c  sert method will
+00010ee0: 2063 7265 6174 6520 7468 6520 6e65 6365   create the nece
+00010ef0: 7373 6172 7920 6d65 7461 6461 7461 2074  ssary metadata t
+00010f00: 6865 2066 6972 7374 2074 696d 6520 6974  he first time it
+00010f10: 2069 730a 2020 2020 2020 2020 696e 766f   is.        invo
+00010f20: 6b65 6420 616e 6420 7772 6974 6573 2074  ked and writes t
+00010f30: 6865 2073 7065 6369 6669 6564 2060 6665  he specified `fe
+00010f40: 6174 7572 6573 6020 6461 7461 6672 616d  atures` datafram
+00010f50: 6520 6173 2066 6561 7475 7265 2067 726f  e as feature gro
+00010f60: 7570 2074 6f20 7468 6520 6f6e 6c69 6e65  up to the online
+00010f70: 2f6f 6666 6c69 6e65 2066 6561 7475 7265  /offline feature
+00010f80: 2073 746f 7265 2e0a 0a20 2020 2020 2020   store...       
+00010f90: 2021 2121 2077 6172 6e69 6e67 2022 4368   !!! warning "Ch
+00010fa0: 616e 6765 6420 696e 2033 2e33 2e30 220a  anged in 3.3.0".
+00010fb0: 2020 2020 2020 2020 2020 2020 6069 6e73              `ins
+00010fc0: 6572 7460 2061 6e64 2060 7361 7665 6020  ert` and `save` 
+00010fd0: 6d65 7468 6f64 7320 6172 6520 6e6f 7720  methods are now 
+00010fe0: 6173 796e 6320 6279 2064 6566 6175 6c74  async by default
+00010ff0: 2069 6e20 6e6f 6e2d 7370 6172 6b20 636c   in non-spark cl
+00011000: 6965 6e74 732e 0a20 2020 2020 2020 2020  ients..         
+00011010: 2020 2054 6f20 6163 6869 6576 6520 7468     To achieve th
+00011020: 6520 6f6c 6420 6265 6861 7669 6f75 722c  e old behaviour,
+00011030: 2073 6574 2060 7761 6974 6020 6172 6775   set `wait` argu
+00011040: 6d65 6e74 2074 6f20 6054 7275 6560 2e0a  ment to `True`..
+00011050: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+00011060: 6d70 6c65 2022 5570 7365 7274 206e 6577  mple "Upsert new
+00011070: 2066 6561 7475 7265 2064 6174 6120 7769   feature data wi
+00011080: 7468 2074 696d 6520 7472 6176 656c 2066  th time travel f
+00011090: 6f72 6d61 7420 6048 5544 4960 220a 2020  ormat `HUDI`".  
+000110a0: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
+000110b0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
+000110c0: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
+000110d0: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
+000110e0: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
+000110f0: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
+00011100: 2066 6720 3d20 6673 2e67 6574 5f6f 725f   fg = fs.get_or_
+00011110: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00011120: 726f 7570 280a 2020 2020 2020 2020 2020  roup(.          
+00011130: 2020 2020 2020 6e61 6d65 3d27 6269 7463        name='bitc
+00011140: 6f69 6e5f 7072 6963 6527 2c0a 2020 2020  oin_price',.    
+00011150: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00011160: 7269 7074 696f 6e3d 2742 6974 636f 696e  ription='Bitcoin
+00011170: 2070 7269 6365 2061 6767 7265 6761 7465   price aggregate
+00011180: 6420 666f 7220 6461 7973 272c 0a20 2020  d for days',.   
+00011190: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+000111a0: 7369 6f6e 3d31 2c0a 2020 2020 2020 2020  sion=1,.        
+000111b0: 2020 2020 2020 2020 7072 696d 6172 795f          primary_
+000111c0: 6b65 793d 5b27 756e 6978 275d 2c0a 2020  key=['unix'],.  
+000111d0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+000111e0: 6c69 6e65 5f65 6e61 626c 6564 3d54 7275  line_enabled=Tru
+000111f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00011200: 2020 2065 7665 6e74 5f74 696d 653d 2775     event_time='u
+00011210: 6e69 7827 0a20 2020 2020 2020 2020 2020  nix'.           
+00011220: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00011230: 6667 2e69 6e73 6572 7428 6466 5f62 6974  fg.insert(df_bit
+00011240: 636f 696e 5f70 726f 6365 7373 6564 290a  coin_processed).
+00011250: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00011260: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+00011270: 6d70 6c65 2022 4173 796e 6320 696e 7365  mple "Async inse
+00011280: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+00011290: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+000112a0: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+000112b0: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+000112c0: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+000112d0: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
+000112e0: 2020 2020 2020 2066 6731 203d 2066 732e         fg1 = fs.
+000112f0: 6765 745f 6f72 5f63 7265 6174 655f 6665  get_or_create_fe
+00011300: 6174 7572 655f 6772 6f75 7028 0a20 2020  ature_group(.   
+00011310: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00011320: 653d 2766 6561 7475 7265 5f67 726f 7570  e='feature_group
+00011330: 5f6e 616d 6531 272c 0a20 2020 2020 2020  _name1',.       
+00011340: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00011350: 7469 6f6e 3d27 4465 7363 7269 7074 696f  tion='Descriptio
+00011360: 6e20 6f66 2074 6865 2066 6972 7374 2046  n of the first F
+00011370: 4727 2c0a 2020 2020 2020 2020 2020 2020  G',.            
+00011380: 2020 2020 7665 7273 696f 6e3d 312c 0a20      version=1,. 
+00011390: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000113a0: 7269 6d61 7279 5f6b 6579 3d5b 2775 6e69  rimary_key=['uni
+000113b0: 7827 5d2c 0a20 2020 2020 2020 2020 2020  x'],.           
+000113c0: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
+000113d0: 6c65 643d 5472 7565 2c0a 2020 2020 2020  led=True,.      
+000113e0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+000113f0: 7469 6d65 3d27 756e 6978 270a 2020 2020  time='unix'.    
+00011400: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00011410: 2020 2020 2020 2320 6173 796e 6320 696e        # async in
+00011420: 7365 7274 696f 6e20 696e 206f 7264 6572  sertion in order
+00011430: 206e 6f74 2074 6f20 7761 6974 2074 696c   not to wait til
+00011440: 6c20 6669 6e69 7368 206f 6620 7468 6520  l finish of the 
+00011450: 6a6f 620a 2020 2020 2020 2020 2020 2020  job.            
+00011460: 6667 2e69 6e73 6572 7428 6466 5f66 6f72  fg.insert(df_for
+00011470: 5f66 6731 2c20 7772 6974 655f 6f70 7469  _fg1, write_opti
+00011480: 6f6e 733d 7b22 7761 6974 5f66 6f72 5f6a  ons={"wait_for_j
+00011490: 6f62 2220 3a20 4661 6c73 657d 290a 0a20  ob" : False}).. 
+000114a0: 2020 2020 2020 2020 2020 2066 6732 203d             fg2 =
+000114b0: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+000114c0: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+000114d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114e0: 206e 616d 653d 2766 6561 7475 7265 5f67   name='feature_g
+000114f0: 726f 7570 5f6e 616d 6532 272c 0a20 2020  roup_name2',.   
+00011500: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00011510: 6372 6970 7469 6f6e 3d27 4465 7363 7269  cription='Descri
+00011520: 7074 696f 6e20 6f66 2074 6865 2073 6563  ption of the sec
+00011530: 6f6e 6420 4647 272c 0a20 2020 2020 2020  ond FG',.       
+00011540: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
+00011550: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
+00011560: 2020 2020 7072 696d 6172 795f 6b65 793d      primary_key=
+00011570: 5b27 756e 6978 275d 2c0a 2020 2020 2020  ['unix'],.      
+00011580: 2020 2020 2020 2020 2020 6f6e 6c69 6e65            online
+00011590: 5f65 6e61 626c 6564 3d54 7275 652c 0a20  _enabled=True,. 
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000115b0: 7665 6e74 5f74 696d 653d 2775 6e69 7827  vent_time='unix'
+000115c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000115d0: 2020 2020 2020 2020 2020 2066 672e 696e             fg.in
+000115e0: 7365 7274 2864 665f 666f 725f 6667 3229  sert(df_for_fg2)
+000115f0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+00011600: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
+00011610: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+00011620: 2020 6665 6174 7572 6573 3a20 4461 7461    features: Data
+00011630: 4672 616d 652c 2052 4444 2c20 4e64 6172  Frame, RDD, Ndar
+00011640: 7261 792c 206c 6973 742e 2046 6561 7475  ray, list. Featu
+00011650: 7265 7320 746f 2062 6520 7361 7665 642e  res to be saved.
+00011660: 0a20 2020 2020 2020 2020 2020 206f 7665  .            ove
+00011670: 7277 7269 7465 3a20 4472 6f70 2061 6c6c  rwrite: Drop all
+00011680: 2064 6174 6120 696e 2074 6865 2066 6561   data in the fea
+00011690: 7475 7265 2067 726f 7570 2062 6566 6f72  ture group befor
+000116a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000116b0: 2020 696e 7365 7274 696e 6720 6e65 7720    inserting new 
+000116c0: 6461 7461 2e20 5468 6973 2064 6f65 7320  data. This does 
+000116d0: 6e6f 7420 6166 6665 6374 206d 6574 6164  not affect metad
+000116e0: 6174 612c 2064 6566 6175 6c74 7320 746f  ata, defaults to
+000116f0: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+00011700: 2020 2020 6f70 6572 6174 696f 6e3a 2041      operation: A
+00011710: 7061 6368 6520 4875 6469 206f 7065 7261  pache Hudi opera
+00011720: 7469 6f6e 2074 7970 6520 6022 696e 7365  tion type `"inse
+00011730: 7274 2260 206f 7220 6022 7570 7365 7274  rt"` or `"upsert
+00011740: 2260 2e0a 2020 2020 2020 2020 2020 2020  "`..            
+00011750: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00011760: 6022 7570 7365 7274 2260 2e0a 2020 2020  `"upsert"`..    
+00011770: 2020 2020 2020 2020 7374 6f72 6167 653a          storage:
+00011780: 204f 7665 7277 7269 7465 2064 6566 6175   Overwrite defau
+00011790: 6c74 2062 6568 6176 696f 7572 2c20 7772  lt behaviour, wr
+000117a0: 6974 6520 746f 206f 6666 6c69 6e65 0a20  ite to offline. 
+000117b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000117c0: 746f 7261 6765 206f 6e6c 7920 7769 7468  torage only with
+000117d0: 2060 226f 6666 6c69 6e65 2260 206f 7220   `"offline"` or 
+000117e0: 6f6e 6c69 6e65 206f 6e6c 7920 7769 7468  online only with
+000117f0: 2060 226f 6e6c 696e 6522 602c 2064 6566   `"online"`, def
+00011800: 6175 6c74 730a 2020 2020 2020 2020 2020  aults.          
+00011810: 2020 2020 2020 746f 2060 4e6f 6e65 602e        to `None`.
+00011820: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
+00011830: 7465 5f6f 7074 696f 6e73 3a20 4164 6469  te_options: Addi
+00011840: 7469 6f6e 616c 2077 7269 7465 206f 7074  tional write opt
+00011850: 696f 6e73 2061 7320 6b65 792d 7661 6c75  ions as key-valu
+00011860: 6520 7061 6972 732c 2064 6566 6175 6c74  e pairs, default
+00011870: 7320 746f 2060 7b7d 602e 0a20 2020 2020  s to `{}`..     
+00011880: 2020 2020 2020 2020 2020 2057 6865 6e20             When 
+00011890: 7573 696e 6720 7468 6520 6070 7974 686f  using the `pytho
+000118a0: 6e60 2065 6e67 696e 652c 2077 7269 7465  n` engine, write
+000118b0: 5f6f 7074 696f 6e73 2063 616e 2063 6f6e  _options can con
+000118c0: 7461 696e 2074 6865 0a20 2020 2020 2020  tain the.       
+000118d0: 2020 2020 2020 2020 2066 6f6c 6c6f 7769           followi
+000118e0: 6e67 2065 6e74 7269 6573 3a0a 2020 2020  ng entries:.    
+000118f0: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
+00011900: 7920 6073 7061 726b 6020 616e 6420 7661  y `spark` and va
+00011910: 6c75 6520 616e 206f 626a 6563 7420 6f66  lue an object of
+00011920: 2074 7970 650a 2020 2020 2020 2020 2020   type.          
+00011930: 2020 2020 2020 5b68 7366 732e 636f 7265        [hsfs.core
+00011940: 2e6a 6f62 5f63 6f6e 6669 6775 7261 7469  .job_configurati
+00011950: 6f6e 2e4a 6f62 436f 6e66 6967 7572 6174  on.JobConfigurat
+00011960: 696f 6e5d 282e 2e2f 6a6f 625f 636f 6e66  ion](../job_conf
+00011970: 6967 7572 6174 696f 6e29 0a20 2020 2020  iguration).     
+00011980: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
+00011990: 636f 6e66 6967 7572 6520 7468 6520 486f  configure the Ho
+000119a0: 7073 776f 726b 7320 4a6f 6220 7573 6564  psworks Job used
+000119b0: 2074 6f20 7772 6974 6520 6461 7461 2069   to write data i
+000119c0: 6e74 6f20 7468 650a 2020 2020 2020 2020  nto the.        
+000119d0: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+000119e0: 6520 6772 6f75 702e 0a20 2020 2020 2020  e group..       
+000119f0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
+00011a00: 7761 6974 5f66 6f72 5f6a 6f62 6020 616e  wait_for_job` an
+00011a10: 6420 7661 6c75 6520 6054 7275 6560 206f  d value `True` o
+00011a20: 7220 6046 616c 7365 6020 746f 2063 6f6e  r `False` to con
+00011a30: 6669 6775 7265 0a20 2020 2020 2020 2020  figure.         
+00011a40: 2020 2020 2020 2020 2077 6865 7468 6572           whether
+00011a50: 206f 7220 6e6f 7420 746f 2074 6865 2069   or not to the i
+00011a60: 6e73 6572 7420 6361 6c6c 2073 686f 756c  nsert call shoul
+00011a70: 6420 7265 7475 726e 206f 6e6c 790a 2020  d return only.  
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 6166 7465 7220 7468 6520 486f 7073 776f  after the Hopswo
+00011aa0: 726b 7320 4a6f 6220 6861 7320 6669 6e69  rks Job has fini
+00011ab0: 7368 6564 2e20 4279 2064 6566 6175 6c74  shed. By default
+00011ac0: 2069 7420 7761 6974 732e 0a20 2020 2020   it waits..     
+00011ad0: 2020 2020 2020 2020 2020 202a 206b 6579             * key
+00011ae0: 2060 7374 6172 745f 6f66 666c 696e 655f   `start_offline_
+00011af0: 6261 636b 6669 6c6c 6020 616e 6420 7661  backfill` and va
+00011b00: 6c75 6520 6054 7275 6560 206f 7220 6046  lue `True` or `F
+00011b10: 616c 7365 6020 746f 2063 6f6e 6669 6775  alse` to configu
+00011b20: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+00011b30: 2020 2020 2077 6865 7468 6572 206f 7220       whether or 
+00011b40: 6e6f 7420 746f 2073 7461 7274 2074 6865  not to start the
+00011b50: 2062 6163 6b66 696c 6c20 6a6f 6220 746f   backfill job to
+00011b60: 2077 7269 7465 2064 6174 6120 746f 2074   write data to t
+00011b70: 6865 206f 6666 6c69 6e65 0a20 2020 2020  he offline.     
+00011b80: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00011b90: 7261 6765 2e20 4279 2064 6566 6175 6c74  rage. By default
+00011ba0: 2074 6865 2062 6163 6b66 696c 6c20 6a6f   the backfill jo
+00011bb0: 6220 6765 7473 2073 7461 7274 6564 2069  b gets started i
+00011bc0: 6d6d 6564 6961 7465 6c79 2e0a 2020 2020  mmediately..    
+00011bd0: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
+00011be0: 7920 6069 6e74 6572 6e61 6c5f 6b61 666b  y `internal_kafk
+00011bf0: 6160 2061 6e64 2076 616c 7565 2060 5472  a` and value `Tr
+00011c00: 7565 6020 6f72 2060 4661 6c73 6560 2069  ue` or `False` i
+00011c10: 6e20 6361 7365 2079 6f75 2065 7374 6162  n case you estab
+00011c20: 6c69 7368 6564 0a20 2020 2020 2020 2020  lished.         
+00011c30: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+00011c40: 6976 6974 7920 6672 6f6d 2079 6f75 2050  ivity from you P
+00011c50: 7974 686f 6e20 656e 7669 726f 6e6d 656e  ython environmen
+00011c60: 7420 746f 2074 6865 2069 6e74 6572 6e61  t to the interna
+00011c70: 6c20 6164 7665 7274 6973 6564 0a20 2020  l advertised.   
+00011c80: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011c90: 6973 7465 6e65 7273 206f 6620 7468 6520  isteners of the 
+00011ca0: 486f 7073 776f 726b 7320 4b61 666b 6120  Hopsworks Kafka 
+00011cb0: 436c 7573 7465 722e 2044 6566 6175 6c74  Cluster. Default
+00011cc0: 7320 746f 2060 4661 6c73 6560 2061 6e64  s to `False` and
+00011cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ce0: 2020 2077 696c 6c20 7573 6520 6578 7465     will use exte
+00011cf0: 726e 616c 206c 6973 7465 6e65 7273 2077  rnal listeners w
+00011d00: 6865 6e20 636f 6e6e 6563 7469 6e67 2066  hen connecting f
+00011d10: 726f 6d20 6f75 7473 6964 6520 6f66 2048  rom outside of H
+00011d20: 6f70 7377 6f72 6b73 2e0a 2020 2020 2020  opsworks..      
+00011d30: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00011d40: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
+00011d50: 6f6e 616c 2076 616c 6964 6174 696f 6e20  onal validation 
+00011d60: 6f70 7469 6f6e 7320 6173 206b 6579 2d76  options as key-v
+00011d70: 616c 7565 2070 6169 7273 2c20 6465 6661  alue pairs, defa
+00011d80: 756c 7473 2074 6f20 607b 7d60 2e0a 2020  ults to `{}`..  
+00011d90: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00011da0: 6b65 7920 6072 756e 5f76 616c 6964 6174  key `run_validat
+00011db0: 696f 6e60 2062 6f6f 6c65 616e 2076 616c  ion` boolean val
+00011dc0: 7565 2c20 7365 7420 746f 2060 4661 6c73  ue, set to `Fals
+00011dd0: 6560 2074 6f20 736b 6970 2076 616c 6964  e` to skip valid
+00011de0: 6174 696f 6e20 7465 6d70 6f72 6172 696c  ation temporaril
+00011df0: 7920 6f6e 2069 6e67 6573 7469 6f6e 2e0a  y on ingestion..
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 2a20 6b65 7920 6073 6176 655f 7265 706f  * key `save_repo
+00011e20: 7274 6020 626f 6f6c 6561 6e20 7661 6c75  rt` boolean valu
+00011e30: 652c 2073 6574 2074 6f20 6046 616c 7365  e, set to `False
+00011e40: 6020 746f 2073 6b69 7020 7570 6c6f 6164  ` to skip upload
+00011e50: 206f 6620 7468 6520 7661 6c69 6461 7469   of the validati
+00011e60: 6f6e 2072 6570 6f72 7420 746f 2048 6f70  on report to Hop
+00011e70: 7377 6f72 6b73 2e0a 2020 2020 2020 2020  sworks..        
+00011e80: 2020 2020 2020 2020 2a20 6b65 7920 6067          * key `g
+00011e90: 655f 7661 6c69 6461 7465 5f6b 7761 7267  e_validate_kwarg
+00011ea0: 7360 2061 2064 6963 7469 6f6e 6172 7920  s` a dictionary 
+00011eb0: 636f 6e74 6169 6e69 6e67 206b 7761 7267  containing kwarg
+00011ec0: 7320 666f 7220 7468 6520 7661 6c69 6461  s for the valida
+00011ed0: 7465 206d 6574 686f 6420 6f66 2047 7265  te method of Gre
+00011ee0: 6174 2045 7870 6563 7461 7469 6f6e 732e  at Expectations.
+00011ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011f00: 202a 206b 6579 2060 6665 7463 685f 6578   * key `fetch_ex
+00011f10: 7065 6374 6174 696f 6e5f 7375 6974 6560  pectation_suite`
+00011f20: 2061 2062 6f6f 6c65 616e 2076 616c 7565   a boolean value
+00011f30: 2c20 6279 2064 6566 6175 6c74 2060 5472  , by default `Tr
+00011f40: 7565 602c 2074 6f20 636f 6e74 726f 6c20  ue`, to control 
+00011f50: 7768 6574 6865 7220 7468 6520 6578 7065  whether the expe
+00011f60: 6374 6174 696f 6e0a 2020 2020 2020 2020  ctation.        
+00011f70: 2020 2020 2020 2020 2020 2073 7569 7465             suite
+00011f80: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00011f90: 6772 6f75 7020 7368 6f75 6c64 2062 6520  group should be 
+00011fa0: 6665 7463 6865 6420 6265 666f 7265 2065  fetched before e
+00011fb0: 7665 7279 2069 6e73 6572 742e 0a20 2020  very insert..   
+00011fc0: 2020 2020 2020 2020 2073 6176 655f 636f           save_co
+00011fd0: 6465 3a20 5768 656e 2072 756e 6e69 6e67  de: When running
+00011fe0: 2048 5346 5320 6f6e 2048 6f70 7377 6f72   HSFS on Hopswor
+00011ff0: 6b73 206f 7220 4461 7461 6272 6963 6b73  ks or Databricks
+00012000: 2c20 4853 4653 2063 616e 2073 6176 6520  , HSFS can save 
+00012010: 7468 6520 636f 6465 2f6e 6f74 6562 6f6f  the code/noteboo
+00012020: 6b20 7573 6564 2074 6f20 6372 6561 7465  k used to create
+00012030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012040: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+00012050: 7570 206f 7220 7573 6564 2074 6f20 696e  up or used to in
+00012060: 7365 7274 2064 6174 6120 746f 2069 742e  sert data to it.
+00012070: 2057 6865 6e20 6361 6c6c 696e 6720 7468   When calling th
+00012080: 6520 6069 6e73 6572 7460 206d 6574 686f  e `insert` metho
+00012090: 6420 7265 7065 6174 6564 6c79 0a20 2020  d repeatedly.   
+000120a0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+000120b0: 6820 736d 616c 6c20 6261 7463 6865 7320  h small batches 
+000120c0: 6f66 2064 6174 612c 2074 6869 7320 6361  of data, this ca
+000120d0: 6e20 736c 6f77 2064 6f77 6e20 7468 6520  n slow down the 
+000120e0: 7772 6974 6573 2e20 5573 6520 7468 6973  writes. Use this
+000120f0: 206f 7074 696f 6e20 746f 2074 7572 6e20   option to turn 
+00012100: 6f66 6620 7361 7669 6e67 0a20 2020 2020  off saving.     
+00012110: 2020 2020 2020 2020 2020 2063 6f64 652e             code.
+00012120: 2044 6566 6175 6c74 7320 746f 2060 5472   Defaults to `Tr
+00012130: 7565 602e 0a20 2020 2020 2020 2020 2020  ue`..           
+00012140: 2077 6169 743a 2057 6169 7420 666f 7220   wait: Wait for 
+00012150: 6a6f 6220 746f 2066 696e 6973 6820 6265  job to finish be
+00012160: 666f 7265 2072 6574 7572 6e69 6e67 2c20  fore returning, 
+00012170: 6465 6661 756c 7473 2074 6f20 6046 616c  defaults to `Fal
+00012180: 7365 602e 0a20 2020 2020 2020 2020 2020  se`..           
+00012190: 2020 2020 2053 686f 7274 6375 7420 666f       Shortcut fo
+000121a0: 7220 7265 6164 5f6f 7074 696f 6e73 2060  r read_options `
+000121b0: 7b22 7761 6974 5f66 6f72 5f6a 6f62 223a  {"wait_for_job":
+000121c0: 2046 616c 7365 7d60 2e0a 0a20 2020 2020   False}`...     
+000121d0: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
+000121e0: 2020 2020 2020 2020 2028 604a 6f62 602c           (`Job`,
+000121f0: 2060 5661 6c69 6461 7469 6f6e 5265 706f   `ValidationRepo
+00012200: 7274 6029 2041 2074 7570 6c65 2077 6974  rt`) A tuple wit
+00012210: 6820 6a6f 6220 696e 666f 726d 6174 696f  h job informatio
+00012220: 6e20 6966 2070 7974 686f 6e20 656e 6769  n if python engi
+00012230: 6e65 2069 7320 7573 6564 2061 6e64 2074  ne is used and t
+00012240: 6865 2076 616c 6964 6174 696f 6e20 7265  he validation re
+00012250: 706f 7274 2069 6620 7661 6c69 6461 7469  port if validati
+00012260: 6f6e 2069 7320 656e 6162 6c65 642e 0a20  on is enabled.. 
+00012270: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012280: 2020 2066 6561 7475 7265 5f64 6174 6166     feature_dataf
+00012290: 7261 6d65 203d 2065 6e67 696e 652e 6765  rame = engine.ge
+000122a0: 745f 696e 7374 616e 6365 2829 2e63 6f6e  t_instance().con
+000122b0: 7665 7274 5f74 6f5f 6465 6661 756c 745f  vert_to_default_
+000122c0: 6461 7461 6672 616d 6528 6665 6174 7572  dataframe(featur
+000122d0: 6573 290a 0a20 2020 2020 2020 2069 6620  es)..        if 
+000122e0: 7772 6974 655f 6f70 7469 6f6e 7320 6973  write_options is
+000122f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012300: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
+00012310: 203d 207b 7d0a 2020 2020 2020 2020 6966   = {}.        if
+00012320: 2022 7761 6974 5f66 6f72 5f6a 6f62 2220   "wait_for_job" 
+00012330: 6e6f 7420 696e 2077 7269 7465 5f6f 7074  not in write_opt
+00012340: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00012350: 2020 7772 6974 655f 6f70 7469 6f6e 735b    write_options[
+00012360: 2277 6169 745f 666f 725f 6a6f 6222 5d20  "wait_for_job"] 
+00012370: 3d20 7761 6974 0a0a 2020 2020 2020 2020  = wait..        
+00012380: 6a6f 622c 2067 655f 7265 706f 7274 203d  job, ge_report =
+00012390: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
+000123a0: 726f 7570 5f65 6e67 696e 652e 696e 7365  roup_engine.inse
+000123b0: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+000123c0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+000123d0: 2020 6665 6174 7572 655f 6461 7461 6672    feature_datafr
+000123e0: 616d 653d 6665 6174 7572 655f 6461 7461  ame=feature_data
+000123f0: 6672 616d 652c 0a20 2020 2020 2020 2020  frame,.         
+00012400: 2020 206f 7665 7277 7269 7465 3d6f 7665     overwrite=ove
+00012410: 7277 7269 7465 2c0a 2020 2020 2020 2020  rwrite,.        
+00012420: 2020 2020 6f70 6572 6174 696f 6e3d 6f70      operation=op
+00012430: 6572 6174 696f 6e2c 0a20 2020 2020 2020  eration,.       
+00012440: 2020 2020 2073 746f 7261 6765 3d73 746f       storage=sto
+00012450: 7261 6765 2e6c 6f77 6572 2829 2069 6620  rage.lower() if 
+00012460: 7374 6f72 6167 6520 6973 206e 6f74 204e  storage is not N
+00012470: 6f6e 6520 656c 7365 204e 6f6e 652c 0a20  one else None,. 
+00012480: 2020 2020 2020 2020 2020 2077 7269 7465             write
+00012490: 5f6f 7074 696f 6e73 3d77 7269 7465 5f6f  _options=write_o
+000124a0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
+000124b0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
+000124c0: 7074 696f 6e73 3d7b 2273 6176 655f 7265  ptions={"save_re
+000124d0: 706f 7274 223a 2054 7275 652c 202a 2a76  port": True, **v
+000124e0: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
+000124f0: 737d 2c0a 2020 2020 2020 2020 290a 2020  s},.        ).  
+00012500: 2020 2020 2020 6966 2073 6176 655f 636f        if save_co
+00012510: 6465 2061 6e64 2028 0a20 2020 2020 2020  de and (.       
+00012520: 2020 2020 2067 655f 7265 706f 7274 2069       ge_report i
+00012530: 7320 4e6f 6e65 206f 7220 6765 5f72 6570  s None or ge_rep
+00012540: 6f72 742e 696e 6765 7374 696f 6e5f 7265  ort.ingestion_re
+00012550: 7375 6c74 203d 3d20 2249 4e47 4553 5445  sult == "INGESTE
+00012560: 4422 0a20 2020 2020 2020 2029 3a0a 2020  D".        ):.  
+00012570: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00012580: 636f 6465 5f65 6e67 696e 652e 7361 7665  code_engine.save
+00012590: 5f63 6f64 6528 7365 6c66 290a 0a20 2020  _code(self)..   
+000125a0: 2020 2020 2069 6620 656e 6769 6e65 2e67       if engine.g
+000125b0: 6574 5f74 7970 6528 2920 3d3d 2022 7370  et_type() == "sp
+000125c0: 6172 6b22 3a0a 2020 2020 2020 2020 2020  ark":.          
+000125d0: 2020 2320 4f6e 6c79 2063 6f6d 7075 7465    # Only compute
+000125e0: 2073 7461 7469 7374 6963 7320 6966 2074   statistics if t
+000125f0: 6865 2065 6e67 696e 6520 6973 2053 7061  he engine is Spa
+00012600: 726b 2c0a 2020 2020 2020 2020 2020 2020  rk,.            
+00012610: 2320 6966 2050 7974 686f 6e2c 2074 6865  # if Python, the
+00012620: 2073 7461 7469 7374 6963 7320 6172 6520   statistics are 
+00012630: 636f 6d70 7574 6564 2062 7920 7468 6520  computed by the 
+00012640: 6170 706c 6963 6174 696f 6e20 646f 696e  application doin
+00012650: 6720 7468 6520 696e 7365 7274 0a20 2020  g the insert.   
+00012660: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00012670: 6d70 7574 655f 7374 6174 6973 7469 6373  mpute_statistics
+00012680: 2829 0a0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00012690: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
+000126a0: 206a 6f62 2c0a 2020 2020 2020 2020 2020   job,.          
+000126b0: 2020 6765 5f72 6570 6f72 742e 746f 5f67    ge_report.to_g
+000126c0: 655f 7479 7065 2829 2069 6620 6765 5f72  e_type() if ge_r
+000126d0: 6570 6f72 7420 6973 206e 6f74 204e 6f6e  eport is not Non
+000126e0: 6520 656c 7365 204e 6f6e 652c 0a20 2020  e else None,.   
+000126f0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00012700: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
+00012710: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+00012720: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00012730: 733a 2055 6e69 6f6e 5b0a 2020 2020 2020  s: Union[.      
+00012740: 2020 2020 2020 7064 2e44 6174 6146 7261        pd.DataFra
+00012750: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00012760: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
+00012770: 2e73 716c 2e44 6174 6146 7261 6d65 2229  .sql.DataFrame")
+00012780: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+00012790: 2020 2020 2020 2020 2020 2020 5479 7065              Type
+000127a0: 5661 7228 2270 7973 7061 726b 2e52 4444  Var("pyspark.RDD
+000127b0: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
+000127c0: 310a 2020 2020 2020 2020 2020 2020 6e70  1.            np
+000127d0: 2e6e 6461 7272 6179 2c0a 2020 2020 2020  .ndarray,.      
+000127e0: 2020 2020 2020 4c69 7374 5b6c 6973 745d        List[list]
+000127f0: 2c0a 2020 2020 2020 2020 5d20 3d20 4e6f  ,.        ] = No
+00012800: 6e65 2c0a 2020 2020 2020 2020 6f76 6572  ne,.        over
+00012810: 7772 6974 653a 204f 7074 696f 6e61 6c5b  write: Optional[
+00012820: 626f 6f6c 5d20 3d20 4661 6c73 652c 0a20  bool] = False,. 
+00012830: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00012840: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00012850: 3d20 2275 7073 6572 7422 2c0a 2020 2020  = "upsert",.    
+00012860: 2020 2020 7374 6f72 6167 653a 204f 7074      storage: Opt
+00012870: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00012880: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+00012890: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
+000128a0: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
+000128b0: 5d5d 203d 207b 7d2c 0a20 2020 2020 2020  ]] = {},.       
+000128c0: 2076 616c 6964 6174 696f 6e5f 6f70 7469   validation_opti
+000128d0: 6f6e 733a 204f 7074 696f 6e61 6c5b 4469  ons: Optional[Di
+000128e0: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
+000128f0: 7b7d 2c0a 2020 2020 2920 2d3e 2055 6e69  {},.    ) -> Uni
+00012900: 6f6e 5b0a 2020 2020 2020 2020 5475 706c  on[.        Tupl
+00012910: 655b 4f70 7469 6f6e 616c 5b4a 6f62 5d2c  e[Optional[Job],
+00012920: 204f 7074 696f 6e61 6c5b 5661 6c69 6461   Optional[Valida
+00012930: 7469 6f6e 5265 706f 7274 5d5d 2c0a 2020  tionReport]],.  
+00012940: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
+00012950: 6f75 705f 7772 6974 6572 2e46 6561 7475  oup_writer.Featu
+00012960: 7265 4772 6f75 7057 7269 7465 722c 0a20  reGroupWriter,. 
+00012970: 2020 205d 3a0a 2020 2020 2020 2020 2222     ]:.        ""
+00012980: 2247 6574 2046 6561 7475 7265 4772 6f75  "Get FeatureGrou
+00012990: 7057 7269 7465 7220 666f 7220 6f70 7469  pWriter for opti
+000129a0: 6d69 7a65 6420 6d75 6c74 6920 7061 7274  mized multi part
+000129b0: 2069 6e73 6572 7473 206f 7220 6361 6c6c   inserts or call
+000129c0: 2074 6869 7320 6d65 7468 6f64 0a20 2020   this method.   
+000129d0: 2020 2020 2074 6f20 7374 6172 7420 6d61       to start ma
+000129e0: 6e75 616c 206d 756c 7469 2070 6172 7420  nual multi part 
+000129f0: 6f70 7469 6d69 7a65 6420 696e 7365 7274  optimized insert
+00012a00: 732e 0a0a 2020 2020 2020 2020 496e 2075  s...        In u
+00012a10: 7365 2063 6173 6573 2077 6865 7265 2076  se cases where v
+00012a20: 6572 7920 736d 616c 6c20 6261 7463 6865  ery small batche
+00012a30: 7320 2831 2074 6f20 3130 3030 2920 726f  s (1 to 1000) ro
+00012a40: 7773 2070 6572 2044 6174 6166 7261 6d65  ws per Dataframe
+00012a50: 206e 6565 640a 2020 2020 2020 2020 746f   need.        to
+00012a60: 2062 6520 7772 6974 7465 6e20 746f 2074   be written to t
+00012a70: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
+00012a80: 2072 6570 6561 7465 646c 792c 2069 7420   repeatedly, it 
+00012a90: 6d69 6768 7420 6265 2069 6e65 6666 6963  might be ineffic
+00012aa0: 6965 6e74 2074 6f20 7573 650a 2020 2020  ient to use.    
+00012ab0: 2020 2020 7468 6520 7374 616e 6461 7264      the standard
+00012ac0: 2060 6665 6174 7572 655f 6772 6f75 702e   `feature_group.
+00012ad0: 696e 7365 7274 2829 6020 6d65 7468 6f64  insert()` method
+00012ae0: 2061 7320 6974 2070 6572 666f 726d 7320   as it performs 
+00012af0: 736f 6d65 2062 6163 6b67 726f 756e 640a  some background.
+00012b00: 2020 2020 2020 2020 6163 7469 6f6e 7320          actions 
+00012b10: 746f 2075 7064 6174 6520 7468 6520 6d65  to update the me
+00012b20: 7461 6461 7461 206f 6620 7468 6520 6665  tadata of the fe
+00012b30: 6174 7572 6520 6772 6f75 7020 6f62 6a65  ature group obje
+00012b40: 6374 2066 6972 7374 2e0a 0a20 2020 2020  ct first...     
+00012b50: 2020 2046 6f72 2074 6865 7365 2063 6173     For these cas
+00012b60: 6573 2c20 7468 6520 6665 6174 7572 6520  es, the feature 
+00012b70: 6772 6f75 7020 7072 6f76 6964 6573 2074  group provides t
+00012b80: 6865 2060 6d75 6c74 695f 7061 7274 5f69  he `multi_part_i
+00012b90: 6e73 6572 7460 2041 5049 2c0a 2020 2020  nsert` API,.    
+00012ba0: 2020 2020 7768 6963 6820 6973 206f 7074      which is opt
+00012bb0: 696d 697a 6564 2066 6f72 2077 7269 7469  imized for writi
+00012bc0: 6e67 206d 616e 7920 736d 616c 6c20 4461  ng many small Da
+00012bd0: 7461 6672 616d 6573 2061 6674 6572 2061  taframes after a
+00012be0: 6e6f 7468 6572 2e0a 0a20 2020 2020 2020  nother...       
+00012bf0: 2054 6865 7265 2061 7265 2074 776f 2077   There are two w
+00012c00: 6179 7320 746f 2075 7365 2074 6869 7320  ays to use this 
+00012c10: 4150 493a 0a20 2020 2020 2020 2021 2121  API:.        !!!
+00012c20: 2065 7861 6d70 6c65 2022 5079 7468 6f6e   example "Python
+00012c30: 2043 6f6e 7465 7874 204d 616e 6167 6572   Context Manager
+00012c40: 220a 2020 2020 2020 2020 2020 2020 5573  ".            Us
+00012c50: 696e 6720 7468 6520 5079 7468 6f6e 2060  ing the Python `
+00012c60: 7769 7468 6020 7379 6e74 6178 2079 6f75  with` syntax you
+00012c70: 2063 616e 2061 6371 7569 7265 2061 2046   can acquire a F
+00012c80: 6561 7475 7265 4772 6f75 7057 7269 7465  eatureGroupWrite
+00012c90: 720a 2020 2020 2020 2020 2020 2020 6f62  r.            ob
+00012ca0: 6a65 6374 2074 6861 7420 696d 706c 656d  ject that implem
+00012cb0: 656e 7473 2074 6865 2073 616d 6520 606d  ents the same `m
+00012cc0: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+00012cd0: 6020 4150 492e 0a20 2020 2020 2020 2020  ` API..         
+00012ce0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00012cf0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00012d00: 5f67 726f 7570 203d 2066 732e 6765 745f  _group = fs.get_
+00012d10: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00012d20: 655f 6772 6f75 7028 2266 675f 6e61 6d65  e_group("fg_name
+00012d30: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
+00012d40: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00012d50: 6665 6174 7572 655f 6772 6f75 702e 6d75  feature_group.mu
+00012d60: 6c74 695f 7061 7274 5f69 6e73 6572 7428  lti_part_insert(
+00012d70: 2920 6173 2077 7269 7465 723a 0a20 2020  ) as writer:.   
+00012d80: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00012d90: 756e 2069 6e73 6572 7473 2069 6e20 6120  un inserts in a 
+00012da0: 6c6f 6f70 3a0a 2020 2020 2020 2020 2020  loop:.          
+00012db0: 2020 2020 2020 7768 696c 6520 6c6f 6f70        while loop
+00012dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012dd0: 2020 2020 2020 736d 616c 6c5f 6261 7463        small_batc
+00012de0: 685f 6466 203d 202e 2e2e 0a20 2020 2020  h_df = ....     
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00012e00: 7269 7465 722e 696e 7365 7274 2873 6d61  riter.insert(sma
+00012e10: 6c6c 5f62 6174 6368 5f64 6629 0a20 2020  ll_batch_df).   
+00012e20: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00012e30: 2020 2020 2020 2020 2054 6865 2077 7269           The wri
+00012e40: 7465 7220 6261 7463 6865 7320 7468 6520  ter batches the 
+00012e50: 736d 616c 6c20 4461 7461 6672 616d 6573  small Dataframes
+00012e60: 2061 6e64 2074 7261 6e73 6d69 7473 2074   and transmits t
+00012e70: 6865 6d20 746f 2048 6f70 7377 6f72 6b73  hem to Hopsworks
+00012e80: 0a20 2020 2020 2020 2020 2020 2065 6666  .            eff
+00012e90: 6963 6965 6e74 6c79 2e0a 2020 2020 2020  iciently..      
+00012ea0: 2020 2020 2020 5768 656e 2065 7869 7469        When exiti
+00012eb0: 6e67 2074 6865 2063 6f6e 7465 7874 2c20  ng the context, 
+00012ec0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+00012ed0: 7020 7772 6974 6572 2069 7320 7375 7265  p writer is sure
+00012ee0: 2074 6f20 6578 6974 0a20 2020 2020 2020   to exit.       
+00012ef0: 2020 2020 206f 6e6c 7920 6f6e 6365 2061       only once a
+00012f00: 6c6c 2074 6865 2072 6f77 7320 6861 7665  ll the rows have
+00012f10: 2062 6565 6e20 7472 616e 736d 6974 7465   been transmitte
+00012f20: 642e 0a0a 2020 2020 2020 2020 2121 2120  d...        !!! 
+00012f30: 6578 616d 706c 6520 224d 756c 7469 2070  example "Multi p
+00012f40: 6172 7420 696e 7365 7274 2077 6974 6820  art insert with 
+00012f50: 6d61 6e75 616c 2063 6f6e 7465 7874 206d  manual context m
+00012f60: 616e 6167 656d 656e 7422 0a20 2020 2020  anagement".     
+00012f70: 2020 2020 2020 2049 6e73 7465 6164 206f         Instead o
+00012f80: 6620 6c65 7474 696e 6720 5079 7468 6f6e  f letting Python
+00012f90: 2068 616e 646c 6520 7468 6520 656e 7465   handle the ente
+00012fa0: 7269 6e67 2061 6e64 2065 7869 7469 6e67  ring and exiting
+00012fb0: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00012fc0: 2020 2020 6d75 6c74 6920 7061 7274 2069      multi part i
+00012fd0: 6e73 6572 7420 636f 6e74 6578 742c 2079  nsert context, y
+00012fe0: 6f75 2063 616e 2073 7461 7274 2061 6e64  ou can start and
+00012ff0: 2066 696e 616c 697a 6520 7468 6520 636f   finalize the co
+00013000: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
+00013010: 2020 6d61 6e75 616c 6c79 2e0a 2020 2020    manually..    
+00013020: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00013030: 6e0a 2020 2020 2020 2020 2020 2020 6665  n.            fe
+00013040: 6174 7572 655f 6772 6f75 7020 3d20 6673  ature_group = fs
+00013050: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00013060: 6561 7475 7265 5f67 726f 7570 2822 6667  eature_group("fg
+00013070: 5f6e 616d 6522 2c20 7665 7273 696f 6e3d  _name", version=
+00013080: 3129 0a0a 2020 2020 2020 2020 2020 2020  1)..            
+00013090: 7768 696c 6520 6c6f 6f70 3a0a 2020 2020  while loop:.    
+000130a0: 2020 2020 2020 2020 2020 2020 736d 616c              smal
+000130b0: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
+000130c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000130d0: 2066 6561 7475 7265 5f67 726f 7570 2e6d   feature_group.m
+000130e0: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+000130f0: 2873 6d61 6c6c 5f62 6174 6368 5f64 6629  (small_batch_df)
+00013100: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00013110: 494d 504f 5254 414e 543a 2066 696e 616c  IMPORTANT: final
+00013120: 697a 6520 7468 6520 6d75 6c74 6920 7061  ize the multi pa
+00013130: 7274 2069 6e73 6572 7420 746f 206d 616b  rt insert to mak
+00013140: 6520 7375 7265 2061 6c6c 2072 6f77 730a  e sure all rows.
+00013150: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
+00013160: 7665 2062 6565 6e20 7472 616e 736d 6974  ve been transmit
+00013170: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00013180: 6665 6174 7572 655f 6772 6f75 702e 6669  feature_group.fi
+00013190: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
+000131a0: 745f 696e 7365 7274 2829 0a20 2020 2020  t_insert().     
+000131b0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000131c0: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+000131d0: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
+000131e0: 746f 2060 6d75 6c74 695f 7061 7274 5f69  to `multi_part_i
+000131f0: 6e73 6572 7460 2069 6e69 7469 6174 6573  nsert` initiates
+00013200: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
+00013210: 2020 2020 2020 2020 2061 6e64 2062 6520           and be 
+00013220: 7375 7265 2074 6f20 6669 6e61 6c69 7a65  sure to finalize
+00013230: 2069 742e 2054 6865 2060 6669 6e61 6c69   it. The `finali
+00013240: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
+00013250: 7365 7274 6020 6973 2061 0a20 2020 2020  sert` is a.     
+00013260: 2020 2020 2020 2062 6c6f 636b 696e 6720         blocking 
+00013270: 6361 6c6c 2074 6861 7420 7265 7475 726e  call that return
+00013280: 7320 6f6e 6365 2061 6c6c 2072 6f77 7320  s once all rows 
+00013290: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
+000132a0: 6974 7465 642e 0a0a 2020 2020 2020 2020  itted...        
+000132b0: 2020 2020 4f6e 6365 2079 6f75 2061 7265      Once you are
+000132c0: 2064 6f6e 6520 7769 7468 2074 6865 206d   done with the m
+000132d0: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
+000132e0: 2c20 6974 2069 7320 676f 6f64 2070 7261  , it is good pra
+000132f0: 6374 6963 6520 746f 0a20 2020 2020 2020  ctice to.       
+00013300: 2020 2020 2073 7461 7274 2074 6865 2062       start the b
+00013310: 6163 6b66 696c 6c20 6a6f 6220 696e 206f  ackfill job in o
+00013320: 7264 6572 2074 6f20 7772 6974 6520 7468  rder to write th
+00013330: 6520 6461 7461 2074 6f20 7468 6520 6f66  e data to the of
+00013340: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
+00013350: 2020 7374 6f72 6167 653a 0a20 2020 2020    storage:.     
+00013360: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00013370: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+00013380: 7475 7265 5f67 726f 7570 2e62 6163 6b66  ture_group.backf
+00013390: 696c 6c5f 6a6f 622e 7275 6e28 6177 6169  ill_job.run(awai
+000133a0: 745f 7465 726d 696e 6174 696f 6e3d 5472  t_termination=Tr
+000133b0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+000133c0: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
+000133d0: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+000133e0: 2020 2020 2066 6561 7475 7265 733a 2044       features: D
+000133f0: 6174 6146 7261 6d65 2c20 5244 442c 204e  ataFrame, RDD, N
+00013400: 6461 7272 6179 2c20 6c69 7374 2e20 4665  darray, list. Fe
+00013410: 6174 7572 6573 2074 6f20 6265 2073 6176  atures to be sav
+00013420: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00013430: 6f76 6572 7772 6974 653a 2044 726f 7020  overwrite: Drop 
+00013440: 616c 6c20 6461 7461 2069 6e20 7468 6520  all data in the 
+00013450: 6665 6174 7572 6520 6772 6f75 7020 6265  feature group be
+00013460: 666f 7265 0a20 2020 2020 2020 2020 2020  fore.           
+00013470: 2020 2020 2069 6e73 6572 7469 6e67 206e       inserting n
+00013480: 6577 2064 6174 612e 2054 6869 7320 646f  ew data. This do
+00013490: 6573 206e 6f74 2061 6666 6563 7420 6d65  es not affect me
+000134a0: 7461 6461 7461 2c20 6465 6661 756c 7473  tadata, defaults
+000134b0: 2074 6f20 4661 6c73 652e 0a20 2020 2020   to False..     
+000134c0: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+000134d0: 3a20 4170 6163 6865 2048 7564 6920 6f70  : Apache Hudi op
+000134e0: 6572 6174 696f 6e20 7479 7065 2060 2269  eration type `"i
+000134f0: 6e73 6572 7422 6020 6f72 2060 2275 7073  nsert"` or `"ups
+00013500: 6572 7422 602e 0a20 2020 2020 2020 2020  ert"`..         
+00013510: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00013520: 746f 2060 2275 7073 6572 7422 602e 0a20  to `"upsert"`.. 
+00013530: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+00013540: 6765 3a20 4f76 6572 7772 6974 6520 6465  ge: Overwrite de
+00013550: 6661 756c 7420 6265 6861 7669 6f75 722c  fault behaviour,
+00013560: 2077 7269 7465 2074 6f20 6f66 666c 696e   write to offlin
+00013570: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00013580: 2020 7374 6f72 6167 6520 6f6e 6c79 2077    storage only w
+00013590: 6974 6820 6022 6f66 666c 696e 6522 6020  ith `"offline"` 
+000135a0: 6f72 206f 6e6c 696e 6520 6f6e 6c79 2077  or online only w
+000135b0: 6974 6820 6022 6f6e 6c69 6e65 2260 2c20  ith `"online"`, 
+000135c0: 6465 6661 756c 7473 0a20 2020 2020 2020  defaults.       
+000135d0: 2020 2020 2020 2020 2074 6f20 604e 6f6e           to `Non
+000135e0: 6560 2e0a 2020 2020 2020 2020 2020 2020  e`..            
+000135f0: 7772 6974 655f 6f70 7469 6f6e 733a 2041  write_options: A
+00013600: 6464 6974 696f 6e61 6c20 7772 6974 6520  dditional write 
+00013610: 6f70 7469 6f6e 7320 6173 206b 6579 2d76  options as key-v
+00013620: 616c 7565 2070 6169 7273 2c20 6465 6661  alue pairs, defa
+00013630: 756c 7473 2074 6f20 607b 7d60 2e0a 2020  ults to `{}`..  
+00013640: 2020 2020 2020 2020 2020 2020 2020 5768                Wh
+00013650: 656e 2075 7369 6e67 2074 6865 2060 7079  en using the `py
+00013660: 7468 6f6e 6020 656e 6769 6e65 2c20 7772  thon` engine, wr
+00013670: 6974 655f 6f70 7469 6f6e 7320 6361 6e20  ite_options can 
+00013680: 636f 6e74 6169 6e20 7468 650a 2020 2020  contain the.    
+00013690: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
+000136a0: 6f77 696e 6720 656e 7472 6965 733a 0a20  owing entries:. 
+000136b0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+000136c0: 206b 6579 2060 7370 6172 6b60 2061 6e64   key `spark` and
+000136d0: 2076 616c 7565 2061 6e20 6f62 6a65 6374   value an object
+000136e0: 206f 6620 7479 7065 0a20 2020 2020 2020   of type.       
+000136f0: 2020 2020 2020 2020 205b 6873 6673 2e63           [hsfs.c
+00013700: 6f72 652e 6a6f 625f 636f 6e66 6967 7572  ore.job_configur
+00013710: 6174 696f 6e2e 4a6f 6243 6f6e 6669 6775  ation.JobConfigu
+00013720: 7261 7469 6f6e 5d28 2e2e 2f6a 6f62 5f63  ration](../job_c
+00013730: 6f6e 6669 6775 7261 7469 6f6e 290a 2020  onfiguration).  
+00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013750: 746f 2063 6f6e 6669 6775 7265 2074 6865  to configure the
+00013760: 2048 6f70 7377 6f72 6b73 204a 6f62 2075   Hopsworks Job u
+00013770: 7365 6420 746f 2077 7269 7465 2064 6174  sed to write dat
+00013780: 6120 696e 746f 2074 6865 0a20 2020 2020  a into the.     
+00013790: 2020 2020 2020 2020 2020 2020 2066 6561               fea
+000137a0: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+000137b0: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
+000137c0: 7920 6077 6169 745f 666f 725f 6a6f 6260  y `wait_for_job`
+000137d0: 2061 6e64 2076 616c 7565 2060 5472 7565   and value `True
+000137e0: 6020 6f72 2060 4661 6c73 6560 2074 6f20  ` or `False` to 
+000137f0: 636f 6e66 6967 7572 650a 2020 2020 2020  configure.      
+00013800: 2020 2020 2020 2020 2020 2020 7768 6574              whet
+00013810: 6865 7220 6f72 206e 6f74 2074 6f20 7468  her or not to th
+00013820: 6520 696e 7365 7274 2063 616c 6c20 7368  e insert call sh
+00013830: 6f75 6c64 2072 6574 7572 6e20 6f6e 6c79  ould return only
+00013840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013850: 2020 2061 6674 6572 2074 6865 2048 6f70     after the Hop
+00013860: 7377 6f72 6b73 204a 6f62 2068 6173 2066  sworks Job has f
+00013870: 696e 6973 6865 642e 2042 7920 6465 6661  inished. By defa
+00013880: 756c 7420 6974 2077 6169 7473 2e0a 2020  ult it waits..  
+00013890: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+000138a0: 6b65 7920 6073 7461 7274 5f6f 6666 6c69  key `start_offli
+000138b0: 6e65 5f62 6163 6b66 696c 6c60 2061 6e64  ne_backfill` and
+000138c0: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
+000138d0: 2060 4661 6c73 6560 2074 6f20 636f 6e66   `False` to conf
+000138e0: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
+000138f0: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
+00013900: 6f72 206e 6f74 2074 6f20 7374 6172 7420  or not to start 
+00013910: 7468 6520 6261 636b 6669 6c6c 206a 6f62  the backfill job
+00013920: 2074 6f20 7772 6974 6520 6461 7461 2074   to write data t
+00013930: 6f20 7468 6520 6f66 666c 696e 650a 2020  o the offline.  
+00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013950: 7374 6f72 6167 652e 2042 7920 6465 6661  storage. By defa
+00013960: 756c 7420 7468 6520 6261 636b 6669 6c6c  ult the backfill
+00013970: 206a 6f62 2064 6f65 7320 6e6f 7420 6765   job does not ge
+00013980: 7420 7374 6172 7465 6420 6175 746f 6d61  t started automa
+00013990: 7469 6361 6c6c 790a 2020 2020 2020 2020  tically.        
+000139a0: 2020 2020 2020 2020 2020 666f 7220 6d75            for mu
+000139b0: 6c74 6920 7061 7274 2069 6e73 6572 7473  lti part inserts
+000139c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000139d0: 2020 2a20 6b65 7920 6069 6e74 6572 6e61    * key `interna
+000139e0: 6c5f 6b61 666b 6160 2061 6e64 2076 616c  l_kafka` and val
+000139f0: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
+00013a00: 6c73 6560 2069 6e20 6361 7365 2079 6f75  lse` in case you
+00013a10: 2065 7374 6162 6c69 7368 6564 0a20 2020   established.   
+00013a20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013a30: 6f6e 6e65 6374 6976 6974 7920 6672 6f6d  onnectivity from
+00013a40: 2079 6f75 2050 7974 686f 6e20 656e 7669   you Python envi
+00013a50: 726f 6e6d 656e 7420 746f 2074 6865 2069  ronment to the i
+00013a60: 6e74 6572 6e61 6c20 6164 7665 7274 6973  nternal advertis
+00013a70: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00013a80: 2020 2020 206c 6973 7465 6e65 7273 206f       listeners o
+00013a90: 6620 7468 6520 486f 7073 776f 726b 7320  f the Hopsworks 
+00013aa0: 4b61 666b 6120 436c 7573 7465 722e 2044  Kafka Cluster. D
+00013ab0: 6566 6175 6c74 7320 746f 2060 4661 6c73  efaults to `Fals
+00013ac0: 6560 2061 6e64 0a20 2020 2020 2020 2020  e` and.         
+00013ad0: 2020 2020 2020 2020 2077 696c 6c20 7573           will us
+00013ae0: 6520 6578 7465 726e 616c 206c 6973 7465  e external liste
+00013af0: 6e65 7273 2077 6865 6e20 636f 6e6e 6563  ners when connec
+00013b00: 7469 6e67 2066 726f 6d20 6f75 7473 6964  ting from outsid
+00013b10: 6520 6f66 2048 6f70 7377 6f72 6b73 2e0a  e of Hopsworks..
+00013b20: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00013b30: 6461 7469 6f6e 5f6f 7074 696f 6e73 3a20  dation_options: 
+00013b40: 4164 6469 7469 6f6e 616c 2076 616c 6964  Additional valid
+00013b50: 6174 696f 6e20 6f70 7469 6f6e 7320 6173  ation options as
+00013b60: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
+00013b70: 2c20 6465 6661 756c 7473 2074 6f20 607b  , defaults to `{
+00013b80: 7d60 2e0a 2020 2020 2020 2020 2020 2020  }`..            
+00013b90: 2020 2020 2a20 6b65 7920 6072 756e 5f76      * key `run_v
+00013ba0: 616c 6964 6174 696f 6e60 2062 6f6f 6c65  alidation` boole
+00013bb0: 616e 2076 616c 7565 2c20 7365 7420 746f  an value, set to
+00013bc0: 2060 4661 6c73 6560 2074 6f20 736b 6970   `False` to skip
+00013bd0: 2076 616c 6964 6174 696f 6e20 7465 6d70   validation temp
+00013be0: 6f72 6172 696c 7920 6f6e 2069 6e67 6573  orarily on inges
+00013bf0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00013c00: 2020 2020 2020 2a20 6b65 7920 6073 6176        * key `sav
+00013c10: 655f 7265 706f 7274 6020 626f 6f6c 6561  e_report` boolea
+00013c20: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
+00013c30: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
+00013c40: 7570 6c6f 6164 206f 6620 7468 6520 7661  upload of the va
+00013c50: 6c69 6461 7469 6f6e 2072 6570 6f72 7420  lidation report 
+00013c60: 746f 2048 6f70 7377 6f72 6b73 2e0a 2020  to Hopsworks..  
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00013c80: 6b65 7920 6067 655f 7661 6c69 6461 7465  key `ge_validate
+00013c90: 5f6b 7761 7267 7360 2061 2064 6963 7469  _kwargs` a dicti
+00013ca0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00013cb0: 206b 7761 7267 7320 666f 7220 7468 6520   kwargs for the 
+00013cc0: 7661 6c69 6461 7465 206d 6574 686f 6420  validate method 
+00013cd0: 6f66 2047 7265 6174 2045 7870 6563 7461  of Great Expecta
+00013ce0: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+00013cf0: 2020 2020 2020 202a 206b 6579 2060 6665         * key `fe
+00013d00: 7463 685f 6578 7065 6374 6174 696f 6e5f  tch_expectation_
+00013d10: 7375 6974 6560 2061 2062 6f6f 6c65 616e  suite` a boolean
+00013d20: 2076 616c 7565 2c20 6279 2064 6566 6175   value, by defau
+00013d30: 6c74 2060 4661 6c73 6560 2066 6f72 206d  lt `False` for m
+00013d40: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
+00013d50: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00013d60: 2020 2020 2020 746f 2063 6f6e 7472 6f6c        to control
+00013d70: 2077 6865 7468 6572 2074 6865 2065 7870   whether the exp
+00013d80: 6563 7461 7469 6f6e 2073 7569 7465 206f  ectation suite o
+00013d90: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+00013da0: 6f75 7020 7368 6f75 6c64 2062 6520 6665  oup should be fe
+00013db0: 7463 6865 6420 6265 666f 7265 2065 7665  tched before eve
+00013dc0: 7279 2069 6e73 6572 742e 0a0a 2020 2020  ry insert...    
+00013dd0: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00013de0: 2020 2020 2020 2020 2020 2860 4a6f 6260            (`Job`
+00013df0: 2c20 6056 616c 6964 6174 696f 6e52 6570  , `ValidationRep
+00013e00: 6f72 7460 2920 4120 7475 706c 6520 7769  ort`) A tuple wi
+00013e10: 7468 206a 6f62 2069 6e66 6f72 6d61 7469  th job informati
+00013e20: 6f6e 2069 6620 7079 7468 6f6e 2065 6e67  on if python eng
+00013e30: 696e 6520 6973 2075 7365 6420 616e 6420  ine is used and 
+00013e40: 7468 6520 7661 6c69 6461 7469 6f6e 2072  the validation r
+00013e50: 6570 6f72 7420 6966 2076 616c 6964 6174  eport if validat
+00013e60: 696f 6e20 6973 2065 6e61 626c 6564 2e0a  ion is enabled..
+00013e70: 2020 2020 2020 2020 2020 2020 6046 6561              `Fea
+00013e80: 7475 7265 4772 6f75 7057 7269 7465 7260  tureGroupWriter`
+00013e90: 2057 6865 6e20 7573 6564 2061 7320 6120   When used as a 
+00013ea0: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
+00013eb0: 7769 7468 2050 7974 686f 6e20 6077 6974  with Python `wit
+00013ec0: 6860 2073 7461 7465 6d65 6e74 2e0a 2020  h` statement..  
+00013ed0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ee0: 2020 7365 6c66 2e5f 6d75 6c74 695f 7061    self._multi_pa
+00013ef0: 7274 5f69 6e73 6572 7420 3d20 5472 7565  rt_insert = True
+00013f00: 0a20 2020 2020 2020 206d 756c 7469 5f70  .        multi_p
+00013f10: 6172 745f 7772 6974 6572 203d 2066 6561  art_writer = fea
+00013f20: 7475 7265 5f67 726f 7570 5f77 7269 7465  ture_group_write
+00013f30: 722e 4665 6174 7572 6547 726f 7570 5772  r.FeatureGroupWr
+00013f40: 6974 6572 2873 656c 6629 0a20 2020 2020  iter(self).     
+00013f50: 2020 2069 6620 6665 6174 7572 6573 2069     if features i
+00013f60: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013f70: 2020 2020 7265 7475 726e 206d 756c 7469      return multi
+00013f80: 5f70 6172 745f 7772 6974 6572 0a20 2020  _part_writer.   
+00013f90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00013fa0: 2020 2020 2020 2023 2067 6f20 7468 726f         # go thro
+00013fb0: 7567 6820 7772 6974 6572 2074 6f20 6176  ugh writer to av
+00013fc0: 6f69 6420 7365 7474 696e 6720 6d75 6c74  oid setting mult
+00013fd0: 6920 696e 7365 7274 2064 6566 6175 6c74  i insert default
+00013fe0: 7320 6167 6169 6e0a 2020 2020 2020 2020  s again.        
+00013ff0: 2020 2020 7265 7475 726e 206d 756c 7469      return multi
+00014000: 5f70 6172 745f 7772 6974 6572 2e69 6e73  _part_writer.ins
+00014010: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00014020: 2020 2020 2066 6561 7475 7265 732c 0a20       features,. 
+00014030: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00014040: 7665 7277 7269 7465 2c0a 2020 2020 2020  verwrite,.      
+00014050: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
+00014060: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00014070: 2020 2020 2073 746f 7261 6765 2c0a 2020       storage,.  
+00014080: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+00014090: 6974 655f 6f70 7469 6f6e 732c 0a20 2020  ite_options,.   
+000140a0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+000140b0: 6964 6174 696f 6e5f 6f70 7469 6f6e 732c  idation_options,
+000140c0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+000140d0: 2020 2020 6465 6620 6669 6e61 6c69 7a65      def finalize
+000140e0: 5f6d 756c 7469 5f70 6172 745f 696e 7365  _multi_part_inse
+000140f0: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+00014100: 2020 2222 2246 696e 616c 697a 6573 2061    """Finalizes a
+00014110: 6e64 2065 7869 7473 2074 6865 206d 756c  nd exits the mul
+00014120: 7469 2070 6172 7420 696e 7365 7274 2063  ti part insert c
+00014130: 6f6e 7465 7874 206f 7065 6e65 6420 6279  ontext opened by
+00014140: 2060 6d75 6c74 695f 7061 7274 5f69 6e73   `multi_part_ins
+00014150: 6572 7460 0a20 2020 2020 2020 2069 6e20  ert`.        in 
+00014160: 6120 626c 6f63 6b69 6e67 2066 6173 6869  a blocking fashi
+00014170: 6f6e 206f 6e63 6520 616c 6c20 726f 7773  on once all rows
+00014180: 2068 6176 6520 6265 656e 2074 7261 6e73   have been trans
+00014190: 6d69 7474 6564 2e0a 0a20 2020 2020 2020  mitted...       
+000141a0: 2021 2121 2065 7861 6d70 6c65 2022 4d75   !!! example "Mu
+000141b0: 6c74 6920 7061 7274 2069 6e73 6572 7420  lti part insert 
+000141c0: 7769 7468 206d 616e 7561 6c20 636f 6e74  with manual cont
+000141d0: 6578 7420 6d61 6e61 6765 6d65 6e74 220a  ext management".
+000141e0: 2020 2020 2020 2020 2020 2020 496e 7374              Inst
+000141f0: 6561 6420 6f66 206c 6574 7469 6e67 2050  ead of letting P
+00014200: 7974 686f 6e20 6861 6e64 6c65 2074 6865  ython handle the
+00014210: 2065 6e74 6572 696e 6720 616e 6420 6578   entering and ex
+00014220: 6974 696e 6720 6f66 2074 6865 0a20 2020  iting of the.   
+00014230: 2020 2020 2020 2020 206d 756c 7469 2070           multi p
+00014240: 6172 7420 696e 7365 7274 2063 6f6e 7465  art insert conte
+00014250: 7874 2c20 796f 7520 6361 6e20 7374 6172  xt, you can star
+00014260: 7420 616e 6420 6669 6e61 6c69 7a65 2074  t and finalize t
+00014270: 6865 2063 6f6e 7465 7874 0a20 2020 2020  he context.     
+00014280: 2020 2020 2020 206d 616e 7561 6c6c 792e         manually.
+00014290: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+000142a0: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
+000142b0: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+000142c0: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+000142d0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+000142e0: 7028 2266 675f 6e61 6d65 222c 2076 6572  p("fg_name", ver
+000142f0: 7369 6f6e 3d31 290a 0a20 2020 2020 2020  sion=1)..       
+00014300: 2020 2020 2077 6869 6c65 206c 6f6f 703a       while loop:
+00014310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014320: 2073 6d61 6c6c 5f62 6174 6368 5f64 6620   small_batch_df 
+00014330: 3d20 2e2e 2e0a 2020 2020 2020 2020 2020  = ....          
+00014340: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
+00014350: 6f75 702e 6d75 6c74 695f 7061 7274 5f69  oup.multi_part_i
+00014360: 6e73 6572 7428 736d 616c 6c5f 6261 7463  nsert(small_batc
+00014370: 685f 6466 290a 0a20 2020 2020 2020 2020  h_df)..         
+00014380: 2020 2023 2049 4d50 4f52 5441 4e54 3a20     # IMPORTANT: 
+00014390: 6669 6e61 6c69 7a65 2074 6865 206d 756c  finalize the mul
+000143a0: 7469 2070 6172 7420 696e 7365 7274 2074  ti part insert t
+000143b0: 6f20 6d61 6b65 2073 7572 6520 616c 6c20  o make sure all 
+000143c0: 726f 7773 0a20 2020 2020 2020 2020 2020  rows.           
+000143d0: 2023 2068 6176 6520 6265 656e 2074 7261   # have been tra
+000143e0: 6e73 6d69 7474 6564 0a20 2020 2020 2020  nsmitted.       
+000143f0: 2020 2020 2066 6561 7475 7265 5f67 726f       feature_gro
+00014400: 7570 2e66 696e 616c 697a 655f 6d75 6c74  up.finalize_mult
+00014410: 695f 7061 7274 5f69 6e73 6572 7428 290a  i_part_insert().
+00014420: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00014430: 2020 2020 2020 2020 2020 2020 4e6f 7465              Note
+00014440: 2074 6861 7420 7468 6520 6669 7273 7420   that the first 
+00014450: 6361 6c6c 2074 6f20 606d 756c 7469 5f70  call to `multi_p
+00014460: 6172 745f 696e 7365 7274 6020 696e 6974  art_insert` init
+00014470: 6961 7465 7320 7468 6520 636f 6e74 6578  iates the contex
+00014480: 740a 2020 2020 2020 2020 2020 2020 616e  t.            an
+00014490: 6420 6265 2073 7572 6520 746f 2066 696e  d be sure to fin
+000144a0: 616c 697a 6520 6974 2e20 5468 6520 6066  alize it. The `f
+000144b0: 696e 616c 697a 655f 6d75 6c74 695f 7061  inalize_multi_pa
+000144c0: 7274 5f69 6e73 6572 7460 2069 7320 610a  rt_insert` is a.
+000144d0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
+000144e0: 6b69 6e67 2063 616c 6c20 7468 6174 2072  king call that r
+000144f0: 6574 7572 6e73 206f 6e63 6520 616c 6c20  eturns once all 
+00014500: 726f 7773 2068 6176 6520 6265 656e 2074  rows have been t
+00014510: 7261 6e73 6d69 7474 6564 2e0a 2020 2020  ransmitted..    
+00014520: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014530: 6966 2073 656c 662e 5f6b 6166 6b61 5f70  if self._kafka_p
+00014540: 726f 6475 6365 7220 6973 206e 6f74 204e  roducer is not N
+00014550: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00014560: 2073 656c 662e 5f6b 6166 6b61 5f70 726f   self._kafka_pro
+00014570: 6475 6365 722e 666c 7573 6828 290a 2020  ducer.flush().  
+00014580: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00014590: 6b61 666b 615f 7072 6f64 7563 6572 203d  kafka_producer =
+000145a0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+000145b0: 6c66 2e5f 6665 6174 7572 655f 7772 6974  lf._feature_writ
+000145c0: 6572 7320 3d20 4e6f 6e65 0a20 2020 2020  ers = None.     
+000145d0: 2020 2073 656c 662e 5f77 7269 7465 7220     self._writer 
+000145e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+000145f0: 656c 662e 5f6d 756c 7469 5f70 6172 745f  elf._multi_part_
+00014600: 696e 7365 7274 203d 2046 616c 7365 0a0a  insert = False..
+00014610: 2020 2020 6465 6620 696e 7365 7274 5f73      def insert_s
+00014620: 7472 6561 6d28 0a20 2020 2020 2020 2073  tream(.        s
+00014630: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
+00014640: 7475 7265 733a 2054 7970 6556 6172 2822  tures: TypeVar("
+00014650: 7079 7370 6172 6b2e 7371 6c2e 4461 7461  pyspark.sql.Data
+00014660: 4672 616d 6522 292c 2020 2320 6e6f 7161  Frame"),  # noqa
+00014670: 3a20 4638 3231 0a20 2020 2020 2020 2071  : F821.        q
+00014680: 7565 7279 5f6e 616d 653a 204f 7074 696f  uery_name: Optio
+00014690: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+000146a0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+000146b0: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b73  mode: Optional[s
+000146c0: 7472 5d20 3d20 2261 7070 656e 6422 2c0a  tr] = "append",.
+000146d0: 2020 2020 2020 2020 6177 6169 745f 7465          await_te
+000146e0: 726d 696e 6174 696f 6e3a 204f 7074 696f  rmination: Optio
+000146f0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+00014700: 652c 0a20 2020 2020 2020 2074 696d 656f  e,.        timeo
+00014710: 7574 3a20 4f70 7469 6f6e 616c 5b69 6e74  ut: Optional[int
+00014720: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00014730: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
+00014740: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00014750: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00014760: 7772 6974 655f 6f70 7469 6f6e 733a 204f  write_options: O
+00014770: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
+00014780: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
+00014790: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+000147a0: 496e 6765 7374 2061 2053 7061 726b 2053  Ingest a Spark S
+000147b0: 7472 7563 7475 7265 6420 5374 7265 616d  tructured Stream
+000147c0: 696e 6720 4461 7461 6672 616d 6520 746f  ing Dataframe to
+000147d0: 2074 6865 206f 6e6c 696e 6520 6665 6174   the online feat
+000147e0: 7572 6520 7374 6f72 652e 0a0a 2020 2020  ure store...    
+000147f0: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
+00014800: 6372 6561 7465 7320 6120 6c6f 6e67 2072  creates a long r
+00014810: 756e 6e69 6e67 2053 7061 726b 2053 7472  unning Spark Str
+00014820: 6561 6d69 6e67 2051 7565 7279 2c20 796f  eaming Query, yo
+00014830: 7520 6361 6e20 636f 6e74 726f 6c20 7468  u can control th
+00014840: 650a 2020 2020 2020 2020 7465 726d 696e  e.        termin
+00014850: 6174 696f 6e20 6f66 2074 6865 2071 7565  ation of the que
+00014860: 7279 2074 6872 6f75 6768 2074 6865 2061  ry through the a
+00014870: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
+00014880: 2020 2049 7420 6973 2070 6f73 7369 626c     It is possibl
+00014890: 6520 746f 2073 746f 7020 7468 6520 7265  e to stop the re
+000148a0: 7475 726e 6564 2071 7565 7279 2077 6974  turned query wit
+000148b0: 6820 7468 6520 602e 7374 6f70 2829 6020  h the `.stop()` 
+000148c0: 616e 6420 6368 6563 6b20 6974 730a 2020  and check its.  
+000148d0: 2020 2020 2020 7374 6174 7573 2077 6974        status wit
+000148e0: 6820 602e 6973 4163 7469 7665 602e 0a0a  h `.isActive`...
+000148f0: 2020 2020 2020 2020 546f 2067 6574 2061          To get a
+00014900: 206c 6973 7420 6f66 2061 6c6c 2061 6374   list of all act
+00014910: 6976 6520 7175 6572 6965 732c 2075 7365  ive queries, use
+00014920: 3a0a 0a20 2020 2020 2020 2060 6060 7079  :..        ```py
+00014930: 7468 6f6e 0a20 2020 2020 2020 2073 716d  thon.        sqm
+00014940: 203d 2073 7061 726b 2e73 7472 6561 6d73   = spark.streams
+00014950: 0a0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
+00014960: 7468 6520 6c69 7374 206f 6620 6163 7469  the list of acti
+00014970: 7665 2073 7472 6561 6d69 6e67 2071 7565  ve streaming que
+00014980: 7269 6573 0a20 2020 2020 2020 205b 712e  ries.        [q.
+00014990: 6e61 6d65 2066 6f72 2071 2069 6e20 7371  name for q in sq
+000149a0: 6d2e 6163 7469 7665 5d0a 2020 2020 2020  m.active].      
+000149b0: 2020 6060 600a 0a20 2020 2020 2020 2021    ```..        !
+000149c0: 2121 2077 6172 6e69 6e67 2022 456e 6769  !! warning "Engi
+000149d0: 6e65 2053 7570 706f 7274 220a 2020 2020  ne Support".    
+000149e0: 2020 2020 2020 2020 2a2a 5370 6172 6b20          **Spark 
+000149f0: 6f6e 6c79 2a2a 0a0a 2020 2020 2020 2020  only**..        
+00014a00: 2020 2020 5374 7265 616d 2069 6e67 6573      Stream inges
+00014a10: 7469 6f6e 2075 7369 6e67 2050 616e 6461  tion using Panda
+00014a20: 732f 5079 7468 6f6e 2061 7320 656e 6769  s/Python as engi
+00014a30: 6e65 2069 7320 6375 7272 656e 746c 7920  ne is currently 
+00014a40: 6e6f 7420 7375 7070 6f72 7465 642e 0a20  not supported.. 
+00014a50: 2020 2020 2020 2020 2020 2050 7974 686f             Pytho
+00014a60: 6e2f 5061 6e64 6173 2068 6173 206e 6f20  n/Pandas has no 
+00014a70: 6e6f 7469 6f6e 206f 6620 7374 7265 616d  notion of stream
+00014a80: 696e 672e 0a0a 2020 2020 2020 2020 2121  ing...        !!
+00014a90: 2120 7761 726e 696e 6720 2244 6174 6120  ! warning "Data 
+00014aa0: 5661 6c69 6461 7469 6f6e 2053 7570 706f  Validation Suppo
+00014ab0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+00014ac0: 6069 6e73 6572 745f 7374 7265 616d 6020  `insert_stream` 
+00014ad0: 646f 6573 206e 6f74 2070 6572 666f 726d  does not perform
+00014ae0: 2061 6e79 2064 6174 6120 7661 6c69 6461   any data valida
+00014af0: 7469 6f6e 2075 7369 6e67 2047 7265 6174  tion using Great
+00014b00: 2045 7870 6563 7461 7469 6f6e 730a 2020   Expectations.  
+00014b10: 2020 2020 2020 2020 2020 6576 656e 2077            even w
+00014b20: 6865 6e20 6120 6578 7065 6374 6174 696f  hen a expectatio
+00014b30: 6e20 7375 6974 6520 6973 2061 7474 6163  n suite is attac
+00014b40: 6865 642e 0a0a 2020 2020 2020 2020 2320  hed...        # 
+00014b50: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+00014b60: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
+00014b70: 4665 6174 7572 6573 2069 6e20 5374 7265  Features in Stre
+00014b80: 616d 696e 6720 4461 7461 6672 616d 6520  aming Dataframe 
+00014b90: 746f 2062 6520 7361 7665 642e 0a20 2020  to be saved..   
+00014ba0: 2020 2020 2020 2020 2071 7565 7279 5f6e           query_n
+00014bb0: 616d 653a 2049 7420 6973 2070 6f73 7369  ame: It is possi
+00014bc0: 626c 6520 746f 206f 7074 696f 6e61 6c6c  ble to optionall
+00014bd0: 7920 7370 6563 6966 7920 6120 6e61 6d65  y specify a name
+00014be0: 2066 6f72 2074 6865 2071 7565 7279 2074   for the query t
+00014bf0: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+00014c00: 2020 6d61 6b65 2069 7420 6561 7369 6572    make it easier
+00014c10: 2074 6f20 7265 636f 676e 6973 6520 696e   to recognise in
+00014c20: 2074 6865 2053 7061 726b 2055 492e 2044   the Spark UI. D
+00014c30: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
+00014c40: 602e 0a20 2020 2020 2020 2020 2020 206f  `..            o
+00014c50: 7574 7075 745f 6d6f 6465 3a20 5370 6563  utput_mode: Spec
+00014c60: 6966 6965 7320 686f 7720 6461 7461 206f  ifies how data o
+00014c70: 6620 6120 7374 7265 616d 696e 6720 4461  f a streaming Da
+00014c80: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
+00014c90: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
+00014ca0: 2020 2077 7269 7474 656e 2074 6f20 6120     written to a 
+00014cb0: 7374 7265 616d 696e 6720 7369 6e6b 2e20  streaming sink. 
+00014cc0: 2831 2920 6022 6170 7065 6e64 2260 3a20  (1) `"append"`: 
+00014cd0: 4f6e 6c79 2074 6865 206e 6577 2072 6f77  Only the new row
+00014ce0: 7320 696e 2074 6865 0a20 2020 2020 2020  s in the.       
+00014cf0: 2020 2020 2020 2020 2073 7472 6561 6d69           streami
+00014d00: 6e67 2044 6174 6146 7261 6d65 2f44 6174  ng DataFrame/Dat
+00014d10: 6173 6574 2077 696c 6c20 6265 2077 7269  aset will be wri
+00014d20: 7474 656e 2074 6f20 7468 6520 7369 6e6b  tten to the sink
+00014d30: 2e20 2832 290a 2020 2020 2020 2020 2020  . (2).          
+00014d40: 2020 2020 2020 6022 636f 6d70 6c65 7465        `"complete
+00014d50: 2260 3a20 416c 6c20 7468 6520 726f 7773  "`: All the rows
+00014d60: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
+00014d70: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
+00014d80: 7365 7420 7769 6c6c 2062 650a 2020 2020  set will be.    
+00014d90: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+00014da0: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
+00014db0: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
+00014dc0: 2069 7320 736f 6d65 2075 7064 6174 652e   is some update.
+00014dd0: 2028 3329 2060 2275 7064 6174 6522 603a   (3) `"update"`:
+00014de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014df0: 206f 6e6c 7920 7468 6520 726f 7773 2074   only the rows t
+00014e00: 6861 7420 7765 7265 2075 7064 6174 6564  hat were updated
+00014e10: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
+00014e20: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
+00014e30: 7365 7420 7769 6c6c 0a20 2020 2020 2020  set will.       
+00014e40: 2020 2020 2020 2020 2062 6520 7772 6974           be writ
+00014e50: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
+00014e60: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
+00014e70: 2061 7265 2073 6f6d 6520 7570 6461 7465   are some update
+00014e80: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00014e90: 2020 2049 6620 7468 6520 7175 6572 7920     If the query 
+00014ea0: 646f 6573 6ee2 8099 7420 636f 6e74 6169  doesn...t contai
+00014eb0: 6e20 6167 6772 6567 6174 696f 6e73 2c20  n aggregations, 
+00014ec0: 6974 2077 696c 6c20 6265 2065 7175 6976  it will be equiv
+00014ed0: 616c 656e 7420 746f 0a20 2020 2020 2020  alent to.       
+00014ee0: 2020 2020 2020 2020 2061 7070 656e 6420           append 
+00014ef0: 6d6f 6465 2e20 4465 6661 756c 7473 2074  mode. Defaults t
+00014f00: 6f20 6022 6170 7065 6e64 2260 2e0a 2020  o `"append"`..  
+00014f10: 2020 2020 2020 2020 2020 6177 6169 745f            await_
+00014f20: 7465 726d 696e 6174 696f 6e3a 2057 6169  termination: Wai
+00014f30: 7473 2066 6f72 2074 6865 2074 6572 6d69  ts for the termi
+00014f40: 6e61 7469 6f6e 206f 6620 7468 6973 2071  nation of this q
+00014f50: 7565 7279 2c20 6569 7468 6572 2062 790a  uery, either by.
+00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f70: 7175 6572 792e 7374 6f70 2829 206f 7220  query.stop() or 
+00014f80: 6279 2061 6e20 6578 6365 7074 696f 6e2e  by an exception.
+00014f90: 2049 6620 7468 6520 7175 6572 7920 6861   If the query ha
+00014fa0: 7320 7465 726d 696e 6174 6564 2077 6974  s terminated wit
+00014fb0: 6820 616e 0a20 2020 2020 2020 2020 2020  h an.           
+00014fc0: 2020 2020 2065 7863 6570 7469 6f6e 2c20       exception, 
+00014fd0: 7468 656e 2074 6865 2065 7863 6570 7469  then the excepti
+00014fe0: 6f6e 2077 696c 6c20 6265 2074 6872 6f77  on will be throw
+00014ff0: 6e2e 2049 6620 7469 6d65 6f75 7420 6973  n. If timeout is
+00015000: 2073 6574 2c20 6974 0a20 2020 2020 2020   set, it.       
+00015010: 2020 2020 2020 2020 2072 6574 7572 6e73           returns
+00015020: 2077 6865 7468 6572 2074 6865 2071 7565   whether the que
+00015030: 7279 2068 6173 2074 6572 6d69 6e61 7465  ry has terminate
+00015040: 6420 6f72 206e 6f74 2077 6974 6869 6e20  d or not within 
+00015050: 7468 6520 7469 6d65 6f75 740a 2020 2020  the timeout.    
+00015060: 2020 2020 2020 2020 2020 2020 7365 636f              seco
+00015070: 6e64 732e 2044 6566 6175 6c74 7320 746f  nds. Defaults to
+00015080: 2060 4661 6c73 6560 2e0a 2020 2020 2020   `False`..      
+00015090: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
+000150a0: 6e6c 7920 7265 6c65 7661 6e74 2069 6e20  nly relevant in 
+000150b0: 636f 6d62 696e 6174 696f 6e20 7769 7468  combination with
+000150c0: 2060 6177 6169 745f 7465 726d 696e 6174   `await_terminat
+000150d0: 696f 6e3d 5472 7565 602e 0a20 2020 2020  ion=True`..     
+000150e0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+000150f0: 6c74 7320 746f 2060 4e6f 6e65 602e 0a20  lts to `None`.. 
+00015100: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00015110: 706f 696e 745f 6469 723a 2043 6865 636b  point_dir: Check
+00015120: 706f 696e 7420 6469 7265 6374 6f72 7920  point directory 
+00015130: 6c6f 6361 7469 6f6e 2e20 5468 6973 2077  location. This w
+00015140: 696c 6c20 6265 2075 7365 6420 746f 2061  ill be used to a
+00015150: 7320 6120 7265 6665 7265 6e63 6520 746f  s a reference to
+00015160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015170: 2066 726f 6d20 7768 6572 6520 746f 2072   from where to r
+00015180: 6573 756d 6520 7468 6520 7374 7265 616d  esume the stream
+00015190: 696e 6720 6a6f 622e 2049 6620 604e 6f6e  ing job. If `Non
+000151a0: 6560 2074 6865 6e20 6873 6673 2077 696c  e` then hsfs wil
+000151b0: 6c20 636f 6e73 7472 7563 7420 6173 0a20  l construct as. 
+000151c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000151d0: 696e 7365 7274 5f73 7472 6561 6d5f 2220  insert_stream_" 
+000151e0: 2b20 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  + online_topic_n
+000151f0: 616d 652e 2044 6566 6175 6c74 7320 746f  ame. Defaults to
+00015200: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
+00015210: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
+00015220: 7074 696f 6e73 3a20 4164 6469 7469 6f6e  ptions: Addition
+00015230: 616c 2077 7269 7465 206f 7074 696f 6e73  al write options
+00015240: 2066 6f72 2053 7061 726b 2061 7320 6b65   for Spark as ke
+00015250: 792d 7661 6c75 6520 7061 6972 732e 0a20  y-value pairs.. 
+00015260: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00015270: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
+00015280: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+00015290: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
+000152a0: 6053 7472 6561 6d69 6e67 5175 6572 7960  `StreamingQuery`
+000152b0: 3a20 5370 6172 6b20 5374 7275 6374 7572  : Spark Structur
+000152c0: 6564 2053 7472 6561 6d69 6e67 2051 7565  ed Streaming Que
+000152d0: 7279 206f 626a 6563 742e 0a20 2020 2020  ry object..     
+000152e0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000152f0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00015300: 6e6f 7420 656e 6769 6e65 2e67 6574 5f69  not engine.get_i
+00015310: 6e73 7461 6e63 6528 292e 6973 5f73 7061  nstance().is_spa
+00015320: 726b 5f64 6174 6166 7261 6d65 2866 6561  rk_dataframe(fea
+00015330: 7475 7265 7329 0a20 2020 2020 2020 2020  tures).         
+00015340: 2020 206f 7220 6e6f 7420 6665 6174 7572     or not featur
+00015350: 6573 2e69 7353 7472 6561 6d69 6e67 0a20  es.isStreaming. 
+00015360: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00015370: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+00015380: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00015390: 2020 2020 2020 2022 4665 6174 7572 6573         "Features
+000153a0: 2068 6176 6520 746f 2062 6520 6120 7374   have to be a st
+000153b0: 7265 616d 696e 6720 7479 7065 2073 7061  reaming type spa
+000153c0: 726b 2064 6174 6166 7261 6d65 2e20 5573  rk dataframe. Us
+000153d0: 6520 6069 6e73 6572 7428 2960 206d 6574  e `insert()` met
+000153e0: 686f 6420 696e 7374 6561 642e 220a 2020  hod instead.".  
+000153f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015400: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015410: 2020 2020 2020 2320 6c6f 7765 7220 6361        # lower ca
+00015420: 7369 6e67 2066 6561 7475 7265 206e 616d  sing feature nam
+00015430: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
+00015440: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+00015450: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
+00015460: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
+00015470: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
+00015480: 6672 616d 6528 0a20 2020 2020 2020 2020  frame(.         
+00015490: 2020 2020 2020 2066 6561 7475 7265 730a         features.
+000154a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000154b0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+000154c0: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+000154d0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+000154e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000154f0: 5374 7265 616d 2069 6e67 6573 7469 6f6e  Stream ingestion
+00015500: 2066 6f72 2066 6561 7475 7265 2067 726f   for feature gro
+00015510: 7570 2060 7b7d 602c 2077 6974 6820 7665  up `{}`, with ve
+00015520: 7273 696f 6e22 0a20 2020 2020 2020 2020  rsion".         
+00015530: 2020 2020 2020 2020 2020 2022 2060 7b7d             " `{}
+00015540: 6020 7769 6c6c 206e 6f74 2063 6f6d 7075  ` will not compu
+00015550: 7465 2073 7461 7469 7374 6963 732e 220a  te statistics.".
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 292e 666f 726d 6174 2873 656c 662e 5f6e  ).format(self._n
+00015580: 616d 652c 2073 656c 662e 5f76 6572 7369  ame, self._versi
+00015590: 6f6e 292c 0a20 2020 2020 2020 2020 2020  on),.           
+000155a0: 2020 2020 2075 7469 6c2e 5374 6174 6973       util.Statis
+000155b0: 7469 6373 5761 726e 696e 672c 0a20 2020  ticsWarning,.   
+000155c0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000155d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000155e0: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+000155f0: 7570 5f65 6e67 696e 652e 696e 7365 7274  up_engine.insert
+00015600: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
+00015610: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00015620: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015630: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+00015640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015650: 2020 7175 6572 795f 6e61 6d65 2c0a 2020    query_name,.  
+00015660: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00015670: 7470 7574 5f6d 6f64 652c 0a20 2020 2020  tput_mode,.     
+00015680: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00015690: 5f74 6572 6d69 6e61 7469 6f6e 2c0a 2020  _termination,.  
+000156a0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+000156b0: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
+000156c0: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
+000156d0: 745f 6469 722c 0a20 2020 2020 2020 2020  t_dir,.         
+000156e0: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
+000156f0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+00015700: 2020 290a 0a20 2020 2064 6566 2063 6f6d    )..    def com
+00015710: 6d69 745f 6465 7461 696c 7328 0a20 2020  mit_details(.   
+00015720: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00015730: 2020 2077 616c 6c63 6c6f 636b 5f74 696d     wallclock_tim
+00015740: 653a 204f 7074 696f 6e61 6c5b 556e 696f  e: Optional[Unio
+00015750: 6e5b 7374 722c 2069 6e74 2c20 6461 7465  n[str, int, date
+00015760: 7469 6d65 2c20 6461 7465 5d5d 203d 204e  time, date]] = N
+00015770: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+00015780: 6974 3a20 4f70 7469 6f6e 616c 5b69 6e74  it: Optional[int
+00015790: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+000157a0: 0a20 2020 2020 2020 2022 2222 5265 7472  .        """Retr
+000157b0: 6965 7665 7320 636f 6d6d 6974 2074 696d  ieves commit tim
+000157c0: 656c 696e 6520 666f 7220 7468 6973 2066  eline for this f
+000157d0: 6561 7475 7265 2067 726f 7570 2e20 5468  eature group. Th
+000157e0: 6973 206d 6574 686f 6420 6361 6e20 6f6e  is method can on
+000157f0: 6c79 2062 6520 7573 6564 0a20 2020 2020  ly be used.     
+00015800: 2020 206f 6e20 7469 6d65 2074 7261 7665     on time trave
+00015810: 6c20 656e 6162 6c65 6420 6665 6174 7572  l enabled featur
+00015820: 6520 6772 6f75 7073 0a0a 2020 2020 2020  e groups..      
+00015830: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
+00015840: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
+00015850: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
+00015860: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
+00015870: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
+00015880: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
+00015890: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
+000158a0: 2023 2067 6574 2074 6865 2046 6561 7475   # get the Featu
+000158b0: 7265 2047 726f 7570 2069 6e73 7461 6e63  re Group instanc
+000158c0: 650a 2020 2020 2020 2020 2020 2020 6667  e.            fg
+000158d0: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+000158e0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+000158f0: 7028 2e2e 2e29 0a0a 2020 2020 2020 2020  p(...)..        
+00015900: 2020 2020 636f 6d6d 6974 5f64 6574 6169      commit_detai
+00015910: 6c73 203d 2066 672e 636f 6d6d 6974 5f64  ls = fg.commit_d
+00015920: 6574 6169 6c73 2829 0a20 2020 2020 2020  etails().       
+00015930: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00015940: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
+00015950: 2020 2020 2020 2020 2020 7761 6c6c 636c            wallcl
+00015960: 6f63 6b5f 7469 6d65 3a20 436f 6d6d 6974  ock_time: Commit
+00015970: 2064 6574 6169 6c73 2061 7320 6f66 2073   details as of s
+00015980: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
+00015990: 2074 696d 652e 2044 6566 6175 6c74 7320   time. Defaults 
+000159a0: 746f 2060 4e6f 6e65 602e 0a20 2020 2020  to `None`..     
+000159b0: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+000159c0: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
+000159d0: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
+000159e0: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+000159f0: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
+00015a00: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
+00015a10: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
+00015a20: 254d 602c 0a20 2020 2020 2020 2020 2020  %M`,.           
+00015a30: 2020 2020 2060 2559 2d25 6d2d 2564 2025       `%Y-%m-%d %
+00015a40: 483a 254d 3a25 5360 2c20 6f72 2060 2559  H:%M:%S`, or `%Y
+00015a50: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+00015a60: 2566 602e 0a20 2020 2020 2020 2020 2020  %f`..           
+00015a70: 206c 696d 6974 3a20 4e75 6d62 6572 206f   limit: Number o
+00015a80: 6620 636f 6d6d 6974 7320 746f 2072 6574  f commits to ret
+00015a90: 7269 6576 652e 2044 6566 6175 6c74 7320  rieve. Defaults 
+00015aa0: 746f 2060 4e6f 6e65 602e 0a0a 2020 2020  to `None`...    
+00015ab0: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00015ac0: 2020 2020 2020 2020 2020 6044 6963 745b            `Dict[
+00015ad0: 7374 722c 2044 6963 745b 7374 722c 2073  str, Dict[str, s
+00015ae0: 7472 5d5d 602e 2044 6963 7469 6f6e 6172  tr]]`. Dictionar
+00015af0: 7920 6f62 6a65 6374 206f 6620 636f 6d6d  y object of comm
+00015b00: 6974 206d 6574 6164 6174 6120 7469 6d65  it metadata time
+00015b10: 6c69 6e65 2c20 7768 6572 6520 4b65 7920  line, where Key 
+00015b20: 6973 2063 6f6d 6d69 7420 6964 2061 6e64  is commit id and
+00015b30: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
+00015b40: 2020 2069 7320 6044 6963 745b 7374 722c     is `Dict[str,
+00015b50: 2073 7472 5d60 2077 6974 6820 6b65 7920   str]` with key 
+00015b60: 7661 6c75 6520 7061 6972 7320 6f66 2064  value pairs of d
+00015b70: 6174 6520 636f 6d6d 6974 7465 6420 6f6e  ate committed on
+00015b80: 2c20 6e75 6d62 6572 206f 6620 726f 7773  , number of rows
+00015b90: 2075 7064 6174 6564 2c20 696e 7365 7274   updated, insert
+00015ba0: 6564 2061 6e64 2064 656c 6574 6564 2e0a  ed and deleted..
+00015bb0: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
+00015bc0: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
+00015bd0: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
+00015be0: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
+00015bf0: 6f72 602e 0a20 2020 2020 2020 2020 2020  or`..           
+00015c00: 2060 6873 6673 2e63 6c69 656e 742e 6578   `hsfs.client.ex
+00015c10: 6365 7074 696f 6e73 2e46 6561 7475 7265  ceptions.Feature
+00015c20: 5374 6f72 6545 7863 6570 7469 6f6e 602e  StoreException`.
+00015c30: 2049 6620 7468 6520 6665 6174 7572 6520   If the feature 
+00015c40: 6772 6f75 7020 646f 6573 206e 6f74 2068  group does not h
+00015c50: 6176 6520 6048 5544 4960 2074 696d 6520  ave `HUDI` time 
+00015c60: 7472 6176 656c 2066 6f72 6d61 740a 2020  travel format.  
+00015c70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015c80: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+00015c90: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
+00015ca0: 696e 652e 636f 6d6d 6974 5f64 6574 6169  ine.commit_detai
+00015cb0: 6c73 2873 656c 662c 2077 616c 6c63 6c6f  ls(self, wallclo
+00015cc0: 636b 5f74 696d 652c 206c 696d 6974 290a  ck_time, limit).
+00015cd0: 0a20 2020 2064 6566 2063 6f6d 6d69 745f  .    def commit_
+00015ce0: 6465 6c65 7465 5f72 6563 6f72 6428 0a20  delete_record(. 
+00015cf0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00015d00: 2020 2020 2064 656c 6574 655f 6466 3a20       delete_df: 
+00015d10: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
+00015d20: 2e73 716c 2e44 6174 6146 7261 6d65 2229  .sql.DataFrame")
+00015d30: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+00015d40: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
+00015d50: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+00015d60: 4469 6374 5b41 6e79 2c20 416e 795d 5d20  Dict[Any, Any]] 
+00015d70: 3d20 7b7d 2c0a 2020 2020 293a 0a20 2020  = {},.    ):.   
+00015d80: 2020 2020 2022 2222 4472 6f70 7320 7265       """Drops re
+00015d90: 636f 7264 7320 7072 6573 656e 7420 696e  cords present in
+00015da0: 2074 6865 2070 726f 7669 6465 6420 4461   the provided Da
+00015db0: 7461 4672 616d 6520 616e 6420 636f 6d6d  taFrame and comm
+00015dc0: 6974 7320 6974 2061 7320 7570 6461 7465  its it as update
+00015dd0: 2074 6f20 7468 6973 0a20 2020 2020 2020   to this.       
+00015de0: 2046 6561 7475 7265 2067 726f 7570 2e20   Feature group. 
+00015df0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
+00015e00: 6f6e 6c79 2062 6520 7573 6564 206f 6e20  only be used on 
+00015e10: 7469 6d65 2074 7261 7665 6c20 656e 6162  time travel enab
+00015e20: 6c65 6420 6665 6174 7572 6520 6772 6f75  led feature grou
+00015e30: 7073 2e0a 0a20 2020 2020 2020 2023 2041  ps...        # A
+00015e40: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00015e50: 2020 2020 2064 656c 6574 655f 6466 3a20       delete_df: 
+00015e60: 6461 7461 4672 616d 6520 636f 6e74 6169  dataFrame contai
+00015e70: 6e69 6e67 2072 6563 6f72 6473 2074 6f20  ning records to 
+00015e80: 6265 2064 656c 6574 6564 2e0a 2020 2020  be deleted..    
+00015e90: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
+00015ea0: 7469 6f6e 733a 2055 7365 7220 7072 6f76  tions: User prov
+00015eb0: 6964 6564 2077 7269 7465 206f 7074 696f  ided write optio
+00015ec0: 6e73 2e20 4465 6661 756c 7473 2074 6f20  ns. Defaults to 
+00015ed0: 607b 7d60 2e0a 0a20 2020 2020 2020 2023  `{}`...        #
+00015ee0: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
+00015ef0: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
+00015f00: 2e65 7863 6570 7469 6f6e 732e 5265 7374  .exceptions.Rest
+00015f10: 4150 4945 7272 6f72 602e 0a20 2020 2020  APIError`..     
+00015f20: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00015f30: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+00015f40: 7570 5f65 6e67 696e 652e 636f 6d6d 6974  up_engine.commit
+00015f50: 5f64 656c 6574 6528 7365 6c66 2c20 6465  _delete(self, de
+00015f60: 6c65 7465 5f64 662c 2077 7269 7465 5f6f  lete_df, write_o
+00015f70: 7074 696f 6e73 290a 0a20 2020 2064 6566  ptions)..    def
+00015f80: 2061 735f 6f66 280a 2020 2020 2020 2020   as_of(.        
+00015f90: 7365 6c66 2c0a 2020 2020 2020 2020 7761  self,.        wa
+00015fa0: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
+00015fb0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+00015fc0: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
+00015fd0: 2064 6174 655d 5d20 3d20 4e6f 6e65 2c0a   date]] = None,.
+00015fe0: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
+00015ff0: 756e 7469 6c3a 204f 7074 696f 6e61 6c5b  until: Optional[
+00016000: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+00016010: 6461 7465 7469 6d65 2c20 6461 7465 5d5d  datetime, date]]
+00016020: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00016030: 2020 2020 2020 2020 2222 2247 6574 2051          """Get Q
+00016040: 7565 7279 206f 626a 6563 7420 746f 2072  uery object to r
+00016050: 6574 7269 6576 6520 616c 6c20 6665 6174  etrieve all feat
+00016060: 7572 6573 206f 6620 7468 6520 6772 6f75  ures of the grou
+00016070: 7020 6174 2061 2070 6f69 6e74 2069 6e20  p at a point in 
+00016080: 7468 6520 7061 7374 2e0a 0a20 2020 2020  the past...     
+00016090: 2020 2054 6869 7320 6d65 7468 6f64 2073     This method s
+000160a0: 656c 6563 7473 2061 6c6c 2066 6561 7475  elects all featu
+000160b0: 7265 7320 696e 2074 6865 2066 6561 7475  res in the featu
+000160c0: 7265 2067 726f 7570 2061 6e64 2072 6574  re group and ret
+000160d0: 7572 6e73 2061 2051 7565 7279 206f 626a  urns a Query obj
+000160e0: 6563 740a 2020 2020 2020 2020 6174 2074  ect.        at t
+000160f0: 6865 2073 7065 6369 6669 6564 2070 6f69  he specified poi
+00016100: 6e74 2069 6e20 7469 6d65 2e20 4f70 7469  nt in time. Opti
+00016110: 6f6e 616c 6c79 2c20 636f 6d6d 6974 7320  onally, commits 
+00016120: 6265 666f 7265 2061 2073 7065 6369 6669  before a specifi
+00016130: 6564 2070 6f69 6e74 2069 6e20 7469 6d65  ed point in time
+00016140: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00016150: 6578 636c 7564 6564 2066 726f 6d20 7468  excluded from th
+00016160: 6520 7175 6572 792e 2054 6865 2051 7565  e query. The Que
+00016170: 7279 2063 616e 2074 6865 6e20 6569 7468  ry can then eith
+00016180: 6572 2062 6520 7265 6164 2069 6e74 6f20  er be read into 
+00016190: 6120 4461 7461 6672 616d 650a 2020 2020  a Dataframe.    
+000161a0: 2020 2020 6f72 2075 7365 6420 6675 7274      or used furt
+000161b0: 6865 7220 746f 2070 6572 666f 726d 206a  her to perform j
+000161c0: 6f69 6e73 206f 7220 636f 6e73 7472 7563  oins or construc
+000161d0: 7420 6120 7472 6169 6e69 6e67 2064 6174  t a training dat
+000161e0: 6173 6574 2e0a 0a20 2020 2020 2020 2021  aset...        !
+000161f0: 2121 2065 7861 6d70 6c65 2022 5265 6164  !! example "Read
+00016200: 696e 6720 6665 6174 7572 6573 2061 7420  ing features at 
+00016210: 6120 7370 6563 6966 6963 2070 6f69 6e74  a specific point
+00016220: 2069 6e20 7469 6d65 3a22 0a20 2020 2020   in time:".     
+00016230: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00016240: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00016250: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+00016260: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+00016270: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+00016280: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00016290: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+000162a0: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+000162b0: 2020 2020 2020 2020 2020 2066 6720 3d20             fg = 
+000162c0: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+000162d0: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+000162e0: 2e2e 290a 0a20 2020 2020 2020 2020 2020  ..)..           
+000162f0: 2023 2067 6574 2064 6174 6120 6174 2061   # get data at a
+00016300: 2073 7065 6369 6669 6320 706f 696e 7420   specific point 
+00016310: 696e 2074 696d 6520 616e 6420 7368 6f77  in time and show
+00016320: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+00016330: 6667 2e61 735f 6f66 2822 3230 3230 2d31  fg.as_of("2020-1
+00016340: 302d 3230 2030 373a 3334 3a31 3122 292e  0-20 07:34:11").
+00016350: 7265 6164 2829 2e73 686f 7728 290a 2020  read().show().  
+00016360: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+00016370: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
+00016380: 6c65 2022 5265 6164 696e 6720 636f 6d6d  le "Reading comm
+00016390: 6974 7320 696e 6372 656d 656e 7461 6c6c  its incrementall
+000163a0: 7920 6265 7477 6565 6e20 7370 6563 6966  y between specif
+000163b0: 6965 6420 706f 696e 7473 2069 6e20 7469  ied points in ti
+000163c0: 6d65 3a22 0a20 2020 2020 2020 2020 2020  me:".           
+000163d0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+000163e0: 2020 2020 2020 2066 672e 6173 5f6f 6628         fg.as_of(
+000163f0: 2232 3032 302d 3130 2d32 3020 3037 3a33  "2020-10-20 07:3
+00016400: 343a 3131 222c 2065 7863 6c75 6465 5f75  4:11", exclude_u
+00016410: 6e74 696c 3d22 3230 3230 2d31 302d 3139  ntil="2020-10-19
+00016420: 2030 373a 3334 3a31 3122 292e 7265 6164   07:34:11").read
+00016430: 2829 2e73 686f 7728 290a 2020 2020 2020  ().show().      
+00016440: 2020 2020 2020 6060 600a 0a20 2020 2020        ```..     
+00016450: 2020 2054 6865 2066 6972 7374 2070 6172     The first par
+00016460: 616d 6574 6572 2069 7320 696e 636c 7573  ameter is inclus
+00016470: 6976 6520 7768 696c 6520 7468 6520 6c61  ive while the la
+00016480: 7474 6572 2069 7320 6578 636c 7573 6976  tter is exclusiv
+00016490: 652e 0a20 2020 2020 2020 2054 6861 7420  e..        That 
+000164a0: 6d65 616e 732c 2069 6e20 6f72 6465 7220  means, in order 
+000164b0: 746f 2071 7565 7279 2061 2073 696e 676c  to query a singl
+000164c0: 6520 636f 6d6d 6974 2c20 796f 7520 6e65  e commit, you ne
+000164d0: 6564 2074 6f20 7175 6572 7920 7468 6174  ed to query that
+000164e0: 2063 6f6d 6d69 7420 7469 6d65 0a20 2020   commit time.   
+000164f0: 2020 2020 2061 6e64 2065 7863 6c75 6465       and exclude
+00016500: 2065 7665 7279 7468 696e 6720 6a75 7374   everything just
+00016510: 2062 6566 6f72 6520 7468 6520 636f 6d6d   before the comm
+00016520: 6974 2e0a 0a20 2020 2020 2020 2021 2121  it...        !!!
+00016530: 2065 7861 6d70 6c65 2022 5265 6164 696e   example "Readin
+00016540: 6720 6f6e 6c79 2074 6865 2063 6861 6e67  g only the chang
+00016550: 6573 2066 726f 6d20 6120 7369 6e67 6c65  es from a single
+00016560: 2063 6f6d 6d69 7422 0a20 2020 2020 2020   commit".       
+00016570: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00016580: 2020 2020 2020 2020 2020 2066 672e 6173             fg.as
+00016590: 5f6f 6628 2232 3032 302d 3130 2d32 3020  _of("2020-10-20 
+000165a0: 3037 3a33 313a 3338 222c 2065 7863 6c75  07:31:38", exclu
+000165b0: 6465 5f75 6e74 696c 3d22 3230 3230 2d31  de_until="2020-1
+000165c0: 302d 3230 2030 373a 3331 3a33 3722 292e  0-20 07:31:37").
+000165d0: 7265 6164 2829 2e73 686f 7728 290a 2020  read().show().  
+000165e0: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+000165f0: 2020 2020 2020 2057 6865 6e20 6e6f 2077         When no w
+00016600: 616c 6c63 6c6f 636b 5f74 696d 6520 6973  allclock_time is
+00016610: 2067 6976 656e 2c20 7468 6520 6c61 7465   given, the late
+00016620: 7374 2073 7461 7465 206f 6620 6665 6174  st state of feat
+00016630: 7572 6573 2069 7320 7265 7475 726e 6564  ures is returned
+00016640: 2e20 4f70 7469 6f6e 616c 6c79 2c20 636f  . Optionally, co
+00016650: 6d6d 6974 7320 6265 666f 7265 0a20 2020  mmits before.   
+00016660: 2020 2020 2061 2073 7065 6369 6669 6564       a specified
+00016670: 2070 6f69 6e74 2069 6e20 7469 6d65 2063   point in time c
+00016680: 616e 2073 7469 6c6c 2062 6520 6578 636c  an still be excl
+00016690: 7564 6564 2e0a 0a20 2020 2020 2020 2021  uded...        !
+000166a0: 2121 2065 7861 6d70 6c65 2022 5265 6164  !! example "Read
+000166b0: 696e 6720 7468 6520 6c61 7465 7374 2073  ing the latest s
+000166c0: 7461 7465 206f 6620 6665 6174 7572 6573  tate of features
+000166d0: 2c20 6578 636c 7564 696e 6720 636f 6d6d  , excluding comm
+000166e0: 6974 7320 6265 666f 7265 2061 2073 7065  its before a spe
+000166f0: 6369 6669 6564 2070 6f69 6e74 2069 6e20  cified point in 
+00016700: 7469 6d65 3a22 0a20 2020 2020 2020 2020  time:".         
+00016710: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00016720: 2020 2020 2020 2020 2066 672e 6173 5f6f           fg.as_o
+00016730: 6628 4e6f 6e65 2c20 6578 636c 7564 655f  f(None, exclude_
+00016740: 756e 7469 6c3d 2232 3032 302d 3130 2d32  until="2020-10-2
+00016750: 3020 3037 3a33 313a 3338 2229 2e72 6561  0 07:31:38").rea
+00016760: 6428 292e 7368 6f77 2829 0a20 2020 2020  d().show().     
+00016770: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
+00016780: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
+00016790: 6520 696e 7465 7276 616c 2077 696c 6c20  e interval will 
+000167a0: 6265 2061 7070 6c69 6564 2074 6f20 616c  be applied to al
+000167b0: 6c20 6a6f 696e 7320 696e 2074 6865 2071  l joins in the q
+000167c0: 7565 7279 2e0a 2020 2020 2020 2020 4966  uery..        If
+000167d0: 2079 6f75 2077 616e 7420 746f 2071 7565   you want to que
+000167e0: 7279 2064 6966 6665 7265 6e74 2069 6e74  ry different int
+000167f0: 6572 7661 6c73 2066 6f72 2064 6966 6665  ervals for diffe
+00016800: 7265 6e74 2066 6561 7475 7265 2067 726f  rent feature gro
+00016810: 7570 7320 696e 0a20 2020 2020 2020 2074  ups in.        t
+00016820: 6865 2071 7565 7279 2c20 796f 7520 6861  he query, you ha
+00016830: 7665 2074 6f20 6170 706c 7920 7468 656d  ve to apply them
+00016840: 2069 6e20 6120 6e65 7374 6564 2066 6173   in a nested fas
+00016850: 6869 6f6e 3a0a 2020 2020 2020 2020 2121  hion:.        !!
+00016860: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
+00016870: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00016880: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00016890: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
+000168a0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
+000168b0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
+000168c0: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+000168d0: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
+000168e0: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
+000168f0: 2020 2020 2020 2020 2020 6667 3120 3d20            fg1 = 
+00016900: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+00016910: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+00016920: 2e2e 290a 2020 2020 2020 2020 2020 2020  ..).            
+00016930: 6667 3220 3d20 6673 2e67 6574 5f6f 725f  fg2 = fs.get_or_
+00016940: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00016950: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
+00016960: 2020 2020 2020 2066 6731 2e73 656c 6563         fg1.selec
+00016970: 745f 616c 6c28 292e 6173 5f6f 6628 2232  t_all().as_of("2
+00016980: 3032 302d 3130 2d32 3022 2c20 6578 636c  020-10-20", excl
+00016990: 7564 655f 756e 7469 6c3d 2232 3032 302d  ude_until="2020-
+000169a0: 3130 2d31 3922 290a 2020 2020 2020 2020  10-19").        
+000169b0: 2020 2020 2020 2020 2e6a 6f69 6e28 6667          .join(fg
+000169c0: 322e 7365 6c65 6374 5f61 6c6c 2829 2e61  2.select_all().a
+000169d0: 735f 6f66 2822 3230 3230 2d31 302d 3230  s_of("2020-10-20
+000169e0: 222c 2065 7863 6c75 6465 5f75 6e74 696c  ", exclude_until
+000169f0: 3d22 3230 3230 2d31 302d 3139 2229 290a  ="2020-10-19")).
+00016a00: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00016a10: 0a20 2020 2020 2020 2049 6620 696e 7374  .        If inst
+00016a20: 6561 6420 796f 7520 6170 706c 7920 616e  ead you apply an
+00016a30: 6f74 6865 7220 6061 735f 6f66 6020 7365  other `as_of` se
+00016a40: 6c65 6374 696f 6e20 6166 7465 7220 7468  lection after th
+00016a50: 6520 6a6f 696e 2c20 616c 6c0a 2020 2020  e join, all.    
+00016a60: 2020 2020 6a6f 696e 6564 2066 6561 7475      joined featu
+00016a70: 7265 2067 726f 7570 7320 7769 6c6c 2062  re groups will b
+00016a80: 6520 7175 6572 6965 6420 7769 7468 2074  e queried with t
+00016a90: 6869 7320 696e 7465 7276 616c 3a0a 2020  his interval:.  
+00016aa0: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
+00016ab0: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
+00016ac0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00016ad0: 2020 2020 6667 312e 7365 6c65 6374 5f61      fg1.select_a
+00016ae0: 6c6c 2829 2e61 735f 6f66 2822 3230 3230  ll().as_of("2020
+00016af0: 2d31 302d 3230 222c 2065 7863 6c75 6465  -10-20", exclude
+00016b00: 5f75 6e74 696c 3d22 3230 3230 2d31 302d  _until="2020-10-
+00016b10: 3139 2229 2020 2320 6173 5f6f 6620 6973  19")  # as_of is
+00016b20: 206e 6f74 2061 7070 6c69 6564 0a20 2020   not applied.   
+00016b30: 2020 2020 2020 2020 2020 2020 202e 6a6f               .jo
+00016b40: 696e 2866 6732 2e73 656c 6563 745f 616c  in(fg2.select_al
+00016b50: 6c28 292e 6173 5f6f 6628 2232 3032 302d  l().as_of("2020-
+00016b60: 3130 2d32 3022 2c20 6578 636c 7564 655f  10-20", exclude_
+00016b70: 756e 7469 6c3d 2232 3032 302d 3130 2d31  until="2020-10-1
+00016b80: 3522 2929 2020 2320 6173 5f6f 6620 6973  5"))  # as_of is
+00016b90: 206e 6f74 2061 7070 6c69 6564 0a20 2020   not applied.   
+00016ba0: 2020 2020 2020 2020 2020 2020 202e 6173               .as
+00016bb0: 5f6f 6628 2232 3032 302d 3130 2d32 3022  _of("2020-10-20"
+00016bc0: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
+00016bd0: 2232 3032 302d 3130 2d31 3922 290a 2020  "2020-10-19").  
+00016be0: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+00016bf0: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
+00016c00: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
+00016c10: 6869 7320 6675 6e63 7469 6f6e 206f 6e6c  his function onl
+00016c20: 7920 776f 726b 7320 666f 7220 6665 6174  y works for feat
+00016c30: 7572 6520 6772 6f75 7073 2077 6974 6820  ure groups with 
+00016c40: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
+00016c50: 6174 3d27 4855 4449 272e 0a0a 2020 2020  at='HUDI'...    
+00016c60: 2020 2020 2121 2120 7761 726e 696e 670a      !!! warning.
+00016c70: 2020 2020 2020 2020 2020 2020 4578 636c              Excl
+00016c80: 7564 696e 6720 636f 6d6d 6974 7320 7669  uding commits vi
+00016c90: 6120 6578 636c 7564 655f 756e 7469 6c20  a exclude_until 
+00016ca0: 6973 206f 6e6c 7920 706f 7373 6962 6c65  is only possible
+00016cb0: 2077 6974 6869 6e20 7468 6520 7261 6e67   within the rang
+00016cc0: 6520 6f66 2074 6865 2048 7564 6920 6163  e of the Hudi ac
+00016cd0: 7469 7665 2074 696d 656c 696e 652e 0a20  tive timeline.. 
+00016ce0: 2020 2020 2020 2020 2020 2042 7920 6465             By de
+00016cf0: 6661 756c 742c 2048 7564 6920 6b65 6570  fault, Hudi keep
+00016d00: 7320 7468 6520 6c61 7374 2032 3020 746f  s the last 20 to
+00016d10: 2033 3020 636f 6d6d 6974 7320 696e 2074   30 commits in t
+00016d20: 6865 2061 6374 6976 6520 7469 6d65 6c69  he active timeli
+00016d30: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
+00016d40: 4966 2079 6f75 206e 6565 6420 746f 206b  If you need to k
+00016d50: 6565 7020 6120 6c6f 6e67 6572 2061 6374  eep a longer act
+00016d60: 6976 6520 7469 6d65 6c69 6e65 2c20 796f  ive timeline, yo
+00016d70: 7520 6361 6e20 6f76 6572 7772 6974 6520  u can overwrite 
+00016d80: 7468 6520 6f70 7469 6f6e 733a 0a20 2020  the options:.   
+00016d90: 2020 2020 2020 2020 2060 686f 6f64 6965           `hoodie
+00016da0: 2e6b 6565 702e 6d69 6e2e 636f 6d6d 6974  .keep.min.commit
+00016db0: 7360 2061 6e64 2060 686f 6f64 6965 2e6b  s` and `hoodie.k
+00016dc0: 6565 702e 6d61 782e 636f 6d6d 6974 7360  eep.max.commits`
+00016dd0: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
+00016de0: 6e20 6361 6c6c 696e 6720 7468 6520 6069  n calling the `i
+00016df0: 6e73 6572 7428 2960 206d 6574 686f 642e  nsert()` method.
+00016e00: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
+00016e10: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+00016e20: 2020 7761 6c6c 636c 6f63 6b5f 7469 6d65    wallclock_time
+00016e30: 3a20 5265 6164 2064 6174 6120 6173 206f  : Read data as o
+00016e40: 6620 7468 6973 2070 6f69 6e74 2069 6e20  f this point in 
+00016e50: 7469 6d65 2e20 5374 7269 6e67 7320 7368  time. Strings sh
+00016e60: 6f75 6c64 2062 6520 666f 726d 6174 7465  ould be formatte
+00016e70: 6420 696e 206f 6e65 206f 6620 7468 650a  d in one of the.
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+00016ea0: 7320 6025 592d 256d 2d25 6460 2c20 6025  s `%Y-%m-%d`, `%
+00016eb0: 592d 256d 2d25 6420 2548 602c 2060 2559  Y-%m-%d %H`, `%Y
+00016ec0: 2d25 6d2d 2564 2025 483a 254d 602c 206f  -%m-%d %H:%M`, o
+00016ed0: 7220 6025 592d 256d 2d25 6420 2548 3a25  r `%Y-%m-%d %H:%
+00016ee0: 4d3a 2553 602e 0a20 2020 2020 2020 2020  M:%S`..         
+00016ef0: 2020 2065 7863 6c75 6465 5f75 6e74 696c     exclude_until
+00016f00: 3a20 4578 636c 7564 6520 636f 6d6d 6974  : Exclude commit
+00016f10: 7320 756e 7469 6c20 7468 6973 2070 6f69  s until this poi
+00016f20: 6e74 2069 6e20 7469 6d65 2e20 5374 7269  nt in time. Stri
+00016f30: 6e67 2073 686f 756c 6420 6265 2066 6f72  ng should be for
+00016f40: 6d61 7474 6564 2069 6e20 6f6e 6520 6f66  matted in one of
+00016f50: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00016f60: 2020 2020 2066 6f6c 6c6f 7769 6e67 2066       following f
+00016f70: 6f72 6d61 7473 2060 2559 2d25 6d2d 2564  ormats `%Y-%m-%d
+00016f80: 602c 2060 2559 2d25 6d2d 2564 2025 4860  `, `%Y-%m-%d %H`
+00016f90: 2c20 6025 592d 256d 2d25 6420 2548 3a25  , `%Y-%m-%d %H:%
+00016fa0: 4d60 2c20 6f72 2060 2559 2d25 6d2d 2564  M`, or `%Y-%m-%d
+00016fb0: 2025 483a 254d 3a25 5360 2e0a 0a20 2020   %H:%M:%S`...   
+00016fc0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+00016fd0: 2020 2020 2020 2020 2020 2060 5175 6572             `Quer
+00016fe0: 7960 2e20 5468 6520 7175 6572 7920 6f62  y`. The query ob
+00016ff0: 6a65 6374 2077 6974 6820 7468 6520 6170  ject with the ap
+00017000: 706c 6965 6420 7469 6d65 2074 7261 7665  plied time trave
+00017010: 6c20 636f 6e64 6974 696f 6e2e 0a20 2020  l condition..   
+00017020: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00017030: 2072 6574 7572 6e20 7365 6c66 2e73 656c   return self.sel
+00017040: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
+00017050: 7761 6c6c 636c 6f63 6b5f 7469 6d65 2c20  wallclock_time, 
+00017060: 6578 636c 7564 655f 756e 7469 6c29 0a0a  exclude_until)..
+00017070: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
+00017080: 7374 6174 6973 7469 6373 280a 2020 2020  statistics(.    
+00017090: 2020 2020 7365 6c66 2c20 7761 6c6c 636c      self, wallcl
+000170a0: 6f63 6b5f 7469 6d65 3a20 4f70 7469 6f6e  ock_time: Option
+000170b0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 696e  al[Union[str, in
+000170c0: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
+000170d0: 655d 5d20 3d20 4e6f 6e65 0a20 2020 2029  e]] = None.    )
+000170e0: 3a0a 2020 2020 2020 2020 2222 2252 6563  :.        """Rec
+000170f0: 6f6d 7075 7465 2074 6865 2073 7461 7469  ompute the stati
+00017100: 7374 6963 7320 666f 7220 7468 6520 6665  stics for the fe
+00017110: 6174 7572 6520 6772 6f75 7020 616e 6420  ature group and 
+00017120: 7361 7665 2074 6865 6d20 746f 2074 6865  save them to the
+00017130: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00017140: 2073 746f 7265 2e0a 0a20 2020 2020 2020   store...       
+00017150: 2053 7461 7469 7374 6963 7320 6172 6520   Statistics are 
+00017160: 6f6e 6c79 2063 6f6d 7075 7465 6420 666f  only computed fo
+00017170: 7220 6461 7461 2069 6e20 7468 6520 6f66  r data in the of
+00017180: 666c 696e 6520 7374 6f72 6167 6520 6f66  fline storage of
+00017190: 2074 6865 2066 6561 7475 7265 0a20 2020   the feature.   
+000171a0: 2020 2020 2067 726f 7570 2e0a 0a20 2020       group...   
+000171b0: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
+000171c0: 0a20 2020 2020 2020 2020 2020 2077 616c  .            wal
+000171d0: 6c63 6c6f 636b 5f74 696d 653a 2049 6620  lclock_time: If 
+000171e0: 7370 6563 6966 6965 6420 7769 6c6c 2072  specified will r
+000171f0: 6563 6f6d 7075 7465 2073 7461 7469 7374  ecompute statist
+00017200: 6963 7320 6f6e 0a20 2020 2020 2020 2020  ics on.         
+00017210: 2020 2020 2020 2066 6561 7475 7265 2067         feature g
+00017220: 726f 7570 2061 7320 6f66 2073 7065 6369  roup as of speci
+00017230: 6669 6320 706f 696e 7420 696e 2074 696d  fic point in tim
+00017240: 652e 2049 6620 6e6f 7420 7370 6563 6966  e. If not specif
+00017250: 6965 6420 7468 656e 2077 696c 6c20 636f  ied then will co
+00017260: 6d70 7574 6520 7374 6174 6973 7469 6373  mpute statistics
+00017270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017280: 2061 7320 6f66 206d 6f73 7420 7265 6365   as of most rece
+00017290: 6e74 2074 696d 6520 6f66 2074 6869 7320  nt time of this 
+000172a0: 6665 6174 7572 6520 6772 6f75 702e 2044  feature group. D
+000172b0: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
+000172c0: 602e 2053 7472 696e 6773 2073 686f 756c  `. Strings shoul
+000172d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000172e0: 2020 6265 2066 6f72 6d61 7474 6564 2069    be formatted i
+000172f0: 6e20 6f6e 6520 6f66 2074 6865 2066 6f6c  n one of the fol
+00017300: 6c6f 7769 6e67 2066 6f72 6d61 7473 2060  lowing formats `
+00017310: 2559 2d25 6d2d 2564 602c 2060 2559 2d25  %Y-%m-%d`, `%Y-%
+00017320: 6d2d 2564 2025 4860 2c20 6025 592d 256d  m-%d %H`, `%Y-%m
+00017330: 2d25 6420 2548 3a25 4d60 2c20 6025 592d  -%d %H:%M`, `%Y-
+00017340: 256d 2d25 6420 2548 3a25 4d3a 2553 602c  %m-%d %H:%M:%S`,
+00017350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017360: 206f 7220 6025 592d 256d 2d25 6420 2548   or `%Y-%m-%d %H
+00017370: 3a25 4d3a 2553 2e25 6660 2e0a 0a20 2020  :%M:%S.%f`...   
+00017380: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+00017390: 2020 2020 2020 2020 2020 2060 5374 6174             `Stat
+000173a0: 6973 7469 6373 602e 2054 6865 2073 7461  istics`. The sta
+000173b0: 7469 7374 6963 7320 6d65 7461 6461 7461  tistics metadata
+000173c0: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
+000173d0: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
+000173e0: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+000173f0: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
+00017400: 6573 7441 5049 4572 726f 7260 2e20 556e  estAPIError`. Un
+00017410: 6162 6c65 2074 6f20 7065 7273 6973 7420  able to persist 
+00017420: 7468 6520 7374 6174 6973 7469 6373 2e0a  the statistics..
+00017430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017440: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00017450: 6973 7469 6373 5f63 6f6e 6669 672e 656e  istics_config.en
+00017460: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
+00017470: 2020 2023 2044 6f6e 2774 2072 6561 6420     # Don't read 
+00017480: 7468 6520 6461 7461 6672 616d 6520 6865  the dataframe he
+00017490: 7265 2c20 746f 2061 766f 6964 2074 7269  re, to avoid tri
+000174a0: 6767 6572 696e 6720 6120 7265 6164 206f  ggering a read o
+000174b0: 7065 7261 7469 6f6e 0a20 2020 2020 2020  peration.       
+000174c0: 2020 2020 2023 2066 6f72 2074 6865 2050       # for the P
+000174d0: 7974 686f 6e20 656e 6769 6e65 2e20 5468  ython engine. Th
+000174e0: 6520 5079 7468 6f6e 2065 6e67 696e 6520  e Python engine 
+000174f0: 6973 2067 6f69 6e67 2074 6f20 7365 7475  is going to setu
+00017500: 7020 6120 5370 6172 6b20 4a6f 620a 2020  p a Spark Job.  
+00017510: 2020 2020 2020 2020 2020 2320 746f 2075            # to u
+00017520: 7064 6174 6520 7468 6520 7374 6174 6973  pdate the statis
+00017530: 7469 6373 2e0a 0a20 2020 2020 2020 2020  tics...         
+00017540: 2020 2066 675f 636f 6d6d 6974 5f69 6420     fg_commit_id 
+00017550: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00017560: 2020 2069 6620 7761 6c6c 636c 6f63 6b5f     if wallclock_
+00017570: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
+00017580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017590: 2020 2320 5265 7472 6965 7665 2066 6720    # Retrieve fg 
+000175a0: 636f 6d6d 6974 2069 6420 7265 6c61 7465  commit id relate
+000175b0: 6420 746f 2074 6869 7320 7761 6c6c 2063  d to this wall c
+000175c0: 6c6f 636b 2074 696d 6520 616e 6420 7265  lock time and re
+000175d0: 636f 6d70 7574 6520 7374 6174 6973 7469  compute statisti
+000175e0: 6373 2e20 4974 2077 696c 6c20 7468 726f  cs. It will thro
+000175f0: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+00017600: 2020 2320 6578 6365 7074 696f 6e20 6966    # exception if
+00017610: 2069 7473 206e 6f74 2074 696d 6520 7472   its not time tr
+00017620: 6176 656c 2065 6e61 626c 6564 2066 6561  avel enabled fea
+00017630: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+00017640: 2020 2020 2020 2020 2020 2020 6667 5f63              fg_c
+00017650: 6f6d 6d69 745f 6964 203d 205b 0a20 2020  ommit_id = [.   
+00017660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017670: 2063 6f6d 6d69 745f 6964 0a20 2020 2020   commit_id.     
+00017680: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017690: 6f72 2063 6f6d 6d69 745f 6964 2069 6e20  or commit_id in 
+000176a0: 7365 6c66 2e5f 6665 6174 7572 655f 6772  self._feature_gr
+000176b0: 6f75 705f 656e 6769 6e65 2e63 6f6d 6d69  oup_engine.commi
+000176c0: 745f 6465 7461 696c 7328 0a20 2020 2020  t_details(.     
+000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176e0: 2020 2073 656c 662c 2077 616c 6c63 6c6f     self, wallclo
+000176f0: 636b 5f74 696d 652c 2031 0a20 2020 2020  ck_time, 1.     
+00017700: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00017710: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
+00017720: 2020 2020 2020 2020 5d5b 305d 0a0a 2020          ][0]..  
+00017730: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017740: 2073 656c 662e 5f73 7461 7469 7374 6963   self._statistic
+00017750: 735f 656e 6769 6e65 2e63 6f6d 7075 7465  s_engine.compute
+00017760: 5f73 7461 7469 7374 6963 7328 0a20 2020  _statistics(.   
+00017770: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017780: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00017790: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+000177a0: 5f63 6f6d 6d69 745f 6964 3d66 675f 636f  _commit_id=fg_co
+000177b0: 6d6d 6974 5f69 640a 2020 2020 2020 2020  mmit_id.        
+000177c0: 2020 2020 2020 2020 6966 2066 675f 636f          if fg_co
+000177d0: 6d6d 6974 5f69 6420 6973 206e 6f74 204e  mmit_id is not N
+000177e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000177f0: 2020 2020 656c 7365 204e 6f6e 652c 0a20      else None,. 
+00017800: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00017810: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00017820: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00017830: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
+00017840: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00017850: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+00017860: 2073 7461 7469 7374 6963 7320 6172 6520   statistics are 
+00017870: 6e6f 7420 656e 6162 6c65 6420 6f66 2066  not enabled of f
+00017880: 6561 7475 7265 2067 726f 7570 2060 7b7d  eature group `{}
+00017890: 602c 2077 6974 6820 7665 7273 696f 6e22  `, with version"
+000178a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178b0: 2020 2020 2022 2060 7b7d 602e 204e 6f20       " `{}`. No 
+000178c0: 7374 6174 6973 7469 6373 2063 6f6d 7075  statistics compu
+000178d0: 7465 642e 220a 2020 2020 2020 2020 2020  ted.".          
+000178e0: 2020 2020 2020 292e 666f 726d 6174 2873        ).format(s
+000178f0: 656c 662e 5f6e 616d 652c 2073 656c 662e  elf._name, self.
+00017900: 5f76 6572 7369 6f6e 292c 0a20 2020 2020  _version),.     
+00017910: 2020 2020 2020 2020 2020 2075 7469 6c2e             util.
+00017920: 5374 6f72 6167 6557 6172 6e69 6e67 2c0a  StorageWarning,.
+00017930: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00017940: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00017950: 2020 2020 6465 6620 6672 6f6d 5f72 6573      def from_res
+00017960: 706f 6e73 655f 6a73 6f6e 2863 6c73 2c20  ponse_json(cls, 
+00017970: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
+00017980: 2020 2020 6a73 6f6e 5f64 6563 616d 656c      json_decamel
+00017990: 697a 6564 203d 2068 756d 7073 2e64 6563  ized = humps.dec
+000179a0: 616d 656c 697a 6528 6a73 6f6e 5f64 6963  amelize(json_dic
+000179b0: 7429 0a20 2020 2020 2020 2069 6620 6973  t).        if is
+000179c0: 696e 7374 616e 6365 286a 736f 6e5f 6465  instance(json_de
+000179d0: 6361 6d65 6c69 7a65 642c 2064 6963 7429  camelized, dict)
+000179e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000179f0: 2022 7479 7065 2220 696e 206a 736f 6e5f   "type" in json_
+00017a00: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
+00017a10: 2020 2020 2020 2020 2020 2020 206a 736f               jso
+00017a20: 6e5f 6465 6361 6d65 6c69 7a65 645b 2273  n_decamelized["s
+00017a30: 7472 6561 6d22 5d20 3d20 280a 2020 2020  tream"] = (.    
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a50: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+00017a60: 5b22 7479 7065 225d 203d 3d20 2273 7472  ["type"] == "str
+00017a70: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+00017a80: 544f 220a 2020 2020 2020 2020 2020 2020  TO".            
+00017a90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00017aa0: 2020 5f20 3d20 6a73 6f6e 5f64 6563 616d    _ = json_decam
+00017ab0: 656c 697a 6564 2e70 6f70 2822 7479 7065  elized.pop("type
+00017ac0: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00017ad0: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
+00017ae0: 6c69 7a65 642e 706f 7028 2276 616c 6964  lized.pop("valid
+00017af0: 6174 696f 6e5f 7479 7065 222c 204e 6f6e  ation_type", Non
+00017b00: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00017b10: 6574 7572 6e20 636c 7328 2a2a 6a73 6f6e  eturn cls(**json
+00017b20: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
+00017b30: 2020 2020 2020 666f 7220 6667 2069 6e20        for fg in 
+00017b40: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+00017b50: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00017b60: 2022 7479 7065 2220 696e 2066 673a 0a20   "type" in fg:. 
+00017b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017b80: 675b 2273 7472 6561 6d22 5d20 3d20 6667  g["stream"] = fg
+00017b90: 5b22 7479 7065 225d 203d 3d20 2273 7472  ["type"] == "str
+00017ba0: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+00017bb0: 544f 220a 2020 2020 2020 2020 2020 2020  TO".            
+00017bc0: 5f20 3d20 6667 2e70 6f70 2822 7479 7065  _ = fg.pop("type
+00017bd0: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00017be0: 2020 2020 2066 672e 706f 7028 2276 616c       fg.pop("val
+00017bf0: 6964 6174 696f 6e5f 7479 7065 222c 204e  idation_type", N
+00017c00: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
+00017c10: 7572 6e20 5b63 6c73 282a 2a66 6729 2066  urn [cls(**fg) f
+00017c20: 6f72 2066 6720 696e 206a 736f 6e5f 6465  or fg in json_de
+00017c30: 6361 6d65 6c69 7a65 645d 0a0a 2020 2020  camelized]..    
+00017c40: 6465 6620 7570 6461 7465 5f66 726f 6d5f  def update_from_
+00017c50: 7265 7370 6f6e 7365 5f6a 736f 6e28 7365  response_json(se
+00017c60: 6c66 2c20 6a73 6f6e 5f64 6963 7429 3a0a  lf, json_dict):.
+00017c70: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
+00017c80: 616d 656c 697a 6564 203d 2068 756d 7073  amelized = humps
+00017c90: 2e64 6563 616d 656c 697a 6528 6a73 6f6e  .decamelize(json
+00017ca0: 5f64 6963 7429 0a20 2020 2020 2020 206a  _dict).        j
+00017cb0: 736f 6e5f 6465 6361 6d65 6c69 7a65 645b  son_decamelized[
+00017cc0: 2273 7472 6561 6d22 5d20 3d20 6a73 6f6e  "stream"] = json
+00017cd0: 5f64 6563 616d 656c 697a 6564 5b22 7479  _decamelized["ty
+00017ce0: 7065 225d 203d 3d20 2273 7472 6561 6d46  pe"] == "streamF
+00017cf0: 6561 7475 7265 4772 6f75 7044 544f 220a  eatureGroupDTO".
+00017d00: 2020 2020 2020 2020 5f20 3d20 6a73 6f6e          _ = json
+00017d10: 5f64 6563 616d 656c 697a 6564 2e70 6f70  _decamelized.pop
+00017d20: 2822 7479 7065 2229 0a20 2020 2020 2020  ("type").       
+00017d30: 2073 656c 662e 5f5f 696e 6974 5f5f 282a   self.__init__(*
+00017d40: 2a6a 736f 6e5f 6465 6361 6d65 6c69 7a65  *json_decamelize
+00017d50: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
+00017d60: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
+00017d70: 6a73 6f6e 2873 656c 6629 3a0a 2020 2020  json(self):.    
+00017d80: 2020 2020 2222 2247 6574 2073 7065 6369      """Get speci
+00017d90: 6669 6320 4665 6174 7572 6520 4772 6f75  fic Feature Grou
+00017da0: 7020 6d65 7461 6461 7461 2069 6e20 6a73  p metadata in js
+00017db0: 6f6e 2066 6f72 6d61 742e 0a0a 2020 2020  on format...    
+00017dc0: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
+00017dd0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00017de0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00017df0: 2020 6667 2e6a 736f 6e28 290a 2020 2020    fg.json().    
+00017e00: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00017e10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017e20: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+00017e30: 7328 7365 6c66 2c20 636c 733d 7574 696c  s(self, cls=util
+00017e40: 2e46 6561 7475 7265 5374 6f72 6545 6e63  .FeatureStoreEnc
+00017e50: 6f64 6572 290a 0a20 2020 2064 6566 2074  oder)..    def t
+00017e60: 6f5f 6469 6374 2873 656c 6629 3a0a 2020  o_dict(self):.  
+00017e70: 2020 2020 2020 2222 2247 6574 2073 7472        """Get str
+00017e80: 7563 7475 7265 6420 696e 666f 2061 626f  uctured info abo
+00017e90: 7574 2073 7065 6369 6669 6320 4665 6174  ut specific Feat
+00017ea0: 7572 6520 4772 6f75 7020 696e 2070 7974  ure Group in pyt
+00017eb0: 686f 6e20 6469 6374 696f 6e61 7279 2066  hon dictionary f
+00017ec0: 6f72 6d61 742e 0a0a 2020 2020 2020 2020  ormat...        
+00017ed0: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
+00017ee0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00017ef0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+00017f00: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
+00017f10: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
+00017f20: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
+00017f30: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
+00017f40: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
+00017f50: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
+00017f60: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
+00017f70: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+00017f80: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+00017f90: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
+00017fa0: 2020 6667 2e74 6f5f 6469 6374 2829 0a20    fg.to_dict(). 
+00017fb0: 2020 2020 2020 2020 2020 2060 6060 0a20             ```. 
+00017fc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017fd0: 2020 2066 675f 6d65 7461 5f64 6963 7420     fg_meta_dict 
+00017fe0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00017ff0: 2269 6422 3a20 7365 6c66 2e5f 6964 2c0a  "id": self._id,.
+00018000: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00018010: 6522 3a20 7365 6c66 2e5f 6e61 6d65 2c0a  e": self._name,.
+00018020: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00018030: 7369 6f6e 223a 2073 656c 662e 5f76 6572  sion": self._ver
+00018040: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00018050: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00018060: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
+00018070: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00018080: 226f 6e6c 696e 6545 6e61 626c 6564 223a  "onlineEnabled":
+00018090: 2073 656c 662e 5f6f 6e6c 696e 655f 656e   self._online_en
+000180a0: 6162 6c65 642c 0a20 2020 2020 2020 2020  abled,.         
+000180b0: 2020 2022 7469 6d65 5472 6176 656c 466f     "timeTravelFo
+000180c0: 726d 6174 223a 2073 656c 662e 5f74 696d  rmat": self._tim
+000180d0: 655f 7472 6176 656c 5f66 6f72 6d61 742c  e_travel_format,
+000180e0: 0a20 2020 2020 2020 2020 2020 2022 6665  .            "fe
+000180f0: 6174 7572 6573 223a 2073 656c 662e 5f66  atures": self._f
+00018100: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
+00018110: 2020 2020 2022 6665 6174 7572 6573 746f       "featuresto
+00018120: 7265 4964 223a 2073 656c 662e 5f66 6561  reId": self._fea
+00018130: 7475 7265 5f73 746f 7265 5f69 642c 0a20  ture_store_id,. 
+00018140: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00018150: 223a 2022 6361 6368 6564 4665 6174 7572  ": "cachedFeatur
+00018160: 6567 726f 7570 4454 4f22 0a20 2020 2020  egroupDTO".     
+00018170: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00018180: 6c66 2e5f 7374 7265 616d 0a20 2020 2020  lf._stream.     
+00018190: 2020 2020 2020 2065 6c73 6520 2273 7472         else "str
+000181a0: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+000181b0: 544f 222c 0a20 2020 2020 2020 2020 2020  TO",.           
+000181c0: 2022 7374 6174 6973 7469 6373 436f 6e66   "statisticsConf
+000181d0: 6967 223a 2073 656c 662e 5f73 7461 7469  ig": self._stati
+000181e0: 7374 6963 735f 636f 6e66 6967 2c0a 2020  stics_config,.  
+000181f0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00018200: 5469 6d65 223a 2073 656c 662e 6576 656e  Time": self.even
+00018210: 745f 7469 6d65 2c0a 2020 2020 2020 2020  t_time,.        
+00018220: 2020 2020 2265 7870 6563 7461 7469 6f6e      "expectation
+00018230: 5375 6974 6522 3a20 7365 6c66 2e5f 6578  Suite": self._ex
+00018240: 7065 6374 6174 696f 6e5f 7375 6974 652c  pectation_suite,
+00018250: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
+00018260: 7265 6e74 7322 3a20 7365 6c66 2e5f 7061  rents": self._pa
+00018270: 7265 6e74 732c 0a20 2020 2020 2020 207d  rents,.        }
+00018280: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00018290: 2e5f 7374 7265 616d 3a0a 2020 2020 2020  ._stream:.      
+000182a0: 2020 2020 2020 6667 5f6d 6574 615f 6469        fg_meta_di
+000182b0: 6374 5b22 6465 6c74 6153 7472 6561 6d65  ct["deltaStreame
+000182c0: 724a 6f62 436f 6e66 225d 203d 2073 656c  rJobConf"] = sel
+000182d0: 662e 5f64 656c 7461 7374 7265 616d 6572  f._deltastreamer
+000182e0: 5f6a 6f62 636f 6e66 0a20 2020 2020 2020  _jobconf.       
+000182f0: 2072 6574 7572 6e20 6667 5f6d 6574 615f   return fg_meta_
+00018300: 6469 6374 0a0a 2020 2020 6465 6620 5f67  dict..    def _g
+00018310: 6574 5f74 6162 6c65 5f6e 616d 6528 7365  et_table_name(se
+00018320: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00018330: 7572 6e20 7365 6c66 2e66 6561 7475 7265  urn self.feature
+00018340: 5f73 746f 7265 5f6e 616d 6520 2b20 222e  _store_name + ".
+00018350: 2220 2b20 7365 6c66 2e6e 616d 6520 2b20  " + self.name + 
+00018360: 225f 2220 2b20 7374 7228 7365 6c66 2e76  "_" + str(self.v
+00018370: 6572 7369 6f6e 290a 0a20 2020 2064 6566  ersion)..    def
+00018380: 205f 6765 745f 6f6e 6c69 6e65 5f74 6162   _get_online_tab
+00018390: 6c65 5f6e 616d 6528 7365 6c66 293a 0a20  le_name(self):. 
+000183a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000183b0: 6c66 2e6e 616d 6520 2b20 225f 2220 2b20  lf.name + "_" + 
+000183c0: 7374 7228 7365 6c66 2e76 6572 7369 6f6e  str(self.version
+000183d0: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
+000183e0: 7072 6f6a 6563 745f 6e61 6d65 2873 656c  project_name(sel
+000183f0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00018400: 656c 662e 6665 6174 7572 655f 7374 6f72  elf.feature_stor
+00018410: 655f 6e61 6d65 2e65 6e64 7377 6974 6828  e_name.endswith(
+00018420: 225f 6665 6174 7572 6573 746f 7265 2229  "_featurestore")
+00018430: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00018440: 7475 726e 2073 656c 662e 6665 6174 7572  turn self.featur
+00018450: 655f 7374 6f72 655f 6e61 6d65 5b3a 2d31  e_store_name[:-1
+00018460: 335d 0a20 2020 2020 2020 2072 6574 7572  3].        retur
+00018470: 6e20 7365 6c66 2e66 6561 7475 7265 5f73  n self.feature_s
+00018480: 746f 7265 5f6e 616d 650a 0a20 2020 2040  tore_name..    @
+00018490: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000184a0: 2069 6428 7365 6c66 293a 0a20 2020 2020   id(self):.     
+000184b0: 2020 2022 2222 4665 6174 7572 6520 6772     """Feature gr
+000184c0: 6f75 7020 6964 2e22 2222 0a20 2020 2020  oup id.""".     
+000184d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000184e0: 6964 0a0a 2020 2020 4070 726f 7065 7274  id..    @propert
+000184f0: 790a 2020 2020 6465 6620 6e61 6d65 2873  y.    def name(s
+00018500: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00018510: 224e 616d 6520 6f66 2074 6865 2066 6561  "Name of the fea
+00018520: 7475 7265 2067 726f 7570 2e22 2222 0a20  ture group.""". 
+00018530: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00018540: 6c66 2e5f 6e61 6d65 0a0a 2020 2020 4070  lf._name..    @p
+00018550: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00018560: 7665 7273 696f 6e28 7365 6c66 293a 0a20  version(self):. 
+00018570: 2020 2020 2020 2022 2222 5665 7273 696f         """Versio
+00018580: 6e20 6e75 6d62 6572 206f 6620 7468 6520  n number of the 
+00018590: 6665 6174 7572 6520 6772 6f75 702e 2222  feature group.""
+000185a0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000185b0: 2073 656c 662e 5f76 6572 7369 6f6e 0a0a   self._version..
+000185c0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000185d0: 2020 6465 6620 6465 7363 7269 7074 696f    def descriptio
+000185e0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+000185f0: 2022 2222 4465 7363 7269 7074 696f 6e20   """Description 
+00018600: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+00018610: 726f 7570 2063 6f6e 7465 6e74 732e 2222  roup contents.""
+00018620: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00018630: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
+00018640: 6f6e 0a0a 2020 2020 4070 726f 7065 7274  on..    @propert
+00018650: 790a 2020 2020 6465 6620 7469 6d65 5f74  y.    def time_t
+00018660: 7261 7665 6c5f 666f 726d 6174 2873 656c  ravel_format(sel
+00018670: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
+00018680: 6574 7469 6e67 206f 6620 7468 6520 6665  etting of the fe
+00018690: 6174 7572 6520 6772 6f75 7020 7469 6d65  ature group time
+000186a0: 2074 7261 7665 6c20 666f 726d 6174 2e22   travel format."
+000186b0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000186c0: 6e20 7365 6c66 2e5f 7469 6d65 5f74 7261  n self._time_tra
+000186d0: 7665 6c5f 666f 726d 6174 0a0a 2020 2020  vel_format..    
+000186e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000186f0: 6620 7061 7274 6974 696f 6e5f 6b65 7928  f partition_key(
+00018700: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00018710: 2222 4c69 7374 206f 6620 6665 6174 7572  ""List of featur
+00018720: 6573 2062 7569 6c64 696e 6720 7468 6520  es building the 
+00018730: 7061 7274 6974 696f 6e20 6b65 792e 2222  partition key.""
+00018740: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00018750: 2073 656c 662e 5f70 6172 7469 7469 6f6e   self._partition
+00018760: 5f6b 6579 0a0a 2020 2020 4070 726f 7065  _key..    @prope
+00018770: 7274 790a 2020 2020 6465 6620 6875 6469  rty.    def hudi
+00018780: 5f70 7265 636f 6d62 696e 655f 6b65 7928  _precombine_key(
+00018790: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000187a0: 2222 4665 6174 7572 6520 6e61 6d65 2074  ""Feature name t
+000187b0: 6861 7420 6973 2074 6865 2068 7564 6920  hat is the hudi 
+000187c0: 7072 6563 6f6d 6269 6e65 206b 6579 2e22  precombine key."
+000187d0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000187e0: 6e20 7365 6c66 2e5f 6875 6469 5f70 7265  n self._hudi_pre
+000187f0: 636f 6d62 696e 655f 6b65 790a 0a20 2020  combine_key..   
+00018800: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00018810: 6566 2066 6561 7475 7265 5f73 746f 7265  ef feature_store
+00018820: 5f69 6428 7365 6c66 293a 0a20 2020 2020  _id(self):.     
+00018830: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00018840: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
+00018850: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00018860: 2020 2020 6465 6620 6665 6174 7572 655f      def feature_
+00018870: 7374 6f72 655f 6e61 6d65 2873 656c 6629  store_name(self)
+00018880: 3a0a 2020 2020 2020 2020 2222 224e 616d  :.        """Nam
+00018890: 6520 6f66 2074 6865 2066 6561 7475 7265  e of the feature
+000188a0: 2073 746f 7265 2069 6e20 7768 6963 6820   store in which 
+000188b0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+000188c0: 7020 6973 206c 6f63 6174 6564 2e22 2222  p is located."""
+000188d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000188e0: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
+000188f0: 6f72 655f 6e61 6d65 0a0a 2020 2020 4070  ore_name..    @p
+00018900: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00018910: 6372 6561 746f 7228 7365 6c66 293a 0a20  creator(self):. 
+00018920: 2020 2020 2020 2022 2222 5573 6572 6e61         """Userna
+00018930: 6d65 206f 6620 7468 6520 6372 6561 746f  me of the creato
+00018940: 722e 2222 220a 2020 2020 2020 2020 7265  r.""".        re
+00018950: 7475 726e 2073 656c 662e 5f63 7265 6174  turn self._creat
+00018960: 6f72 0a0a 2020 2020 4070 726f 7065 7274  or..    @propert
+00018970: 790a 2020 2020 6465 6620 6372 6561 7465  y.    def create
+00018980: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+00018990: 2022 2222 5469 6d65 7374 616d 7020 7768   """Timestamp wh
+000189a0: 656e 2074 6865 2066 6561 7475 7265 2067  en the feature g
+000189b0: 726f 7570 2077 6173 2063 7265 6174 6564  roup was created
+000189c0: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
+000189d0: 7572 6e20 7365 6c66 2e5f 6372 6561 7465  urn self._create
+000189e0: 640a 0a20 2020 2040 7072 6f70 6572 7479  d..    @property
+000189f0: 0a20 2020 2064 6566 2073 7472 6561 6d28  .    def stream(
+00018a00: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00018a10: 2222 5768 6574 6865 7220 746f 2065 6e61  ""Whether to ena
+00018a20: 626c 6520 7265 616c 2074 696d 6520 7374  ble real time st
+00018a30: 7265 616d 2077 7269 7469 6e67 2063 6170  ream writing cap
+00018a40: 6162 696c 6974 6965 732e 2222 220a 2020  abilities.""".  
+00018a50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00018a60: 662e 5f73 7472 6561 6d0a 0a20 2020 2040  f._stream..    @
+00018a70: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00018a80: 2070 6172 656e 7473 2873 656c 6629 3a0a   parents(self):.
+00018a90: 2020 2020 2020 2020 2222 2250 6172 656e          """Paren
+00018aa0: 7420 6665 6174 7572 6520 6772 6f75 7073  t feature groups
+00018ab0: 2061 7320 6f72 6967 696e 206f 6620 7468   as origin of th
+00018ac0: 6520 6461 7461 2069 6e20 7468 6520 6375  e data in the cu
+00018ad0: 7272 656e 7420 6665 6174 7572 6520 6772  rrent feature gr
+00018ae0: 6f75 702e 0a20 2020 2020 2020 2054 6869  oup..        Thi
+00018af0: 7320 6973 2070 6172 7420 6f66 2065 7870  s is part of exp
+00018b00: 6c69 6369 7420 7072 6f76 656e 616e 6365  licit provenance
+00018b10: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00018b20: 726e 2073 656c 662e 5f70 6172 656e 7473  rn self._parents
+00018b30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00018b40: 2020 2020 6465 6620 6261 636b 6669 6c6c      def backfill
+00018b50: 5f6a 6f62 2873 656c 6629 3a0a 2020 2020  _job(self):.    
+00018b60: 2020 2020 2222 2247 6574 2074 6865 204a      """Get the J
+00018b70: 6f62 206f 626a 6563 7420 7265 6665 7265  ob object refere
+00018b80: 6e63 6520 666f 7220 7468 6520 6261 636b  nce for the back
+00018b90: 6669 6c6c 206a 6f62 2066 6f72 2074 6869  fill job for thi
+00018ba0: 730a 2020 2020 2020 2020 4665 6174 7572  s.        Featur
+00018bb0: 6520 4772 6f75 702e 2222 220a 2020 2020  e Group.""".    
+00018bc0: 2020 2020 6966 2073 656c 662e 5f62 6163      if self._bac
+00018bd0: 6b66 696c 6c5f 6a6f 6220 6973 204e 6f6e  kfill_job is Non
+00018be0: 653a 0a20 2020 2020 2020 2020 2020 206a  e:.            j
+00018bf0: 6f62 5f6e 616d 6520 3d20 227b 6667 5f6e  ob_name = "{fg_n
+00018c00: 616d 657d 5f7b 7665 7273 696f 6e7d 5f6f  ame}_{version}_o
+00018c10: 6666 6c69 6e65 5f66 675f 6261 636b 6669  ffline_fg_backfi
+00018c20: 6c6c 222e 666f 726d 6174 280a 2020 2020  ll".format(.    
+00018c30: 2020 2020 2020 2020 2020 2020 6667 5f6e              fg_n
+00018c40: 616d 653d 7365 6c66 2e5f 6e61 6d65 2c20  ame=self._name, 
+00018c50: 7665 7273 696f 6e3d 7365 6c66 2e5f 7665  version=self._ve
+00018c60: 7273 696f 6e0a 2020 2020 2020 2020 2020  rsion.          
+00018c70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00018c80: 7365 6c66 2e5f 6261 636b 6669 6c6c 5f6a  self._backfill_j
+00018c90: 6f62 203d 206a 6f62 5f61 7069 2e4a 6f62  ob = job_api.Job
+00018ca0: 4170 6928 292e 6765 7428 6a6f 625f 6e61  Api().get(job_na
+00018cb0: 6d65 290a 2020 2020 2020 2020 7265 7475  me).        retu
+00018cc0: 726e 2073 656c 662e 5f62 6163 6b66 696c  rn self._backfil
+00018cd0: 6c5f 6a6f 620a 0a20 2020 2040 7665 7273  l_job..    @vers
+00018ce0: 696f 6e2e 7365 7474 6572 0a20 2020 2064  ion.setter.    d
+00018cf0: 6566 2076 6572 7369 6f6e 2873 656c 662c  ef version(self,
+00018d00: 2076 6572 7369 6f6e 293a 0a20 2020 2020   version):.     
+00018d10: 2020 2073 656c 662e 5f76 6572 7369 6f6e     self._version
+00018d20: 203d 2076 6572 7369 6f6e 0a0a 2020 2020   = version..    
+00018d30: 4064 6573 6372 6970 7469 6f6e 2e73 6574  @description.set
+00018d40: 7465 720a 2020 2020 6465 6620 6465 7363  ter.    def desc
+00018d50: 7269 7074 696f 6e28 7365 6c66 2c20 6e65  ription(self, ne
+00018d60: 775f 6465 7363 7269 7074 696f 6e29 3a0a  w_description):.
+00018d70: 2020 2020 2020 2020 7365 6c66 2e5f 6465          self._de
+00018d80: 7363 7269 7074 696f 6e20 3d20 6e65 775f  scription = new_
+00018d90: 6465 7363 7269 7074 696f 6e0a 0a20 2020  description..   
+00018da0: 2040 7469 6d65 5f74 7261 7665 6c5f 666f   @time_travel_fo
+00018db0: 726d 6174 2e73 6574 7465 720a 2020 2020  rmat.setter.    
+00018dc0: 6465 6620 7469 6d65 5f74 7261 7665 6c5f  def time_travel_
+00018dd0: 666f 726d 6174 2873 656c 662c 206e 6577  format(self, new
+00018de0: 5f74 696d 655f 7472 6176 656c 5f66 6f72  _time_travel_for
+00018df0: 6d61 7429 3a0a 2020 2020 2020 2020 7365  mat):.        se
+00018e00: 6c66 2e5f 7469 6d65 5f74 7261 7665 6c5f  lf._time_travel_
+00018e10: 666f 726d 6174 203d 206e 6577 5f74 696d  format = new_tim
+00018e20: 655f 7472 6176 656c 5f66 6f72 6d61 740a  e_travel_format.
+00018e30: 0a20 2020 2040 7061 7274 6974 696f 6e5f  .    @partition_
+00018e40: 6b65 792e 7365 7474 6572 0a20 2020 2064  key.setter.    d
+00018e50: 6566 2070 6172 7469 7469 6f6e 5f6b 6579  ef partition_key
+00018e60: 2873 656c 662c 206e 6577 5f70 6172 7469  (self, new_parti
+00018e70: 7469 6f6e 5f6b 6579 293a 0a20 2020 2020  tion_key):.     
+00018e80: 2020 2073 656c 662e 5f70 6172 7469 7469     self._partiti
+00018e90: 6f6e 5f6b 6579 203d 205b 706b 2e6c 6f77  on_key = [pk.low
+00018ea0: 6572 2829 2066 6f72 2070 6b20 696e 206e  er() for pk in n
+00018eb0: 6577 5f70 6172 7469 7469 6f6e 5f6b 6579  ew_partition_key
+00018ec0: 5d0a 0a20 2020 2040 6875 6469 5f70 7265  ]..    @hudi_pre
+00018ed0: 636f 6d62 696e 655f 6b65 792e 7365 7474  combine_key.sett
+00018ee0: 6572 0a20 2020 2064 6566 2068 7564 695f  er.    def hudi_
+00018ef0: 7072 6563 6f6d 6269 6e65 5f6b 6579 2873  precombine_key(s
+00018f00: 656c 662c 2068 7564 695f 7072 6563 6f6d  elf, hudi_precom
+00018f10: 6269 6e65 5f6b 6579 293a 0a20 2020 2020  bine_key):.     
+00018f20: 2020 2073 656c 662e 5f68 7564 695f 7072     self._hudi_pr
+00018f30: 6563 6f6d 6269 6e65 5f6b 6579 203d 2068  ecombine_key = h
+00018f40: 7564 695f 7072 6563 6f6d 6269 6e65 5f6b  udi_precombine_k
+00018f50: 6579 2e6c 6f77 6572 2829 0a0a 2020 2020  ey.lower()..    
+00018f60: 4073 7472 6561 6d2e 7365 7474 6572 0a20  @stream.setter. 
+00018f70: 2020 2064 6566 2073 7472 6561 6d28 7365     def stream(se
+00018f80: 6c66 2c20 7374 7265 616d 293a 0a20 2020  lf, stream):.   
+00018f90: 2020 2020 2073 656c 662e 5f73 7472 6561       self._strea
+00018fa0: 6d20 3d20 7374 7265 616d 0a0a 2020 2020  m = stream..    
+00018fb0: 4070 6172 656e 7473 2e73 6574 7465 720a  @parents.setter.
+00018fc0: 2020 2020 6465 6620 7061 7265 6e74 7328      def parents(
+00018fd0: 7365 6c66 2c20 6e65 775f 7061 7265 6e74  self, new_parent
+00018fe0: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+00018ff0: 2e5f 7061 7265 6e74 7320 3d20 6e65 775f  ._parents = new_
+00019000: 7061 7265 6e74 730a 0a0a 636c 6173 7320  parents...class 
+00019010: 4578 7465 726e 616c 4665 6174 7572 6547  ExternalFeatureG
+00019020: 726f 7570 2846 6561 7475 7265 4772 6f75  roup(FeatureGrou
+00019030: 7042 6173 6529 3a0a 2020 2020 4558 5445  pBase):.    EXTE
+00019040: 524e 414c 5f46 4541 5455 5245 5f47 524f  RNAL_FEATURE_GRO
+00019050: 5550 203d 2022 4f4e 5f44 454d 414e 445f  UP = "ON_DEMAND_
+00019060: 4645 4154 5552 455f 4752 4f55 5022 0a20  FEATURE_GROUP". 
+00019070: 2020 2045 4e54 4954 595f 5459 5045 203d     ENTITY_TYPE =
+00019080: 2022 6665 6174 7572 6567 726f 7570 7322   "featuregroups"
+00019090: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+000190a0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000190b0: 2c0a 2020 2020 2020 2020 7374 6f72 6167  ,.        storag
+000190c0: 655f 636f 6e6e 6563 746f 722c 0a20 2020  e_connector,.   
+000190d0: 2020 2020 2071 7565 7279 3d4e 6f6e 652c       query=None,
+000190e0: 0a20 2020 2020 2020 2064 6174 615f 666f  .        data_fo
+000190f0: 726d 6174 3d4e 6f6e 652c 0a20 2020 2020  rmat=None,.     
+00019100: 2020 2070 6174 683d 4e6f 6e65 2c0a 2020     path=None,.  
+00019110: 2020 2020 2020 6f70 7469 6f6e 733d 7b7d        options={}
+00019120: 2c0a 2020 2020 2020 2020 6e61 6d65 3d4e  ,.        name=N
+00019130: 6f6e 652c 0a20 2020 2020 2020 2076 6572  one,.        ver
+00019140: 7369 6f6e 3d4e 6f6e 652c 0a20 2020 2020  sion=None,.     
+00019150: 2020 2064 6573 6372 6970 7469 6f6e 3d4e     description=N
+00019160: 6f6e 652c 0a20 2020 2020 2020 2070 7269  one,.        pri
+00019170: 6d61 7279 5f6b 6579 3d4e 6f6e 652c 0a20  mary_key=None,. 
+00019180: 2020 2020 2020 2066 6561 7475 7265 7374         featurest
+00019190: 6f72 655f 6964 3d4e 6f6e 652c 0a20 2020  ore_id=None,.   
+000191a0: 2020 2020 2066 6561 7475 7265 7374 6f72       featurestor
+000191b0: 655f 6e61 6d65 3d4e 6f6e 652c 0a20 2020  e_name=None,.   
+000191c0: 2020 2020 2063 7265 6174 6564 3d4e 6f6e       created=Non
+000191d0: 652c 0a20 2020 2020 2020 2063 7265 6174  e,.        creat
+000191e0: 6f72 3d4e 6f6e 652c 0a20 2020 2020 2020  or=None,.       
+000191f0: 2069 643d 4e6f 6e65 2c0a 2020 2020 2020   id=None,.      
+00019200: 2020 6665 6174 7572 6573 3d4e 6f6e 652c    features=None,
+00019210: 0a20 2020 2020 2020 206c 6f63 6174 696f  .        locatio
+00019220: 6e3d 4e6f 6e65 2c0a 2020 2020 2020 2020  n=None,.        
+00019230: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+00019240: 673d 4e6f 6e65 2c0a 2020 2020 2020 2020  g=None,.        
+00019250: 6576 656e 745f 7469 6d65 3d4e 6f6e 652c  event_time=None,
+00019260: 0a20 2020 2020 2020 2065 7870 6563 7461  .        expecta
+00019270: 7469 6f6e 5f73 7569 7465 3d4e 6f6e 652c  tion_suite=None,
+00019280: 0a20 2020 2020 2020 206f 6e6c 696e 655f  .        online_
+00019290: 656e 6162 6c65 643d 4661 6c73 652c 0a20  enabled=False,. 
+000192a0: 2020 2020 2020 2068 7265 663d 4e6f 6e65         href=None
+000192b0: 2c0a 2020 2020 2020 2020 6f6e 6c69 6e65  ,.        online
+000192c0: 5f74 6f70 6963 5f6e 616d 653d 4e6f 6e65  _topic_name=None
+000192d0: 2c0a 2020 2020 2020 2020 7370 696e 653d  ,.        spine=
+000192e0: 4661 6c73 652c 0a20 2020 2029 3a0a 2020  False,.    ):.  
+000192f0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00019300: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00019310: 2020 2020 6665 6174 7572 6573 746f 7265      featurestore
+00019320: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00019330: 206c 6f63 6174 696f 6e2c 0a20 2020 2020   location,.     
+00019340: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
+00019350: 653d 6576 656e 745f 7469 6d65 2c0a 2020  e=event_time,.  
+00019360: 2020 2020 2020 2020 2020 6f6e 6c69 6e65            online
+00019370: 5f65 6e61 626c 6564 3d6f 6e6c 696e 655f  _enabled=online_
+00019380: 656e 6162 6c65 642c 0a20 2020 2020 2020  enabled,.       
+00019390: 2020 2020 2069 643d 6964 2c0a 2020 2020       id=id,.    
+000193a0: 2020 2020 2020 2020 6578 7065 6374 6174          expectat
+000193b0: 696f 6e5f 7375 6974 653d 6578 7065 6374  ion_suite=expect
+000193c0: 6174 696f 6e5f 7375 6974 652c 0a20 2020  ation_suite,.   
+000193d0: 2020 2020 2020 2020 206f 6e6c 696e 655f           online_
+000193e0: 746f 7069 635f 6e61 6d65 3d6f 6e6c 696e  topic_name=onlin
+000193f0: 655f 746f 7069 635f 6e61 6d65 2c0a 2020  e_topic_name,.  
+00019400: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00019410: 2073 656c 662e 5f66 6561 7475 7265 5f73   self._feature_s
+00019420: 746f 7265 5f6e 616d 6520 3d20 6665 6174  tore_name = feat
+00019430: 7572 6573 746f 7265 5f6e 616d 650a 2020  urestore_name.  
+00019440: 2020 2020 2020 7365 6c66 2e5f 6465 7363        self._desc
+00019450: 7269 7074 696f 6e20 3d20 6465 7363 7269  ription = descri
+00019460: 7074 696f 6e0a 2020 2020 2020 2020 7365  ption.        se
+00019470: 6c66 2e5f 6372 6561 7465 6420 3d20 6372  lf._created = cr
+00019480: 6561 7465 640a 2020 2020 2020 2020 7365  eated.        se
+00019490: 6c66 2e5f 6372 6561 746f 7220 3d20 7573  lf._creator = us
+000194a0: 6572 2e55 7365 722e 6672 6f6d 5f72 6573  er.User.from_res
+000194b0: 706f 6e73 655f 6a73 6f6e 2863 7265 6174  ponse_json(creat
+000194c0: 6f72 290a 2020 2020 2020 2020 7365 6c66  or).        self
+000194d0: 2e5f 7665 7273 696f 6e20 3d20 7665 7273  ._version = vers
+000194e0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+000194f0: 2e5f 6e61 6d65 203d 206e 616d 650a 2020  ._name = name.  
+00019500: 2020 2020 2020 7365 6c66 2e5f 7175 6572        self._quer
+00019510: 7920 3d20 7175 6572 790a 2020 2020 2020  y = query.      
+00019520: 2020 7365 6c66 2e5f 6461 7461 5f66 6f72    self._data_for
+00019530: 6d61 7420 3d20 6461 7461 5f66 6f72 6d61  mat = data_forma
+00019540: 742e 7570 7065 7228 2920 6966 2064 6174  t.upper() if dat
+00019550: 615f 666f 726d 6174 2065 6c73 6520 4e6f  a_format else No
+00019560: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00019570: 5f70 6174 6820 3d20 7061 7468 0a0a 2020  _path = path..  
+00019580: 2020 2020 2020 7365 6c66 2e5f 6665 6174        self._feat
+00019590: 7572 6573 203d 205b 0a20 2020 2020 2020  ures = [.       
+000195a0: 2020 2020 2066 6561 7475 7265 2e46 6561       feature.Fea
+000195b0: 7475 7265 2e66 726f 6d5f 7265 7370 6f6e  ture.from_respon
+000195c0: 7365 5f6a 736f 6e28 6665 6174 2920 6966  se_json(feat) if
+000195d0: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
+000195e0: 2c20 6469 6374 2920 656c 7365 2066 6561  , dict) else fea
+000195f0: 740a 2020 2020 2020 2020 2020 2020 666f  t.            fo
+00019600: 7220 6665 6174 2069 6e20 2866 6561 7475  r feat in (featu
+00019610: 7265 7320 6f72 205b 5d29 0a20 2020 2020  res or []).     
+00019620: 2020 205d 0a0a 2020 2020 2020 2020 7365     ]..        se
+00019630: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+00019640: 705f 656e 6769 6e65 203d 2028 0a20 2020  p_engine = (.   
+00019650: 2020 2020 2020 2020 2065 7874 6572 6e61           externa
+00019660: 6c5f 6665 6174 7572 655f 6772 6f75 705f  l_feature_group_
+00019670: 656e 6769 6e65 2e45 7874 6572 6e61 6c46  engine.ExternalF
+00019680: 6561 7475 7265 4772 6f75 7045 6e67 696e  eatureGroupEngin
+00019690: 6528 6665 6174 7572 6573 746f 7265 5f69  e(featurestore_i
+000196a0: 6429 0a20 2020 2020 2020 2029 0a0a 2020  d).        )..  
+000196b0: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
+000196c0: 643a 0a20 2020 2020 2020 2020 2020 2023  d:.            #
+000196d0: 2047 6f74 2066 726f 6d20 486f 7073 776f   Got from Hopswo
+000196e0: 726b 732c 2064 6573 6572 6961 6c69 7a65  rks, deserialize
+000196f0: 2066 6561 7475 7265 7320 616e 6420 7374   features and st
+00019700: 6f72 6167 6520 636f 6e6e 6563 746f 720a  orage connector.
+00019710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019720: 2e5f 6665 6174 7572 6573 203d 2028 0a20  ._features = (. 
+00019730: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00019740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019750: 2020 2020 2066 6561 7475 7265 2e46 6561       feature.Fea
+00019760: 7475 7265 2e66 726f 6d5f 7265 7370 6f6e  ture.from_respon
+00019770: 7365 5f6a 736f 6e28 6665 6174 290a 2020  se_json(feat).  
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000197a0: 6665 6174 2c20 6469 6374 290a 2020 2020  feat, dict).    
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 656c 7365 2066 6561 740a 2020 2020 2020  else feat.      
+000197d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000197e0: 7220 6665 6174 2069 6e20 6665 6174 7572  r feat in featur
+000197f0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00019800: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00019810: 2020 2020 2069 6620 6665 6174 7572 6573       if features
+00019820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019830: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00019840: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019850: 2020 2020 2073 656c 662e 7072 696d 6172       self.primar
+00019860: 795f 6b65 7920 3d20 280a 2020 2020 2020  y_key = (.      
+00019870: 2020 2020 2020 2020 2020 5b66 6561 742e            [feat.
+00019880: 6e61 6d65 2066 6f72 2066 6561 7420 696e  name for feat in
+00019890: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+000198a0: 6966 2066 6561 742e 7072 696d 6172 7920  if feat.primary 
+000198b0: 6973 2054 7275 655d 0a20 2020 2020 2020  is True].       
+000198c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000198d0: 2e5f 6665 6174 7572 6573 0a20 2020 2020  ._features.     
+000198e0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000198f0: 5b5d 0a20 2020 2020 2020 2020 2020 2029  [].            )
+00019900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019910: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
+00019920: 6669 6720 3d20 7374 6174 6973 7469 6373  fig = statistics
+00019930: 5f63 6f6e 6669 670a 0a20 2020 2020 2020  _config..       
+00019940: 2020 2020 2073 656c 662e 5f6f 7074 696f       self._optio
+00019950: 6e73 203d 2028 0a20 2020 2020 2020 2020  ns = (.         
+00019960: 2020 2020 2020 207b 6f70 7469 6f6e 5b22         {option["
+00019970: 6e61 6d65 225d 3a20 6f70 7469 6f6e 5b22  name"]: option["
+00019980: 7661 6c75 6522 5d20 666f 7220 6f70 7469  value"] for opti
+00019990: 6f6e 2069 6e20 6f70 7469 6f6e 737d 0a20  on in options}. 
+000199a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000199b0: 6620 6f70 7469 6f6e 730a 2020 2020 2020  f options.      
+000199c0: 2020 2020 2020 2020 2020 656c 7365 204e            else N
+000199d0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000199e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+000199f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019a00: 2e70 7269 6d61 7279 5f6b 6579 203d 2070  .primary_key = p
+00019a10: 7269 6d61 7279 5f6b 6579 0a20 2020 2020  rimary_key.     
+00019a20: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00019a30: 6973 7469 6373 5f63 6f6e 6669 6720 3d20  istics_config = 
+00019a40: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+00019a50: 670a 2020 2020 2020 2020 2020 2020 7365  g.            se
+00019a60: 6c66 2e5f 6665 6174 7572 6573 203d 2066  lf._features = f
+00019a70: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+00019a80: 2020 2020 7365 6c66 2e5f 6f70 7469 6f6e      self._option
+00019a90: 7320 3d20 6f70 7469 6f6e 730a 0a20 2020  s = options..   
+00019aa0: 2020 2020 2069 6620 7374 6f72 6167 655f       if storage_
+00019ab0: 636f 6e6e 6563 746f 7220 6973 206e 6f74  connector is not
+00019ac0: 204e 6f6e 6520 616e 6420 6973 696e 7374   None and isinst
+00019ad0: 616e 6365 2873 746f 7261 6765 5f63 6f6e  ance(storage_con
+00019ae0: 6e65 6374 6f72 2c20 6469 6374 293a 0a20  nector, dict):. 
+00019af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019b00: 5f73 746f 7261 6765 5f63 6f6e 6e65 6374  _storage_connect
+00019b10: 6f72 203d 2073 632e 5374 6f72 6167 6543  or = sc.StorageC
+00019b20: 6f6e 6e65 6374 6f72 2e66 726f 6d5f 7265  onnector.from_re
+00019b30: 7370 6f6e 7365 5f6a 736f 6e28 0a20 2020  sponse_json(.   
+00019b40: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00019b50: 7261 6765 5f63 6f6e 6e65 6374 6f72 0a20  rage_connector. 
+00019b60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00019b70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00019b80: 2020 2020 2020 2073 656c 662e 5f73 746f         self._sto
+00019b90: 7261 6765 5f63 6f6e 6e65 6374 6f72 203d  rage_connector =
+00019ba0: 2073 746f 7261 6765 5f63 6f6e 6e65 6374   storage_connect
+00019bb0: 6f72 0a0a 2020 2020 2020 2020 7365 6c66  or..        self
+00019bc0: 2e5f 6872 6566 203d 2068 7265 660a 0a20  ._href = href.. 
+00019bd0: 2020 2064 6566 2073 6176 6528 7365 6c66     def save(self
+00019be0: 293a 0a20 2020 2020 2020 2022 2222 5065  ):.        """Pe
+00019bf0: 7273 6973 7420 7468 6520 6d65 7461 6461  rsist the metada
+00019c00: 7461 2066 6f72 2074 6869 7320 6578 7465  ta for this exte
+00019c10: 726e 616c 2066 6561 7475 7265 2067 726f  rnal feature gro
+00019c20: 7570 2e0a 0a20 2020 2020 2020 2057 6974  up...        Wit
+00019c30: 686f 7574 2063 616c 6c69 6e67 2074 6869  hout calling thi
+00019c40: 7320 6d65 7468 6f64 2c20 796f 7572 2066  s method, your f
+00019c50: 6561 7475 7265 2067 726f 7570 2077 696c  eature group wil
+00019c60: 6c20 6f6e 6c79 2065 7869 7374 0a20 2020  l only exist.   
+00019c70: 2020 2020 2069 6e20 796f 7572 2050 7974       in your Pyt
+00019c80: 686f 6e20 4b65 726e 656c 2c20 6275 7420  hon Kernel, but 
+00019c90: 6e6f 7420 696e 2048 6f70 7377 6f72 6b73  not in Hopsworks
+00019ca0: 2e0a 0a20 2020 2020 2020 2060 6060 7079  ...        ```py
+00019cb0: 7468 6f6e 0a20 2020 2020 2020 2071 7565  thon.        que
+00019cc0: 7279 203d 2022 5345 4c45 4354 202a 2046  ry = "SELECT * F
+00019cd0: 524f 4d20 7361 6c65 7322 0a0a 2020 2020  ROM sales"..    
+00019ce0: 2020 2020 6667 203d 2066 6561 7475 7265      fg = feature
+00019cf0: 5f73 746f 7265 2e63 7265 6174 655f 6578  _store.create_ex
+00019d00: 7465 726e 616c 5f66 6561 7475 7265 5f67  ternal_feature_g
+00019d10: 726f 7570 286e 616d 653d 2273 616c 6573  roup(name="sales
+00019d20: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
+00019d30: 6572 7369 6f6e 3d31 2c0a 2020 2020 2020  ersion=1,.      
+00019d40: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00019d50: 6e3d 2250 6879 7369 6361 6c20 7368 6f70  n="Physical shop
+00019d60: 2073 616c 6573 2066 6561 7475 7265 7322   sales features"
+00019d70: 2c0a 2020 2020 2020 2020 2020 2020 7175  ,.            qu
+00019d80: 6572 793d 7175 6572 792c 0a20 2020 2020  ery=query,.     
+00019d90: 2020 2020 2020 2073 746f 7261 6765 5f63         storage_c
+00019da0: 6f6e 6e65 6374 6f72 3d63 6f6e 6e65 6374  onnector=connect
+00019db0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00019dc0: 7072 696d 6172 795f 6b65 793d 5b27 7373  primary_key=['ss
+00019dd0: 5f73 746f 7265 5f73 6b27 5d2c 0a20 2020  _store_sk'],.   
+00019de0: 2020 2020 2020 2020 2065 7665 6e74 5f74           event_t
+00019df0: 696d 653d 2773 616c 655f 6461 7465 270a  ime='sale_date'.
+00019e00: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019e10: 2020 2066 672e 7361 7665 2829 0a20 2020     fg.save().   
+00019e20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00019e30: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
+00019e40: 726f 7570 5f65 6e67 696e 652e 7361 7665  roup_engine.save
+00019e50: 2873 656c 6629 0a20 2020 2020 2020 2073  (self).        s
+00019e60: 656c 662e 5f63 6f64 655f 656e 6769 6e65  elf._code_engine
+00019e70: 2e73 6176 655f 636f 6465 2873 656c 6629  .save_code(self)
+00019e80: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00019e90: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
+00019ea0: 6669 672e 656e 6162 6c65 643a 0a20 2020  fig.enabled:.   
+00019eb0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00019ec0: 7461 7469 7374 6963 735f 656e 6769 6e65  tatistics_engine
+00019ed0: 2e63 6f6d 7075 7465 5f73 7461 7469 7374  .compute_statist
+00019ee0: 6963 7328 7365 6c66 290a 0a20 2020 2064  ics(self)..    d
+00019ef0: 6566 2069 6e73 6572 7428 0a20 2020 2020  ef insert(.     
+00019f00: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00019f10: 2066 6561 7475 7265 733a 2055 6e69 6f6e   features: Union
+00019f20: 5b0a 2020 2020 2020 2020 2020 2020 7064  [.            pd
+00019f30: 2e44 6174 6146 7261 6d65 2c0a 2020 2020  .DataFrame,.    
+00019f40: 2020 2020 2020 2020 5479 7065 5661 7228          TypeVar(
+00019f50: 2270 7973 7061 726b 2e73 716c 2e44 6174  "pyspark.sql.Dat
+00019f60: 6146 7261 6d65 2229 2c20 2023 206e 6f71  aFrame"),  # noq
+00019f70: 613a 2046 3832 310a 2020 2020 2020 2020  a: F821.        
+00019f80: 2020 2020 5479 7065 5661 7228 2270 7973      TypeVar("pys
+00019f90: 7061 726b 2e52 4444 2229 2c20 2023 206e  park.RDD"),  # n
+00019fa0: 6f71 613a 2046 3832 310a 2020 2020 2020  oqa: F821.      
+00019fb0: 2020 2020 2020 6e70 2e6e 6461 7272 6179        np.ndarray
+00019fc0: 2c0a 2020 2020 2020 2020 2020 2020 4c69  ,.            Li
+00019fd0: 7374 5b6c 6973 745d 2c0a 2020 2020 2020  st[list],.      
+00019fe0: 2020 5d2c 0a20 2020 2020 2020 2077 7269    ],.        wri
+00019ff0: 7465 5f6f 7074 696f 6e73 3a20 4f70 7469  te_options: Opti
+0001a000: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
+0001a010: 6e79 5d5d 203d 207b 7d2c 0a20 2020 2020  ny]] = {},.     
+0001a020: 2020 2076 616c 6964 6174 696f 6e5f 6f70     validation_op
+0001a030: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+0001a040: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
+0001a050: 3d20 7b7d 2c0a 2020 2020 2020 2020 7361  = {},.        sa
+0001a060: 7665 5f63 6f64 653a 204f 7074 696f 6e61  ve_code: Optiona
+0001a070: 6c5b 626f 6f6c 5d20 3d20 5472 7565 2c0a  l[bool] = True,.
+0001a080: 2020 2020 2020 2020 7761 6974 3a20 626f          wait: bo
+0001a090: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0001a0a0: 2920 2d3e 2054 7570 6c65 5b4f 7074 696f  ) -> Tuple[Optio
+0001a0b0: 6e61 6c5b 4a6f 625d 2c20 4f70 7469 6f6e  nal[Job], Option
+0001a0c0: 616c 5b56 616c 6964 6174 696f 6e52 6570  al[ValidationRep
+0001a0d0: 6f72 745d 5d3a 0a20 2020 2020 2020 2066  ort]]:.        f
+0001a0e0: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+0001a0f0: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
+0001a100: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
+0001a110: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
+0001a120: 6672 616d 6528 6665 6174 7572 6573 290a  frame(features).
+0001a130: 0a20 2020 2020 2020 2069 6620 7772 6974  .        if writ
+0001a140: 655f 6f70 7469 6f6e 7320 6973 204e 6f6e  e_options is Non
+0001a150: 653a 0a20 2020 2020 2020 2020 2020 2077  e:.            w
+0001a160: 7269 7465 5f6f 7074 696f 6e73 203d 207b  rite_options = {
+0001a170: 7d0a 2020 2020 2020 2020 6966 2022 7761  }.        if "wa
+0001a180: 6974 5f66 6f72 5f6a 6f62 2220 6e6f 7420  it_for_job" not 
+0001a190: 696e 2077 7269 7465 5f6f 7074 696f 6e73  in write_options
+0001a1a0: 3a0a 2020 2020 2020 2020 2020 2020 7772  :.            wr
+0001a1b0: 6974 655f 6f70 7469 6f6e 735b 2277 6169  ite_options["wai
+0001a1c0: 745f 666f 725f 6a6f 6222 5d20 3d20 7761  t_for_job"] = wa
+0001a1d0: 6974 0a0a 2020 2020 2020 2020 6a6f 622c  it..        job,
+0001a1e0: 2067 655f 7265 706f 7274 203d 2073 656c   ge_report = sel
+0001a1f0: 662e 5f66 6561 7475 7265 5f67 726f 7570  f._feature_group
+0001a200: 5f65 6e67 696e 652e 696e 7365 7274 280a  _engine.insert(.
+0001a210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a220: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
+0001a230: 6174 7572 655f 6461 7461 6672 616d 653d  ature_dataframe=
+0001a240: 6665 6174 7572 655f 6461 7461 6672 616d  feature_datafram
+0001a250: 652c 0a20 2020 2020 2020 2020 2020 2077  e,.            w
+0001a260: 7269 7465 5f6f 7074 696f 6e73 3d77 7269  rite_options=wri
+0001a270: 7465 5f6f 7074 696f 6e73 2c0a 2020 2020  te_options,.    
+0001a280: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+0001a290: 6f6e 5f6f 7074 696f 6e73 3d7b 2273 6176  on_options={"sav
+0001a2a0: 655f 7265 706f 7274 223a 2054 7275 652c  e_report": True,
+0001a2b0: 202a 2a76 616c 6964 6174 696f 6e5f 6f70   **validation_op
+0001a2c0: 7469 6f6e 737d 2c0a 2020 2020 2020 2020  tions},.        
+0001a2d0: 290a 0a20 2020 2020 2020 2069 6620 7361  )..        if sa
+0001a2e0: 7665 5f63 6f64 6520 616e 6420 280a 2020  ve_code and (.  
+0001a2f0: 2020 2020 2020 2020 2020 6765 5f72 6570            ge_rep
+0001a300: 6f72 7420 6973 204e 6f6e 6520 6f72 2067  ort is None or g
+0001a310: 655f 7265 706f 7274 2e69 6e67 6573 7469  e_report.ingesti
+0001a320: 6f6e 5f72 6573 756c 7420 3d3d 2022 494e  on_result == "IN
+0001a330: 4745 5354 4544 220a 2020 2020 2020 2020  GESTED".        
+0001a340: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0001a350: 656c 662e 5f63 6f64 655f 656e 6769 6e65  elf._code_engine
+0001a360: 2e73 6176 655f 636f 6465 2873 656c 6629  .save_code(self)
+0001a370: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0001a380: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
+0001a390: 6669 672e 656e 6162 6c65 643a 0a20 2020  fig.enabled:.   
+0001a3a0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0001a3b0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0001a3c0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+0001a3e0: 7461 7469 7374 6963 7320 6172 6520 6e6f  tatistics are no
+0001a3f0: 7420 636f 6d70 7574 6564 2066 6f72 2069  t computed for i
+0001a400: 6e73 6572 7469 6f6e 2074 6f20 6f6e 6c69  nsertion to onli
+0001a410: 6e65 2065 6e61 626c 6564 2065 7874 6572  ne enabled exter
+0001a420: 6e61 6c20 6665 6174 7572 6520 6772 6f75  nal feature grou
+0001a430: 7020 607b 7d60 2c20 7769 7468 2076 6572  p `{}`, with ver
+0001a440: 7369 6f6e 220a 2020 2020 2020 2020 2020  sion".          
+0001a450: 2020 2020 2020 2020 2020 2220 607b 7d60            " `{}`
+0001a460: 2e20 4361 6c6c 2060 636f 6d70 7574 655f  . Call `compute_
+0001a470: 7374 6174 6973 7469 6373 6020 6578 706c  statistics` expl
+0001a480: 6963 6974 6c79 2074 6f20 636f 6d70 7574  icitly to comput
+0001a490: 6520 7374 6174 6973 7469 6373 206f 7665  e statistics ove
+0001a4a0: 7220 7468 6520 6461 7461 2069 6e20 7468  r the data in th
+0001a4b0: 6520 6578 7465 726e 616c 2073 746f 7261  e external stora
+0001a4c0: 6765 2073 7973 7465 6d2e 220a 2020 2020  ge system.".    
+0001a4d0: 2020 2020 2020 2020 2020 2020 292e 666f              ).fo
+0001a4e0: 726d 6174 2873 656c 662e 5f6e 616d 652c  rmat(self._name,
+0001a4f0: 2073 656c 662e 5f76 6572 7369 6f6e 292c   self._version),
+0001a500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a510: 2075 7469 6c2e 5374 6f72 6167 6557 6172   util.StorageWar
+0001a520: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
+0001a530: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+0001a540: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+0001a550: 2020 6a6f 622c 0a20 2020 2020 2020 2020    job,.         
+0001a560: 2020 2067 655f 7265 706f 7274 2e74 6f5f     ge_report.to_
+0001a570: 6765 5f74 7970 6528 2920 6966 2067 655f  ge_type() if ge_
+0001a580: 7265 706f 7274 2069 7320 6e6f 7420 4e6f  report is not No
+0001a590: 6e65 2065 6c73 6520 4e6f 6e65 2c0a 2020  ne else None,.  
+0001a5a0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0001a5b0: 2072 6561 6428 0a20 2020 2020 2020 2073   read(.        s
+0001a5c0: 656c 662c 2064 6174 6166 7261 6d65 5f74  elf, dataframe_t
+0001a5d0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+0001a5e0: 725d 203d 2022 6465 6661 756c 7422 2c20  r] = "default", 
+0001a5f0: 6f6e 6c69 6e65 3a20 4f70 7469 6f6e 616c  online: Optional
+0001a600: 5b62 6f6f 6c5d 203d 2046 616c 7365 0a20  [bool] = False. 
+0001a610: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0001a620: 2247 6574 2074 6865 2066 6561 7475 7265  "Get the feature
+0001a630: 2067 726f 7570 2061 7320 6120 4461 7461   group as a Data
+0001a640: 4672 616d 652e 0a0a 2020 2020 2020 2020  Frame...        
+0001a650: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
+0001a660: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+0001a670: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+0001a680: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
+0001a690: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
+0001a6a0: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
+0001a6b0: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
+0001a6c0: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
+0001a6d0: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
+0001a6e0: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
+0001a6f0: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+0001a700: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+0001a710: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
+0001a720: 2020 6466 203d 2066 672e 7265 6164 2829    df = fg.read()
+0001a730: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+0001a740: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
+0001a750: 726e 696e 6720 2245 6e67 696e 6520 5375  rning "Engine Su
+0001a760: 7070 6f72 7422 0a20 2020 2020 2020 2020  pport".         
+0001a770: 2020 202a 2a53 7061 726b 206f 6e6c 792a     **Spark only*
+0001a780: 2a0a 0a20 2020 2020 2020 2020 2020 2052  *..            R
+0001a790: 6561 6469 6e67 2061 6e20 4578 7465 726e  eading an Extern
+0001a7a0: 616c 2046 6561 7475 7265 2047 726f 7570  al Feature Group
+0001a7b0: 2064 6972 6563 746c 7920 696e 746f 2061   directly into a
+0001a7c0: 2050 616e 6461 7320 4461 7461 6672 616d   Pandas Datafram
+0001a7d0: 6520 7573 696e 670a 2020 2020 2020 2020  e using.        
+0001a7e0: 2020 2020 5079 7468 6f6e 2f50 616e 6461      Python/Panda
+0001a7f0: 7320 6173 2045 6e67 696e 6520 6973 206e  s as Engine is n
+0001a800: 6f74 2073 7570 706f 7274 6564 2c20 686f  ot supported, ho
+0001a810: 7765 7665 722c 2079 6f75 2063 616e 2075  wever, you can u
+0001a820: 7365 2074 6865 0a20 2020 2020 2020 2020  se the.         
+0001a830: 2020 2051 7565 7279 2041 5049 2074 6f20     Query API to 
+0001a840: 6372 6561 7465 2046 6561 7475 7265 2056  create Feature V
+0001a850: 6965 7773 2f54 7261 696e 696e 6720 4461  iews/Training Da
+0001a860: 7461 2063 6f6e 7461 696e 696e 6720 4578  ta containing Ex
+0001a870: 7465 726e 616c 0a20 2020 2020 2020 2020  ternal.         
+0001a880: 2020 2046 6561 7475 7265 2047 726f 7570     Feature Group
+0001a890: 732e 0a0a 2020 2020 2020 2020 2320 4172  s...        # Ar
+0001a8a0: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+0001a8b0: 2020 2020 6461 7461 6672 616d 655f 7479      dataframe_ty
+0001a8c0: 7065 3a20 7374 722c 206f 7074 696f 6e61  pe: str, optiona
+0001a8d0: 6c2e 2050 6f73 7369 626c 6520 7661 6c75  l. Possible valu
+0001a8e0: 6573 2061 7265 2060 2264 6566 6175 6c74  es are `"default
+0001a8f0: 2260 2c20 6022 7370 6172 6b22 602c 0a20  "`, `"spark"`,. 
+0001a900: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0001a910: 2270 616e 6461 7322 602c 2060 226e 756d  "pandas"`, `"num
+0001a920: 7079 2260 206f 7220 6022 7079 7468 6f6e  py"` or `"python
+0001a930: 2260 2c20 6465 6661 756c 7473 2074 6f20  "`, defaults to 
+0001a940: 6022 6465 6661 756c 7422 602e 0a20 2020  `"default"`..   
+0001a950: 2020 2020 2020 2020 206f 6e6c 696e 653a           online:
+0001a960: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c2e   bool, optional.
+0001a970: 2049 6620 6054 7275 6560 2072 6561 6420   If `True` read 
+0001a980: 6672 6f6d 206f 6e6c 696e 6520 6665 6174  from online feat
+0001a990: 7572 6520 7374 6f72 652c 2064 6566 6175  ure store, defau
+0001a9a0: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
+0001a9b0: 2020 2020 746f 2060 4661 6c73 6560 2e0a      to `False`..
+0001a9c0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+0001a9d0: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+0001a9e0: 4461 7461 4672 616d 6560 3a20 5468 6520  DataFrame`: The 
+0001a9f0: 7370 6172 6b20 6461 7461 6672 616d 6520  spark dataframe 
+0001aa00: 636f 6e74 6169 6e69 6e67 2074 6865 2066  containing the f
+0001aa10: 6561 7475 7265 2064 6174 612e 0a20 2020  eature data..   
+0001aa20: 2020 2020 2020 2020 2060 7079 7370 6172           `pyspar
+0001aa30: 6b2e 4461 7461 4672 616d 6560 2e20 4120  k.DataFrame`. A 
+0001aa40: 5370 6172 6b20 4461 7461 4672 616d 652e  Spark DataFrame.
+0001aa50: 0a20 2020 2020 2020 2020 2020 2060 7061  .            `pa
+0001aa60: 6e64 6173 2e44 6174 6146 7261 6d65 602e  ndas.DataFrame`.
+0001aa70: 2041 2050 616e 6461 7320 4461 7461 4672   A Pandas DataFr
+0001aa80: 616d 652e 0a20 2020 2020 2020 2020 2020  ame..           
+0001aa90: 2060 6e75 6d70 792e 6e64 6172 7261 7960   `numpy.ndarray`
+0001aaa0: 2e20 4120 7477 6f2d 6469 6d65 6e73 696f  . A two-dimensio
+0001aab0: 6e61 6c20 4e75 6d70 7920 6172 7261 792e  nal Numpy array.
+0001aac0: 0a20 2020 2020 2020 2020 2020 2060 6c69  .            `li
+0001aad0: 7374 602e 2041 2074 776f 2d64 696d 656e  st`. A two-dimen
+0001aae0: 7369 6f6e 616c 2050 7974 686f 6e20 6c69  sional Python li
+0001aaf0: 7374 2e0a 0a20 2020 2020 2020 2023 2052  st...        # R
+0001ab00: 6169 7365 730a 2020 2020 2020 2020 2020  aises.          
+0001ab10: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
+0001ab20: 7863 6570 7469 6f6e 732e 5265 7374 4150  xceptions.RestAP
+0001ab30: 4945 7272 6f72 602e 0a20 2020 2020 2020  IError`..       
+0001ab40: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0001ab50: 656e 6769 6e65 2e67 6574 5f74 7970 6528  engine.get_type(
+0001ab60: 2920 3d3d 2022 7079 7468 6f6e 2220 616e  ) == "python" an
+0001ab70: 6420 6e6f 7420 6f6e 6c69 6e65 3a0a 2020  d not online:.  
+0001ab80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001ab90: 4665 6174 7572 6553 746f 7265 4578 6365  FeatureStoreExce
+0001aba0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
+0001abb0: 2020 2020 2020 2022 5265 6164 696e 6720         "Reading 
+0001abc0: 616e 2045 7874 6572 6e61 6c20 4665 6174  an External Feat
+0001abd0: 7572 6520 4772 6f75 7020 6469 7265 6374  ure Group direct
+0001abe0: 6c79 2069 6e74 6f20 6120 5061 6e64 6173  ly into a Pandas
+0001abf0: 2044 6174 6166 7261 6d65 2075 7369 6e67   Dataframe using
+0001ac00: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0001ac10: 2020 202b 2022 5079 7468 6f6e 2f50 616e     + "Python/Pan
+0001ac20: 6461 7320 6173 2045 6e67 696e 6520 6672  das as Engine fr
+0001ac30: 6f6d 2074 6865 2065 7874 6572 6e61 6c20  om the external 
+0001ac40: 7374 6f72 6167 6520 7379 7374 656d 2022  storage system "
+0001ac50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ac60: 202b 2022 6973 206e 6f74 2073 7570 706f   + "is not suppo
+0001ac70: 7274 6564 2c20 686f 7765 7665 722c 2069  rted, however, i
+0001ac80: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+0001ac90: 6f75 7020 6973 206f 6e6c 696e 6520 656e  oup is online en
+0001aca0: 6162 6c65 642c 2079 6f75 2063 616e 2072  abled, you can r
+0001acb0: 6561 6420 220a 2020 2020 2020 2020 2020  ead ".          
+0001acc0: 2020 2020 2020 2b20 2266 726f 6d20 6f6e        + "from on
+0001acd0: 6c69 6e65 2073 746f 7261 6765 206f 7220  line storage or 
+0001ace0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
+0001acf0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001ad00: 2020 2b20 2251 7565 7279 2041 5049 2074    + "Query API t
+0001ad10: 6f20 6372 6561 7465 2046 6561 7475 7265  o create Feature
+0001ad20: 2056 6965 7773 2f54 7261 696e 696e 6720   Views/Training 
+0001ad30: 4461 7461 2063 6f6e 7461 696e 696e 6720  Data containing 
+0001ad40: 4578 7465 726e 616c 2022 0a20 2020 2020  External ".     
+0001ad50: 2020 2020 2020 2020 2020 202b 2022 4665             + "Fe
+0001ad60: 6174 7572 6520 4772 6f75 7073 2e22 0a20  ature Groups.". 
+0001ad70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001ad80: 2020 2020 2065 6e67 696e 652e 6765 745f       engine.get_
+0001ad90: 696e 7374 616e 6365 2829 2e73 6574 5f6a  instance().set_j
+0001ada0: 6f62 5f67 726f 7570 280a 2020 2020 2020  ob_group(.      
+0001adb0: 2020 2020 2020 2246 6574 6368 696e 6720        "Fetching 
+0001adc0: 4665 6174 7572 6520 6772 6f75 7022 2c0a  Feature group",.
+0001add0: 2020 2020 2020 2020 2020 2020 2247 6574              "Get
+0001ade0: 7469 6e67 2066 6561 7475 7265 2067 726f  ting feature gro
+0001adf0: 7570 3a20 7b7d 2066 726f 6d20 7468 6520  up: {} from the 
+0001ae00: 6665 6174 7572 6573 746f 7265 207b 7d22  featurestore {}"
+0001ae10: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+0001ae20: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+0001ae30: 616d 652c 2073 656c 662e 5f66 6561 7475  ame, self._featu
+0001ae40: 7265 5f73 746f 7265 5f6e 616d 650a 2020  re_store_name.  
+0001ae50: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+0001ae60: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0001ae70: 6574 7572 6e20 7365 6c66 2e73 656c 6563  eturn self.selec
+0001ae80: 745f 616c 6c28 292e 7265 6164 2864 6174  t_all().read(dat
+0001ae90: 6166 7261 6d65 5f74 7970 653d 6461 7461  aframe_type=data
+0001aea0: 6672 616d 655f 7479 7065 2c20 6f6e 6c69  frame_type, onli
+0001aeb0: 6e65 3d6f 6e6c 696e 6529 0a0a 2020 2020  ne=online)..    
+0001aec0: 6465 6620 7368 6f77 2873 656c 662c 206e  def show(self, n
+0001aed0: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
+0001aee0: 6f77 2074 6865 2066 6972 7374 206e 2072  ow the first n r
+0001aef0: 6f77 7320 6f66 2074 6865 2066 6561 7475  ows of the featu
+0001af00: 7265 2067 726f 7570 2e0a 0a20 2020 2020  re group...     
+0001af10: 2020 2021 2121 2065 7861 6d70 6c65 0a20     !!! example. 
+0001af20: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
+0001af30: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
+0001af40: 2023 2063 6f6e 6e65 6374 2074 6f20 7468   # connect to th
+0001af50: 6520 4665 6174 7572 6520 5374 6f72 650a  e Feature Store.
+0001af60: 2020 2020 2020 2020 2020 2020 6673 203d              fs =
+0001af70: 202e 2e2e 0a0a 2020 2020 2020 2020 2020   .....          
+0001af80: 2020 2320 6765 7420 7468 6520 4665 6174    # get the Feat
+0001af90: 7572 6520 4772 6f75 7020 696e 7374 616e  ure Group instan
+0001afa0: 6365 0a20 2020 2020 2020 2020 2020 2066  ce.            f
+0001afb0: 6720 3d20 6673 2e67 6574 5f6f 725f 6372  g = fs.get_or_cr
+0001afc0: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
+0001afd0: 7570 282e 2e2e 290a 0a20 2020 2020 2020  up(...)..       
+0001afe0: 2020 2020 2066 672e 7368 6f77 2835 290a       fg.show(5).
+0001aff0: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+0001b000: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001b010: 2020 2020 656e 6769 6e65 2e67 6574 5f69      engine.get_i
+0001b020: 6e73 7461 6e63 6528 292e 7365 745f 6a6f  nstance().set_jo
+0001b030: 625f 6772 6f75 7028 0a20 2020 2020 2020  b_group(.       
+0001b040: 2020 2020 2022 4665 7463 6869 6e67 2046       "Fetching F
+0001b050: 6561 7475 7265 2067 726f 7570 222c 0a20  eature group",. 
+0001b060: 2020 2020 2020 2020 2020 2022 4765 7474             "Gett
+0001b070: 696e 6720 6665 6174 7572 6520 6772 6f75  ing feature grou
+0001b080: 703a 207b 7d20 6672 6f6d 2074 6865 2066  p: {} from the f
+0001b090: 6561 7475 7265 7374 6f72 6520 7b7d 222e  eaturestore {}".
+0001b0a0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+0001b0b0: 2020 2020 2020 2020 7365 6c66 2e5f 6e61          self._na
+0001b0c0: 6d65 2c20 7365 6c66 2e5f 6665 6174 7572  me, self._featur
+0001b0d0: 655f 7374 6f72 655f 6e61 6d65 0a20 2020  e_store_name.   
+0001b0e0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+0001b0f0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0001b100: 7475 726e 2073 656c 662e 7365 6c65 6374  turn self.select
+0001b110: 5f61 6c6c 2829 2e73 686f 7728 6e29 0a0a  _all().show(n)..
+0001b120: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+0001b130: 0a20 2020 2064 6566 2066 726f 6d5f 7265  .    def from_re
+0001b140: 7370 6f6e 7365 5f6a 736f 6e28 636c 732c  sponse_json(cls,
+0001b150: 206a 736f 6e5f 6469 6374 293a 0a20 2020   json_dict):.   
+0001b160: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
+0001b170: 6c69 7a65 6420 3d20 6875 6d70 732e 6465  lized = humps.de
+0001b180: 6361 6d65 6c69 7a65 286a 736f 6e5f 6469  camelize(json_di
+0001b190: 6374 290a 2020 2020 2020 2020 6966 2069  ct).        if i
+0001b1a0: 7369 6e73 7461 6e63 6528 6a73 6f6e 5f64  sinstance(json_d
+0001b1b0: 6563 616d 656c 697a 6564 2c20 6469 6374  ecamelized, dict
+0001b1c0: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+0001b1d0: 203d 206a 736f 6e5f 6465 6361 6d65 6c69   = json_decameli
+0001b1e0: 7a65 642e 706f 7028 2274 7970 6522 2c20  zed.pop("type", 
+0001b1f0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
+0001b200: 2020 7265 7475 726e 2063 6c73 282a 2a6a    return cls(**j
+0001b210: 736f 6e5f 6465 6361 6d65 6c69 7a65 6429  son_decamelized)
+0001b220: 0a20 2020 2020 2020 2066 6f72 2066 6720  .        for fg 
+0001b230: 696e 206a 736f 6e5f 6465 6361 6d65 6c69  in json_decameli
+0001b240: 7a65 643a 0a20 2020 2020 2020 2020 2020  zed:.           
+0001b250: 205f 203d 2066 672e 706f 7028 2274 7970   _ = fg.pop("typ
+0001b260: 6522 2c20 4e6f 6e65 290a 2020 2020 2020  e", None).      
+0001b270: 2020 7265 7475 726e 205b 636c 7328 2a2a    return [cls(**
+0001b280: 6667 2920 666f 7220 6667 2069 6e20 6a73  fg) for fg in js
+0001b290: 6f6e 5f64 6563 616d 656c 697a 6564 5d0a  on_decamelized].
+0001b2a0: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
+0001b2b0: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
+0001b2c0: 6f6e 2873 656c 662c 206a 736f 6e5f 6469  on(self, json_di
+0001b2d0: 6374 293a 0a20 2020 2020 2020 206a 736f  ct):.        jso
+0001b2e0: 6e5f 6465 6361 6d65 6c69 7a65 6420 3d20  n_decamelized = 
+0001b2f0: 6875 6d70 732e 6465 6361 6d65 6c69 7a65  humps.decamelize
+0001b300: 286a 736f 6e5f 6469 6374 290a 2020 2020  (json_dict).    
+0001b310: 2020 2020 6966 2022 7479 7065 2220 696e      if "type" in
+0001b320: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001b330: 643a 0a20 2020 2020 2020 2020 2020 205f  d:.            _
+0001b340: 203d 206a 736f 6e5f 6465 6361 6d65 6c69   = json_decameli
+0001b350: 7a65 642e 706f 7028 2274 7970 6522 290a  zed.pop("type").
+0001b360: 2020 2020 2020 2020 7365 6c66 2e5f 5f69          self.__i
+0001b370: 6e69 745f 5f28 2a2a 6a73 6f6e 5f64 6563  nit__(**json_dec
+0001b380: 616d 656c 697a 6564 290a 2020 2020 2020  amelized).      
+0001b390: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+0001b3a0: 2020 2064 6566 206a 736f 6e28 7365 6c66     def json(self
+0001b3b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001b3c0: 6e20 6a73 6f6e 2e64 756d 7073 2873 656c  n json.dumps(sel
+0001b3d0: 662c 2063 6c73 3d75 7469 6c2e 4665 6174  f, cls=util.Feat
+0001b3e0: 7572 6553 746f 7265 456e 636f 6465 7229  ureStoreEncoder)
+0001b3f0: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
+0001b400: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001b410: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
+0001b420: 2020 2020 2020 2269 6422 3a20 7365 6c66        "id": self
+0001b430: 2e5f 6964 2c0a 2020 2020 2020 2020 2020  ._id,.          
+0001b440: 2020 226e 616d 6522 3a20 7365 6c66 2e5f    "name": self._
+0001b450: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+0001b460: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+0001b470: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
+0001b480: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0001b490: 2276 6572 7369 6f6e 223a 2073 656c 662e  "version": self.
+0001b4a0: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
+0001b4b0: 2020 2020 2020 2266 6561 7475 7265 7322        "features"
+0001b4c0: 3a20 7365 6c66 2e5f 6665 6174 7572 6573  : self._features
+0001b4d0: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
+0001b4e0: 6561 7475 7265 7374 6f72 6549 6422 3a20  eaturestoreId": 
+0001b4f0: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
+0001b500: 6f72 655f 6964 2c0a 2020 2020 2020 2020  ore_id,.        
+0001b510: 2020 2020 2271 7565 7279 223a 2073 656c      "query": sel
+0001b520: 662e 5f71 7565 7279 2c0a 2020 2020 2020  f._query,.      
+0001b530: 2020 2020 2020 2264 6174 6146 6f72 6d61        "dataForma
+0001b540: 7422 3a20 7365 6c66 2e5f 6461 7461 5f66  t": self._data_f
+0001b550: 6f72 6d61 742c 0a20 2020 2020 2020 2020  ormat,.         
+0001b560: 2020 2022 7061 7468 223a 2073 656c 662e     "path": self.
+0001b570: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0001b580: 2020 2022 6f70 7469 6f6e 7322 3a20 5b7b     "options": [{
+0001b590: 226e 616d 6522 3a20 6b2c 2022 7661 6c75  "name": k, "valu
+0001b5a0: 6522 3a20 767d 2066 6f72 206b 2c20 7620  e": v} for k, v 
+0001b5b0: 696e 2073 656c 662e 5f6f 7074 696f 6e73  in self._options
+0001b5c0: 2e69 7465 6d73 2829 5d0a 2020 2020 2020  .items()].      
+0001b5d0: 2020 2020 2020 6966 2073 656c 662e 5f6f        if self._o
+0001b5e0: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
+0001b5f0: 2020 2065 6c73 6520 4e6f 6e65 2c0a 2020     else None,.  
+0001b600: 2020 2020 2020 2020 2020 2273 746f 7261            "stora
+0001b610: 6765 436f 6e6e 6563 746f 7222 3a20 7365  geConnector": se
+0001b620: 6c66 2e5f 7374 6f72 6167 655f 636f 6e6e  lf._storage_conn
+0001b630: 6563 746f 722e 746f 5f64 6963 7428 292c  ector.to_dict(),
+0001b640: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+0001b650: 7065 223a 2022 6f6e 4465 6d61 6e64 4665  pe": "onDemandFe
+0001b660: 6174 7572 6567 726f 7570 4454 4f22 2c0a  aturegroupDTO",.
+0001b670: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+0001b680: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
+0001b690: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
+0001b6a0: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
+0001b6b0: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
+0001b6c0: 3a20 7365 6c66 2e5f 6576 656e 745f 7469  : self._event_ti
+0001b6d0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0001b6e0: 2265 7870 6563 7461 7469 6f6e 5375 6974  "expectationSuit
+0001b6f0: 6522 3a20 7365 6c66 2e5f 6578 7065 6374  e": self._expect
+0001b700: 6174 696f 6e5f 7375 6974 652c 0a20 2020  ation_suite,.   
+0001b710: 2020 2020 2020 2020 2022 6f6e 6c69 6e65           "online
+0001b720: 456e 6162 6c65 6422 3a20 7365 6c66 2e5f  Enabled": self._
+0001b730: 6f6e 6c69 6e65 5f65 6e61 626c 6564 2c0a  online_enabled,.
+0001b740: 2020 2020 2020 2020 2020 2020 2273 7069              "spi
+0001b750: 6e65 223a 2046 616c 7365 2c0a 2020 2020  ne": False,.    
+0001b760: 2020 2020 7d0a 0a20 2020 2040 7072 6f70      }..    @prop
+0001b770: 6572 7479 0a20 2020 2064 6566 2069 6428  erty.    def id(
+0001b780: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001b790: 6574 7572 6e20 7365 6c66 2e5f 6964 0a0a  eturn self._id..
+0001b7a0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001b7b0: 2020 6465 6620 6e61 6d65 2873 656c 6629    def name(self)
+0001b7c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001b7d0: 2073 656c 662e 5f6e 616d 650a 0a20 2020   self._name..   
+0001b7e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0001b7f0: 6566 2076 6572 7369 6f6e 2873 656c 6629  ef version(self)
+0001b800: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001b810: 2073 656c 662e 5f76 6572 7369 6f6e 0a0a   self._version..
+0001b820: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001b830: 2020 6465 6620 6465 7363 7269 7074 696f    def descriptio
+0001b840: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+0001b850: 2072 6574 7572 6e20 7365 6c66 2e5f 6465   return self._de
+0001b860: 7363 7269 7074 696f 6e0a 0a20 2020 2040  scription..    @
+0001b870: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001b880: 2071 7565 7279 2873 656c 6629 3a0a 2020   query(self):.  
+0001b890: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001b8a0: 662e 5f71 7565 7279 0a0a 2020 2020 4070  f._query..    @p
+0001b8b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0001b8c0: 6461 7461 5f66 6f72 6d61 7428 7365 6c66  data_format(self
+0001b8d0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001b8e0: 6e20 7365 6c66 2e5f 6461 7461 5f66 6f72  n self._data_for
+0001b8f0: 6d61 740a 0a20 2020 2040 7072 6f70 6572  mat..    @proper
+0001b900: 7479 0a20 2020 2064 6566 2070 6174 6828  ty.    def path(
+0001b910: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001b920: 6574 7572 6e20 7365 6c66 2e5f 7061 7468  eturn self._path
+0001b930: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0001b940: 2020 2020 6465 6620 6f70 7469 6f6e 7328      def options(
+0001b950: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001b960: 6574 7572 6e20 7365 6c66 2e5f 6f70 7469  eturn self._opti
+0001b970: 6f6e 730a 0a20 2020 2040 7072 6f70 6572  ons..    @proper
+0001b980: 7479 0a20 2020 2064 6566 2073 746f 7261  ty.    def stora
+0001b990: 6765 5f63 6f6e 6e65 6374 6f72 2873 656c  ge_connector(sel
+0001b9a0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0001b9b0: 726e 2073 656c 662e 5f73 746f 7261 6765  rn self._storage
+0001b9c0: 5f63 6f6e 6e65 6374 6f72 0a0a 2020 2020  _connector..    
+0001b9d0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001b9e0: 6620 6372 6561 746f 7228 7365 6c66 293a  f creator(self):
+0001b9f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001ba00: 7365 6c66 2e5f 6372 6561 746f 720a 0a20  self._creator.. 
+0001ba10: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0001ba20: 2064 6566 2063 7265 6174 6564 2873 656c   def created(sel
+0001ba30: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0001ba40: 726e 2073 656c 662e 5f63 7265 6174 6564  rn self._created
+0001ba50: 0a0a 2020 2020 4076 6572 7369 6f6e 2e73  ..    @version.s
+0001ba60: 6574 7465 720a 2020 2020 6465 6620 7665  etter.    def ve
+0001ba70: 7273 696f 6e28 7365 6c66 2c20 7665 7273  rsion(self, vers
+0001ba80: 696f 6e29 3a0a 2020 2020 2020 2020 7365  ion):.        se
+0001ba90: 6c66 2e5f 7665 7273 696f 6e20 3d20 7665  lf._version = ve
+0001baa0: 7273 696f 6e0a 0a20 2020 2040 6465 7363  rsion..    @desc
+0001bab0: 7269 7074 696f 6e2e 7365 7474 6572 0a20  ription.setter. 
+0001bac0: 2020 2064 6566 2064 6573 6372 6970 7469     def descripti
+0001bad0: 6f6e 2873 656c 662c 206e 6577 5f64 6573  on(self, new_des
+0001bae0: 6372 6970 7469 6f6e 293a 0a20 2020 2020  cription):.     
+0001baf0: 2020 2073 656c 662e 5f64 6573 6372 6970     self._descrip
+0001bb00: 7469 6f6e 203d 206e 6577 5f64 6573 6372  tion = new_descr
+0001bb10: 6970 7469 6f6e 0a0a 2020 2020 4070 726f  iption..    @pro
+0001bb20: 7065 7274 790a 2020 2020 6465 6620 6665  perty.    def fe
+0001bb30: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
+0001bb40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001bb50: 2222 224e 616d 6520 6f66 2074 6865 2066  """Name of the f
+0001bb60: 6561 7475 7265 2073 746f 7265 2069 6e20  eature store in 
+0001bb70: 7768 6963 6820 7468 6520 6665 6174 7572  which the featur
+0001bb80: 6520 6772 6f75 7020 6973 206c 6f63 6174  e group is locat
+0001bb90: 6564 2e22 2222 0a20 2020 2020 2020 2072  ed.""".        r
+0001bba0: 6574 7572 6e20 7365 6c66 2e5f 6665 6174  eturn self._feat
+0001bbb0: 7572 655f 7374 6f72 655f 6e61 6d65 0a0a  ure_store_name..
+0001bbc0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001bbd0: 2020 6465 6620 6665 6174 7572 655f 7374    def feature_st
+0001bbe0: 6f72 655f 6964 2873 656c 6629 3a0a 2020  ore_id(self):.  
+0001bbf0: 2020 2020 2020 2222 2249 6420 6f66 2074        """Id of t
+0001bc00: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
+0001bc10: 2069 6e20 7768 6963 6820 7468 6520 6665   in which the fe
+0001bc20: 6174 7572 6520 6772 6f75 7020 6973 206c  ature group is l
+0001bc30: 6f63 6174 6564 2e22 2222 0a20 2020 2020  ocated.""".     
+0001bc40: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0001bc50: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
+0001bc60: 0a0a 0a63 6c61 7373 2053 7069 6e65 4772  ...class SpineGr
+0001bc70: 6f75 7028 4665 6174 7572 6547 726f 7570  oup(FeatureGroup
+0001bc80: 4261 7365 293a 0a20 2020 2053 5049 4e45  Base):.    SPINE
+0001bc90: 5f47 524f 5550 203d 2022 4f4e 5f44 454d  _GROUP = "ON_DEM
+0001bca0: 414e 445f 4645 4154 5552 455f 4752 4f55  AND_FEATURE_GROU
+0001bcb0: 5022 0a20 2020 2045 4e54 4954 595f 5459  P".    ENTITY_TY
+0001bcc0: 5045 203d 2022 6665 6174 7572 6567 726f  PE = "featuregro
+0001bcd0: 7570 7322 0a0a 2020 2020 6465 6620 5f5f  ups"..    def __
+0001bce0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0001bcf0: 7365 6c66 2c0a 2020 2020 2020 2020 7374  self,.        st
+0001bd00: 6f72 6167 655f 636f 6e6e 6563 746f 723d  orage_connector=
+0001bd10: 4e6f 6e65 2c0a 2020 2020 2020 2020 7175  None,.        qu
+0001bd20: 6572 793d 4e6f 6e65 2c0a 2020 2020 2020  ery=None,.      
+0001bd30: 2020 6461 7461 5f66 6f72 6d61 743d 4e6f    data_format=No
+0001bd40: 6e65 2c0a 2020 2020 2020 2020 7061 7468  ne,.        path
+0001bd50: 3d4e 6f6e 652c 0a20 2020 2020 2020 206f  =None,.        o
+0001bd60: 7074 696f 6e73 3d7b 7d2c 0a20 2020 2020  ptions={},.     
+0001bd70: 2020 206e 616d 653d 4e6f 6e65 2c0a 2020     name=None,.  
+0001bd80: 2020 2020 2020 7665 7273 696f 6e3d 4e6f        version=No
+0001bd90: 6e65 2c0a 2020 2020 2020 2020 6465 7363  ne,.        desc
+0001bda0: 7269 7074 696f 6e3d 4e6f 6e65 2c0a 2020  ription=None,.  
+0001bdb0: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
+0001bdc0: 793d 4e6f 6e65 2c0a 2020 2020 2020 2020  y=None,.        
+0001bdd0: 6665 6174 7572 6573 746f 7265 5f69 643d  featurestore_id=
+0001bde0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6665  None,.        fe
+0001bdf0: 6174 7572 6573 746f 7265 5f6e 616d 653d  aturestore_name=
+0001be00: 4e6f 6e65 2c0a 2020 2020 2020 2020 6372  None,.        cr
+0001be10: 6561 7465 643d 4e6f 6e65 2c0a 2020 2020  eated=None,.    
+0001be20: 2020 2020 6372 6561 746f 723d 4e6f 6e65      creator=None
+0001be30: 2c0a 2020 2020 2020 2020 6964 3d4e 6f6e  ,.        id=Non
+0001be40: 652c 0a20 2020 2020 2020 2066 6561 7475  e,.        featu
+0001be50: 7265 733d 4e6f 6e65 2c0a 2020 2020 2020  res=None,.      
+0001be60: 2020 6c6f 6361 7469 6f6e 3d4e 6f6e 652c    location=None,
+0001be70: 0a20 2020 2020 2020 2073 7461 7469 7374  .        statist
+0001be80: 6963 735f 636f 6e66 6967 3d4e 6f6e 652c  ics_config=None,
+0001be90: 0a20 2020 2020 2020 2065 7665 6e74 5f74  .        event_t
+0001bea0: 696d 653d 4e6f 6e65 2c0a 2020 2020 2020  ime=None,.      
+0001beb0: 2020 6578 7065 6374 6174 696f 6e5f 7375    expectation_su
+0001bec0: 6974 653d 4e6f 6e65 2c0a 2020 2020 2020  ite=None,.      
+0001bed0: 2020 6f6e 6c69 6e65 5f65 6e61 626c 6564    online_enabled
+0001bee0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0001bef0: 6872 6566 3d4e 6f6e 652c 0a20 2020 2020  href=None,.     
+0001bf00: 2020 206f 6e6c 696e 655f 746f 7069 635f     online_topic_
+0001bf10: 6e61 6d65 3d4e 6f6e 652c 0a20 2020 2020  name=None,.     
+0001bf20: 2020 2073 7069 6e65 3d54 7275 652c 0a20     spine=True,. 
+0001bf30: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
+0001bf40: 3d22 7370 696e 6522 2c0a 2020 2020 293a  ="spine",.    ):
+0001bf50: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0001bf60: 2e5f 5f69 6e69 745f 5f28 0a20 2020 2020  .__init__(.     
+0001bf70: 2020 2020 2020 2066 6561 7475 7265 7374         featurest
+0001bf80: 6f72 655f 6964 2c0a 2020 2020 2020 2020  ore_id,.        
+0001bf90: 2020 2020 6c6f 6361 7469 6f6e 2c0a 2020      location,.  
+0001bfa0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
+0001bfb0: 7469 6d65 3d65 7665 6e74 5f74 696d 652c  time=event_time,
+0001bfc0: 0a20 2020 2020 2020 2020 2020 206f 6e6c  .            onl
+0001bfd0: 696e 655f 656e 6162 6c65 643d 6f6e 6c69  ine_enabled=onli
+0001bfe0: 6e65 5f65 6e61 626c 6564 2c0a 2020 2020  ne_enabled,.    
+0001bff0: 2020 2020 2020 2020 6964 3d69 642c 0a20          id=id,. 
+0001c000: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+0001c010: 7461 7469 6f6e 5f73 7569 7465 3d65 7870  tation_suite=exp
+0001c020: 6563 7461 7469 6f6e 5f73 7569 7465 2c0a  ectation_suite,.
+0001c030: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
+0001c040: 6e65 5f74 6f70 6963 5f6e 616d 653d 6f6e  ne_topic_name=on
+0001c050: 6c69 6e65 5f74 6f70 6963 5f6e 616d 652c  line_topic_name,
+0001c060: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001c070: 2020 2020 7365 6c66 2e5f 6665 6174 7572      self._featur
+0001c080: 655f 7374 6f72 655f 6e61 6d65 203d 2066  e_store_name = f
+0001c090: 6561 7475 7265 7374 6f72 655f 6e61 6d65  eaturestore_name
+0001c0a0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+0001c0b0: 6573 6372 6970 7469 6f6e 203d 2064 6573  escription = des
+0001c0c0: 6372 6970 7469 6f6e 0a20 2020 2020 2020  cription.       
+0001c0d0: 2073 656c 662e 5f63 7265 6174 6564 203d   self._created =
+0001c0e0: 2063 7265 6174 6564 0a20 2020 2020 2020   created.       
+0001c0f0: 2073 656c 662e 5f63 7265 6174 6f72 203d   self._creator =
+0001c100: 2075 7365 722e 5573 6572 2e66 726f 6d5f   user.User.from_
+0001c110: 7265 7370 6f6e 7365 5f6a 736f 6e28 6372  response_json(cr
+0001c120: 6561 746f 7229 0a20 2020 2020 2020 2073  eator).        s
+0001c130: 656c 662e 5f76 6572 7369 6f6e 203d 2076  elf._version = v
+0001c140: 6572 7369 6f6e 0a20 2020 2020 2020 2073  ersion.        s
+0001c150: 656c 662e 5f6e 616d 6520 3d20 6e61 6d65  elf._name = name
+0001c160: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0001c170: 6665 6174 7572 6573 203d 205b 0a20 2020  features = [.   
+0001c180: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+0001c190: 2e46 6561 7475 7265 2e66 726f 6d5f 7265  .Feature.from_re
+0001c1a0: 7370 6f6e 7365 5f6a 736f 6e28 6665 6174  sponse_json(feat
+0001c1b0: 2920 6966 2069 7369 6e73 7461 6e63 6528  ) if isinstance(
+0001c1c0: 6665 6174 2c20 6469 6374 2920 656c 7365  feat, dict) else
+0001c1d0: 2066 6561 740a 2020 2020 2020 2020 2020   feat.          
+0001c1e0: 2020 666f 7220 6665 6174 2069 6e20 2866    for feat in (f
+0001c1f0: 6561 7475 7265 7320 6f72 205b 5d29 0a20  eatures or []). 
+0001c200: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+0001c210: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
+0001c220: 6772 6f75 705f 656e 6769 6e65 203d 2073  group_engine = s
+0001c230: 7069 6e65 5f67 726f 7570 5f65 6e67 696e  pine_group_engin
+0001c240: 652e 5370 696e 6547 726f 7570 456e 6769  e.SpineGroupEngi
+0001c250: 6e65 280a 2020 2020 2020 2020 2020 2020  ne(.            
+0001c260: 6665 6174 7572 6573 746f 7265 5f69 640a  featurestore_id.
+0001c270: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001c280: 2020 2069 6620 7365 6c66 2e5f 6964 3a0a     if self._id:.
+0001c290: 2020 2020 2020 2020 2020 2020 2320 476f              # Go
+0001c2a0: 7420 6672 6f6d 2048 6f70 7377 6f72 6b73  t from Hopsworks
+0001c2b0: 2c20 6465 7365 7269 616c 697a 6520 6665  , deserialize fe
+0001c2c0: 6174 7572 6573 2061 6e64 2073 746f 7261  atures and stora
+0001c2d0: 6765 2063 6f6e 6e65 6374 6f72 0a20 2020  ge connector.   
+0001c2e0: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+0001c2f0: 6561 7475 7265 7320 3d20 280a 2020 2020  eatures = (.    
+0001c300: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+0001c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c320: 2020 6665 6174 7572 652e 4665 6174 7572    feature.Featur
+0001c330: 652e 6672 6f6d 5f72 6573 706f 6e73 655f  e.from_response_
+0001c340: 6a73 6f6e 2866 6561 7429 0a20 2020 2020  json(feat).     
+0001c350: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001c360: 6620 6973 696e 7374 616e 6365 2866 6561  f isinstance(fea
+0001c370: 742c 2064 6963 7429 0a20 2020 2020 2020  t, dict).       
+0001c380: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001c390: 6520 6665 6174 0a20 2020 2020 2020 2020  e feat.         
+0001c3a0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0001c3b0: 6561 7420 696e 2066 6561 7475 7265 730a  eat in features.
+0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001c3e0: 2020 6966 2066 6561 7475 7265 730a 2020    if features.  
+0001c3f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001c400: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
+0001c410: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001c420: 2020 7365 6c66 2e70 7269 6d61 7279 5f6b    self.primary_k
+0001c430: 6579 203d 2028 0a20 2020 2020 2020 2020  ey = (.         
+0001c440: 2020 2020 2020 205b 6665 6174 2e6e 616d         [feat.nam
+0001c450: 6520 666f 7220 6665 6174 2069 6e20 7365  e for feat in se
+0001c460: 6c66 2e5f 6665 6174 7572 6573 2069 6620  lf._features if 
+0001c470: 6665 6174 2e70 7269 6d61 7279 2069 7320  feat.primary is 
+0001c480: 5472 7565 5d0a 2020 2020 2020 2020 2020  True].          
+0001c490: 2020 2020 2020 6966 2073 656c 662e 5f66        if self._f
+0001c4a0: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+0001c4b0: 2020 2020 2020 2020 656c 7365 205b 5d0a          else [].
+0001c4c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001c4d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0001c4e0: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
+0001c4f0: 203d 2073 7461 7469 7374 6963 735f 636f   = statistics_co
+0001c500: 6e66 6967 0a20 2020 2020 2020 2065 6c73  nfig.        els
+0001c510: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001c520: 656c 662e 7072 696d 6172 795f 6b65 7920  elf.primary_key 
+0001c530: 3d20 7072 696d 6172 795f 6b65 790a 2020  = primary_key.  
+0001c540: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0001c550: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
+0001c560: 203d 2073 7461 7469 7374 6963 735f 636f   = statistics_co
+0001c570: 6e66 6967 0a20 2020 2020 2020 2020 2020  nfig.           
+0001c580: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+0001c590: 3d20 6665 6174 7572 6573 0a0a 2020 2020  = features..    
+0001c5a0: 2020 2020 7365 6c66 2e5f 6872 6566 203d      self._href =
+0001c5b0: 2068 7265 660a 0a20 2020 2020 2020 2023   href..        #
+0001c5c0: 2068 6173 2074 6f20 6861 7070 656e 206c   has to happen l
+0001c5d0: 6173 7420 2d3e 2066 6561 7475 7265 7320  ast -> features 
+0001c5e0: 616e 6420 6964 2061 7265 206e 6565 6465  and id are neede
+0001c5f0: 6420 666f 7220 7363 6865 6d61 2076 6572  d for schema ver
+0001c600: 6966 6963 6174 696f 6e0a 2020 2020 2020  ification.      
+0001c610: 2020 2320 7573 6520 7365 7474 6572 2074    # use setter t
+0001c620: 6f20 636f 6e76 6572 7420 746f 2064 6566  o convert to def
+0001c630: 6175 6c74 2064 6174 6166 7261 6d65 2074  ault dataframe t
+0001c640: 7970 6520 666f 7220 656e 6769 6e65 0a20  ype for engine. 
+0001c650: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+0001c660: 6672 616d 6520 3d20 6461 7461 6672 616d  frame = datafram
+0001c670: 650a 0a20 2020 2064 6566 205f 7361 7665  e..    def _save
+0001c680: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001c690: 2222 2250 6572 7369 7374 2074 6865 206d  """Persist the m
+0001c6a0: 6574 6164 6174 6120 666f 7220 7468 6973  etadata for this
+0001c6b0: 2073 7069 6e65 2067 726f 7570 2e0a 0a20   spine group... 
+0001c6c0: 2020 2020 2020 2057 6974 686f 7574 2063         Without c
+0001c6d0: 616c 6c69 6e67 2074 6869 7320 6d65 7468  alling this meth
+0001c6e0: 6f64 2c20 796f 7572 2066 6561 7475 7265  od, your feature
+0001c6f0: 2067 726f 7570 2077 696c 6c20 6f6e 6c79   group will only
+0001c700: 2065 7869 7374 0a20 2020 2020 2020 2069   exist.        i
+0001c710: 6e20 796f 7572 2050 7974 686f 6e20 4b65  n your Python Ke
+0001c720: 726e 656c 2c20 6275 7420 6e6f 7420 696e  rnel, but not in
+0001c730: 2048 6f70 7377 6f72 6b73 2e0a 0a20 2020   Hopsworks...   
+0001c740: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+0001c750: 2020 2020 2020 2071 7565 7279 203d 2022         query = "
+0001c760: 5345 4c45 4354 202a 2046 524f 4d20 7361  SELECT * FROM sa
+0001c770: 6c65 7322 0a0a 2020 2020 2020 2020 6667  les"..        fg
+0001c780: 203d 2066 6561 7475 7265 5f73 746f 7265   = feature_store
+0001c790: 2e63 7265 6174 655f 7370 696e 655f 6772  .create_spine_gr
+0001c7a0: 6f75 7028 6e61 6d65 3d22 7361 6c65 7322  oup(name="sales"
+0001c7b0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+0001c7c0: 7273 696f 6e3d 312c 0a20 2020 2020 2020  rsion=1,.       
+0001c7d0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0001c7e0: 3d22 5068 7973 6963 616c 2073 686f 7020  ="Physical shop 
+0001c7f0: 7361 6c65 7320 6665 6174 7572 6573 222c  sales features",
+0001c800: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0001c810: 6d61 7279 5f6b 6579 3d5b 2773 735f 7374  mary_key=['ss_st
+0001c820: 6f72 655f 736b 275d 2c0a 2020 2020 2020  ore_sk'],.      
+0001c830: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
+0001c840: 3d27 7361 6c65 5f64 6174 6527 2c0a 2020  ='sale_date',.  
+0001c850: 2020 2020 2020 2020 2020 6461 7461 6672            datafr
+0001c860: 616d 653d 6466 2c0a 2020 2020 2020 2020  ame=df,.        
+0001c870: 290a 0a20 2020 2020 2020 2066 672e 5f73  )..        fg._s
+0001c880: 6176 6528 290a 2020 2020 2020 2020 2222  ave().        ""
+0001c890: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+0001c8a0: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+0001c8b0: 6769 6e65 2e73 6176 6528 7365 6c66 290a  gine.save(self).
+0001c8c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001c8d0: 656c 660a 0a20 2020 2040 7072 6f70 6572  elf..    @proper
+0001c8e0: 7479 0a20 2020 2064 6566 2064 6174 6166  ty.    def dataf
+0001c8f0: 7261 6d65 2873 656c 6629 3a0a 2020 2020  rame(self):.    
+0001c900: 2020 2020 2222 2253 7069 6e65 2064 6174      """Spine dat
+0001c910: 6166 7261 6d65 2077 6974 6820 7072 696d  aframe with prim
+0001c920: 6172 7920 6b65 792c 2065 7665 6e74 2074  ary key, event t
+0001c930: 696d 6520 616e 640a 2020 2020 2020 2020  ime and.        
+0001c940: 6c61 6265 6c20 636f 6c75 6d6e 2074 6f20  label column to 
+0001c950: 7573 6520 666f 7220 706f 696e 7420 696e  use for point in
+0001c960: 2074 696d 6520 6a6f 696e 2077 6865 6e20   time join when 
+0001c970: 6665 7463 6869 6e67 2066 6561 7475 7265  fetching feature
+0001c980: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0001c990: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001c9a0: 6c66 2e5f 6461 7461 6672 616d 650a 0a20  lf._dataframe.. 
+0001c9b0: 2020 2040 6461 7461 6672 616d 652e 7365     @dataframe.se
+0001c9c0: 7474 6572 0a20 2020 2064 6566 2064 6174  tter.    def dat
+0001c9d0: 6166 7261 6d65 2873 656c 662c 2064 6174  aframe(self, dat
+0001c9e0: 6166 7261 6d65 293a 0a20 2020 2020 2020  aframe):.       
+0001c9f0: 2022 2222 5570 6461 7465 2074 6865 2073   """Update the s
+0001ca00: 7069 6e65 2064 6174 6166 7261 6d65 2063  pine dataframe c
+0001ca10: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
+0001ca20: 7370 696e 6520 6772 6f75 702e 2222 220a  spine group.""".
+0001ca30: 2020 2020 2020 2020 7365 6c66 2e5f 6461          self._da
+0001ca40: 7461 6672 616d 6520 3d20 656e 6769 6e65  taframe = engine
+0001ca50: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+0001ca60: 636f 6e76 6572 745f 746f 5f64 6566 6175  convert_to_defau
+0001ca70: 6c74 5f64 6174 6166 7261 6d65 2864 6174  lt_dataframe(dat
+0001ca80: 6166 7261 6d65 290a 0a20 2020 2020 2020  aframe)..       
+0001ca90: 2023 2069 6e20 6673 2071 7565 7279 2074   # in fs query t
+0001caa0: 6865 2066 6561 7475 7265 7320 6172 6520  he features are 
+0001cab0: 6e6f 7420 7365 6e74 2c20 736f 2074 6865  not sent, so the
+0001cac0: 6e20 646f 6e27 7420 646f 2076 616c 6964  n don't do valid
+0001cad0: 6174 696f 6e0a 2020 2020 2020 2020 6966  ation.        if
+0001cae0: 2028 0a20 2020 2020 2020 2020 2020 2073   (.            s
+0001caf0: 656c 662e 5f69 6420 6973 206e 6f74 204e  elf._id is not N
+0001cb00: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0001cb10: 616e 6420 7365 6c66 2e5f 6461 7461 6672  and self._datafr
+0001cb20: 616d 6520 6973 206e 6f74 204e 6f6e 650a  ame is not None.
+0001cb30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001cb40: 7365 6c66 2e5f 6665 6174 7572 6573 2069  self._features i
+0001cb50: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+0001cb60: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001cb70: 2020 6461 7461 6672 616d 655f 6665 6174    dataframe_feat
+0001cb80: 7572 6573 203d 2065 6e67 696e 652e 6765  ures = engine.ge
+0001cb90: 745f 696e 7374 616e 6365 2829 2e70 6172  t_instance().par
+0001cba0: 7365 5f73 6368 656d 615f 6665 6174 7572  se_schema_featur
+0001cbb0: 655f 6772 6f75 7028 0a20 2020 2020 2020  e_group(.       
+0001cbc0: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
+0001cbd0: 6174 6166 7261 6d65 0a20 2020 2020 2020  ataframe.       
+0001cbe0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0001cbf0: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
+0001cc00: 5f67 726f 7570 5f65 6e67 696e 652e 5f76  _group_engine._v
+0001cc10: 6572 6966 795f 7363 6865 6d61 5f63 6f6d  erify_schema_com
+0001cc20: 7061 7469 6269 6c69 7479 280a 2020 2020  patibility(.    
+0001cc30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001cc40: 2e5f 6665 6174 7572 6573 2c20 6461 7461  ._features, data
+0001cc50: 6672 616d 655f 6665 6174 7572 6573 0a20  frame_features. 
+0001cc60: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001cc70: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+0001cc80: 2020 2064 6566 2066 726f 6d5f 7265 7370     def from_resp
+0001cc90: 6f6e 7365 5f6a 736f 6e28 636c 732c 206a  onse_json(cls, j
+0001cca0: 736f 6e5f 6469 6374 293a 0a20 2020 2020  son_dict):.     
+0001ccb0: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
+0001ccc0: 7a65 6420 3d20 6875 6d70 732e 6465 6361  zed = humps.deca
+0001ccd0: 6d65 6c69 7a65 286a 736f 6e5f 6469 6374  melize(json_dict
+0001cce0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+0001ccf0: 6e73 7461 6e63 6528 6a73 6f6e 5f64 6563  nstance(json_dec
+0001cd00: 616d 656c 697a 6564 2c20 6469 6374 293a  amelized, dict):
+0001cd10: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+0001cd20: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001cd30: 642e 706f 7028 2274 7970 6522 2c20 4e6f  d.pop("type", No
+0001cd40: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+0001cd50: 7265 7475 726e 2063 6c73 282a 2a6a 736f  return cls(**jso
+0001cd60: 6e5f 6465 6361 6d65 6c69 7a65 6429 0a20  n_decamelized). 
+0001cd70: 2020 2020 2020 2066 6f72 2066 6720 696e         for fg in
+0001cd80: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001cd90: 643a 0a20 2020 2020 2020 2020 2020 205f  d:.            _
+0001cda0: 203d 2066 672e 706f 7028 2274 7970 6522   = fg.pop("type"
+0001cdb0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0001cdc0: 7265 7475 726e 205b 636c 7328 2a2a 6667  return [cls(**fg
+0001cdd0: 2920 666f 7220 6667 2069 6e20 6a73 6f6e  ) for fg in json
+0001cde0: 5f64 6563 616d 656c 697a 6564 5d0a 0a20  _decamelized].. 
+0001cdf0: 2020 2064 6566 2075 7064 6174 655f 6672     def update_fr
+0001ce00: 6f6d 5f72 6573 706f 6e73 655f 6a73 6f6e  om_response_json
+0001ce10: 2873 656c 662c 206a 736f 6e5f 6469 6374  (self, json_dict
+0001ce20: 293a 0a20 2020 2020 2020 206a 736f 6e5f  ):.        json_
+0001ce30: 6465 6361 6d65 6c69 7a65 6420 3d20 6875  decamelized = hu
+0001ce40: 6d70 732e 6465 6361 6d65 6c69 7a65 286a  mps.decamelize(j
+0001ce50: 736f 6e5f 6469 6374 290a 2020 2020 2020  son_dict).      
+0001ce60: 2020 6966 2022 7479 7065 2220 696e 206a    if "type" in j
+0001ce70: 736f 6e5f 6465 6361 6d65 6c69 7a65 643a  son_decamelized:
+0001ce80: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+0001ce90: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001cea0: 642e 706f 7028 2274 7970 6522 290a 2020  d.pop("type").  
+0001ceb0: 2020 2020 2020 7365 6c66 2e5f 5f69 6e69        self.__ini
+0001cec0: 745f 5f28 2a2a 6a73 6f6e 5f64 6563 616d  t__(**json_decam
+0001ced0: 656c 697a 6564 290a 2020 2020 2020 2020  elized).        
+0001cee0: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
+0001cef0: 2064 6566 206a 736f 6e28 7365 6c66 293a   def json(self):
+0001cf00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001cf10: 6a73 6f6e 2e64 756d 7073 2873 656c 662c  json.dumps(self,
+0001cf20: 2063 6c73 3d75 7469 6c2e 4665 6174 7572   cls=util.Featur
+0001cf30: 6553 746f 7265 456e 636f 6465 7229 0a0a  eStoreEncoder)..
+0001cf40: 2020 2020 6465 6620 746f 5f64 6963 7428      def to_dict(
+0001cf50: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001cf60: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+0001cf70: 2020 2020 2269 6422 3a20 7365 6c66 2e5f      "id": self._
+0001cf80: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0001cf90: 226e 616d 6522 3a20 7365 6c66 2e5f 6e61  "name": self._na
+0001cfa0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0001cfb0: 2264 6573 6372 6970 7469 6f6e 223a 2073  "description": s
+0001cfc0: 656c 662e 5f64 6573 6372 6970 7469 6f6e  elf._description
+0001cfd0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+0001cfe0: 6572 7369 6f6e 223a 2073 656c 662e 5f76  ersion": self._v
+0001cff0: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
+0001d000: 2020 2020 2266 6561 7475 7265 7322 3a20      "features": 
+0001d010: 7365 6c66 2e5f 6665 6174 7572 6573 2c0a  self._features,.
+0001d020: 2020 2020 2020 2020 2020 2020 2266 6561              "fea
+0001d030: 7475 7265 7374 6f72 6549 6422 3a20 7365  turestoreId": se
+0001d040: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
+0001d050: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+0001d060: 2020 2274 7970 6522 3a20 226f 6e44 656d    "type": "onDem
+0001d070: 616e 6446 6561 7475 7265 6772 6f75 7044  andFeaturegroupD
+0001d080: 544f 222c 0a20 2020 2020 2020 2020 2020  TO",.           
+0001d090: 2022 7374 6174 6973 7469 6373 436f 6e66   "statisticsConf
+0001d0a0: 6967 223a 2073 656c 662e 5f73 7461 7469  ig": self._stati
+0001d0b0: 7374 6963 735f 636f 6e66 6967 2c0a 2020  stics_config,.  
+0001d0c0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+0001d0d0: 5469 6d65 223a 2073 656c 662e 5f65 7665  Time": self._eve
+0001d0e0: 6e74 5f74 696d 652c 0a20 2020 2020 2020  nt_time,.       
+0001d0f0: 2020 2020 2022 7370 696e 6522 3a20 5472       "spine": Tr
+0001d100: 7565 2c0a 2020 2020 2020 2020 7d0a       ue,.        }.
```

### Comparing `hsfs-3.3.0rc0/hsfs/feature_group_commit.py` & `hsfs-3.3.0rc1/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/feature_group_writer.py` & `hsfs-3.3.0rc1/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/feature_store.py` & `hsfs-3.3.0rc1/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/feature_view.py` & `hsfs-3.3.0rc1/hsfs/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,15 +528,19 @@
         # Arguments
             start_time: Start event time for the batch query, inclusive. Optional. Strings should be
                 formatted in one of the following formats `%Y-%m-%d`, `%Y-%m-%d %H`, `%Y-%m-%d %H:%M`, `%Y-%m-%d %H:%M:%S`,
                 or `%Y-%m-%d %H:%M:%S.%f`. Int, i.e Unix Epoch should be in seconds.
             end_time: End event time for the batch query, exclusive. Optional. Strings should be
                 formatted in one of the following formats `%Y-%m-%d`, `%Y-%m-%d %H`, `%Y-%m-%d %H:%M`, `%Y-%m-%d %H:%M:%S`,
                 or `%Y-%m-%d %H:%M:%S.%f`. Int, i.e Unix Epoch should be in seconds.
-            read_options: User provided read options. Defaults to `{}`.
+            read_options: User provided read options.
+                Dictionary of read options for python engine:
+                * key `"use_hive"` and value `True` to read batch data with Hive instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
+                Defaults to `{}`.
             spine: Spine dataframe with primary key, event time and
                 label column to use for point in time join when fetching features. Defaults to `None` and is only required
                 when feature view was created with spine group in the feature query.
                 It is possible to directly pass a spine group instead of a dataframe to overwrite the left side of the
                 feature join, however, the same features as in the original feature group that is being replaced need to
                 be available in the spine group.
 
@@ -1580,20 +1584,23 @@
                 this feature group, `"correlations`" to turn on feature correlation
                 computation and `"histograms"` to compute feature value frequencies. The
                 values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
-                When using the `python` engine, write_options can contain the
+                When using the `python` engine, read_options can contain the
                 following entries:
+                * key `"use_hive"` and value `True` to create in-memory training dataset
+                  with Hive instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 * key `spark` and value an object of type
-                [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
+                  [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
                   to configure the Hopsworks Job used to compute the training dataset.
                 Defaults to `{}`.
             spine: Spine dataframe with primary key, event time and
                 label column to use for point in time join when fetching features. Defaults to `None` and is only required
                 when feature view was created with spine group in the feature query.
                 It is possible to directly pass a spine group instead of a dataframe to overwrite the left side of the
                 feature join, however, the same features as in the original feature group that is being replaced need to
@@ -1721,20 +1728,23 @@
                 this feature group, `"correlations`" to turn on feature correlation
                 computation and `"histograms"` to compute feature value frequencies. The
                 values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
-                When using the `python` engine, write_options can contain the
+                When using the `python` engine, read_options can contain the
                 following entries:
+                * key `"use_hive"` and value `True` to create in-memory training dataset
+                  with Hive instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 * key `spark` and value an object of type
-                [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
+                  [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
                   to configure the Hopsworks Job used to compute the training dataset.
                 Defaults to `{}`.
             spine: Spine dataframe with primary key, event time and
                 label column to use for point in time join when fetching features. Defaults to `None` and is only required
                 when feature view was created with spine group in the feature query.
                 It is possible to directly pass a spine group instead of a dataframe to overwrite the left side of the
                 feature join, however, the same features as in the original feature group that is being replaced need to
@@ -1899,20 +1909,23 @@
                 this feature group, `"correlations`" to turn on feature correlation
                 computation and `"histograms"` to compute feature value frequencies. The
                 values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
-                When using the `python` engine, write_options can contain the
+                When using the `python` engine, read_options can contain the
                 following entries:
+                * key `"use_hive"` and value `True` to create in-memory training dataset
+                  with Hive instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 * key `spark` and value an object of type
-                [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
+                  [hsfs.core.job_configuration.JobConfiguration](../job_configuration)
                   to configure the Hopsworks Job used to compute the training dataset.
                 Defaults to `{}`.
             spine: Spine dataframe with primary key, event time and
                 label column to use for point in time join when fetching features. Defaults to `None` and is only required
                 when feature view was created with spine group in the feature query.
                 It is possible to directly pass a spine group instead of a dataframe to overwrite the left side of the
                 feature join, however, the same features as in the original feature group that is being replaced need to
@@ -2018,14 +2031,17 @@
             Python as Engine, instead you will have to use the storage's native client.
 
         # Arguments
             training_dataset_version: training dataset version
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
                 For python engine:
+                * key `"use_hive"` and value `True` to read training dataset
+                  with the Hopsworks API instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 Defaults to `{}`.
 
         # Returns
             (X, y): Tuple of dataframe of features and labels
         """
@@ -2056,14 +2072,17 @@
             ```
 
         # Arguments
             training_dataset_version: training dataset version
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
                 For python engine:
+                * key `"use_hive"` and value `True` to read training dataset
+                  with the Hopsworks API instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 Defaults to `{}`.
 
         # Returns
             (X_train, X_test, y_train, y_test):
                 Tuple of dataframe of features and labels
@@ -2098,14 +2117,17 @@
             ```
 
         # Arguments
             training_dataset_version: training dataset version
             read_options: Additional options as key/value pairs to pass to the execution engine.
                 For spark engine: Dictionary of read options for Spark.
                 For python engine:
+                * key `"use_hive"` and value `True` to read training dataset
+                  with the Hopsworks API instead of
+                  [ArrowFlight Server](https://docs.hopsworks.ai/latest/setup_installation/common/arrow_flight_duckdb/).
                 * key `"hive_config"` to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 Defaults to `{}`.
 
         # Returns
             (X_train, X_val, X_test, y_train, y_val, y_test):
                 Tuple of dataframe of features and labels
```

### Comparing `hsfs-3.3.0rc0/hsfs/ge_expectation.py` & `hsfs-3.3.0rc1/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/ge_validation_result.py` & `hsfs-3.3.0rc1/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/split_statistics.py` & `hsfs-3.3.0rc1/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/statistics.py` & `hsfs-3.3.0rc1/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/statistics_config.py` & `hsfs-3.3.0rc1/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/storage_connector.py` & `hsfs-3.3.0rc1/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/tag.py` & `hsfs-3.3.0rc1/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/training_dataset.py` & `hsfs-3.3.0rc1/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/training_dataset_feature.py` & `hsfs-3.3.0rc1/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/training_dataset_split.py` & `hsfs-3.3.0rc1/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/transformation_function.py` & `hsfs-3.3.0rc1/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/transformation_function_attached.py` & `hsfs-3.3.0rc1/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/user.py` & `hsfs-3.3.0rc1/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/util.py` & `hsfs-3.3.0rc1/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/validation_report.py` & `hsfs-3.3.0rc1/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs/version.py` & `hsfs-3.3.0rc1/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.3.0rc0"
+__version__ = "3.3.0rc1"
```

### Comparing `hsfs-3.3.0rc0/hsfs.egg-info/PKG-INFO` & `hsfs-3.3.0rc1/hsfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.3.0rc0
+Version: 3.3.0rc1
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc0
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc1
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.3.0rc0 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.3.0rc1 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc0
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.3.0rc1
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.3.0rc0/hsfs.egg-info/SOURCES.txt` & `hsfs-3.3.0rc1/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.3.0rc0/hsfs.egg-info/requires.txt` & `hsfs-3.3.0rc1/hsfs.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 mkdocs-minify-plugin>=0.2.0
 mkdocs==1.3.0
 pymdown-extensions
 sphinx==3.5.4
 
 [hive]
 confluent-kafka<=1.9.0
-fastavro<=1.7.3,>=1.4.11
+fastavro<=1.8.2,>=1.4.11
 pyarrow>=10.0
 pyhopshive[thrift]
 
 [python]
 confluent-kafka<=1.9.0
-fastavro<=1.7.3,>=1.4.11
+fastavro<=1.8.2,>=1.4.11
 pyarrow>=10.0
 pyhopshive[thrift]
 tqdm
```

### Comparing `hsfs-3.3.0rc0/setup.py` & `hsfs-3.3.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,21 +65,21 @@
             "mkdocs-macros-plugin==0.7.0",
             "mkdocs-minify-plugin>=0.2.0",
         ],
         "hive": [
             "pyhopshive[thrift]",
             "pyarrow>=10.0",
             "confluent-kafka<=1.9.0",
-            "fastavro>=1.4.11,<=1.7.3",
+            "fastavro>=1.4.11,<=1.8.2",
         ],
         "python": [
             "pyhopshive[thrift]",
             "pyarrow>=10.0",
             "confluent-kafka<=1.9.0",
-            "fastavro>=1.4.11,<=1.7.3",
+            "fastavro>=1.4.11,<=1.8.2",
             "tqdm",
         ],
     },
     author="Hopsworks AB",
     author_email="moritz@logicalclocks.com",
     description="HSFS: An environment independent client to interact with the Hopsworks Featurestore",
     license="Apache License 2.0",
```

