# Comparing `tmp/pyatlan-0.4.0.tar.gz` & `tmp/pyatlan-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.4.0.tar", last modified: Wed Jul  5 03:43:15 2023, max compression
+gzip compressed data, was "pyatlan-0.4.1.tar", last modified: Mon Jul 24 09:17:41 2023, max compression
```

## Comparing `pyatlan-0.4.0.tar` & `pyatlan-0.4.1.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.251740 pyatlan-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-05 03:43:03.000000 pyatlan-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 03:43:03.000000 pyatlan-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 03:43:03.000000 pyatlan-0.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 03:43:15.251740 pyatlan-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 03:43:03.000000 pyatlan-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.235740 pyatlan-0.4.0/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50168 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/atlan_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.243740 pyatlan-0.4.0/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60934 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 03:43:03.000000 pyatlan-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 03:43:03.000000 pyatlan-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:43:15.251740 pyatlan-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-05 03:43:03.000000 pyatlan-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.243740 pyatlan-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.247740 pyatlan-0.4.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.247740 pyatlan-0.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.251740 pyatlan-0.4.0/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-24 09:17:30.000000 pyatlan-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 09:17:30.000000 pyatlan-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 09:17:30.000000 pyatlan-0.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 09:17:41.830475 pyatlan-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 09:17:30.000000 pyatlan-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.818475 pyatlan-0.4.1/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52173 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63801 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60988 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 09:17:30.000000 pyatlan-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 09:17:30.000000 pyatlan-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:17:41.830475 pyatlan-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-24 09:17:30.000000 pyatlan-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36655 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.4.0/LICENSE` & `pyatlan-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/PKG-INFO` & `pyatlan-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.0
+Version: 0.4.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.0/README.md` & `pyatlan-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-0.4.1/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.4.1/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/enum_cache.py` & `pyatlan-0.4.1/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/group_cache.py` & `pyatlan-0.4.1/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/role_cache.py` & `pyatlan-0.4.1/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/cache/user_cache.py` & `pyatlan-0.4.1/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/client/atlan.py` & `pyatlan-0.4.1/pyatlan/client/atlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
+from __future__ import annotations
+
 import abc
 import contextlib
 import copy
 import json
 import logging
 import os
 from abc import ABC
@@ -23,14 +25,15 @@
 )
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
     ADD_BUSINESS_ATTRIBUTE_BY_ID,
     ADD_USER_TO_GROUPS,
+    ADMIN_EVENTS,
     BULK_UPDATE,
     CHANGE_USER_ROLE,
     CREATE_GROUP,
     CREATE_TYPE_DEFS,
     CREATE_USERS,
     DELETE_ENTITY_BY_ATTRIBUTE,
     DELETE_ENTITY_BY_GUID,
@@ -45,14 +48,15 @@
     GET_GROUPS,
     GET_LINEAGE,
     GET_LINEAGE_LIST,
     GET_ROLES,
     GET_USER_GROUPS,
     GET_USERS,
     INDEX_SEARCH,
+    KEYCLOAK_EVENTS,
     PARSE_QUERY,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
     REMOVE_USERS_FROM_GROUP,
     UPDATE_ENTITY_BY_ATTRIBUTE,
     UPDATE_GROUP,
     UPDATE_TYPE_DEFS,
     UPDATE_USER,
@@ -279,16 +283,24 @@
             raw_json = self._client._call_api(
                 self._endpoint,
                 request_obj=self._criteria,
             )
             if "entities" not in raw_json:
                 self._assets = []
                 return None
-            self._assets = parse_obj_as(list[Asset], raw_json["entities"])
-            return raw_json
+            try:
+                for entity in raw_json["entities"]:
+                    unflatten_custom_metadata_for_entity(
+                        entity=entity, attributes=self._criteria.attributes
+                    )
+                self._assets = parse_obj_as(list[Asset], raw_json["entities"])
+                return raw_json
+            except ValidationError as err:
+                LOGGER.error("Problem parsing JSON: %s", raw_json["entities"])
+                raise err
 
         def __iter__(self) -> Generator[Asset, None, None]:
             while True:
                 yield from self.current_page()
                 if not self.next_page():
                     break
 
@@ -766,17 +778,14 @@
         try:
             raw_json = self._call_api(
                 GET_ENTITY_BY_UNIQUE_ATTRIBUTE.format_path_with_params(
                     asset_type.__name__
                 ),
                 query_params,
             )
-            raw_json["entity"]["attributes"].update(
-                raw_json["entity"]["relationshipAttributes"]
-            )
             asset = self.handle_relationships(raw_json)
             if not isinstance(asset, asset_type):
                 raise NotFoundError(
                     message=f"Asset with qualifiedName {qualified_name} "
                     f"is not of the type requested: {asset_type.__name__}.",
                     code="ATLAN-PYTHON-404-002",
                 )
@@ -1323,14 +1332,56 @@
             criteria=lineage_request,
             start=lineage_request.offset or 0,
             size=lineage_request.size or 10,
             has_more=has_more,
             assets=assets,
         )
 
+    def get_keycloak_events(
+        self, keycloak_request: KeycloakEventRequest
+    ) -> KeycloakEventResponse:
+        if raw_json := self._call_api(
+            KEYCLOAK_EVENTS,
+            query_params=keycloak_request.query_params,
+            exclude_unset=True,
+        ):
+            try:
+                events = parse_obj_as(list[KeycloakEvent], raw_json)
+            except ValidationError as err:
+                LOGGER.error("Problem parsing JSON: %s", raw_json)
+                raise err
+        else:
+            events = []
+        return KeycloakEventResponse(
+            client=self,
+            criteria=keycloak_request,
+            start=keycloak_request.offset or 0,
+            size=keycloak_request.size or 100,
+            events=events,
+        )
+
+    def get_admin_events(self, admin_request: AdminEventRequest) -> AdminEventResponse:
+        if raw_json := self._call_api(
+            ADMIN_EVENTS, query_params=admin_request.query_params, exclude_unset=True
+        ):
+            try:
+                events = parse_obj_as(list[AdminEvent], raw_json)
+            except ValidationError as err:
+                LOGGER.error("Problem parsing JSON: %s", raw_json)
+                raise err
+        else:
+            events = []
+        return AdminEventResponse(
+            client=self,
+            criteria=admin_request,
+            start=admin_request.offset or 0,
+            size=admin_request.size or 100,
+            events=events,
+        )
+
     @validate_arguments()
     def find_personas_by_name(
         self,
         name: str,
         attributes: Optional[list[str]] = None,
     ) -> list[Persona]:
         if attributes is None:
@@ -1471,7 +1522,17 @@
     ):
         glossary = self.find_glossary_by_name(name=glossary_name)
         return self.find_term_fast_by_name(
             name=name,
             glossary_qualified_name=glossary.qualified_name,
             attributes=attributes,
         )
+
+
+from pyatlan.model.keycloak_events import (  # noqa: E402
+    AdminEvent,
+    AdminEventRequest,
+    AdminEventResponse,
+    KeycloakEvent,
+    KeycloakEventRequest,
+    KeycloakEventResponse,
+)
```

### Comparing `pyatlan-0.4.0/pyatlan/client/constants.py` & `pyatlan-0.4.1/pyatlan/client/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 
 ROLE_API = f"{ADMIN_URI}roles"
 GROUP_API = f"{ADMIN_URI}groups"
 USER_API = f"{ADMIN_URI}users"
 QUERY_API = f"{SQL_URI}query"
 IMAGE_API = f"{ADMIN_URI}images"
+LOGS_API = f"{ADMIN_URI}events"
 
 # Role APIs
 GET_ROLES = API(ROLE_API, HTTPMethod.GET, HTTPStatus.OK)
 
 # Group APIs
 GET_GROUPS = API(GROUP_API, HTTPMethod.GET, HTTPStatus.OK)
 CREATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
@@ -50,14 +51,18 @@
 
 # SQL parsing APIs
 PARSE_QUERY = API(f"{QUERY_API}/parse", HTTPMethod.POST, HTTPStatus.OK)
 
 # File upload APIs
 UPLOAD_IMAGE = API(IMAGE_API, HTTPMethod.POST, HTTPStatus.OK)
 
+# Keycloak event APIs
+KEYCLOAK_EVENTS = API(f"{LOGS_API}/login", HTTPMethod.GET, HTTPStatus.OK)
+ADMIN_EVENTS = API(f"{LOGS_API}/main", HTTPMethod.GET, HTTPStatus.OK)
+
 ENTITY_API = f"{BASE_URI}entity/"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
 BULK_SET_CLASSIFICATIONS = "bulk/setClassifications"
```

### Comparing `pyatlan-0.4.0/pyatlan/error.py` & `pyatlan-0.4.1/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/events/atlan_event_handler.py` & `pyatlan-0.4.1/pyatlan/events/atlan_event_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,23 @@
         dsl=dsl,
         attributes=attributes,
         relation_attributes=["guid"],
         exclude_meanings=~include_meanings,
         exclude_atlan_tags=~include_atlan_tags,
     )
     response = client.search(criteria=request)
-    return result if (result := response.current_page()[0]) else None
+    return (
+        result
+        if (
+            result := response.current_page()[0]
+            if len(response.current_page()) > 0
+            else None
+        )
+        else None
+    )
 
 
 def has_description(asset: Asset) -> bool:
     """
     Check if the asset has either a user-provided or system-provided description.
     """
     description = asset.user_description or asset.description
```

### Comparing `pyatlan-0.4.0/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-0.4.1/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/exceptions.py` & `pyatlan-0.4.1/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.4.1/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/assets.py` & `pyatlan-0.4.1/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/atlan_image.py` & `pyatlan-0.4.1/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/core.py` & `pyatlan-0.4.1/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/custom_metadata.py` & `pyatlan-0.4.1/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/enums.py` & `pyatlan-0.4.1/pyatlan/model/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -386,14 +386,171 @@
     POSTGRESQL = "postgresql"
     REDSHIFT = "redshift"
     SNOWFLAKE = "snowflake"
     SPARKSQL = "sparksql"
     ATHENA = "athena"
 
 
+# Source: keycloak > server-spi-private/src/main/java/org/keycloak/events/admin/OperationType.java
+class AdminOperationType(str, Enum):
+    CREATE = "CREATE"
+    UPDATE = "UPDATE"
+    DELETE = "DELETE"
+    ACTION = "ACTION"
+
+
+# Source: keycloak > server-spi-private/src/main/java/org/keycloak/events/admin/ResourceType.java
+class AdminResourceType(str, Enum):
+    REALM = "REALM"
+    REALM_ROLE = "REALM_ROLE"
+    REALM_ROLE_MAPPING = "REALM_ROLE_MAPPING"
+    REALM_SCOPE_MAPPING = "REALM_SCOPE_MAPPING"
+    AUTH_FLOW = "AUTH_FLOW"
+    AUTH_EXECUTION_FLOW = "AUTH_EXECUTION_FLOW"
+    AUTH_EXECUTION = "AUTH_EXECUTION"
+    AUTHENTICATOR_CONFIG = "AUTHENTICATOR_CONFIG"
+    REQUIRED_ACTION = "REQUIRED_ACTION"
+    IDENTITY_PROVIDER = "IDENTITY_PROVIDER"
+    IDENTITY_PROVIDER_MAPPER = "IDENTITY_PROVIDER_MAPPER"
+    PROTOCOL_MAPPER = "PROTOCOL_MAPPER"
+    USER = "USER"
+    USER_LOGIN_FAILURE = "USER_LOGIN_FAILURE"
+    USER_SESSION = "USER_SESSION"
+    USER_FEDERATION_PROVIDER = "USER_FEDERATION_PROVIDER"
+    USER_FEDERATION_MAPPER = "USER_FEDERATION_MAPPER"
+    GROUP = "GROUP"
+    GROUP_MEMBERSHIP = "GROUP_MEMBERSHIP"
+    CLIENT = "CLIENT"
+    CLIENT_INITIAL_ACCESS_MODEL = "CLIENT_INITIAL_ACCESS_MODEL"
+    CLIENT_ROLE = "CLIENT_ROLE"
+    CLIENT_ROLE_MAPPING = "CLIENT_ROLE_MAPPING"
+    CLIENT_SCOPE = "CLIENT_SCOPE"
+    CLIENT_SCOPE_MAPPING = "CLIENT_SCOPE_MAPPING"
+    CLIENT_SCOPE_CLIENT_MAPPING = "CLIENT_SCOPE_CLIENT_MAPPING"
+    CLUSTER_NODE = "CLUSTER_NODE"
+    COMPONENT = "COMPONENT"
+    AUTHORIZATION_RESOURCE_SERVER = "AUTHORIZATION_RESOURCE_SERVER"
+    AUTHORIZATION_RESOURCE = "AUTHORIZATION_RESOURCE"
+    AUTHORIZATION_SCOPE = "AUTHORIZATION_SCOPE"
+    AUTHORIZATION_POLICY = "AUTHORIZATION_POLICY"
+    CUSTOM = "CUSTOM"
+
+
+# Source: keycloak > server-spi-private/src/main/java/org/keycloak/events/EventType.java
+class KeycloakEventType(str, Enum):
+    LOGIN = "LOGIN"
+    LOGIN_ERROR = "LOGIN_ERROR"
+    REGISTER = "REGISTER"
+    REGISTER_ERROR = "REGISTER_ERROR"
+    LOGOUT = "LOGOUT"
+    LOGOUT_ERROR = "LOGOUT_ERROR"
+    CODE_TO_TOKEN = "CODE_TO_TOKEN"  # noqa: S105
+    CODE_TO_TOKEN_ERROR = "CODE_TO_TOKEN_ERROR"  # noqa: S105
+    CLIENT_LOGIN = "CLIENT_LOGIN"
+    CLIENT_LOGIN_ERROR = "CLIENT_LOGIN_ERROR"
+    REFRESH_TOKEN = "REFRESH_TOKEN"  # noqa: S105
+    REFRESH_TOKEN_ERROR = "REFRESH_TOKEN_ERROR"  # noqa: S105
+    VALIDATE_ACCESS_TOKEN = "VALIDATE_ACCESS_TOKEN"  # noqa: S105
+    VALIDATE_ACCESS_TOKEN_ERROR = "VALIDATE_ACCESS_TOKEN_ERROR"  # noqa: S105
+    INTROSPECT_TOKEN = "INTROSPECT_TOKEN"  # noqa: S105
+    INTROSPECT_TOKEN_ERROR = "INTROSPECT_TOKEN_ERROR"  # noqa: S105
+    FEDERATED_IDENTITY_LINK = "FEDERATED_IDENTITY_LINK"
+    FEDERATED_IDENTITY_LINK_ERROR = "FEDERATED_IDENTITY_LINK_ERROR"
+    REMOVE_FEDERATED_IDENTITY = "REMOVE_FEDERATED_IDENTITY"
+    REMOVE_FEDERATED_IDENTITY_ERROR = "REMOVE_FEDERATED_IDENTITY_ERROR"
+    UPDATE_EMAIL = "UPDATE_EMAIL"
+    UPDATE_EMAIL_ERROR = "UPDATE_EMAIL_ERROR"
+    UPDATE_PROFILE = "UPDATE_PROFILE"
+    UPDATE_PROFILE_ERROR = "UPDATE_PROFILE_ERROR"
+    UPDATE_PASSWORD = "UPDATE_PASSWORD"  # noqa: S105
+    UPDATE_PASSWORD_ERROR = "UPDATE_PASSWORD_ERROR"  # noqa: S105
+    UPDATE_TOTP = "UPDATE_TOTP"
+    UPDATE_TOTP_ERROR = "UPDATE_TOTP_ERROR"
+    VERIFY_EMAIL = "VERIFY_EMAIL"
+    VERIFY_EMAIL_ERROR = "VERIFY_EMAIL_ERROR"
+    VERIFY_PROFILE = "VERIFY_PROFILE"
+    VERIFY_PROFILE_ERROR = "VERIFY_PROFILE_ERROR"
+    REMOVE_TOTP = "REMOVE_TOTP"
+    REMOVE_TOTP_ERROR = "REMOVE_TOTP_ERROR"
+    GRANT_CONSENT = "GRANT_CONSENT"
+    GRANT_CONSENT_ERROR = "GRANT_CONSENT_ERROR"
+    UPDATE_CONSENT = "UPDATE_CONSENT"
+    UPDATE_CONSENT_ERROR = "UPDATE_CONSENT_ERROR"
+    REVOKE_GRANT = "REVOKE_GRANT"
+    REVOKE_GRANT_ERROR = "REVOKE_GRANT_ERROR"
+    SEND_VERIFY_EMAIL = "SEND_VERIFY_EMAIL"
+    SEND_VERIFY_EMAIL_ERROR = "SEND_VERIFY_EMAIL_ERROR"
+    SEND_RESET_PASSWORD = "SEND_RESET_PASSWORD"  # noqa: S105
+    SEND_RESET_PASSWORD_ERROR = "SEND_RESET_PASSWORD_ERROR"  # noqa: S105
+    SEND_IDENTITY_PROVIDER_LINK = "SEND_IDENTITY_PROVIDER_LINK"
+    SEND_IDENTITY_PROVIDER_LINK_ERROR = "SEND_IDENTITY_PROVIDER_LINK_ERROR"
+    RESET_PASSWORD = "RESET_PASSWORD"  # noqa: S105
+    RESET_PASSWORD_ERROR = "RESET_PASSWORD_ERROR"  # noqa: S105
+    RESTART_AUTHENTICATION = "RESTART_AUTHENTICATION"
+    RESTART_AUTHENTICATION_ERROR = "RESTART_AUTHENTICATION_ERROR"
+    INVALID_SIGNATURE = "INVALID_SIGNATURE"
+    INVALID_SIGNATURE_ERROR = "INVALID_SIGNATURE_ERROR"
+    REGISTER_NODE = "REGISTER_NODE"
+    REGISTER_NODE_ERROR = "REGISTER_NODE_ERROR"
+    UNREGISTER_NODE = "UNREGISTER_NODE"
+    UNREGISTER_NODE_ERROR = "UNREGISTER_NODE_ERROR"
+    USER_INFO_REQUEST = "USER_INFO_REQUEST"
+    USER_INFO_REQUEST_ERROR = "USER_INFO_REQUEST_ERROR"
+    IDENTITY_PROVIDER_LINK_ACCOUNT = "IDENTITY_PROVIDER_LINK_ACCOUNT"
+    IDENTITY_PROVIDER_LINK_ACCOUNT_ERROR = "IDENTITY_PROVIDER_LINK_ACCOUNT_ERROR"
+    IDENTITY_PROVIDER_LOGIN = "IDENTITY_PROVIDER_LOGIN"
+    IDENTITY_PROVIDER_LOGIN_ERROR = "IDENTITY_PROVIDER_LOGIN_ERROR"
+    IDENTITY_PROVIDER_FIRST_LOGIN = "IDENTITY_PROVIDER_FIRST_LOGIN"
+    IDENTITY_PROVIDER_FIRST_LOGIN_ERROR = "IDENTITY_PROVIDER_FIRST_LOGIN_ERROR"
+    IDENTITY_PROVIDER_POST_LOGIN = "IDENTITY_PROVIDER_POST_LOGIN"
+    IDENTITY_PROVIDER_POST_LOGIN_ERROR = "IDENTITY_PROVIDER_POST_LOGIN_ERROR"
+    IDENTITY_PROVIDER_RESPONSE = "IDENTITY_PROVIDER_RESPONSE"
+    IDENTITY_PROVIDER_RESPONSE_ERROR = "IDENTITY_PROVIDER_RESPONSE_ERROR"
+    IDENTITY_PROVIDER_RETRIEVE_TOKEN = "IDENTITY_PROVIDER_RETRIEVE_TOKEN"  # noqa: S105
+    IDENTITY_PROVIDER_RETRIEVE_TOKEN_ERROR = (
+        "IDENTITY_PROVIDER_RETRIEVE_TOKEN_ERROR"  # noqa: S105
+    )
+    IMPERSONATE = "IMPERSONATE"
+    IMPERSONATE_ERROR = "IMPERSONATE_ERROR"
+    CUSTOM_REQUIRED_ACTION = "CUSTOM_REQUIRED_ACTION"
+    CUSTOM_REQUIRED_ACTION_ERROR = "CUSTOM_REQUIRED_ACTION_ERROR"
+    EXECUTE_ACTIONS = "EXECUTE_ACTIONS"
+    EXECUTE_ACTIONS_ERROR = "EXECUTE_ACTIONS_ERROR"
+    EXECUTE_ACTION_TOKEN = "EXECUTE_ACTION_TOKEN"  # noqa: S105
+    EXECUTE_ACTION_TOKEN_ERROR = "EXECUTE_ACTION_TOKEN_ERROR"  # noqa: S105
+    CLIENT_INFO = "CLIENT_INFO"
+    CLIENT_INFO_ERROR = "CLIENT_INFO_ERROR"
+    CLIENT_REGISTER = "CLIENT_REGISTER"
+    CLIENT_REGISTER_ERROR = "CLIENT_REGISTER_ERROR"
+    CLIENT_UPDATE = "CLIENT_UPDATE"
+    CLIENT_UPDATE_ERROR = "CLIENT_UPDATE_ERROR"
+    CLIENT_DELETE = "CLIENT_DELETE"
+    CLIENT_DELETE_ERROR = "CLIENT_DELETE_ERROR"
+    CLIENT_INITIATED_ACCOUNT_LINKING = "CLIENT_INITIATED_ACCOUNT_LINKING"
+    CLIENT_INITIATED_ACCOUNT_LINKING_ERROR = "CLIENT_INITIATED_ACCOUNT_LINKING_ERROR"
+    TOKEN_EXCHANGE = "TOKEN_EXCHANGE"  # noqa: S105
+    TOKEN_EXCHANGE_ERROR = "TOKEN_EXCHANGE_ERROR"  # noqa: S105
+    OAUTH2_DEVICE_AUTH = "OAUTH2_DEVICE_AUTH"
+    OAUTH2_DEVICE_AUTH_ERROR = "OAUTH2_DEVICE_AUTH_ERROR"
+    OAUTH2_DEVICE_VERIFY_USER_CODE = "OAUTH2_DEVICE_VERIFY_USER_CODE"
+    OAUTH2_DEVICE_VERIFY_USER_CODE_ERROR = "OAUTH2_DEVICE_VERIFY_USER_CODE_ERROR"
+    OAUTH2_DEVICE_CODE_TO_TOKEN = "OAUTH2_DEVICE_CODE_TO_TOKEN"  # noqa: S105
+    OAUTH2_DEVICE_CODE_TO_TOKEN_ERROR = (
+        "OAUTH2_DEVICE_CODE_TO_TOKEN_ERROR"  # noqa: S105
+    )
+    AUTHREQID_TO_TOKEN = "AUTHREQID_TO_TOKEN"  # noqa: S105
+    AUTHREQID_TO_TOKEN_ERROR = "AUTHREQID_TO_TOKEN_ERROR"  # noqa: S105
+    PERMISSION_TOKEN = "PERMISSION_TOKEN"  # noqa: S105
+    PERMISSION_TOKEN_ERROR = "PERMISSION_TOKEN_ERROR"  # noqa: S105
+    DELETE_ACCOUNT = "DELETE_ACCOUNT"
+    DELETE_ACCOUNT_ERROR = "DELETE_ACCOUNT_ERROR"
+    PUSHED_AUTHORIZATION_REQUEST = "PUSHED_AUTHORIZATION_REQUEST"
+    PUSHED_AUTHORIZATION_REQUEST_ERROR = "PUSHED_AUTHORIZATION_REQUEST_ERROR"
+
+
 class AuthPolicyType(str, Enum):
     ALLOW = "allow"
     DENY = "deny"
     ALLOWEXCEPTIONS = "allowExceptions"
     DENYEXCEPTIONS = "denyExceptions"
     DATAMASK = "dataMask"
     ROWFILTER = "rowFilter"
```

### Comparing `pyatlan-0.4.0/pyatlan/model/events.py` & `pyatlan-0.4.1/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/group.py` & `pyatlan-0.4.1/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/lineage.py` & `pyatlan-0.4.1/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/query.py` & `pyatlan-0.4.1/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/response.py` & `pyatlan-0.4.1/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/role.py` & `pyatlan-0.4.1/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/search.py` & `pyatlan-0.4.1/pyatlan/model/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     MODIFIED_BY = ("__modifiedBy", StrictStr)
     NAME = ("name.keyword", StrictStr)
     OWNER_GROUPS = ("ownerGroups", StrictStr)
     OWNER_USERS = ("ownerUsers", StrictStr)
     PARENT_CATEGORY = ("__parentCategory", StrictStr)
     POPULARITY_SCORE = ("popularityScore", float)
     QUALIFIED_NAME = ("qualifiedName", StrictStr)
-    STATE = ("__state", Literal["ACTIVE", "DELETED"])
+    STATE = ("__state", Literal["ACTIVE", "DELETED", "PURGED"])
     SUPER_TYPE_NAMES = ("__superTypeNames.keyword", StrictStr)
     TYPE_NAME = ("__typeName.keyword", StrictStr)
     UPDATE_TIME_AS_TIMESTAMP = ("__modificationTimestamp", datetime)
 
 
 class TextAttributes(Attributes):
     CLASSIFICATION_NAMES = ("__classificationNames", StrictStr)
@@ -431,15 +431,15 @@
     @classmethod
     @validate_arguments()
     def with_super_type_names(cls, value: StrictStr):
         return cls(field=TermAttributes.SUPER_TYPE_NAMES.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_state(cls, value: Literal["ACTIVE", "DELETE"]):
+    def with_state(cls, value: Literal["ACTIVE", "DELETED", "PURGED"]):
         return cls(field=TermAttributes.STATE.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_create_time_as_timestamp(cls, value: datetime):
         return cls(field=TermAttributes.CREATE_TIME_AS_TIMESTAMP.value, value=value)
 
@@ -663,15 +663,15 @@
     @classmethod
     @validate_arguments()
     def with_qualified_name(cls, value: StrictStr):
         return cls(field=TermAttributes.QUALIFIED_NAME.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_state(cls, value: Literal["ACTIVE", "DELETE"]):
+    def with_state(cls, value: Literal["ACTIVE", "DELETED", "PURGED"]):
         return cls(field=TermAttributes.STATE.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_super_type_names(cls, value: StrictStr):
         return cls(field=TermAttributes.SUPER_TYPE_NAMES.value, value=value)
 
@@ -926,15 +926,15 @@
     @classmethod
     @validate_arguments()
     def with_super_type_names(cls, value: StrictStr):
         return cls(field=TermAttributes.SUPER_TYPE_NAMES.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_state(cls, value: Literal["ACTIVE", "DELETE"]):
+    def with_state(cls, value: Literal["ACTIVE", "DELETED", "PURGED"]):
         return cls(field=TermAttributes.STATE.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_type_name(cls, value: StrictStr):
         return cls(field=TermAttributes.TYPE_NAME.value, value=value)
 
@@ -1018,15 +1018,15 @@
     @classmethod
     @validate_arguments()
     def with_super_type_names(cls, value: StrictStr):
         return cls(field=TermAttributes.SUPER_TYPE_NAMES.value, value=value)
 
     @classmethod
     @validate_arguments()
-    def with_state(cls, value: Literal["ACTIVE", "DELETE"]):
+    def with_state(cls, value: Literal["ACTIVE", "DELETED", "PURGED"]):
         return cls(field=TermAttributes.STATE.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_type_name(cls, value: StrictStr):
         return cls(field=TermAttributes.TYPE_NAME.value, value=value)
```

### Comparing `pyatlan-0.4.0/pyatlan/model/structs.py` & `pyatlan-0.4.1/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/typedef.py` & `pyatlan-0.4.1/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/model/user.py` & `pyatlan-0.4.1/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/multipart_data_generator.py` & `pyatlan-0.4.1/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan/utils.py` & `pyatlan-0.4.1/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.4.1/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.0
+Version: 0.4.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.0/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.4.1/pyatlan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 pyatlan/model/atlan_image.py
 pyatlan/model/core.py
 pyatlan/model/custom_metadata.py
 pyatlan/model/enums.py
 pyatlan/model/events.py
 pyatlan/model/group.py
 pyatlan/model/internal.py
+pyatlan/model/keycloak_events.py
 pyatlan/model/lineage.py
 pyatlan/model/query.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
```

### Comparing `pyatlan-0.4.0/setup.py` & `pyatlan-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/admin_test.py` & `pyatlan-0.4.1/tests/integration/admin_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.cache.role_cache import RoleCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
+from pyatlan.model.keycloak_events import AdminEventRequest, KeycloakEventRequest
 from pyatlan.model.user import AtlanUser
 from tests.integration.client import TestId
 
 MODULE_NAME = TestId.make_unique("Admin")
 GROUP_NAME1 = f"{MODULE_NAME}1"
 GROUP_NAME2 = f"{MODULE_NAME}2"
 
@@ -274,7 +275,35 @@
     assert user1.id
     response = client.get_groups_for_user(user1.id)
     assert (
         response.records is None
         or len(response.records) == 0
         or len(response.records) == _default_group_count
     )
+
+
+@pytest.mark.order(after="test_final_user_state")
+def test_retrieve_logs(
+    client: AtlanClient,
+    users: list[AtlanUser],
+):
+    request = KeycloakEventRequest(date_from="2023-07-12", date_to="2023-07-13")
+    events = client.get_keycloak_events(request)
+    assert events
+    count = 0
+    for _ in events:
+        count += 1
+    assert count > 0
+
+
+@pytest.mark.order(after="test_final_user_state")
+def test_retrieve_admin_logs(
+    client: AtlanClient,
+    users: list[AtlanUser],
+):
+    request = AdminEventRequest(date_from="2023-07-12", date_to="2023-07-13")
+    events = client.get_admin_events(request)
+    assert events
+    count = 0
+    for _ in events:
+        count += 1
+    assert count > 0
```

### Comparing `pyatlan-0.4.0/tests/integration/atlan_tag_test.py` & `pyatlan-0.4.1/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/client.py` & `pyatlan-0.4.1/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/connection_test.py` & `pyatlan-0.4.1/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/custom_metadata_test.py` & `pyatlan-0.4.1/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/file_test.py` & `pyatlan-0.4.1/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/glossary_test.py` & `pyatlan-0.4.1/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/lineage_test.py` & `pyatlan-0.4.1/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/persona_test.py` & `pyatlan-0.4.1/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/purpose_test.py` & `pyatlan-0.4.1/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/query_parser_test.py` & `pyatlan-0.4.1/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/s3_asset_test.py` & `pyatlan-0.4.1/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/test_client.py` & `pyatlan-0.4.1/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/test_index_search.py` & `pyatlan-0.4.1/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/integration/test_sql_assets.py` & `pyatlan-0.4.1/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/conftest.py` & `pyatlan-0.4.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/badge_condition_test.py` & `pyatlan-0.4.1/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/badge_test.py` & `pyatlan-0.4.1/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/column_test.py` & `pyatlan-0.4.1/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/connection_test.py` & `pyatlan-0.4.1/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/constants.py` & `pyatlan-0.4.1/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/database_test.py` & `pyatlan-0.4.1/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/file_test.py` & `pyatlan-0.4.1/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/glossary_category_test.py` & `pyatlan-0.4.1/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/glossary_term_test.py` & `pyatlan-0.4.1/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/glossary_test.py` & `pyatlan-0.4.1/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/materialised_view_test.py` & `pyatlan-0.4.1/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/process_test.py` & `pyatlan-0.4.1/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/readme_test.py` & `pyatlan-0.4.1/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.4.1/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/s3object_test.py` & `pyatlan-0.4.1/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/schema_test.py` & `pyatlan-0.4.1/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/table_test.py` & `pyatlan-0.4.1/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/model/view_test.py` & `pyatlan-0.4.1/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_atlan_tag_name.py` & `pyatlan-0.4.1/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_client.py` & `pyatlan-0.4.1/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_custom_metadata.py` & `pyatlan-0.4.1/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_events.py` & `pyatlan-0.4.1/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_glossary_term.py` & `pyatlan-0.4.1/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_lineage.py` & `pyatlan-0.4.1/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_model.py` & `pyatlan-0.4.1/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_search_model.py` & `pyatlan-0.4.1/tests/unit/test_search_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 )
 
 NOW = datetime.now()
 VALUES_BY_TYPE: dict[Union[type, object], Union[str, datetime, object]] = {
     StrictStr: "abc",
     StrictBool: True,
     datetime: NOW,
-    Literal["ACTIVE", "DELETED"]: "ACTIVE",
+    Literal["ACTIVE", "DELETED", "PURGED"]: "ACTIVE",
     float: 1.0,
     AtlanConnectorType: AtlanConnectorType.SNOWFLAKE,
 }
 
 INCOMPATIPLE_QUERY: dict[type, set[TermAttributes]] = {
     Wildcard: {
         TermAttributes.CONNECTOR_NAME,
```

### Comparing `pyatlan-0.4.0/tests/unit/test_typedef_model.py` & `pyatlan-0.4.1/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.0/tests/unit/test_utils.py` & `pyatlan-0.4.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

