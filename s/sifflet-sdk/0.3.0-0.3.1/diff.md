# Comparing `tmp/sifflet_sdk-0.3.0.tar.gz` & `tmp/sifflet_sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sifflet_sdk-0.3.0.tar", last modified: Fri Jul 21 09:34:36 2023, max compression
+gzip compressed data, was "sifflet_sdk-0.3.1.tar", last modified: Mon Jul 24 16:51:46 2023, max compression
```

## Comparing `sifflet_sdk-0.3.0.tar` & `sifflet_sdk-0.3.1.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.125417 sifflet_sdk-0.3.0/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/LICENSE
--rw-r--r--   0 baptiste   (501) staff       (20)       25 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/MANIFEST.in
--rw-r--r--   0 baptiste   (501) staff       (20)      493 2023-07-21 09:34:36.125230 sifflet_sdk-0.3.0/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)       99 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/README.md
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.068977 sifflet_sdk-0.3.0/client/
--rw-r--r--   0 baptiste   (501) staff       (20)      881 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/__init__.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.075529 sifflet_sdk-0.3.0/client/api/
--rw-r--r--   0 baptiste   (501) staff       (20)      214 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)    21202 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/access_token_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17481 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/alerting_hook_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    92775 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/asset_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    20877 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/automation_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5576 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/aws_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5931 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/chart_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5961 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/collection_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17344 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/config_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5931 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dags_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11200 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dashboard_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    22004 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/datapoint_qualification_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     7540 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dataset_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16282 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dataset_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17765 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dataset_field_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6452 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dataset_field_tag_prediction_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    64547 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/datasource_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16837 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/datasource_connection_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     7477 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/dbt_integration_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    31999 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/domain_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5777 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/feature_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    31836 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/idp_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    51924 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/incident_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    42422 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/lineage_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    10919 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/mail_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6170 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/notification_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6472 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/query_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    90078 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/rule_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    46406 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/rule_run_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16095 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/rule_template_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    24821 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/secret_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    50837 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/slack_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    21135 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/statistics_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    26998 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/tag_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    39199 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/term_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6019 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/time_zone_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6043 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/usage_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    65847 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/user_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5610 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/versions_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    24220 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/api/workspace_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    39383 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/api_client.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17626 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/configuration.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5277 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/exceptions.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.121436 sifflet_sdk-0.3.0/client/model/
--rw-r--r--   0 baptiste   (501) staff       (20)      340 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12136 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/access_token_creation_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13008 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/access_token_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12649 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/action_condition_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14504 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/airflow_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11783 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/airflow_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13226 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/alerting_hook_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12114 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/apply_automation_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11977 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_incident_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    18915 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_monitor_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15923 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_monitor_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12524 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_notifications_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12557 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_object_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11607 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_reference_by_id_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11803 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_reference_by_id_or_name_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14899 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_workspace_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11833 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/as_code_workspace_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12439 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_data_quality_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15448 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17248 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12074 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_full_schema_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16273 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_header_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13838 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12800 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_orchestrator_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12195 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    18499 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_overview_details.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14602 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11831 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_schema_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14463 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11823 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_search_filter_element_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13545 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14503 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/asset_usage_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12591 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/assets_catalog_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14512 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/assign_owners_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11924 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/assign_owners_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15672 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/athena_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12856 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/athena_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12125 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/automation_platform_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11682 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/automation_platform_metadata_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11889 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/automation_suggested_rules_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12569 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/base_search_filter_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15590 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/base_search_filter_dto_children_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11644 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/base_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14917 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/big_query_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12090 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/big_query_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17017 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/big_query_partitioned_table_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12361 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/big_query_partitioned_table_properties_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12157 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/big_query_partitioning_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12375 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/catalog_filter_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13026 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/change_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14518 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/chart_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12276 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/checked_rule_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14742 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/collection_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11813 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/connection_test_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11623 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/create_access_token_request.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11806 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/create_comment_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14234 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/create_comment_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11641 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/create_comment_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11605 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/csv_content_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14817 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11776 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17388 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11610 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_details_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17704 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12859 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dag_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15061 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dashboard_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11990 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dashboard_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16917 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dashboard_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12228 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/data_quality_rule_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11711 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/data_stack_group_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12067 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/data_stack_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15439 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/databricks_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12603 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/databricks_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14379 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datapoint_qualification_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17504 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14507 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12605 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_brief_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17999 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12265 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_details_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17761 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    19922 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_dto_dataset_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14572 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_field_node_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12096 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_field_node_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12047 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_field_patch_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12277 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_field_tag_prediction_batch_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12988 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_field_tag_prediction_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12893 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12620 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_name_and_source_type_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14364 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_node_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11864 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_node_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13272 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dataset_params_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17136 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_batch_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15659 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16784 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14147 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_ingestion_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11649 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_overview_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15117 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12675 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/datasource_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14909 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dbt_cloud_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12282 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dbt_cloud_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14521 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dbt_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11820 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/dbt_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12569 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/declarative_lineage_edge_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15004 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/declarative_lineage_edge_dto_downstream_node.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12553 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/description_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12242 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/description_prediction_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12411 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/description_prediction_feedback_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13471 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/domain_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12424 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/entity_urn.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13466 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/event_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16176 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/event_dto_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12550 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/event_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11854 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/export_as_csv_request_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16783 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/external_table_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12120 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/external_table_properties_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11809 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/feature_consumption_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    18055 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    18547 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/field_level_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13303 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/field_level_search_field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11831 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/field_name_type_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13699 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/field_search_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12002 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14820 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/firebolt_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11994 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/firebolt_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15886 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/full_schema_field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    25469 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/get_all_datasource_params_type200_response_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    18272 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/get_asset_overview_by_urn200_response.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16308 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/get_sifflet_rule_graph200_response_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12476 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/git_connection.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11822 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/git_connection_test_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11403 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/graph_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14556 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/health_status_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11880 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/health_status_search_filter_element_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15887 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/histogram_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11888 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/histogram_graph_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14479 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/histogram_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12233 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/histogram_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15482 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/hive_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12676 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/hive_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12474 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/idp_json_schema_params_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13157 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/impacted_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12361 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/impacted_assets_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12260 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/import_report_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14988 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_detail_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12150 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_group_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12448 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_heat_map_cell_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12156 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_heat_map_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14127 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12547 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_scope.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12583 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14932 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_status_update_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12303 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_status_update_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12777 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/incident_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11624 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/ingestion_run_summary.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12014 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/input_cardinality_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12191 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/issue_brief_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14350 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/issue_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11988 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/job_dbt_metadata_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11996 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/job_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12184 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/last_ingestion_status_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/last_run_status_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13642 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/lineage_attached_entity.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16136 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/lineage_entity_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12116 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/lineage_urn_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11922 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/log_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14741 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/looker_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12039 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/looker_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12139 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/message_report_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17164 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/model_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14177 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/model_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16648 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/monitor_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12247 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/monitor_summary_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12567 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/monitoring_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14974 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/mssql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12163 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/mssql_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15686 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/multi_metrics_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11671 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/multi_metrics_graph_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14113 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/multi_metrics_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11851 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/multi_metrics_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15132 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/mysql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12321 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/mysql_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12220 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/node_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14977 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/oracle_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12312 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/parameterized_query_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12227 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/pipeline_declarative_lineage_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15438 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/platform_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12847 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/platform_search_filter_element_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11820 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/positional_parameter_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14989 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/postgresql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14720 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/power_bi_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12048 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/power_bi_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12347 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/preview_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12943 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/problem.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13104 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/query_generate_request_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12025 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/query_parameter_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14734 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/quick_sight_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12047 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/quick_sight_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15174 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/redshift_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12348 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/redshift_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11594 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/resource_ids_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16838 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14086 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12477 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_dry_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12434 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_dry_run_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15287 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13149 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16476 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_graph_dto_graph_points_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12387 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_group_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16232 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_info_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13036 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_monitoring_recommendation_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12007 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_monitoring_recommendation_update_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11631 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_overview_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12949 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_run_details_by_group.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13743 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_run_details_by_group_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15868 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13412 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_run_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13042 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_template_brief.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13225 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_template_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11905 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_template_index_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11836 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/rule_template_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11779 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/saml2_auth_n_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13225 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/saml2_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11931 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/save_mail_addresses_summary.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12228 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/schema_version_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12081 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_access_token_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12091 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_alerting_hook_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12071 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_asset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12270 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_asset_summary_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16690 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_asset_summary_dto_data_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12091 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_dataset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_datasource_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_datasource_ingestion_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12030 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_domain_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12132 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_field_level_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12183 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_field_level_search_field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12101 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_impacted_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12101 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_incident_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12132 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_rule_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12252 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_rule_monitoring_recommendation_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12184 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_rule_run_details_by_group_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12041 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_rule_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12000 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_tag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12143 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_tag_with_asset_count_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12051 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/search_collection_time_zone_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11974 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/secret_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11647 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_add_channel_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11764 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_channel_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12061 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_connect_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12244 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_fetch_channels_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11786 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_remove_channel_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11669 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/slack_workspace_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15100 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/snowflake_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12269 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/snowflake_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17758 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/snowflake_stream_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13085 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/snowflake_stream_properties_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11837 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/status_type.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14447 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/status_update_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11859 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/status_update_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11595 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/string_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11616 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/system_alert_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14504 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tableau_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11783 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tableau_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13505 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12179 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tag_prediction_feedback_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13759 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tag_with_asset_count_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14263 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/tag_with_assets_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14902 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/time_series_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12950 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/time_series_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13254 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/time_window.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11925 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/time_zone_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14117 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/unknown_datasource_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11864 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/unlinking_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11703 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/upstream_of_field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11977 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/usage_per_datasource_user_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14435 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/usage_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11795 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/usage_search_filter_element_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12826 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/user_asset_bookmark_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14902 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/user_detail_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15136 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/user_detail_with_password_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11923 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/user_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11821 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/user_patch_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14447 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/uuid_search_filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11812 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/uuid_search_filter_element_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13041 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/versions_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13316 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/workspace_apply_object_response_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12008 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/workspace_apply_request_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    19175 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/workspace_apply_request_dto_changes_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11975 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/workspace_apply_response_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11968 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/client/model/workspace_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    82788 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/model_utils.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14599 2023-07-20 17:29:07.000000 sifflet_sdk-0.3.0/client/rest.py
--rw-r--r--   0 baptiste   (501) staff       (20)      666 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/pyproject.toml
--rw-r--r--   0 baptiste   (501) staff       (20)       74 2023-07-21 09:10:10.000000 sifflet_sdk-0.3.0/requirements.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-21 09:34:36.125465 sifflet_sdk-0.3.0/setup.cfg
--rw-r--r--   0 baptiste   (501) staff       (20)      878 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/setup.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.122071 sifflet_sdk-0.3.0/sifflet_sdk/
--rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/__init__.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.122973 sifflet_sdk-0.3.0/sifflet_sdk/apis/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/apis/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      607 2023-07-20 17:50:56.000000 sifflet_sdk-0.3.0/sifflet_sdk/apis/base.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.123113 sifflet_sdk-0.3.0/sifflet_sdk/code/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/code/__init__.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.123451 sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1791 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     4385 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)      232 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/config.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.123699 sifflet_sdk-0.3.0/sifflet_sdk/configure/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/configure/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5078 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/configure/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1276 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/constants.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2561 2023-07-20 17:52:32.000000 sifflet_sdk-0.3.0/sifflet_sdk/errors.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.124110 sifflet_sdk-0.3.0/sifflet_sdk/ingest/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/ingest/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1245 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/ingest/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)      523 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/ingest/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)      276 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/logger.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.124483 sifflet_sdk-0.3.0/sifflet_sdk/rules/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/rules/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2910 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/rules/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5219 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/rules/service.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.124857 sifflet_sdk-0.3.0/sifflet_sdk/status/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/status/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      965 2023-07-20 17:15:19.000000 sifflet_sdk-0.3.0/sifflet_sdk/status/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2190 2023-07-20 17:52:09.000000 sifflet_sdk-0.3.0/sifflet_sdk/status/service.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:34:36.122726 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/
--rw-r--r--   0 baptiste   (501) staff       (20)      493 2023-07-21 09:34:36.000000 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)    13710 2023-07-21 09:34:36.000000 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-21 09:34:36.000000 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       74 2023-07-21 09:34:36.000000 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/requires.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       19 2023-07-21 09:34:36.000000 sifflet_sdk-0.3.0/sifflet_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.640033 sifflet_sdk-0.3.1/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/LICENSE
+-rw-r--r--   0 baptiste   (501) staff       (20)       25 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 baptiste   (501) staff       (20)      493 2023-07-24 16:51:46.639730 sifflet_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)       99 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/README.md
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.569776 sifflet_sdk-0.3.1/client/
+-rw-r--r--   0 baptiste   (501) staff       (20)      881 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/__init__.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.578379 sifflet_sdk-0.3.1/client/api/
+-rw-r--r--   0 baptiste   (501) staff       (20)      214 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    21202 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/access_token_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17481 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/alerting_hook_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    92775 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/asset_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    20877 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/automation_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5576 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/aws_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5931 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/chart_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5961 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/collection_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17344 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/config_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5931 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dags_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11200 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dashboard_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    22004 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/datapoint_qualification_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     7540 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dataset_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16282 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dataset_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17765 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dataset_field_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6452 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dataset_field_tag_prediction_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    64547 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/datasource_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16837 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/datasource_connection_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     7477 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/dbt_integration_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    31999 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/domain_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5777 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/feature_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    31836 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/idp_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    51924 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/incident_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    42422 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/lineage_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    10919 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/mail_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6170 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/notification_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6472 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/query_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    90078 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/rule_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    46406 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/rule_run_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16095 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/rule_template_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    24821 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/secret_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    50837 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/slack_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    21135 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/statistics_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    26998 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/tag_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    39199 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/term_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6019 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/time_zone_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6043 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/usage_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    65847 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/user_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5610 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/versions_controller_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    24220 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api/workspace_api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    39383 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/api_client.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17626 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/configuration.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5277 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/exceptions.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.635232 sifflet_sdk-0.3.1/client/model/
+-rw-r--r--   0 baptiste   (501) staff       (20)      340 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12136 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/access_token_creation_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13008 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/access_token_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12649 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/action_condition_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14504 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/airflow_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11783 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/airflow_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13226 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/alerting_hook_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12114 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/apply_automation_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11977 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_incident_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    18915 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_monitor_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15923 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_monitor_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12524 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_notifications_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12557 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_object_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11607 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_reference_by_id_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11803 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_reference_by_id_or_name_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14899 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_workspace_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11833 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/as_code_workspace_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12439 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_data_quality_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15448 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_details_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17248 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12074 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_full_schema_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16273 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_header_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13838 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12800 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_orchestrator_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12195 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_overview.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    18499 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_overview_details.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14602 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11831 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_schema_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14463 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11823 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_search_filter_element_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13545 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14503 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/asset_usage_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12591 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/assets_catalog_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14512 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/assign_owners_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11924 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/assign_owners_payload_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15672 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/athena_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12856 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/athena_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12125 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/automation_platform_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11682 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/automation_platform_metadata_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11889 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/automation_suggested_rules_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12569 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/base_search_filter_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15590 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/base_search_filter_dto_children_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11644 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/base_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14917 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/big_query_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12090 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/big_query_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17017 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/big_query_partitioned_table_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12361 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/big_query_partitioned_table_properties_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12157 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/big_query_partitioning_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12375 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/catalog_filter_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13026 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/change_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14518 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/chart_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12276 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/checked_rule_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14742 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/collection_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11813 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/connection_test_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11623 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/create_access_token_request.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11806 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/create_comment_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14234 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/create_comment_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11641 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/create_comment_payload_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11605 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/csv_content_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14817 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_asset_overview.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11776 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_asset_overview_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17388 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_details_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11610 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_details_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17704 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12859 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dag_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15061 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dashboard_asset_overview.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11990 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dashboard_asset_overview_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16917 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dashboard_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12228 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/data_quality_rule_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11711 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/data_stack_group_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12067 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/data_stack_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15439 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/databricks_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12603 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/databricks_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14379 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datapoint_qualification_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17504 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_asset_overview.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14507 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_asset_overview_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12605 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_brief_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17999 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_details_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12265 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_details_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17761 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    19922 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_dto_dataset_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14572 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_field_node_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12096 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_field_node_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12047 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_field_patch_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12277 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_field_tag_prediction_batch_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12988 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_field_tag_prediction_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12893 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12620 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_name_and_source_type_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14364 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_node_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11864 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_node_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13272 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dataset_params_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17136 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_batch_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15659 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_catalog_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16784 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14147 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_ingestion_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11649 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_overview_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15117 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12675 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/datasource_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14909 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dbt_cloud_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12282 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dbt_cloud_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14521 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dbt_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11820 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/dbt_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12569 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/declarative_lineage_edge_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15004 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/declarative_lineage_edge_dto_downstream_node.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12553 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/description_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12242 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/description_prediction_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12411 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/description_prediction_feedback_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13471 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/domain_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12424 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/entity_urn.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13466 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/event_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16176 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/event_dto_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12550 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/event_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11854 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/export_as_csv_request_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16783 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/external_table_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12120 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/external_table_properties_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11809 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/feature_consumption_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    18055 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/field_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    18547 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/field_level_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13303 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/field_level_search_field_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11831 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/field_name_type_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13699 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/field_search_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12002 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14820 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/firebolt_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11994 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/firebolt_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15886 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/full_schema_field_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    25469 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/get_all_datasource_params_type200_response_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    18272 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/get_asset_overview_by_urn200_response.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16308 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/get_sifflet_rule_graph200_response_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12476 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/git_connection.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11822 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/git_connection_test_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11403 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/graph_point.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14556 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/health_status_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11880 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/health_status_search_filter_element_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15887 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/histogram_graph_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11888 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/histogram_graph_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14479 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/histogram_point.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12233 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/histogram_point_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15482 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/hive_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12676 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/hive_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12474 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/idp_json_schema_params_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13157 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/impacted_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12361 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/impacted_assets_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12260 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/import_report_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14988 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_detail_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12150 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_group_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12448 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_heat_map_cell_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12156 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_heat_map_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14127 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12547 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_scope.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12583 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14932 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_status_update_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12303 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_status_update_payload_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12777 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/incident_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11624 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/ingestion_run_summary.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12014 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/input_cardinality_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12191 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/issue_brief_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14350 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/issue_details_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11988 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/job_dbt_metadata_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11996 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/job_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12184 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/last_ingestion_status_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/last_run_status_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13642 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/lineage_attached_entity.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16136 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/lineage_entity_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12116 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/lineage_urn_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11922 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/log_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14741 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/looker_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12039 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/looker_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12139 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/message_report_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17164 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/model_asset_overview.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14177 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/model_asset_overview_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16648 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/monitor_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12247 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/monitor_summary_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12567 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/monitoring_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14974 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/mssql_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12163 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/mssql_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15686 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/multi_metrics_graph_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11671 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/multi_metrics_graph_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14113 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/multi_metrics_point.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11851 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/multi_metrics_point_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15132 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/mysql_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12321 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/mysql_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12220 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/node_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14977 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/oracle_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12312 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/parameterized_query_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12227 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/pipeline_declarative_lineage_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15438 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/platform_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12847 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/platform_search_filter_element_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11820 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/positional_parameter_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14989 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/postgresql_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14720 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/power_bi_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12048 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/power_bi_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12347 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/preview_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12943 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/problem.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13104 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/query_generate_request_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12025 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/query_parameter_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14734 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/quick_sight_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12047 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/quick_sight_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15174 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/redshift_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12348 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/redshift_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11594 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/resource_ids_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16838 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_catalog_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14086 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_details_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12477 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_dry_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12434 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_dry_run_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15287 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13149 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_graph_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16476 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_graph_dto_graph_points_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12387 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_group_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16232 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_info_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13036 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_monitoring_recommendation_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12007 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_monitoring_recommendation_update_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11631 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_overview_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12949 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_run_details_by_group.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13743 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_run_details_by_group_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15868 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13412 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_run_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13042 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_template_brief.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13225 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_template_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11905 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_template_index_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11836 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/rule_template_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11779 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/saml2_auth_n_config_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13225 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/saml2_config_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11931 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/save_mail_addresses_summary.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12228 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/schema_version_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12081 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_access_token_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12091 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_alerting_hook_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12071 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_asset_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12270 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_asset_summary_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    16690 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_asset_summary_dto_data_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12091 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_dataset_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_datasource_catalog_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12192 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_datasource_ingestion_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12030 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_domain_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12132 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_field_level_search_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12183 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_field_level_search_field_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12101 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_impacted_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12101 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_incident_light_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12132 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_rule_catalog_asset_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12252 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_rule_monitoring_recommendation_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12184 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_rule_run_details_by_group_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12041 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_rule_run_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12000 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_tag_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12143 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_tag_with_asset_count_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12051 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/search_collection_time_zone_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11974 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/secret_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11647 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_add_channel_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11764 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_channel_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12061 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_connect_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12244 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_fetch_channels_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11786 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_remove_channel_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11669 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/slack_workspace_config_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15100 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/snowflake_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12269 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/snowflake_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    17758 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/snowflake_stream_properties.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13085 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/snowflake_stream_properties_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11837 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/status_type.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14447 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/status_update_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11859 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/status_update_payload_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11595 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/string_payload.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11616 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/system_alert_config_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14504 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tableau_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11783 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tableau_params_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13505 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tag_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12179 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tag_prediction_feedback_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13759 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tag_with_asset_count_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14263 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/tag_with_assets_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14902 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/time_series_point.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12950 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/time_series_point_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13254 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/time_window.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11925 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/time_zone_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14117 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/unknown_datasource_params.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11864 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/unlinking_result_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11703 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/upstream_of_field_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11977 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/usage_per_datasource_user_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14435 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/usage_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11795 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/usage_search_filter_element_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12826 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/user_asset_bookmark_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14902 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/user_detail_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    15136 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/user_detail_with_password_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11923 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/user_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11821 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/user_patch_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14447 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/uuid_search_filter_element_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11812 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/uuid_search_filter_element_dto_all_of.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13041 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/versions_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    13316 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/workspace_apply_object_response_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    12008 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/workspace_apply_request_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    19175 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/workspace_apply_request_dto_changes_inner.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11975 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/workspace_apply_response_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    11968 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model/workspace_dto.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    82788 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/model_utils.py
+-rw-r--r--   0 baptiste   (501) staff       (20)    14599 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/client/rest.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      666 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/pyproject.toml
+-rw-r--r--   0 baptiste   (501) staff       (20)       52 2023-07-24 16:34:55.000000 sifflet_sdk-0.3.1/requirements.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-24 16:51:46.640092 sifflet_sdk-0.3.1/setup.cfg
+-rw-r--r--   0 baptiste   (501) staff       (20)      878 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/setup.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.636371 sifflet_sdk-0.3.1/sifflet_sdk/
+-rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-24 15:42:08.000000 sifflet_sdk-0.3.1/sifflet_sdk/__init__.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.637303 sifflet_sdk-0.3.1/sifflet_sdk/apis/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/apis/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      607 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/apis/base.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.637464 sifflet_sdk-0.3.1/sifflet_sdk/code/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/code/__init__.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.637834 sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1791 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     4385 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/service.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      232 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/config.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.638105 sifflet_sdk-0.3.1/sifflet_sdk/configure/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/configure/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5078 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/configure/service.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1276 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/constants.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     2561 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/errors.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.638520 sifflet_sdk-0.3.1/sifflet_sdk/ingest/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/ingest/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1245 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/ingest/api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      523 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/ingest/service.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      276 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/logger.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.638951 sifflet_sdk-0.3.1/sifflet_sdk/rules/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/rules/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     2910 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/rules/api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     5219 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/rules/service.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.639365 sifflet_sdk-0.3.1/sifflet_sdk/status/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/status/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      965 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/status/api.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     2190 2023-07-24 14:37:03.000000 sifflet_sdk-0.3.1/sifflet_sdk/status/service.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-24 16:51:46.637061 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/
+-rw-r--r--   0 baptiste   (501) staff       (20)      493 2023-07-24 16:51:46.000000 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)    13710 2023-07-24 16:51:46.000000 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-24 16:51:46.000000 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       52 2023-07-24 16:51:46.000000 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/requires.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       19 2023-07-24 16:51:46.000000 sifflet_sdk-0.3.1/sifflet_sdk.egg-info/top_level.txt
```

### Comparing `sifflet_sdk-0.3.0/client/__init__.py` & `sifflet_sdk-0.3.1/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/access_token_api.py` & `sifflet_sdk-0.3.1/client/api/access_token_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/alerting_hook_api.py` & `sifflet_sdk-0.3.1/client/api/alerting_hook_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/asset_api.py` & `sifflet_sdk-0.3.1/client/api/asset_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/automation_controller_api.py` & `sifflet_sdk-0.3.1/client/api/automation_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/aws_controller_api.py` & `sifflet_sdk-0.3.1/client/api/aws_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/chart_controller_api.py` & `sifflet_sdk-0.3.1/client/api/chart_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/collection_controller_api.py` & `sifflet_sdk-0.3.1/client/api/collection_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/config_api.py` & `sifflet_sdk-0.3.1/client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dags_api.py` & `sifflet_sdk-0.3.1/client/api/dags_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dashboard_controller_api.py` & `sifflet_sdk-0.3.1/client/api/dashboard_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/datapoint_qualification_controller_api.py` & `sifflet_sdk-0.3.1/client/api/datapoint_qualification_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dataset_api.py` & `sifflet_sdk-0.3.1/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dataset_controller_api.py` & `sifflet_sdk-0.3.1/client/api/dataset_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dataset_field_controller_api.py` & `sifflet_sdk-0.3.1/client/api/dataset_field_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dataset_field_tag_prediction_api.py` & `sifflet_sdk-0.3.1/client/api/dataset_field_tag_prediction_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/datasource_api.py` & `sifflet_sdk-0.3.1/client/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/datasource_connection_api.py` & `sifflet_sdk-0.3.1/client/api/datasource_connection_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/dbt_integration_api.py` & `sifflet_sdk-0.3.1/client/api/dbt_integration_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/domain_api.py` & `sifflet_sdk-0.3.1/client/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/feature_api.py` & `sifflet_sdk-0.3.1/client/api/feature_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/idp_api.py` & `sifflet_sdk-0.3.1/client/api/idp_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/incident_api.py` & `sifflet_sdk-0.3.1/client/api/incident_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/lineage_api.py` & `sifflet_sdk-0.3.1/client/api/lineage_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/mail_api.py` & `sifflet_sdk-0.3.1/client/api/mail_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/notification_api.py` & `sifflet_sdk-0.3.1/client/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/query_api.py` & `sifflet_sdk-0.3.1/client/api/query_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/rule_api.py` & `sifflet_sdk-0.3.1/client/api/rule_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/rule_run_api.py` & `sifflet_sdk-0.3.1/client/api/rule_run_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/rule_template_api.py` & `sifflet_sdk-0.3.1/client/api/rule_template_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/secret_controller_api.py` & `sifflet_sdk-0.3.1/client/api/secret_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/slack_api.py` & `sifflet_sdk-0.3.1/client/api/slack_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/statistics_api.py` & `sifflet_sdk-0.3.1/client/api/statistics_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/tag_api.py` & `sifflet_sdk-0.3.1/client/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/term_api.py` & `sifflet_sdk-0.3.1/client/api/term_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/time_zone_api.py` & `sifflet_sdk-0.3.1/client/api/time_zone_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/usage_api.py` & `sifflet_sdk-0.3.1/client/api/usage_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/user_api.py` & `sifflet_sdk-0.3.1/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/versions_controller_api.py` & `sifflet_sdk-0.3.1/client/api/versions_controller_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api/workspace_api.py` & `sifflet_sdk-0.3.1/client/api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/api_client.py` & `sifflet_sdk-0.3.1/client/api_client.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/configuration.py` & `sifflet_sdk-0.3.1/client/configuration.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/exceptions.py` & `sifflet_sdk-0.3.1/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/access_token_creation_result_dto.py` & `sifflet_sdk-0.3.1/client/model/access_token_creation_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/access_token_dto.py` & `sifflet_sdk-0.3.1/client/model/access_token_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/action_condition_dto.py` & `sifflet_sdk-0.3.1/client/model/action_condition_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/airflow_params.py` & `sifflet_sdk-0.3.1/client/model/airflow_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/airflow_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/airflow_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/alerting_hook_dto.py` & `sifflet_sdk-0.3.1/client/model/alerting_hook_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/apply_automation_dto.py` & `sifflet_sdk-0.3.1/client/model/apply_automation_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_incident_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_incident_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_monitor_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_monitor_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_monitor_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/as_code_monitor_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_notifications_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_object_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_object_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_reference_by_id_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_reference_by_id_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_reference_by_id_or_name_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_reference_by_id_or_name_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_workspace_dto.py` & `sifflet_sdk-0.3.1/client/model/as_code_workspace_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/as_code_workspace_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/as_code_workspace_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_data_quality_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_data_quality_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_details_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_details_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_full_schema_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_full_schema_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_header_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_header_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_light_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_orchestrator_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_orchestrator_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_overview.py` & `sifflet_sdk-0.3.1/client/model/asset_overview.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_overview_details.py` & `sifflet_sdk-0.3.1/client/model/asset_overview_details.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_properties.py` & `sifflet_sdk-0.3.1/client/model/asset_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_schema_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_schema_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_search_filter_element_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/asset_search_filter_element_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/asset_usage_dto.py` & `sifflet_sdk-0.3.1/client/model/asset_usage_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/assets_catalog_dto.py` & `sifflet_sdk-0.3.1/client/model/assets_catalog_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/assign_owners_payload.py` & `sifflet_sdk-0.3.1/client/model/assign_owners_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/assign_owners_payload_all_of.py` & `sifflet_sdk-0.3.1/client/model/assign_owners_payload_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/athena_params.py` & `sifflet_sdk-0.3.1/client/model/athena_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/athena_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/athena_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/automation_platform_dto.py` & `sifflet_sdk-0.3.1/client/model/automation_platform_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/automation_platform_metadata_dto.py` & `sifflet_sdk-0.3.1/client/model/automation_platform_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/automation_suggested_rules_dto.py` & `sifflet_sdk-0.3.1/client/model/automation_suggested_rules_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/base_search_filter_dto.py` & `sifflet_sdk-0.3.1/client/model/base_search_filter_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/base_search_filter_dto_children_inner.py` & `sifflet_sdk-0.3.1/client/model/base_search_filter_dto_children_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/base_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/base_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/big_query_params.py` & `sifflet_sdk-0.3.1/client/model/big_query_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/big_query_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/big_query_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/big_query_partitioned_table_properties.py` & `sifflet_sdk-0.3.1/client/model/big_query_partitioned_table_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/big_query_partitioned_table_properties_all_of.py` & `sifflet_sdk-0.3.1/client/model/big_query_partitioned_table_properties_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/big_query_partitioning_properties.py` & `sifflet_sdk-0.3.1/client/model/big_query_partitioning_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/catalog_filter_dto.py` & `sifflet_sdk-0.3.1/client/model/catalog_filter_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/change_dto.py` & `sifflet_sdk-0.3.1/client/model/change_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/chart_dto.py` & `sifflet_sdk-0.3.1/client/model/chart_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/checked_rule_dto.py` & `sifflet_sdk-0.3.1/client/model/checked_rule_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/collection_dto.py` & `sifflet_sdk-0.3.1/client/model/collection_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/connection_test_dto.py` & `sifflet_sdk-0.3.1/client/model/connection_test_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/create_access_token_request.py` & `sifflet_sdk-0.3.1/client/model/create_access_token_request.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/create_comment_dto.py` & `sifflet_sdk-0.3.1/client/model/create_comment_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/create_comment_payload.py` & `sifflet_sdk-0.3.1/client/model/create_comment_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/create_comment_payload_all_of.py` & `sifflet_sdk-0.3.1/client/model/create_comment_payload_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/csv_content_dto.py` & `sifflet_sdk-0.3.1/client/model/csv_content_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_asset_overview.py` & `sifflet_sdk-0.3.1/client/model/dag_asset_overview.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_asset_overview_all_of.py` & `sifflet_sdk-0.3.1/client/model/dag_asset_overview_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_details_dto.py` & `sifflet_sdk-0.3.1/client/model/dag_details_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_details_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/dag_details_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_dto.py` & `sifflet_sdk-0.3.1/client/model/dag_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dag_run_dto.py` & `sifflet_sdk-0.3.1/client/model/dag_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dashboard_asset_overview.py` & `sifflet_sdk-0.3.1/client/model/dashboard_asset_overview.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dashboard_asset_overview_all_of.py` & `sifflet_sdk-0.3.1/client/model/dashboard_asset_overview_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dashboard_dto.py` & `sifflet_sdk-0.3.1/client/model/dashboard_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/data_quality_rule_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/data_quality_rule_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/data_stack_group_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/data_stack_group_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/data_stack_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/data_stack_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/databricks_params.py` & `sifflet_sdk-0.3.1/client/model/databricks_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/databricks_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/databricks_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datapoint_qualification_dto.py` & `sifflet_sdk-0.3.1/client/model/datapoint_qualification_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_asset_overview.py` & `sifflet_sdk-0.3.1/client/model/dataset_asset_overview.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_asset_overview_all_of.py` & `sifflet_sdk-0.3.1/client/model/dataset_asset_overview_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_brief_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_brief_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_details_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_details_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_details_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/dataset_details_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_dto_dataset_properties.py` & `sifflet_sdk-0.3.1/client/model/dataset_dto_dataset_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_field_node_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_field_node_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_field_node_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/dataset_field_node_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_field_patch_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_field_patch_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_field_tag_prediction_batch_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_field_tag_prediction_batch_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_field_tag_prediction_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_field_tag_prediction_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_light_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_name_and_source_type_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_name_and_source_type_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_node_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_node_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_node_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/dataset_node_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dataset_params_dto.py` & `sifflet_sdk-0.3.1/client/model/dataset_params_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_batch_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_batch_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_catalog_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_catalog_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_ingestion_run_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_ingestion_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_overview_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_overview_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_params.py` & `sifflet_sdk-0.3.1/client/model/datasource_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/datasource_search_dto.py` & `sifflet_sdk-0.3.1/client/model/datasource_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dbt_cloud_params.py` & `sifflet_sdk-0.3.1/client/model/dbt_cloud_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dbt_cloud_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/dbt_cloud_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dbt_params.py` & `sifflet_sdk-0.3.1/client/model/dbt_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/dbt_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/dbt_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/declarative_lineage_edge_dto.py` & `sifflet_sdk-0.3.1/client/model/declarative_lineage_edge_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/declarative_lineage_edge_dto_downstream_node.py` & `sifflet_sdk-0.3.1/client/model/declarative_lineage_edge_dto_downstream_node.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/description_dto.py` & `sifflet_sdk-0.3.1/client/model/description_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/description_prediction_dto.py` & `sifflet_sdk-0.3.1/client/model/description_prediction_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/description_prediction_feedback_dto.py` & `sifflet_sdk-0.3.1/client/model/description_prediction_feedback_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/domain_dto.py` & `sifflet_sdk-0.3.1/client/model/domain_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/entity_urn.py` & `sifflet_sdk-0.3.1/client/model/entity_urn.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/event_dto.py` & `sifflet_sdk-0.3.1/client/model/event_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/event_dto_payload.py` & `sifflet_sdk-0.3.1/client/model/event_dto_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/event_payload.py` & `sifflet_sdk-0.3.1/client/model/event_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/export_as_csv_request_dto.py` & `sifflet_sdk-0.3.1/client/model/export_as_csv_request_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/external_table_properties.py` & `sifflet_sdk-0.3.1/client/model/external_table_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/external_table_properties_all_of.py` & `sifflet_sdk-0.3.1/client/model/external_table_properties_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/feature_consumption_dto.py` & `sifflet_sdk-0.3.1/client/model/feature_consumption_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/field_dto.py` & `sifflet_sdk-0.3.1/client/model/field_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/field_level_search_dto.py` & `sifflet_sdk-0.3.1/client/model/field_level_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/field_level_search_field_dto.py` & `sifflet_sdk-0.3.1/client/model/field_level_search_field_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/field_name_type_dto.py` & `sifflet_sdk-0.3.1/client/model/field_name_type_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/field_search_result_dto.py` & `sifflet_sdk-0.3.1/client/model/field_search_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/firebolt_params.py` & `sifflet_sdk-0.3.1/client/model/firebolt_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/firebolt_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/firebolt_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/full_schema_field_dto.py` & `sifflet_sdk-0.3.1/client/model/full_schema_field_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/get_all_datasource_params_type200_response_inner.py` & `sifflet_sdk-0.3.1/client/model/get_all_datasource_params_type200_response_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/get_asset_overview_by_urn200_response.py` & `sifflet_sdk-0.3.1/client/model/get_asset_overview_by_urn200_response.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/get_sifflet_rule_graph200_response_inner.py` & `sifflet_sdk-0.3.1/client/model/get_sifflet_rule_graph200_response_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/git_connection.py` & `sifflet_sdk-0.3.1/client/model/git_connection.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/git_connection_test_dto.py` & `sifflet_sdk-0.3.1/client/model/git_connection_test_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/graph_point.py` & `sifflet_sdk-0.3.1/client/model/graph_point.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/health_status_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/health_status_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/health_status_search_filter_element_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/health_status_search_filter_element_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/histogram_graph_dto.py` & `sifflet_sdk-0.3.1/client/model/histogram_graph_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/histogram_graph_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/histogram_graph_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/histogram_point.py` & `sifflet_sdk-0.3.1/client/model/histogram_point.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/histogram_point_all_of.py` & `sifflet_sdk-0.3.1/client/model/histogram_point_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/hive_params.py` & `sifflet_sdk-0.3.1/client/model/hive_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/hive_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/hive_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/idp_json_schema_params_dto.py` & `sifflet_sdk-0.3.1/client/model/idp_json_schema_params_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/impacted_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/impacted_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/impacted_assets_search_dto.py` & `sifflet_sdk-0.3.1/client/model/impacted_assets_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/import_report_dto.py` & `sifflet_sdk-0.3.1/client/model/import_report_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_detail_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_detail_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_group_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_group_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_heat_map_cell_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_heat_map_cell_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_heat_map_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_heat_map_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_light_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_scope.py` & `sifflet_sdk-0.3.1/client/model/incident_scope.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_search_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_status_update_payload.py` & `sifflet_sdk-0.3.1/client/model/incident_status_update_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_status_update_payload_all_of.py` & `sifflet_sdk-0.3.1/client/model/incident_status_update_payload_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/incident_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/incident_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/ingestion_run_summary.py` & `sifflet_sdk-0.3.1/client/model/ingestion_run_summary.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/input_cardinality_dto.py` & `sifflet_sdk-0.3.1/client/model/input_cardinality_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/issue_brief_dto.py` & `sifflet_sdk-0.3.1/client/model/issue_brief_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/issue_details_dto.py` & `sifflet_sdk-0.3.1/client/model/issue_details_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/job_dbt_metadata_dto.py` & `sifflet_sdk-0.3.1/client/model/job_dbt_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/job_dto.py` & `sifflet_sdk-0.3.1/client/model/job_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/last_ingestion_status_dto.py` & `sifflet_sdk-0.3.1/client/model/last_ingestion_status_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/last_run_status_dto.py` & `sifflet_sdk-0.3.1/client/model/last_run_status_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/lineage_attached_entity.py` & `sifflet_sdk-0.3.1/client/model/lineage_attached_entity.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/lineage_entity_dto.py` & `sifflet_sdk-0.3.1/client/model/lineage_entity_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/lineage_urn_dto.py` & `sifflet_sdk-0.3.1/client/model/lineage_urn_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/log_dto.py` & `sifflet_sdk-0.3.1/client/model/log_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/looker_params.py` & `sifflet_sdk-0.3.1/client/model/looker_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/looker_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/looker_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/message_report_dto.py` & `sifflet_sdk-0.3.1/client/model/message_report_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/model_asset_overview.py` & `sifflet_sdk-0.3.1/client/model/model_asset_overview.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/model_asset_overview_all_of.py` & `sifflet_sdk-0.3.1/client/model/model_asset_overview_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/monitor_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/monitor_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/monitor_summary_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/monitor_summary_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/monitoring_search_dto.py` & `sifflet_sdk-0.3.1/client/model/monitoring_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/mssql_params.py` & `sifflet_sdk-0.3.1/client/model/mssql_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/mssql_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/mssql_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/multi_metrics_graph_dto.py` & `sifflet_sdk-0.3.1/client/model/multi_metrics_graph_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/multi_metrics_graph_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/multi_metrics_graph_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/multi_metrics_point.py` & `sifflet_sdk-0.3.1/client/model/multi_metrics_point.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/multi_metrics_point_all_of.py` & `sifflet_sdk-0.3.1/client/model/multi_metrics_point_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/mysql_params.py` & `sifflet_sdk-0.3.1/client/model/mysql_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/mysql_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/mysql_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/node_dto.py` & `sifflet_sdk-0.3.1/client/model/node_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/oracle_params.py` & `sifflet_sdk-0.3.1/client/model/oracle_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/parameterized_query_dto.py` & `sifflet_sdk-0.3.1/client/model/parameterized_query_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/pipeline_declarative_lineage_dto.py` & `sifflet_sdk-0.3.1/client/model/pipeline_declarative_lineage_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/platform_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/platform_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/platform_search_filter_element_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/platform_search_filter_element_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/positional_parameter_dto.py` & `sifflet_sdk-0.3.1/client/model/positional_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/postgresql_params.py` & `sifflet_sdk-0.3.1/client/model/postgresql_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/power_bi_params.py` & `sifflet_sdk-0.3.1/client/model/power_bi_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/power_bi_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/power_bi_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/preview_result_dto.py` & `sifflet_sdk-0.3.1/client/model/preview_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/problem.py` & `sifflet_sdk-0.3.1/client/model/problem.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/query_generate_request_dto.py` & `sifflet_sdk-0.3.1/client/model/query_generate_request_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/query_parameter_dto.py` & `sifflet_sdk-0.3.1/client/model/query_parameter_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/quick_sight_params.py` & `sifflet_sdk-0.3.1/client/model/quick_sight_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/quick_sight_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/quick_sight_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/redshift_params.py` & `sifflet_sdk-0.3.1/client/model/redshift_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/redshift_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/redshift_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/resource_ids_dto.py` & `sifflet_sdk-0.3.1/client/model/resource_ids_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_catalog_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_catalog_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_details_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_details_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_dry_run_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_dry_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_dry_run_result_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_dry_run_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_graph_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_graph_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_graph_dto_graph_points_inner.py` & `sifflet_sdk-0.3.1/client/model/rule_graph_dto_graph_points_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_group_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_group_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_info_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_info_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_monitoring_recommendation_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_monitoring_recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_monitoring_recommendation_update_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_monitoring_recommendation_update_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_overview_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_overview_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_run_details_by_group.py` & `sifflet_sdk-0.3.1/client/model/rule_run_details_by_group.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_run_details_by_group_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_run_details_by_group_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_run_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_run_result_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_run_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_template_brief.py` & `sifflet_sdk-0.3.1/client/model/rule_template_brief.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_template_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_template_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_template_index_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_template_index_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/rule_template_light_dto.py` & `sifflet_sdk-0.3.1/client/model/rule_template_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/saml2_auth_n_config_dto.py` & `sifflet_sdk-0.3.1/client/model/saml2_auth_n_config_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/saml2_config_dto.py` & `sifflet_sdk-0.3.1/client/model/saml2_config_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/save_mail_addresses_summary.py` & `sifflet_sdk-0.3.1/client/model/save_mail_addresses_summary.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/schema_version_dto.py` & `sifflet_sdk-0.3.1/client/model/schema_version_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_access_token_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_access_token_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_alerting_hook_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_alerting_hook_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_asset_light_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_asset_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_asset_summary_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_asset_summary_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_asset_summary_dto_data_inner.py` & `sifflet_sdk-0.3.1/client/model/search_collection_asset_summary_dto_data_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_dataset_light_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_dataset_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_datasource_catalog_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_datasource_catalog_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_datasource_ingestion_run_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_datasource_ingestion_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_domain_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_domain_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_field_level_search_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_field_level_search_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_field_level_search_field_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_field_level_search_field_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_impacted_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_impacted_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_incident_light_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_incident_light_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_rule_catalog_asset_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_rule_catalog_asset_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_rule_monitoring_recommendation_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_rule_monitoring_recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_rule_run_details_by_group_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_rule_run_details_by_group_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_rule_run_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_rule_run_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_tag_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_tag_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_tag_with_asset_count_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_tag_with_asset_count_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/search_collection_time_zone_dto.py` & `sifflet_sdk-0.3.1/client/model/search_collection_time_zone_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/secret_dto.py` & `sifflet_sdk-0.3.1/client/model/secret_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_add_channel_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_add_channel_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_channel_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_channel_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_connect_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_connect_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_fetch_channels_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_fetch_channels_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_remove_channel_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_remove_channel_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/slack_workspace_config_dto.py` & `sifflet_sdk-0.3.1/client/model/slack_workspace_config_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/snowflake_params.py` & `sifflet_sdk-0.3.1/client/model/snowflake_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/snowflake_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/snowflake_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/snowflake_stream_properties.py` & `sifflet_sdk-0.3.1/client/model/snowflake_stream_properties.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/snowflake_stream_properties_all_of.py` & `sifflet_sdk-0.3.1/client/model/snowflake_stream_properties_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/status_type.py` & `sifflet_sdk-0.3.1/client/model/status_type.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/status_update_payload.py` & `sifflet_sdk-0.3.1/client/model/status_update_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/status_update_payload_all_of.py` & `sifflet_sdk-0.3.1/client/model/status_update_payload_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/string_payload.py` & `sifflet_sdk-0.3.1/client/model/string_payload.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/system_alert_config_dto.py` & `sifflet_sdk-0.3.1/client/model/system_alert_config_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tableau_params.py` & `sifflet_sdk-0.3.1/client/model/tableau_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tableau_params_all_of.py` & `sifflet_sdk-0.3.1/client/model/tableau_params_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tag_dto.py` & `sifflet_sdk-0.3.1/client/model/tag_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tag_prediction_feedback_dto.py` & `sifflet_sdk-0.3.1/client/model/tag_prediction_feedback_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tag_with_asset_count_dto.py` & `sifflet_sdk-0.3.1/client/model/tag_with_asset_count_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/tag_with_assets_dto.py` & `sifflet_sdk-0.3.1/client/model/tag_with_assets_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/time_series_point.py` & `sifflet_sdk-0.3.1/client/model/time_series_point.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/time_series_point_all_of.py` & `sifflet_sdk-0.3.1/client/model/time_series_point_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/time_window.py` & `sifflet_sdk-0.3.1/client/model/time_window.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/time_zone_dto.py` & `sifflet_sdk-0.3.1/client/model/time_zone_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/unknown_datasource_params.py` & `sifflet_sdk-0.3.1/client/model/unknown_datasource_params.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/unlinking_result_dto.py` & `sifflet_sdk-0.3.1/client/model/unlinking_result_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/upstream_of_field_dto.py` & `sifflet_sdk-0.3.1/client/model/upstream_of_field_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/usage_per_datasource_user_dto.py` & `sifflet_sdk-0.3.1/client/model/usage_per_datasource_user_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/usage_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/usage_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/usage_search_filter_element_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/usage_search_filter_element_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/user_asset_bookmark_dto.py` & `sifflet_sdk-0.3.1/client/model/user_asset_bookmark_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/user_detail_dto.py` & `sifflet_sdk-0.3.1/client/model/user_detail_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/user_detail_with_password_dto.py` & `sifflet_sdk-0.3.1/client/model/user_detail_with_password_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/user_dto.py` & `sifflet_sdk-0.3.1/client/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/user_patch_dto.py` & `sifflet_sdk-0.3.1/client/model/user_patch_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/uuid_search_filter_element_dto.py` & `sifflet_sdk-0.3.1/client/model/uuid_search_filter_element_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/uuid_search_filter_element_dto_all_of.py` & `sifflet_sdk-0.3.1/client/model/uuid_search_filter_element_dto_all_of.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/versions_dto.py` & `sifflet_sdk-0.3.1/client/model/versions_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/workspace_apply_object_response_dto.py` & `sifflet_sdk-0.3.1/client/model/workspace_apply_object_response_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/workspace_apply_request_dto.py` & `sifflet_sdk-0.3.1/client/model/workspace_apply_request_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/workspace_apply_request_dto_changes_inner.py` & `sifflet_sdk-0.3.1/client/model/workspace_apply_request_dto_changes_inner.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/workspace_apply_response_dto.py` & `sifflet_sdk-0.3.1/client/model/workspace_apply_response_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model/workspace_dto.py` & `sifflet_sdk-0.3.1/client/model/workspace_dto.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/model_utils.py` & `sifflet_sdk-0.3.1/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/client/rest.py` & `sifflet_sdk-0.3.1/client/rest.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/pyproject.toml` & `sifflet_sdk-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/setup.py` & `sifflet_sdk-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/apis/base.py` & `sifflet_sdk-0.3.1/sifflet_sdk/apis/base.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/api.py` & `sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/code/workspace/service.py` & `sifflet_sdk-0.3.1/sifflet_sdk/code/workspace/service.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/configure/service.py` & `sifflet_sdk-0.3.1/sifflet_sdk/configure/service.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/constants.py` & `sifflet_sdk-0.3.1/sifflet_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/errors.py` & `sifflet_sdk-0.3.1/sifflet_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/ingest/api.py` & `sifflet_sdk-0.3.1/sifflet_sdk/ingest/api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/ingest/service.py` & `sifflet_sdk-0.3.1/sifflet_sdk/ingest/service.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/rules/api.py` & `sifflet_sdk-0.3.1/sifflet_sdk/rules/api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/rules/service.py` & `sifflet_sdk-0.3.1/sifflet_sdk/rules/service.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/status/api.py` & `sifflet_sdk-0.3.1/sifflet_sdk/status/api.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk/status/service.py` & `sifflet_sdk-0.3.1/sifflet_sdk/status/service.py`

 * *Files identical despite different names*

### Comparing `sifflet_sdk-0.3.0/sifflet_sdk.egg-info/SOURCES.txt` & `sifflet_sdk-0.3.1/sifflet_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

