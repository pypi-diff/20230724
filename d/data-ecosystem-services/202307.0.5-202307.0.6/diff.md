# Comparing `tmp/data_ecosystem_services-202307.0.5.tar.gz` & `tmp/data_ecosystem_services-202307.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202307.0.5.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202307.0.6.tar", max compression
```

## Comparing `data_ecosystem_services-202307.0.5.tar` & `data_ecosystem_services-202307.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      918 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0     1264 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     5030 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/column.py
--rw-r--r--   0        0        0    24777 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0    13817 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     2037 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0    12009 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/excelmetadata.py
--rw-r--r--   0        0        0      566 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/execution_session.py
--rw-r--r--   0        0        0     4530 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    16621 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0     5003 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/query.py
--rw-r--r--   0        0        0    51042 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     7345 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/table.py
--rw-r--r--   0        0        0     1486 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    25982 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0     1044 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/__init__.py
--rw-r--r--   0        0        0       41 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/az_client.py
--rw-r--r--   0        0        0     4570 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/azd_client.py
--rw-r--r--   0        0        0     1050 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/__init__.py
--rw-r--r--   0        0        0     8967 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/az_key_vault.py
--rw-r--r--   0        0        0     1073 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0     2665 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0     1024 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/__init__.py
--rw-r--r--   0        0        0    15940 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_logging.py
--rw-r--r--   0        0        0     8398 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1013 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_base64.py
--rw-r--r--   0        0        0    21410 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_core.py
--rw-r--r--   0        0        0     1175 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/__init__.py
--rw-r--r--   0        0        0    42751 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/dataset_metadata.py
--rw-r--r--   0        0        0    40188 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/environment_metadata.py
--rw-r--r--   0        0        0    36068 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/job_metadata.py
--rw-r--r--   0        0        0     2254 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/logging_metadata.py
--rw-r--r--   0        0        0    22352 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1727 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33787 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8962 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    25880 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3825 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     3949 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    48455 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     5323 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
--rw-r--r--   0        0        0     4903 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17832 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
--rw-r--r--   0        0        0     8956 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/directory_paths.txt
--rw-r--r--   0        0        0      827 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/__init__.py
--rw-r--r--   0        0        0     7250 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/github_secret.py
--rw-r--r--   0        0        0     1707 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/__init__.py
--rw-r--r--   0        0        0     6295 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/jira_client.py
--rw-r--r--   0        0        0       44 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/output.txt
--rw-r--r--   0        0        0      869 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/__init__.py
--rw-r--r--   0        0        0    21086 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/posit_connect.py
--rw-r--r--   0        0        0      825 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/python_client.py
--rw-r--r--   0        0        0    15021 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/requirements.txt
--rw-r--r--   0        0        0      832 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/windows_credential.py
--rw-r--r--   0        0        0    11357 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/license.md
--rw-r--r--   0        0        0     3914 2023-07-21 03:15:32.962769 data_ecosystem_services-202307.0.5/pyproject.toml
--rw-r--r--   0        0        0    52292 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/readme.md
--rw-r--r--   0        0        0      130 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/setup.py
--rw-r--r--   0        0        0    55802 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.5/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-24 15:19:54.886852 data_ecosystem_services-202307.0.6/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1264 2023-07-24 15:19:54.886852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/column.py
+-rw-r--r--   0        0        0    25117 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0    13816 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     2037 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    11758 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/excelmetadata.py
+-rw-r--r--   0        0        0      566 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     7568 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    16676 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    10973 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0    55031 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     7368 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/table.py
+-rw-r--r--   0        0        0     1486 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    25982 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0     1044 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4570 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     8967 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    15940 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8398 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21410 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40188 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1727 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33787 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25880 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3825 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    50039 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5323 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4903 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-07-24 15:19:54.890852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0     8956 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/directory_paths.txt
+-rw-r--r--   0        0        0      827 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7250 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0     1707 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6295 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0       44 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/output.txt
+-rw-r--r--   0        0        0      869 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    21086 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    15021 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0      832 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-24 15:19:54.894852 data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0    11357 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/license.md
+-rw-r--r--   0        0        0     3914 2023-07-24 15:22:32.315117 data_ecosystem_services-202307.0.6/pyproject.toml
+-rw-r--r--   0        0        0    52428 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/readme.md
+-rw-r--r--   0        0        0      129 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-24 15:19:54.898852 data_ecosystem_services-202307.0.6/setup.py
+-rw-r--r--   0        0        0    55938 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.6/PKG-INFO
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/column.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/column.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,45 @@
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 # Default limit item number of items to retrieve
 LIMIT = 500
 
 
 class EdcAlationError(Exception):
+    """
+    This class is a custom exception class for handling errors related to EdcAlation.
+
+    It inherits from the built-in Exception class in Python and extends it by providing a custom message.
+
+    Attributes
+    ----------
+    message : str
+        The error message to be displayed when the exception is raised.
+
+    Methods
+    -------
+    __init__(self, message):
+        Constructs a new 'EdcAlationError' object.
+
+    Parameters
+    ----------
+    message : str
+        The error message to be displayed when the exception is raised.
+    """
+
     def __init__(self, message):
+        """
+        Constructs a new 'EdcAlationError' object.
+
+        Parameters
+        ----------
+        message : str
+            The error message to be displayed when the exception is raised.
+        """
+        self.message = message
         super().__init__(message)
 
 
 class CustomFieldsEndpoint():
     """
     A class for interacting with the bulk metadata upload from the Alation API.
     """
@@ -168,24 +198,21 @@
             parameters['table_name'] = table_name
         if column:
             parameters['name'] = column
         parameters['limit'] = LIMIT
 
         return parameters
 
-    def get_object_by_key(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key):
+    def get_custom_fields(self, edc_alation_api_token, edc_alation_base_url):
         """
         Retrieves data from a specified API endpoint.
 
         Args:
             edc_alation_api_token (str): The API token for authentication.
             edc_alation_base_url (str): The base URL of the API.
-            object_type (str): The type of object to retrieve.
-            alation_datasource_id (int): The ID of the data source.
-            key (str): The key used for retrieval.
 
         Returns:
             dict: A dictionary containing the retrieved data.
 
         Raises:
             EdcAlationError: If there is an error during the retrieval process.
         """
@@ -193,43 +220,27 @@
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span("get_objet_by_key"):
+        with tracer.start_as_current_span("get_custom_fields"):
             try:
-
-                # Check if the alation_datasource_id is an integer
-                if not isinstance(alation_datasource_id, int):
-                    raise EdcAlationError(
-                        "alation_datasource_id must be an integer.")
-
-                # Remove the data source ID from the key if it exists to avoid duplicate data source ID
-                key = key.replace(str(alation_datasource_id) + ".", "")
-
-                # Add the data source ID to the key
-                full_key = f"{alation_datasource_id}.{key}"
-
-                # Check if the key contains special characters
-                if self.has_special_chars(full_key):
-                    logger.warning(
-                        f"The following submitted key contains special characters: {str(full_key)}")
+                params = {"limit": "1000"}
 
                 # Create headers
                 headers = {'Token': edc_alation_api_token,
-                           'Content-Type': 'application/json',
                            'Accept': 'application/json',
                            'cache-control': "no-cache"
                            }
 
-                params = self.parse_key(full_key)
                 obj_http = pade_env_http.EnvironmentHttp()
                 metadata_endpoint = '/integration/v2'
+                object_type = 'custom_field'
                 api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
                 response_custom = obj_http.get(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=params)
 
                 response_custom.raise_for_status()
 
                 custom_result = response_custom.json()
@@ -252,20 +263,20 @@
                     error_message = "No objects updated or created"
                     raise EdcAlationError(
                         f"Errors occurred: {error_message}: api_url {api_url} : params {params}")
 
                 return custom_result
 
             except Exception as ex:
-                error_msg = f"Error: {str(ex)} : {str(key)}: {str(object_type)}"
+                error_msg = f"Error: {str(ex)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    def get_custom_by_key(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key):
+    def get_object_by_key(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key):
         """
         Retrieves data from a specified API endpoint.
 
         Args:
             edc_alation_api_token (str): The API token for authentication.
             edc_alation_base_url (str): The base URL of the API.
             object_type (str): The type of object to retrieve.
@@ -282,15 +293,15 @@
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span("get_custom_by_key"):
+        with tracer.start_as_current_span("get_object_by_key"):
             try:
 
                 # Check if the alation_datasource_id is an integer
                 if not isinstance(alation_datasource_id, int):
                     raise EdcAlationError(
                         "alation_datasource_id must be an integer.")
 
@@ -308,40 +319,45 @@
                 # Create headers
                 headers = {'Token': edc_alation_api_token,
                            'Content-Type': 'application/json',
                            'Accept': 'application/json',
                            'cache-control': "no-cache"
                            }
 
-                data = {"key": full_key}
-                metadata_endpoint = '/api/v1/bulk_metadata/custom_fields/default'
+                params = self.parse_key(full_key)
+                obj_http = pade_env_http.EnvironmentHttp()
+                metadata_endpoint = '/integration/v2'
                 api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
-                response_custom = requests.post(
-                    api_url, headers=headers, timeout=REQUEST_TIMEOUT, json=data)
+                response_custom = obj_http.get(
+                    api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=params)
 
                 response_custom.raise_for_status()
+
                 custom_result = response_custom.json()
                 number_received = custom_result.get('number_received')
                 logger.info(f"number_received: {number_received}")
                 updated_objects = custom_result.get('updated_objects')
-                logger.info(f"updated_objects: {updated_objects}")
                 new_objects = custom_result.get('new_objects')
-                logger.info(f"new_objects: {new_objects}")
                 error_objects = custom_result.get('error_objects')
                 if error_objects and len(error_objects) > 0:
                     error_message = ', '.join(str(e)
                                               for e in error_objects)
                     raise EdcAlationError(
-                        f"Errors occurred: {error_message}: api_url {api_url}")
+                        f"Errors occurred: {error_message}: api_url {api_url} : params {params}")
                 error = custom_result.get('error')
                 if len(error) > 0:
                     raise EdcAlationError(
-                        f"Errors occurred: {error}: api_url {api_url} ")
+                        f"Errors occurred: {error}: api_url {api_url}  : params {params}")
 
-                return response_custom
+                if updated_objects == 0 and new_objects == 0:
+                    error_message = "No objects updated or created"
+                    raise EdcAlationError(
+                        f"Errors occurred: {error_message}: api_url {api_url} : params {params}")
+
+                return custom_result
 
             except Exception as ex:
                 error_msg = f"Error: {str(ex)} : {str(key)}: {str(object_type)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
@@ -367,19 +383,19 @@
         """
 
         if key.startswith("\"") and key.endswith("\""):
             return key  # Key is already wrapped
 
         return f"\"{key}\""  # Wrap the key with double quotes
 
-    def get_data(self, u):
+    def get_data(self, object_to_update):
         """Get data from an object or its 'get_alation_data' method.
 
         Args:
-            u: The object from which to retrieve the data.
+            object_to_update: The object from which to retrieve the data.
 
         Returns:
             str: JSON representation of the data.
 
         This function retrieves data from the provided object 'u' by either calling its
         'get_alation_data' method (if available) or directly using the object itself.
         The retrieved data is then returned as a JSON string.
@@ -400,25 +416,25 @@
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_data"):
             try:
 
                 # If the object has a get_alation_data method, use it to get the data
-                if hasattr(u, 'get_alation_data'):
-                    data = u.get_alation_data()
+                if hasattr(object_to_update, 'get_alation_data'):
+                    data = object_to_update.get_alation_data()
                 # Otherwise, just use the object itself
                 else:
-                    data = u
+                    data = object_to_update
                 return json.dumps(data)
             except Exception as ex:
-                error_msg = "Error: %s : %s", ex, str(u)
+                error_msg = "Error: %s : %s", ex, str(object_to_update)
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
-                raise EdcAlationError(error_msg)
+                raise
 
     def update(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key, fields, force_submit):
         """
         Update business metadata on an object in Alation.
 
         Parameters
         ----------
@@ -477,22 +493,22 @@
                 # If the fields is a dictionary, then it is already processed
                 if isinstance(fields, dict):
                     processed_fields = {k: v for k, v in fields.items()}
                 else:
                     raise EdcAlationError(
                         f"Errors occurred and cannot process object because it is missing get_alation_data: {str(fields)}")
 
-                # Remove the data source ID from the key if it exists to avoid duplicate data source ID
+                # Remove the datasource id from the key if it exists to avoid duplicate datasource id
                 key = key.replace(str(alation_datasource_id) + ".", "")
 
-                if object_type == 'schema':
+                if object_type == 'schema' and '.' in key:
                     key = self.wrap_with_quotes(key)
                     # key = key.replace('.', '%2E')
 
-                # Add the data source ID to the key
+                # Add the datasource id to the key
                 full_key = f"{alation_datasource_id}.{key}"
 
                 # Check if the key contains special characters
                 if self.has_special_chars(full_key):
                     logger.warning(
                         f"The following submitted key contains special characters: {str(full_key)}")
 
@@ -502,80 +518,88 @@
 
                 params = {
                     "create_new": "false",
                     "replace_values": "true"
                 }
 
                 # Add the key to the fields
-                single_update = {
-                    "key": full_key, **processed_fields}
+                single_update = {"key": full_key, **processed_fields}
+                logger.info(f"single_update: {single_update}")
                 self.updates.append(single_update)
 
                 # Submit the updates if the batch size is reached or if force_submit is True
                 if len(self.updates) >= batch_size or force_submit:
                     # Create the request body with array if needed
-                    array_of_json = [json.dumps(u) for u in self.updates]
+                    data = ""
+                    array_of_json = [json.dumps(
+                        u, separators=(',', ':')) for u in self.updates]
                     if len(array_of_json) > 1:
-                        request_body = "[" + ", ".join(array_of_json) + "]"
-                        # request_body = ", ".join(array_of_json)
+                        data = ",".join(array_of_json)
+                        data = "[" + data + "]"
                     else:
-                        request_body = array_of_json[0]
+                        data = array_of_json[0]
 
                     # Validate json
                     try:
-                        # Parse the request_body to check for JSON parsing errors
-                        data = json.loads(request_body)
+                        # Parse the data to check for JSON parsing errors
+                        data_json = json.loads(data)
                         logger.info(
-                            f"Successfully parsed request_body: {len(data)}")
+                            f"Successfully parsed data_json: {len(data_json)}")
                     except json.JSONDecodeError as ex:
-                        error_msg = f"Error parsing request_body: {ex} : {request_body}"
+                        error_msg = f"Error parsing data_json: {ex} : {data}"
                         logger.error(error_msg)
-                        raise EdcAlationError(error_msg)
+                        raise
+
+                    # data = json.dumps(data_json, separators=(',', ':'))
+                    # =data = "\n".join(json.dumps(item, separators=(',', ':'))
+                    #                 for item in self.updates)
+                    data_str = '\n'.join(json.dumps(item)
+                                         for item in self.updates)
 
                     # submit the batch
                     logger.info(
                         f"Submitting {object_type} batch")
                     metadata_endpoint = '/api/v1/bulk_metadata/custom_fields/default'
                     api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
 
                     # Create headers
-                    headers = {"TOKEN": edc_alation_api_token,
-                               "Token": edc_alation_api_token,
-                               "content-type": 'application/json'}
+                    headers = {"Token": edc_alation_api_token,
+                               "Content-Type": "application/json",
+                               "accept": 'application/json'}
 
-                    # Submit the updates using the constructed URL and request_body
+                    # Submit the updates using the constructed URL and data
                     response = requests.post(
-                        api_url, headers=headers, json=data, params=params, verify=True, timeout=REQUEST_TIMEOUT)
+                        api_url, headers=headers, data=data_str, params=params, verify=True, timeout=REQUEST_TIMEOUT)
                     response_json = response.json()
 
                     # Clear updates after submission
                     self.updates = []
                     logger.info(
-                        f"Response Status {object_type} batch of {request_body}")
+                        f"Response Status {object_type} batch of {data}")
                     response.raise_for_status()
                     result = response_json
                     number_received = result.get('number_received')
                     logger.info(f"number_received: {number_received}")
                     updated_objects = result.get('updated_objects')
                     new_objects = result.get('new_objects')
                     error_objects = result.get('error_objects')
                     if error_objects and len(error_objects) > 0:
                         error_message = ', '.join(str(e)
                                                   for e in error_objects)
                         raise EdcAlationError(
-                            f"Errors occurred: {error_message}: api_url {api_url} : request_body {request_body}")
+                            f"Errors occurred: {error_message}: api_url {api_url} : data {data}")
                     error = result.get('error')
                     if len(error) > 0:
                         raise EdcAlationError(
-                            f"Errors occurred: {error}: api_url {api_url} : request_body {request_body}")
+                            f"Errors occurred: {error}: api_url {api_url} : data {data}")
 
                     if updated_objects == 0 and new_objects == 0:
                         error_message = "No objects updated or created"
                         raise EdcAlationError(
-                            f"Errors occurred: {error_message}: api_url {api_url} : request_body {request_body}")
+                            f"Errors occurred: {error_message}: api_url {api_url} : data {data}")
 
                     return {"status": "success", "message": "Batch complete"}, response_json
                 else:
                     return {"status": "success", "message": "Batch not submitted"}, {"number_of_updates", len(self.updates), "batch_size", batch_size, "force_submit", force_submit}
 
             except Exception as ex:
                 error_msg = f"Error: {str(ex)} : {str(key)}: {str(fields)}"
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("update_datasource"):
 
             try:
 
                 # Must use v1 of the API - v2 returns a 404
-                api_url = f"{edc_alation_base_url}/integration/v1/datasource/{str(alation_datasource_id)}/"
+                api_url = f"{edc_alation_base_url}/integration/v2/datasource/{str(alation_datasource_id)}"
 
                 # Set the headers for the API request
                 headers = {"accept": "application/json",
                            "content-type": "application/json",
                            "Token": edc_alation_api_token}
                 # Intentionally not set
                 response_datasource_text = "not_set"
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/excelmetadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/excelmetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import os
 import sys
 import pandas as pd
 import numpy as np
 import xlsxwriter
-from openpyxl.utils import get_column_letter
+
 
 from data_ecosystem_services.cdc_admin_service import (
     environment_tracing as pade_env_tracing,
     environment_logging as pade_env_logging
 )
 
 from .tokenendpoint import TokenEndpoint
-from .customfieldsendpoint import CustomFieldsEndpoint
-from .tagsendpoint import TagsEndpoint
-from .idfinderendpoint import IdFinderEndpoint
-from .datasource import DataSource
-from .manifest import Manifest
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 TIMEOUT_ONE_MIN = 60  # or set to whatever value you want
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/execution_session.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/execution_session.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,45 +189,42 @@
             description += '<br><table><tr><th>Field</th><th>Value</th></tr>'
             for key in self.extra_description_fields:
                 description += '<tr><td>' + key + '</td><td>' + \
                     self.extra_description_fields[key] + '</td></tr>'
             description += '</table>'
         return description
 
-    def get_alation_data(self):
+    def get_schema_data(self):
         """
-        Retrieves Alation data from the Manifest object.
+        Retrieves Alation schema data from the Manifest object.
 
         Returns:
-            dict: A dictionary containing Alation data extracted from the Manifest.
+            dict: A dictionary containing Alation schema data extracted from the Manifest.
 
         Raises:
             Exception: If an error occurs while retrieving the Alation data.
 
         """
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span("get_alation_data"):
+        with tracer.start_as_current_span("get_schema_data"):
             try:
                 data = {}
                 data['title'] = self.title
                 data['description'] = self.format_description()
-                # data['description']     = self.description
                 # data['Release Date']    = self.releasedate
                 data['Homepage URL'] = self.homepageUrl
                 data['Identifier'] = self.identifier
                 # data['Format']          = self.dataformat
                 data['License'] = self.license
-
                 # arrays
                 # data['tags']            = self.tags
                 # data['Language']        = self.language
                 data['Is Referenced By'] = self.referencedBy
                 data['Geographic Coverage'] = self.geographicCoverage
                 data['Temporal Applicability'] = self.temporalApplicability
                 data['References'] = self.references
@@ -369,40 +366,40 @@
             FileNotFoundError: If the specified schema file does not exist.
             JSONDecodeError: If the schema file is not a valid JSON.
 
         """
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_manifest_expected_fields"):
-
             try:
-
                 schema_file_path = open(
                     self.schema_file_path, encoding="utf-8")
                 schema = json.load(schema_file_path)
                 schema_fields = {}
                 table_fields = {}
                 column_fields = {}
-                for p in schema['properties']:
+                for prop_field in schema['properties']:
                     # do not add properties blank_field_examples for tables, columns, this info will be extracted from alation obj strucutre
-                    if p not in ["tables", "columns"]:
-                        schema_fields[p] = schema['properties'][p].get(
+                    if prop_field not in ["tables", "columns"]:
+                        schema_fields[prop_field] = schema['properties'][prop_field].get(
                             'blank_field_examples')
-                for p in schema['$defs']['table']['properties']:
+                for prop_field in schema['$defs']['table']['properties']:
                     # do not add properties blank_field_examples for tables, columns, this info will be extracted from alation obj strucutre
-                    if p not in ["columns"]:
-                        table_fields[p] = schema['$defs']['table']['properties'][p]['blank_field_examples']
-                for p in schema['$defs']['column']['properties']:
-                    column_fields[p] = schema['$defs']['column']['properties'][p]['blank_field_examples']
-                return schema_fields, table_fields, column_fields
+                    if prop_field not in ["columns"]:
+                        table_fields[prop_field] = schema['$defs']['table']['properties'][prop_field]['blank_field_examples']
+                for prop_field in schema['$defs']['column']['properties']:
+                    column_fields[prop_field] = schema['$defs']['column']['properties'][prop_field]['blank_field_examples']
+
+                table_required_fields = schema['$defs']['table']['required']
+
+                return schema_fields, table_fields, column_fields, table_required_fields
 
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,14 @@
-from io import BytesIO
-
-from opentelemetry import trace
-from azure.storage.queue import QueueServiceClient, QueueClient, BinaryBase64EncodePolicy, BinaryBase64DecodePolicy
-from urllib.parse import quote
-
 import requests
 import json
-import traceback
 import os
 import sys
 import concurrent.futures
 import platform
 import datetime
-import openpyxl
-from openpyxl.utils import get_column_letter
-from io import BytesIO
-import xlsxwriter
-import pandas as pd
-
-
 from .tokenendpoint import TokenEndpoint
 from .customfieldsendpoint import CustomFieldsEndpoint
 from .tagsendpoint import TagsEndpoint
 from .idfinderendpoint import IdFinderEndpoint
 from .datasource import DataSource
 from .manifest import Manifest
 
@@ -32,18 +18,14 @@
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
     environment_file as pade_env_file,
     environment_http as pade_env_http
 )
 
-from data_ecosystem_services.az_storage_service import (
-    az_storage_queue as pade_az_storage_queue
-)
-
 import data_ecosystem_services.alation_service.excelmetadata as alation_excelmetadata
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 TIMEOUT_ONE_MIN = 60  # or set to whatever value you want
@@ -57,14 +39,20 @@
 else:
     NUM_THREADS_MAX = 4
 
 ENCODE_PERIOD = False
 REQUEST_TIMEOUT = 45
 
 
+class EdcAlationError(Exception):
+    def __init__(self, message):
+        self.message = message
+        super().__init__(message)
+
+
 class Schema:
     """
     A base class for interacting with Alation Schema. 
     """
 
     @staticmethod
     def get_schema(edc_alation_api_token, edc_alation_base_url, alation_schema_id):
@@ -129,31 +117,32 @@
                     datasource_id = -1
                     if "title" in schema_result:
                         datasource_id = schema_result.get("ds_id")
                         pade_datasource = DataSource()
                         response_datasource = pade_datasource.get_datasource(
                             edc_alation_api_token, edc_alation_base_url, datasource_id)
                         datasource_result = response_datasource.json()
-                        return schema_result, datasource_result
+                        return response_schema, datasource_result
                     else:
                         response_schema_text = schema_result.get("reason")
                         error_msg = "Failed to get schema:" + \
                             str(response_schema_text)
                         error_msg = error_msg + \
                             " for api_url: " + str(api_url)
                         error_msg = error_msg + \
                             " for schema_id: " + str(schema_id)
                         error_msg = error_msg + \
                             " and datasource_id: " + str(datasource_id)
                         error_msg = error_msg + \
                             " and schema_result: " + str(schema_result)
                         logger.error(error_msg)
-                        raise ValueError(error_msg)
+                        raise EdcAlationError(error_msg)
                 else:
-                    raise ValueError("Failed to get schema_result")
+                    error_msg = "Failed to get schema_result"
+                    raise EdcAlationError(error_msg)
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
@@ -169,15 +158,14 @@
 
         Returns:
             list: List of tables in the schema. Each table is represented as a dictionary.
         """
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
         with tracer.start_as_current_span("get_schema_tables"):
 
             try:
 
@@ -340,34 +328,34 @@
 
         with tracer.start_as_current_span("get_manifest_excel_file_name"):
             try:
 
                 # Get current time
                 current_date = datetime.datetime.now()
 
-                yyyy = current_date.year
-                mm = current_date.month
-                dd = current_date.day
+                yyyy_string = current_date.year
+                mm_string = current_date.month
+                dd_string = current_date.day
                 # Format as a 24-hour time string
                 time_str = current_date.strftime("%H_%M_%S")
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
                 obj_file = pade_env_file.EnvironmentFile()
 
                 file_name = (
                     obj_file.scrub_file_name(datasource_title)
                     + "_"
                     + obj_file.scrub_file_name(schema_name)
-                    + str(yyyy)
+                    + str(yyyy_string)
                     + "_"
-                    + str(mm)
+                    + str(mm_string)
                     + "_"
-                    + str(dd)
+                    + str(dd_string)
                     + "_"
                     + str(time_str)
                     + "_" + str(alation_user_id) + "_" +
                     upload_or_download + ".xlsx"
                 )
 
                 right_most_200_chars = file_name[-200:]
@@ -382,15 +370,16 @@
                 logger.info("manifest_path: " + manifest_path)
 
                 manifest_excel_file = manifest_path + file_name
                 logger.info("manifest_excel_file: " + manifest_excel_file)
 
                 return manifest_excel_file
             except Exception as ex:
-                error_msg = "Excel Error: %s" % ex  # Corrected error message formatting
+                # Corrected error message formatting
+                error_msg = f"Excel Error: {str(ex)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
     def get_manifest_json_file_name(upload_or_download, repository_path, datasource_title, schema_name, environment, alation_user_id):
         """Get the file name for the manifest JSON file.
@@ -416,17 +405,17 @@
 
         with tracer.start_as_current_span("get_manifest_file_name"):
             try:
 
                 # Get current time
                 current_date = datetime.datetime.now()
 
-                yyyy = current_date.year
-                mm = current_date.month
-                dd = current_date.day
+                yyyy_string = current_date.year
+                mm_string = current_date.month
+                dd_string = current_date.day
                 # Format as a 24-hour time string
                 time_str = current_date.strftime("%H_%M_%S")
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
                 obj_file = pade_env_file.EnvironmentFile()
@@ -438,19 +427,19 @@
 
                 logger.info("manifest_path: " + manifest_path)
 
                 file_name = (
                     obj_file.scrub_file_name(datasource_title)
                     + "_"
                     + obj_file.scrub_file_name(schema_name)
-                    + str(yyyy)
+                    + str(yyyy_string)
                     + "_"
-                    + str(mm)
+                    + str(mm_string)
                     + "_"
-                    + str(dd)
+                    + str(dd_string)
                     + "_"
                     + str(time_str)
                     + "_" + str(alation_user_id) + "_" +
                     upload_or_download + ".json"
                 )
 
                 right_most_200_chars = file_name[-200:]
@@ -467,24 +456,46 @@
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @classmethod
     def download_schema_manifest_excel_file(cls, alation_schema_id, config):
+        """
+        Downloads the schema manifest Excel file for a given Alation schema ID.
+
+        This method generates the Excel file data using the `generate_excel_file_data` method of the 
+        `alation_excelmetadata.ExcelMetadata` class, then generates the Excel file using the 
+        `generate_excel_file_from_data` method of the same class.
+
+        Parameters
+        ----------
+        alation_schema_id : int
+            The ID of the Alation schema for which to download the manifest Excel file.
+        config : dict
+            The configuration parameters for the operation.
+
+        Returns
+        -------
+        str
+            The path to the downloaded manifest Excel file.
+
+        Raises
+        ------
+        Exception
+            If an error occurs during the operation, an exception is raised and logged.
+        """
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        schema_name = None
-
         with tracer.start_as_current_span("download_schema_manifest"):
 
             try:
                 logger.info("alation_schema_id: " + str(alation_schema_id))
 
                 excelmetadata = alation_excelmetadata.ExcelMetadata()
                 df_schema, df_table_list, df_table_raw, df_table_transposed, manifest_excel_file = excelmetadata.generate_excel_file_data(
@@ -649,15 +660,14 @@
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("upload_schema_manifest"):
-
             try:
 
                 # Get the configuration data
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 # Format as a 24-hour time string
                 repository_path = config.get("repository_path")
                 environment = config.get("environment")
@@ -702,16 +712,14 @@
                     manifest_json_file)
                 logger.info(msg)
 
                 manifest = Manifest(schema_file_path)
                 metadata = manifest.validate_manifest(manifest_json_file)
                 logger.info(
                     f"Metadata File Validated file of length {str(len(metadata))}")
-                manifest_updates_list = {}
-                manifest_updates_list['tables'] = []
 
                 # Update based on Manifest file
                 if token_endpoint.validate_refresh_token(alation_user_id, alation_refresh_token) is not None:
 
                     custom_fields_endpoint = CustomFieldsEndpoint()
                     logger.info(
                         'Created custom fields endpoint for updating custom fields via API')
@@ -721,64 +729,82 @@
                     logger.info(
                         'Created tags endpoint for updating tags via API')
 
                     id_finder_endpoint = IdFinderEndpoint(
                         edc_alation_api_token, edc_alation_base_url)
 
                     # encode key
-                    if ENCODE_PERIOD:
-                        encoded_schema_name = quote(schema_name)
-                        encoded_schema_name = encoded_schema_name.replace(
-                            ".", "%2E")
+                    # always encode schema name regardless of ENCODE_PERIOD
+                    if '.' in schema_name:
+                        encoded_schema_name = f"\"{schema_name}\""
                     else:
                         encoded_schema_name = schema_name
 
                     # Update the schema
                     logger.info(
                         'Created id finder for getting detailed information on Alation objects')
                     logger.info('Updating the schema fields for data source {0} and schema {1}'.format(
                         alation_data_source_id, schema_name))
+
+                    schema = manifest.get_schema_data()
                     response_content = custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url,
-                                                                     "schema", alation_data_source_id, encoded_schema_name, manifest.get_alation_data(), True)
+                                                                     "schema", alation_data_source_id, encoded_schema_name, schema, True)
+                    logger.info("response_content: " + str(response_content))
                     schema_key = str(alation_data_source_id) + \
-                        "_" + encoded_schema_name
+                        "." + encoded_schema_name
                     schema_id = id_finder_endpoint.find('schema', schema_key)
                     for tag in manifest.tags:
                         tags_endpoint.apply('schema', schema_id, tag)
 
                     # Update the tables
                     tables_dict = manifest.get_tables_data()
                     if tables_dict:
-                        # The number of threads you want to use
-                        num_threads = min(NUM_THREADS_MAX, len(tables_dict))
+                        total_items = len(tables_dict.items())
+                        # reinit endpoint
+                        obj_custom_fields_endpoint = CustomFieldsEndpoint()
+
+                        for idx, (key, value) in enumerate(tables_dict.items()):
+                            # Set force_submit to True on the last item
+                            force_submit = (idx == total_items - 1)
+                            table_result = cls.update_table_structure(edc_alation_api_token,
+                                                                      edc_alation_base_url, alation_data_source_id, schema_name,
+                                                                      value, force_submit=force_submit, obj_custom_fields_endpoint=obj_custom_fields_endpoint)
+                            logger.info("table_result: " + str(table_result))
+                        # Commented out the threading because complexity not worth it
+                        # compared to batching updates in sets of 50
+                        # and limiting updates to differences
+
+                        # num_threads = min(NUM_THREADS_MAX, len(tables_dict))
 
                         # Using ThreadPoolExecutor
-                        with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
-                            futures = []
-                            items = list(tables_dict.items())
-                            total_items = len(items)
-
-                            for idx, (key, value) in enumerate(items):
-                                # Set force_submit to True on the last item
-                                force_submit = (idx == total_items - 1)
-                                future = executor.submit(cls.update_table_structure, edc_alation_api_token,
-                                                         edc_alation_base_url, alation_data_source_id, schema_name,
-                                                         value, force_submit=force_submit)
-                                futures.append(future)
+                        # with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+                        #    futures = []
+                        #    items = list(tables_dict.items())
+                        #    total_items = len(items)
 
-                        # Wait for all futures to complete
-                        concurrent.futures.wait(futures)
+                            # for idx, (key, value) in enumerate(items):
+                            # Set force_submit to True on the last item
 
-                    else:
-                        raise Exception(ValueError, "No tables found")
+                            #    future = executor.submit(cls.update_table_structure, edc_alation_api_token,
+                            #                             edc_alation_base_url, alation_data_source_id, schema_name,
+                            #                             value, force_submit=force_submit)
+                            #    futures.append(future)
 
-                return manifest_updates_list
+                        # Wait for all futures to complete
+                        # concurrent.futures.wait(futures)
+                        return tables_dict
 
+                    else:
+                        error_msg = "No tables found"
+                        raise EdcAlationError(error_msg)
+                else:
+                    error_msg = "Refresh token is not valid"
+                    raise EdcAlationError(error_msg)
             except Exception as ex:
-                error_msg = f"Error: {str(ex)}",
+                error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
     def get_column_name(schema_name, table_name, column):
         """
@@ -808,16 +834,16 @@
                 return full_column_name
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    @classmethod
-    def update_table_structure(cls, edc_alation_api_token, edc_alation_base_url, alation_data_source_id, schema_name, table, force_submit):
+    @staticmethod
+    def update_table_structure(edc_alation_api_token, edc_alation_base_url, alation_data_source_id, schema_name, table, force_submit, obj_custom_fields_endpoint):
         """
         Updates the structure of a table in Alation.
 
         This method updates the table information, applies tags to the table, and
         updates the columns of the table. It uses Alation's custom fields API
         endpoint for updating the table and columns and applies tags using Alation's
         tags API endpoint.
@@ -840,47 +866,66 @@
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
         with tracer.start_as_current_span("upload_schema_manifest"):
 
             try:
 
-                custom_fields_endpoint = CustomFieldsEndpoint()
                 id_finder_endpoint = IdFinderEndpoint(
                     edc_alation_api_token, edc_alation_base_url)
                 tags_endpoint = TagsEndpoint(
                     edc_alation_api_token, edc_alation_base_url)
 
                 logger.info('Updating table {}'.format(table.name))
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
-                # Update the table
-                if ENCODE_PERIOD:
+                # encode the schema
+                if '.' in schema_name and ENCODE_PERIOD:
                     encoded_schema_name = f"\"{schema_name}\""
                 else:
                     encoded_schema_name = schema_name
 
+                # encode the table
+                special_chars = set('!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
                 table_name = table.name
-                if ENCODE_PERIOD:
-                    encoded_table_name = quote(table_name)
-                    encoded_table_name = encoded_table_name.replace(
-                        ".", "%2E")
+                if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
+                    encoded_table_name = f"\"{table_name}\""
                 else:
                     encoded_table_name = table_name
 
                 key = f"{encoded_schema_name}.{encoded_table_name}"
-                response_content = custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url, "table",
-                                                                 alation_data_source_id,
-                                                                 key,
-                                                                 table, force_submit=force_submit)
+                # Update the table
+                # Should only be one - ensure force_submit
+                response_content = obj_custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url, "table",
+                                                                     alation_data_source_id,
+                                                                     key,
+                                                                     table, force_submit=True)
+
+                last_result = response_content
+                logger.info(f"response_content: {response_content}")
 
                 # Update the tags
+                # Encode ignoring ENCODE_PERIOD
+                # encode the schema
+                if '.' in schema_name:
+                    encoded_schema_name = f"\"{schema_name}\""
+                else:
+                    encoded_schema_name = schema_name
+
+                table_name = table.name
+                if '.' in table_name:
+                    encoded_table_name = f"\"{table_name}\""
+                else:
+                    encoded_table_name = table_name
+
                 table_key = f"{alation_data_source_id}.{encoded_schema_name}.{encoded_table_name}"
+
+                # Apply tags to the table
                 if table.tags is not None:
                     table_id = id_finder_endpoint.find(
                         'table', table_key)
                     for table_tag in table.tags:
                         tags_endpoint.apply(
                             'table', table_id, table_tag)
 
@@ -890,53 +935,69 @@
 
                 # Update the columns
                 if columns_dict is not None:
 
                     # Using ThreadPoolExecutor
                     num_threads = min(NUM_THREADS_MAX, len(columns_dict))
 
-                    if ENCODE_PERIOD:
-                        encoded_schema_name = quote(schema_name)
-                        encoded_schema_name = encoded_schema_name.replace(
-                            ".", "%2E")
+                    if '.' in schema_name and ENCODE_PERIOD:
+                        encoded_schema_name = f"\"{schema_name}\""
                     else:
-                        encoded_schema_name = table_name
+                        encoded_schema_name = schema_name
+
+                    special_chars = set('!"#$%&\'()*+,-./:;<=>?@[\]^_`{}~')
 
                     table_name = table.name
-                    if ENCODE_PERIOD:
-                        encoded_table_name = quote(table_name)
-                        encoded_table_name = encoded_table_name.replace(
-                            ".", "%2E")
+                    if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
+                        encoded_table_name = f"\"{table_name}\""
                     else:
                         encoded_table_name = table_name
 
                     with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+                        last_future_result = ""
                         futures = []
-                        items = list(columns_dict.items())
-                        total_items = len(items)
+                        total_items = len(columns_dict.items())
+                        special_chars = set(
+                            '!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
 
-                        for idx, (key, value) in enumerate(items):
+                        for idx, (key, value) in enumerate(columns_dict.items()):
                             # Set force_submit to True on the last item
                             force_submit = (idx == total_items - 1)
-                            encoded_column_name = quote(key)
-                            encoded_column_name = encoded_column_name.replace(
-                                ".", "%2E")
+                            if any(char in special_chars for char in key) and ENCODE_PERIOD:
+                                encoded_column_name = f"\"{key}\""
+                            else:
+                                encoded_column_name = key
 
-                            future = executor.submit(custom_fields_endpoint.update, "attribute",
+                            future = executor.submit(obj_custom_fields_endpoint.update, edc_alation_api_token, edc_alation_base_url, "attribute",
                                                      alation_data_source_id,
                                                      f"{encoded_schema_name}.{encoded_table_name}.{encoded_column_name}",
                                                      value, force_submit=force_submit)
                             futures.append(future)
 
-                    # Wait for all futures to complete
-                    concurrent.futures.wait(futures)
-                return "OK"
+                        # Wait for all futures to complete
+                        concurrent.futures.wait(futures)
+
+                        # Retrieve the result of the last future
+                        if futures:
+                            last_future_result = futures[-1].result()
+                        else:
+                            last_future_result = "No return value from last update call"
+
+                        last_result = str(last_result) + \
+                            str(last_future_result)
+
+                else:
+                    warning_msg = f"No columns supplied to update for table: {table_name}"
+                    logger.warning(warning_msg)
+                    last_result = str(last_result) + warning_msg
+
+                return last_result
 
             except Exception as ex:
-                error_msg = "Error: %s", ex
+                error_msg = f"Error: {str(ex)}",
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @classmethod
     def get_table_structure(cls, edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id, unfetched_table, expected_table_fields, expected_column_fields):
         """
@@ -967,14 +1028,15 @@
                 # see if this field is already populated, otherwise use a default value
                 if tf in unfetched_table:
                     fetched_table[tf] = unfetched_table[tf]
                 else:
                     fetched_table[tf] = expected_table_fields[tf]
 
         # iterate through each column associated with this table and add a manifest template entry
+        custom_field_dict = unfetched_table.get('custom_fields')
         alation_table_id = unfetched_table.get('id')
         columns_dict = cls.get_table_columns(
             edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id, alation_table_id)
         if columns_dict:
             fetched_table["columns"] = []
             # for each column associated with this table...
             for c in columns_dict:
@@ -982,14 +1044,23 @@
                 for cf in expected_column_fields:
                     if cf in columns_dict[c]:
                         this_column_dict[cf] = columns_dict[c][cf]
                     else:
                         this_column_dict[cf] = expected_column_fields[cf]
                 fetched_table["columns"].append(
                     this_column_dict)
+            # iterate through each custom_field_dict
+            if custom_field_dict:
+                fetched_table["customfields"] = []
+            # for each custon field associated with this table...
+            for i in custom_field_dict:
+                this_custom_flds_dict = {}
+                this_custom_flds_dict[i['field_name']] = i['value']
+                fetched_table["customfields"].append(
+                    this_custom_flds_dict)
 
         return fetched_table
 
     @classmethod
     def get_schema_structure(cls, edc_alation_api_token, edc_alation_base_url, manifest, alation_data_source_id, alation_schema_id):
         """
         Retrieves the structure of a specific schema from Alation using the provided schema ID and manifest.
@@ -1030,15 +1101,15 @@
                     error_msg = "Error: %s", str(ex_)
                     exc_info = sys.exc_info()
                     logger_singleton.error_with_exception(error_msg, exc_info)
                     raise
 
                 logger.info(f'Info for schema ID: {alation_schema_id}')
                 found_schema = False
-                schema_fields, expected_table_fields, expected_column_fields = manifest.get_manifest_expected_fields()
+                schema_fields, expected_table_fields, expected_column_fields, required_table_fields = manifest.get_manifest_expected_fields()
                 manifest_dict = {}
                 manifest_dict['tables'] = []
 
                 for schema in response_schema_json:
                     logger.info(f"schema_id: {str(schema['id'])}")
                     if schema['id'] == int(alation_schema_id):
                         found_schema = True
@@ -1089,21 +1160,22 @@
                                                              table_info, expected_table_fields, expected_column_fields)
                                     futures[unfetched_table] = future
 
                                 for future in concurrent.futures.as_completed(futures.values()):
                                     manifest_dict["tables"].append(
                                         future.result())
                         else:
-                            raise ValueError("No tables found")
+                            error_msg = "No tables found"
+                            raise EdcAlationError(error_msg)
 
                 if not found_schema:
-                    raise Exception(
-                        "Could not find the schema ID in the list of schemas for this data source")
+                    error_msg = "Could not find the schema ID in the list of schemas for this data source"
+                    raise EdcAlationError(error_msg)
 
                 # Create a JSON structure containing the schema, tables, and columns
                 return manifest_dict
 
         except Exception as ex:
             error_msg = "Error: %s", ex
             exc_info = sys.exc_info()
             logger_singleton.error_with_exception(error_msg, exc_info)
-            raise
+            raise EdcAlationError(error_msg) from ex
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/table.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,29 @@
 
             try:
 
                 self.schema_file_path = schema_file_path
                 manifest = Manifest(schema_file_path)
 
                 # get the expected fields from the manifest
-                schema_fields, expected_table_fields, expected_column_fields = manifest.get_manifest_expected_fields()
+                schema_fields, expected_table_fields, expected_column_fields, required_table_fields = manifest.get_manifest_expected_fields()
 
                 msg = "Schema fields length: " + str(len(schema_fields))
                 logger.info(msg)
                 msg = "Expected table fields length: " + \
                     str(len(expected_column_fields))
                 logger.info(msg)
 
                 # add specified tables fields to the table object and update if necessary
                 for key in expected_table_fields:
                     if key in table_json:
                         setattr(self, key, table_json[key])
 
                 missing_keys = [
-                    key for key in expected_table_fields if not hasattr(self, key)]
+                    key for key in required_table_fields if not hasattr(self, key)]
 
                 if missing_keys:
                     logger.error(f"Missing keys: {missing_keys}")
 
                 # get the extra description fields from the table JSON
                 self.extra_description_fields = self.get_table_extra_description_fields(
                     table_json)
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/azd_client.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_client_service/azd_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/az_key_vault.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_key_vault_service/az_key_vault.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_logging.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_tracing.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_core.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/dataset_metadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/environment_metadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/job_metadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/logging_metadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/pipeline_metadata.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_core.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_file.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """ Module for spark and os environment for cdc_tech_environment_service with
  minimal dependencies. """
 
 # library management
 from importlib import util  # library management
 import subprocess
+import fnmatch
 
 # error handling
 from subprocess import check_output, Popen, PIPE, CalledProcessError
 
 import sys  # don't remove required for error handling
 import os
+import importlib
 
 # files
 import glob
 import json
 import platform
 
 # http
@@ -22,15 +24,14 @@
 
 import data_ecosystem_services.cdc_tech_environment_service.repo_core as pade_repo
 
 # azcopy and adls
 from azure.identity import ClientSecretCredential
 from azure.storage.filedatalake import DataLakeServiceClient
 from azure.storage.filedatalake import DataLakeDirectoryClient
-from azure.keyvault.secrets import SecretClient
 
 # spark
 from pyspark.sql import (SparkSession)
 from pyspark.sql.types import (IntegerType, LongType, StringType, StructField,
                                StructType)
 
 from data_ecosystem_services.cdc_admin_service import (
@@ -95,30 +96,50 @@
         print(f"storage_account:{storage_account}")
         https_path = abfss_path.replace(
             hostname, storage_account + '/' + file_system)
         https_path = https_path.replace('abfss', 'https')
         return https_path
 
     @staticmethod
-    def delete_directory_files(directory, file_extension='*'):
+    def delete_directory_files(directory, file_extension='*', files_to_keep=[]):
+        """
+        Deletes all files in a given directory with a specified extension, except for the files that match patterns in files_to_keep.
 
-        # Join the directory and file_extension with glob pattern
+        Parameters
+        ----------
+        directory : str
+            The directory from which files will be deleted.
+        file_extension : str, optional
+            The extension of the files that will be deleted. By default, all files ('*') will be deleted.
+        files_to_keep : list of str, optional
+            A list of filename patterns to keep. Files that match these patterns will not be deleted, even if their extension matches file_extension.
+            example, files_to_keep=['*.csv', 'important*']
+
+        Returns
+        -------
+        msg : str
+            A message that lists which files have been deleted.
+        """
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("delete_directory_files"):
 
             files = glob.glob(os.path.join(directory, f'*.{file_extension}'))
             msg = ""
             for file in files:
+                # Check if the file matches any of the patterns in the list of files to keep
+                if any(fnmatch.fnmatch(os.path.basename(file), pattern) for pattern in files_to_keep):
+                    continue  # Skip this file
+
                 try:
                     os.remove(file)
                     msg = msg + f"{file} has been deleted\n"
                     logger.info(msg)
 
                 except OSError as e:
                     error_msg = f'Error: {file} : {e}'
@@ -370,15 +391,30 @@
         # Create the .local/bin folder if it doesn't exist
         bin_folder = os.path.join(home_dir, ".local", "bin")
         os.makedirs(bin_folder, exist_ok=True)
 
         return bin_folder
 
     @staticmethod
-    def set_file_metadata(file_path, key, value):
+    def import_xattr():
+        if sys.platform.startswith('linux') or sys.platform == 'darwin':
+            try:
+                xattr_module = importlib.import_module('xattr')
+                return xattr_module
+            except ImportError:
+                print("Unable to import 'xattr'. Please install the 'xattr' package.")
+                # Handle the ImportError or use a fallback method if necessary.
+                return None
+        else:
+            print("The 'xattr' module is not supported on this operating system.")
+            # Handle the case where the module is not supported on the current OS.
+            return None
+
+    @classmethod
+    def set_file_metadata(cls, file_path, key, value):
 
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
@@ -398,15 +434,15 @@
                     win32api.SetFileAttributes(file_path, win32api.GetFileAttributes(
                         file_path) & ~win32con.FILE_ATTRIBUTE_ARCHIVE)
                     win32api.SetFileExtendedAttribute(file_path, key, value)
                     win32api.SetFileAttributes(file_path, win32api.GetFileAttributes(
                         file_path) | win32con.FILE_ATTRIBUTE_ARCHIVE)
 
                 elif sys.platform.startswith('darwin') or sys.platform.startswith('linux'):
-                    import xattr
+                    xattr = cls.import_xattr()
 
                     # Convert the key and value to strings
                     key_str = str(key)
                     value_str = str(value)
 
                     # Encode the key and value as bytes
                     key_bytes = key_str.encode('utf-8')
@@ -723,15 +759,14 @@
 
         credential = ClientSecretCredential(
             tenant_id, client_id, client_secret)
         service_client = DataLakeServiceClient(
             account_url=account_url, credential=credential)
         file_system_client = service_client.get_file_system_client(
             storage_container)
-        directory_client = file_system_client.create_directory(dir_path)
 
         return "True"
 
     @classmethod
     def file_adls_copy(cls, config, source_path: str, destination_path: str, from_to: str, dbutils) -> str:
         """
         Copies a file from the local filesystem to Azure Data Lake Storage (ADLS), or vice versa.
```

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_http.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_http.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/job_core.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/repo_core.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/directory_paths.txt` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/directory_paths.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/github_secret.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/github_service/github_secret.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/jira_client.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/jira_service/jira_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/posit_connect.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/posit_service/posit_connect.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/python_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/requirements.txt` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/__init__.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/windows_credential.py` & `data_ecosystem_services-202307.0.6/data_ecosystem_services/windows_service/windows_credential.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/license.md` & `data_ecosystem_services-202307.0.6/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.5/pyproject.toml` & `data_ecosystem_services-202307.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202307.0.5"
+version="202307.0.6"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202307.0.5/readme.md` & `data_ecosystem_services-202307.0.6/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 Run in bash or powershell
 
 1. Check Python Version
 
         ```sh
         python3 --version
         ```
+        
+        or
+        
+        ```sh
+        python --version
+        ```
+
+    - Ensure it is python 3.9.9
 
 ### Install Python 3.9
 
 #### Run Install Python on Ubuntu or WSL (Primary)
 
         ```sh
         sudo apt update
@@ -38,17 +46,16 @@
         source ~/.bashrc
         ```
   
 #### Run Install Python on windows
 
 Run Application
 
-        ```sh
-        C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
-        ```
+        Download: https://www.python.org/ftp/python/3.9.9/python-3.9.9-embed-amd64.zip
+        Install as a non global user
 
 ### Install Pip
 
 #### Run Install Pip on Ubuntu or WSL (Primary)
 
         ```sh
         sudo apt update
@@ -238,14 +245,15 @@
 ## Run Unit Test Coverage Report
 
 ### Run Unit Test Coverage Report on Ubuntu or WSL (Primary)
 
 Run the following command
 
 ```sh
+cd data_ecosystem_services
 pytest --cov-report html tests/
 ```
 
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
```

### Comparing `data_ecosystem_services-202307.0.5/PKG-INFO` & `data_ecosystem_services-202307.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202307.0.5
+Version: 202307.0.6
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -96,14 +96,22 @@
 Run in bash or powershell
 
 1. Check Python Version
 
         ```sh
         python3 --version
         ```
+        
+        or
+        
+        ```sh
+        python --version
+        ```
+
+    - Ensure it is python 3.9.9
 
 ### Install Python 3.9
 
 #### Run Install Python on Ubuntu or WSL (Primary)
 
         ```sh
         sudo apt update
@@ -118,17 +126,16 @@
         source ~/.bashrc
         ```
   
 #### Run Install Python on windows
 
 Run Application
 
-        ```sh
-        C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
-        ```
+        Download: https://www.python.org/ftp/python/3.9.9/python-3.9.9-embed-amd64.zip
+        Install as a non global user
 
 ### Install Pip
 
 #### Run Install Pip on Ubuntu or WSL (Primary)
 
         ```sh
         sudo apt update
@@ -318,14 +325,15 @@
 ## Run Unit Test Coverage Report
 
 ### Run Unit Test Coverage Report on Ubuntu or WSL (Primary)
 
 Run the following command
 
 ```sh
+cd data_ecosystem_services
 pytest --cov-report html tests/
 ```
 
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
```

