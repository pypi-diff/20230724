# Comparing `tmp/tecton-0.7.0rc2.tar.gz` & `tmp/tecton-0.7.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.7.0rc2.tar", last modified: Thu Jul 20 02:14:45 2023, max compression
+gzip compressed data, was "tecton-0.7.0rc3.tar", last modified: Mon Jul 24 21:00:50 2023, max compression
```

## Comparing `tecton-0.7.0rc2.tar` & `tecton-0.7.0rc3.tar`

### file list

```diff
@@ -1,555 +1,555 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.859595 tecton-0.7.0rc2/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-20 02:14:45.859595 tecton-0.7.0rc2/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.807592 tecton-0.7.0rc2/protoc_gen_swagger/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/protoc_gen_swagger/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.807592 tecton-0.7.0rc2/protoc_gen_swagger/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/protoc_gen_swagger/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-07-20 02:14:45.859595 tecton-0.7.0rc2/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2094 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.807592 tecton-0.7.0rc2/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5361 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.811592 tecton-0.7.0rc2/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2259 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6181 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      944 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26511 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.811592 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3115 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2628 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/query_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.811592 tecton-0.7.0rc2/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11417 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15439 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12522 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9019 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26066 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15669 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_internals/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.815592 tecton-0.7.0rc2/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34602 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2953 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14945 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3348 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5832 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.815592 tecton-0.7.0rc2/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      810 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    89131 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20716 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31597 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10597 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34112 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   165950 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21844 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22879 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.815592 tecton-0.7.0rc2/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.815592 tecton-0.7.0rc2/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.815592 tecton-0.7.0rc2/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.819593 tecton-0.7.0rc2/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.819593 tecton-0.7.0rc2/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.819593 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.823593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.823593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.827593 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.831594 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.831594 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.831594 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.831594 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.807592 tecton-0.7.0rc2/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19035 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      833 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-07-20 02:14:44.000000 tecton-0.7.0rc2/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.835594 tecton-0.7.0rc2/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14608 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8482 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/odfv_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.835594 tecton-0.7.0rc2/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2291 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17764 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.835594 tecton-0.7.0rc2/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.835594 tecton-0.7.0rc2/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13329 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19520 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7206 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5415 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4818 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17300 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2300 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7393 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/materialization_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6916 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6304 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/pipeline_common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4393 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/pipeline_sql_builder.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10765 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26314 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8446 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    66482 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2677 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8340 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      610 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9133 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      397 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4835 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5562 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/schema_derivation_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38770 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30873 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4912 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.839594 tecton-0.7.0rc2/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    85094 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4122 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33904 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19265 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3544 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/common/spark_schema_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.843594 tecton-0.7.0rc2/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.847595 tecton-0.7.0rc2/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/data_source_access_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15392 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1907 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12187 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1743 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.847595 tecton-0.7.0rc2/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8185 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13426 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13314 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   107952 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/online_store_writer/config_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/snowflake/location_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7339 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.851595 tecton-0.7.0rc2/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.855595 tecton-0.7.0rc2/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29228 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32077 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.855595 tecton-0.7.0rc2/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6695 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.855595 tecton-0.7.0rc2/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25652 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2090 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35854 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.855595 tecton-0.7.0rc2/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1604241 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4039 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22766 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11048 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34132 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:45.859595 tecton-0.7.0rc2/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18310 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4229 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5861 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5087 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11252 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5410 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2135 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1677 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4842 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-07-20 02:14:42.000000 tecton-0.7.0rc2/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.989688 tecton-0.7.0rc3/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-24 21:00:50.989688 tecton-0.7.0rc3/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.865618 tecton-0.7.0rc3/protoc_gen_swagger/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/protoc_gen_swagger/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.865618 tecton-0.7.0rc3/protoc_gen_swagger/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/protoc_gen_swagger/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-07-24 21:00:50.989688 tecton-0.7.0rc3/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2094 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.865618 tecton-0.7.0rc3/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5361 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.873622 tecton-0.7.0rc3/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2259 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6181 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      944 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26511 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.881627 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3115 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2628 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/query_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.881627 tecton-0.7.0rc3/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11417 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15439 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12522 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9021 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26066 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15669 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_internals/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      273 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.889631 tecton-0.7.0rc3/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34144 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2953 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14945 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3281 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5832 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.893634 tecton-0.7.0rc3/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      810 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    89131 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20233 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31597 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10597 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34112 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   165809 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21844 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22879 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.893634 tecton-0.7.0rc3/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.893634 tecton-0.7.0rc3/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.893634 tecton-0.7.0rc3/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.897636 tecton-0.7.0rc3/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.897636 tecton-0.7.0rc3/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.901638 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.909643 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.909643 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.917647 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.917647 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.917647 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.921650 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.921650 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.921650 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.921650 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.921650 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.925652 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.929654 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.929654 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.933656 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.933656 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.869620 tecton-0.7.0rc3/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-24 21:00:48.000000 tecton-0.7.0rc3/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19035 2023-07-24 21:00:49.000000 tecton-0.7.0rc3/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-07-24 21:00:48.000000 tecton-0.7.0rc3/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-07-24 21:00:48.000000 tecton-0.7.0rc3/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      833 2023-07-24 21:00:48.000000 tecton-0.7.0rc3/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-07-24 21:00:49.000000 tecton-0.7.0rc3/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.933656 tecton-0.7.0rc3/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14608 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8482 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/odfv_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.933656 tecton-0.7.0rc3/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2291 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17764 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.937659 tecton-0.7.0rc3/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.941661 tecton-0.7.0rc3/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13329 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19520 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7206 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5415 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4818 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17300 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2300 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7393 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/materialization_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6916 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6304 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/pipeline_common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4393 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/pipeline_sql_builder.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.945663 tecton-0.7.0rc3/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10765 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26314 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8446 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    66482 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.945663 tecton-0.7.0rc3/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2677 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8340 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      610 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9133 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      397 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4835 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5562 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/schema_derivation_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.945663 tecton-0.7.0rc3/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38770 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30873 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4912 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.945663 tecton-0.7.0rc3/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.949665 tecton-0.7.0rc3/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.949665 tecton-0.7.0rc3/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.949665 tecton-0.7.0rc3/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.949665 tecton-0.7.0rc3/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.949665 tecton-0.7.0rc3/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    85094 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.953668 tecton-0.7.0rc3/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4122 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34203 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.953668 tecton-0.7.0rc3/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19265 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3544 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.953668 tecton-0.7.0rc3/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.953668 tecton-0.7.0rc3/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.957670 tecton-0.7.0rc3/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/common/spark_schema_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.957670 tecton-0.7.0rc3/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.965674 tecton-0.7.0rc3/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/data_source_access_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15392 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1907 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12187 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1743 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8185 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13426 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13314 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.969677 tecton-0.7.0rc3/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   107952 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/online_store_writer/config_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/snowflake/location_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.973679 tecton-0.7.0rc3/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7339 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.977681 tecton-0.7.0rc3/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.977681 tecton-0.7.0rc3/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29228 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32077 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.981684 tecton-0.7.0rc3/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6695 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.985686 tecton-0.7.0rc3/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25814 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2090 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35854 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.985686 tecton-0.7.0rc3/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1600615 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4039 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22766 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11048 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34132 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:50.989688 tecton-0.7.0rc3/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18310 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4229 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5861 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5087 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11252 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5410 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2135 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1677 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4842 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-07-24 21:00:44.000000 tecton-0.7.0rc3/tecton_spark/udfs.py
```

### Comparing `tecton-0.7.0rc2/PKG-INFO` & `tecton-0.7.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0rc2
+Version: 0.7.0rc3
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0rc2/README.md` & `tecton-0.7.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/protoc_gen_swagger/options/annotations_pb2.py` & `tecton-0.7.0rc3/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/protoc_gen_swagger/options/openapiv2_pb2.py` & `tecton-0.7.0rc3/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/setup.py` & `tecton-0.7.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.7.0rc2',
+    version='0.7.0rc3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version'],
     extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'snowflake': ['snowflake-connector-python[pandas]~=2.8'], 'snowpark': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=2.15']},
     packages=packages,
 )
```

### Comparing `tecton-0.7.0rc2/tecton/__init__.py` & `tecton-0.7.0rc3/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/analytics.py` & `tecton-0.7.0rc3/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/athena_api.py` & `tecton-0.7.0rc3/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/data_frame_helper.py` & `tecton-0.7.0rc3/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/delete_keys_api.py` & `tecton-0.7.0rc3/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/display.py` & `tecton-0.7.0rc3/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/env_utils.py` & `tecton-0.7.0rc3/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/errors.py` & `tecton-0.7.0rc3/tecton/_internals/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/find_spark.py` & `tecton-0.7.0rc3/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/ingest_utils.py` & `tecton-0.7.0rc3/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/materialization_api.py` & `tecton-0.7.0rc3/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/error_lib.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/http_client.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/response.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/metadata_service_impl/service_calls.py` & `tecton-0.7.0rc3/tecton/_internals/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/mock_source_utils.py` & `tecton-0.7.0rc3/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/query_helper.py` & `tecton-0.7.0rc3/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/repo/function_serialization.py` & `tecton-0.7.0rc3/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/rewrite.py` & `tecton-0.7.0rc3/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/run_api.py` & `tecton-0.7.0rc3/tecton/_internals/run_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/sdk_decorators.py` & `tecton-0.7.0rc3/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/snowflake_api.py` & `tecton-0.7.0rc3/tecton/_internals/snowflake_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     start_time = get_timezone_aware_datetime(start_time)
     end_time = get_timezone_aware_datetime(end_time)
 
     if conf.get_bool("ALPHA_SNOWFLAKE_SNOWPARK_ENABLED"):
         if entities is not None:
             # Convert entities to a snowflake dataframe
             if isinstance(entities, pandas.DataFrame):
-                entities = TectonDataFrame._create(entities).to_snowflake()
+                entities = TectonDataFrame._create(entities).to_snowpark()()
             elif isinstance(entities, TectonDataFrame):
-                entities = entities.to_snowflake()
+                entities = entities.to_snowpark()()
 
         return TectonDataFrame._create_with_snowflake(
             sql_helper.get_historical_features_with_snowpark(
                 spine=spine,
                 session=SnowflakeContext.get_instance().get_session(),
                 timestamp_key=timestamp_key,
                 feature_set_config=feature_set_config,
```

### Comparing `tecton-0.7.0rc2/tecton/_internals/spark_api.py` & `tecton-0.7.0rc3/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/spark_utils.py` & `tecton-0.7.0rc3/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/time_utils.py` & `tecton-0.7.0rc3/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/type_utils.py` & `tecton-0.7.0rc3/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/utils.py` & `tecton-0.7.0rc3/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/_internals/validations_api.py` & `tecton-0.7.0rc3/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/aggregation_functions.py` & `tecton-0.7.0rc3/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/access_control.py` & `tecton-0.7.0rc3/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/api_key.py` & `tecton-0.7.0rc3/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/cli.py` & `tecton-0.7.0rc3/tecton/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,26 +174,24 @@
         def callback(
             ctx,
             yes,
             safety_checks,
             no_safety_checks,
             json_out,
             suppress_warnings,
-            server_side_rendering,
             workspace,  # Not used but it needs to be here to match params list.
             suppress_recreates=False,
             plan_id=None,
             skip_tests=None,
         ):
             args = EngineArgs(
                 skip_tests=skip_tests,
                 json_out=json_out,
                 no_safety_checks=yes or no_safety_checks,
                 suppress_warnings=suppress_warnings,
-                server_side_rendering=server_side_rendering,
                 debug=common.get_debug(ctx),
             )
 
             assert not (plan_id and suppress_recreates), (
                 "The flag --suppress-recreates is only used when computing a new plan. If the plan passed "
                 "in using --plan-id was already computed using --suppress-recreates, that behavior persists "
                 "as part of the plan."
@@ -248,20 +246,14 @@
             click.Option(
                 ["--suppress-warnings"],
                 is_flag=True,
                 default=False,
                 help="Disable tecton plan linting warnings.",
             ),
             click.Option(
-                ["--server-side-rendering/--no-server-side-rendering"],
-                default=True,
-                help="Render tecton plan output on the server side instead of client side.",
-                hidden=True,
-            ),
-            click.Option(
                 ["--workspace"],
                 default=None,
                 type=WorkspaceType(),
                 help="Name of the target workspace that tecton state update request applies to.",
             ),
         ]
         if not destroy:
@@ -553,15 +545,14 @@
 # do a deep refactoring of the code that depends on it. It should be replaced.
 @dataclass
 class EngineArgs:
     skip_tests: bool
     no_safety_checks: bool
     json_out: str
     suppress_warnings: bool
-    server_side_rendering: bool
 
     debug: bool
 
 
 def _no_color_convention() -> bool:
     """Follow convention for ANSI coloring of CLI tools. See no-color.org."""
     for key, value in os.environ.items():
@@ -614,15 +605,14 @@
         upgrade_all=upgrade_all,
         suppress_warnings=args.suppress_warnings,
         suppress_recreates=suppress_recreates,
         json_out_path=json_out_path,
         plan_id=plan_id,
         workspace_name=tecton_context.get_current_workspace(),
         no_color=no_color,
-        enable_server_side_rendering=args.server_side_rendering,
     )
 
 
 @cli.command(requires_auth=False)
 def init() -> None:
     """Initialize feature repo."""
     init_feature_repo()
```

### Comparing `tecton-0.7.0rc2/tecton/cli/cli_utils.py` & `tecton-0.7.0rc3/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/command.py` & `tecton-0.7.0rc3/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/common.py` & `tecton-0.7.0rc3/tecton/cli/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/engine.py` & `tecton-0.7.0rc3/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/engine_renderer.py` & `tecton-0.7.0rc3/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/environment.py` & `tecton-0.7.0rc3/tecton/cli/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,18 @@
 def environment():
     """Manage environments"""
 
 
 @environment.command("list-all")
 def list_all():
     response = _list_environments()
-    headings = ["Id", "Name", "Status", "Image"]
+    headings = ["Id", "Name", "Status"]
     display_table(
         headings,
-        [
-            (i.id, i.name, RemoteEnvironmentStatus.Name(i.status), i.image_info.image_uri)
-            for i in response.remote_environments
-        ],
+        [(i.id, i.name, RemoteEnvironmentStatus.Name(i.status)) for i in response.remote_environments],
     )
 
 
 @environment.command("create")
 @click.option("-n", "--name", help="Environment name", required=True, type=str)
 @click.option("-d", "--description", help="Environment description", required=True, type=str)
 @click.option("-i", "--image-uri", help="Image URI", required=True, type=str)
```

### Comparing `tecton-0.7.0rc2/tecton/cli/error_utils.py` & `tecton-0.7.0rc3/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/printer.py` & `tecton-0.7.0rc3/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/service_account.py` & `tecton-0.7.0rc3/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/user.py` & `tecton-0.7.0rc3/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/workspace.py` & `tecton-0.7.0rc3/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/cli/workspace_utils.py` & `tecton-0.7.0rc3/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/fco_listers.py` & `tecton-0.7.0rc3/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/base_tecton_object.py` & `tecton-0.7.0rc3/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/compute_mode.py` & `tecton-0.7.0rc3/tecton/framework/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/configs.py` & `tecton-0.7.0rc3/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/data_frame.py` & `tecton-0.7.0rc3/tecton/framework/data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,38 +304,25 @@
         )
 
     def _get_querytree_views(self):
         qt_views = []
         recurse_query_tree(self._querytree, lambda node: qt_views.extend(node.get_sql_views()))
         return qt_views
 
-    # TODO(TEC-11097): Deprecate this method after version 0.7.0
     @sdk_public_method
     def to_snowflake(self) -> snowpark_dataframe:
         """
         Deprecated. Please use to_snowpark() instead.
         Returns data as a Snowflake DataFrame.
 
         :return: A Snowflake DataFrame.
         :meta private:
         """
-        logger.warning("to_snowflake() is deprecated - please use to_snowpark() instead.")
-
-        if self._snowflake_df is not None:
-            return self._snowflake_df
-
-        assert self._pandas_df is not None
-
-        from tecton.snowflake_context import SnowflakeContext
-
-        if conf.get_bool("ALPHA_SNOWFLAKE_SNOWPARK_ENABLED"):
-            return SnowflakeContext.get_instance().get_session().createDataFrame(self._pandas_df)
-        else:
-            msg = "to_snowflake() is only available with Snowpark enabled"
-            raise Exception(msg)
+        msg = "to_snowflake() is deprecated and is no longer supported in 0.7 PLease use to_snowpark() instead."
+        raise RuntimeError(msg)
 
     @sdk_public_method
     def to_snowpark(self) -> snowpark_dataframe:
         """
         Returns data as a Snowpark DataFrame.
 
         :return: A Snowpark DataFrame.
```

### Comparing `tecton-0.7.0rc2/tecton/framework/data_source.py` & `tecton-0.7.0rc3/tecton/framework/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/dataset.py` & `tecton-0.7.0rc3/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/entity.py` & `tecton-0.7.0rc3/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/feature_service.py` & `tecton-0.7.0rc3/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/feature_view.py` & `tecton-0.7.0rc3/tecton/framework/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1526,15 +1526,15 @@
                     {credit_scores_batch}
             '''
     """
 
     if max_batch_aggregation_interval is not None:
         assert max_backfill_interval is None, "Cannot set both max_backfill_interval and max_batch_aggregation_interval"
         logger.warning(
-            "FeatureView.max_batch_aggregation_interval is deprecated. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
+            "FeatureView.max_batch_aggregation_interval is deprecated and will be removed in 0.8. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
         )
 
     def decorator(feature_view_function):
         return BatchFeatureView(
             name=name or feature_view_function.__name__,
             description=description,
             owner=owner,
@@ -1643,21 +1643,16 @@
         """Construct a StreamFeatureView.
 
         `init` should not be used directly, and instead :py:func:`tecton.stream_feature_view` decorator is recommended.
         """
         from tecton.cli import common as cli_common
 
         if aggregation_mode is not None:
-            logger.warning(
-                f"StreamFeatureView '{name}' sets aggregation_mode, which is deprecated and will be removed in tecton 0.7. Use stream_processing_mode=StreamProcessingMode.CONTINUOUS (or TIME_INTERVAL) instead."
-            )
-            if stream_processing_mode is not None:
-                msg = "Cannot set both aggregation_mode and stream_processing_mode. aggregation_mode is deprecated. Use stream_processing_mode instead."
-                raise core_errors.TectonValidationError(msg)
-            stream_processing_mode = aggregation_mode
+            msg = "aggregation_mode is deprecated and is no longer supported in 0.7. Please use stream_processing_mode instead."
+            raise ValueError(msg)
 
         data_source = source.source if isinstance(source, filtered_source.FilteredSource) else source
         has_push_source = isinstance(data_source, framework_data_source.PushSource)
         _validate_fv_input_count([source], feature_view_function)
 
         if has_push_source:
             # Stream Feature Views with Push Sources do not have transformations, so the entire pipeline is the source.
@@ -1954,15 +1949,15 @@
                     {transactions_stream}
                 '''
     """
 
     if max_batch_aggregation_interval is not None:
         assert max_backfill_interval is None, "Cannot set both max_backfill_interval and max_batch_aggregation_interval"
         logger.warning(
-            "FeatureView.max_batch_aggregation_interval is deprecated. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
+            "FeatureView.max_batch_aggregation_interval is deprecated and will be removed in 0.8. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
         )
 
     def decorator(feature_view_function):
         return StreamFeatureView(
             name=name or feature_view_function.__name__,
             description=description,
             owner=owner,
@@ -2068,14 +2063,15 @@
                 configs.EMRClusterConfig,
                 configs.DatabricksJsonClusterConfig,
                 configs.DataprocJsonClusterConfig,
                 configs.EMRJsonClusterConfig,
             ]
         ] = None,
         online_serving_index: Optional[List[str]] = None,
+        alert_email: Optional[str] = None,
     ):
         """Instantiate a new FeatureTable.
 
         :param name: Unique, human friendly name that identifies the FeatureTable.
         :param description: A human readable description.
         :param owner: Owner name (typically the email of the primary maintainer).
         :param tags: Tags associated with this Tecton Object (key-value pairs of arbitrary metadata).
@@ -2095,14 +2091,15 @@
         :param offline_store: Configuration for how data is written to the offline feature store.
         :param online_store: Configuration for how data is written to the online feature store.
         :param batch_compute: Configuration for batch materialization clusters. Should be one of:
             [:class:`EMRClusterConfig`, :class:`DatabricksClusterConfig`, :class:`EMRJsonClusterConfig`, :class:`DatabricksJsonClusterConfig`, :class:`DataprocJsonClusterConfig`]
         :param online_serving_index: (Advanced) Defines the set of join keys that will be indexed and queryable during online serving.
             Defaults to the complete set of join keys. Up to one join key may be omitted. If one key is omitted, online requests to a Feature Service will
             return all feature vectors that match the specified join keys.
+        :param alert_email: Email that alerts for this FeatureView will be sent to.
         """
         from tecton.cli import common as cli_common
 
         if isinstance(schema, list):
             wrapper = type_utils.to_spark_schema_wrapper(schema)
         else:
             wrapper = spark_schema_wrapper.SparkSchemaWrapper(schema)
@@ -2116,14 +2113,15 @@
 
         feature_table_args = feature_view__args_pb2.FeatureTableArgs(
             schema=wrapper.to_proto(),
             serving_ttl=time_utils.timedelta_to_proto(ttl),
             batch_compute=batch_compute_proto,
             offline_store=offline_store._to_proto(),
             online_store=online_store._to_proto() if online_store else None,
+            monitoring=configs.MonitoringConfig(monitor_freshness=False, alert_email=alert_email)._to_proto(),
         )
 
         # If unspecified, online_serving_index defaults to the join_keys of the Feature Table.
         join_keys = []
         for entity in entities:
             join_keys.extend(entity.join_keys)
 
@@ -3364,15 +3362,15 @@
             timestamp_field=timestamp_field,
             feature_start_time=time_utils.datetime_to_proto(feature_start_time),
             manual_trigger_backfill_end_time=time_utils.datetime_to_proto(manual_trigger_backfill_end_time),
             batch_schedule=time_utils.timedelta_to_proto(batch_schedule),
             offline_store=offline_store._to_proto(),
             online_store=online_store._to_proto() if online_store else None,
             max_backfill_interval=time_utils.timedelta_to_proto(max_backfill_interval),
-            monitoring=monitoring._to_proto() if monitoring else None,
+            monitoring=monitoring._to_proto(),
             data_source_type=data_source_type,
             incremental_backfills=incremental_backfills,
             batch_trigger=batch_trigger.value,
             output_stream=output_stream._to_proto() if output_stream else None,
             batch_compute=batch_compute_proto,
             stream_compute=stream_compute_proto,
             serving_ttl=time_utils.timedelta_to_proto(ttl),
```

### Comparing `tecton-0.7.0rc2/tecton/framework/filtered_source.py` & `tecton-0.7.0rc3/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/transformation.py` & `tecton-0.7.0rc3/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/utils.py` & `tecton-0.7.0rc3/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/validation_mode.py` & `tecton-0.7.0rc3/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/framework/workspace.py` & `tecton-0.7.0rc3/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/identities/api_keys.py` & `tecton-0.7.0rc3/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/identities/credentials.py` & `tecton-0.7.0rc3/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/identities/okta.py` & `tecton-0.7.0rc3/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/pytest_tecton.py` & `tecton-0.7.0rc3/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/snowflake_context.py` & `tecton-0.7.0rc3/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/tecton_context.py` & `tecton-0.7.0rc3/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/types.py` & `tecton-0.7.0rc3/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/__diff.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/_dill.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/_objects.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/detect.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/info.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/pointers.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/settings.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/source.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/dill/dill/temp.py` & `tecton-0.7.0rc3/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.7.0rc3/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/vendor_dill.py` & `tecton-0.7.0rc3/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/vendor/vendor_pyspark.py` & `tecton-0.7.0rc3/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton/version.py` & `tecton-0.7.0rc3/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton.egg-info/PKG-INFO` & `tecton-0.7.0rc3/tecton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0rc2
+Version: 0.7.0rc3
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0rc2/tecton.egg-info/SOURCES.txt` & `tecton-0.7.0rc3/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton.egg-info/requires.txt` & `tecton-0.7.0rc3/tecton.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/athena_session.py` & `tecton-0.7.0rc3/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/data_catalog_helper.py` & `tecton-0.7.0rc3/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/odfv_helper.py` & `tecton-0.7.0rc3/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/pipeline_helper.py` & `tecton-0.7.0rc3/tecton_athena/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/query/translate.py` & `tecton-0.7.0rc3/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/sql_helper.py` & `tecton-0.7.0rc3/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates/create_table.sql` & `tecton-0.7.0rc3/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates/historical_features.sql` & `tecton-0.7.0rc3/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates/materialization_tile.sql` & `tecton-0.7.0rc3/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.7.0rc3/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates/time_limit.sql` & `tecton-0.7.0rc3/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_athena/templates_utils.py` & `tecton-0.7.0rc3/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/aggregation_utils.py` & `tecton-0.7.0rc3/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/conf.py` & `tecton-0.7.0rc3/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/data_types.py` & `tecton-0.7.0rc3/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/errors.py` & `tecton-0.7.0rc3/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/fco_container.py` & `tecton-0.7.0rc3/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/feature_definition_wrapper.py` & `tecton-0.7.0rc3/tecton_core/feature_definition_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/feature_set_config.py` & `tecton-0.7.0rc3/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/feature_view_utils.py` & `tecton-0.7.0rc3/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/function_deserialization.py` & `tecton-0.7.0rc3/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/id_helper.py` & `tecton-0.7.0rc3/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/materialization_context.py` & `tecton-0.7.0rc3/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/offline_store.py` & `tecton-0.7.0rc3/tecton_core/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/online_serving_index.py` & `tecton-0.7.0rc3/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/pipeline_common.py` & `tecton-0.7.0rc3/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/pipeline_sql_builder.py` & `tecton-0.7.0rc3/tecton_core/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/aggregation_plans.py` & `tecton-0.7.0rc3/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/builder.py` & `tecton-0.7.0rc3/tecton_core/query/builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/node_interface.py` & `tecton-0.7.0rc3/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/nodes.py` & `tecton-0.7.0rc3/tecton_core/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/pandas/node.py` & `tecton-0.7.0rc3/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/pandas/nodes.py` & `tecton-0.7.0rc3/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/rewrite.py` & `tecton-0.7.0rc3/tecton_core/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/query/sql_compat.py` & `tecton-0.7.0rc3/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/repo_file_handler.py` & `tecton-0.7.0rc3/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/request_context.py` & `tecton-0.7.0rc3/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/schema.py` & `tecton-0.7.0rc3/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/schema_derivation_utils.py` & `tecton-0.7.0rc3/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/__init__.py` & `tecton-0.7.0rc3/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/data_source_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/entity_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/feature_service_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/feature_view_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/feature_view_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/tecton_object_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/transformation_spec.py` & `tecton-0.7.0rc3/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/specs/utils.py` & `tecton-0.7.0rc3/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/time_utils.py` & `tecton-0.7.0rc3/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/__init__.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/misc.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/node.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/plugins.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/treelib/tree.py` & `tecton-0.7.0rc3/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_core/vendor/vendor_treelib.py` & `tecton-0.7.0rc3/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.7.0rc3/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.7.0rc3/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.7.0rc3/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/basic_info_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/data_source_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/diff_options_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/diff_test_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/entity_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/fco_args_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/feature_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/feature_view_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/feature_view_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from tecton_proto.common import schema_pb2 as tecton__proto_dot_common_dot_schema__pb2
 from tecton_proto.common import spark_schema_pb2 as tecton__proto_dot_common_dot_spark__schema__pb2
 from tecton_proto.common import data_source_type_pb2 as tecton__proto_dot_common_dot_data__source__type__pb2
 from tecton_proto.args import version_constraints_pb2 as tecton__proto_dot_args_dot_version__constraints__pb2
 from tecton_proto.common import analytics_options_pb2 as tecton__proto_dot_common_dot_analytics__options__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a tecton_proto/args/pipeline.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a\x1ctecton_proto/common/id.proto\x1a+tecton_proto/common/framework_version.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\"\xc9\x0b\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02\x08\x01R\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0eofflineEnabled\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchemaB\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xd6\x0b\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12@\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x80\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB1\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Q\n\roffline_store\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12\x33\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x06schema\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\xf3\x05\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12X\n\roffline_store\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x08\x05R\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\"\xec\x03\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12\x41\n\x0btime_window\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\ntimeWindow\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xe9\x04\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataprocB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"\x8a\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12?\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tB\x05\x92M\x02\x18\x05R\x16\x64\x61tabricksSparkVersion\x12\x31\n\x11\x65mr_spark_version\x18\x02 \x01(\tB\x05\x92M\x02\x18\x05R\x0f\x65mrSparkVersion\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xe9\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12+\n\x0btls_enabled\x18\x06 \x01(\x08\x42\n\x92M\x02\x08\x01\x92M\x02\x18\x05R\ntlsEnabled\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail*\xe9\x01\n\x0f\x46\x65\x61tureViewType\x12\x1d\n\x19\x46\x45\x41TURE_VIEW_TYPE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbb\x01\n\x12\x42\x61\x63kfillConfigMode\x12 \n\x1c\x42\x41\x43KFILL_CONFIG_MODE_UNKNOWN\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8b\x01\n\x14StreamProcessingMode\x12\"\n\x1eSTREAM_PROCESSING_MODE_UNKNOWN\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa4\x01\n\x10\x42\x61tchTriggerType\x12\x1e\n\x1a\x42\x41TCH_TRIGGER_TYPE_UNKNOWN\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a tecton_proto/args/pipeline.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a\x1ctecton_proto/common/id.proto\x1a+tecton_proto/common/framework_version.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\"\xc9\x0b\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02\x08\x01R\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0eofflineEnabled\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchemaB\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xd6\x0b\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12@\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x80\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB1\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Q\n\roffline_store\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12\x33\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x06schema\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\xc4\x06\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12X\n\roffline_store\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x08\x05R\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\x12O\n\nmonitoring\x18\n \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\"\xec\x03\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12\x41\n\x0btime_window\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\ntimeWindow\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xe9\x04\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataprocB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"\x8a\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12?\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tB\x05\x92M\x02\x18\x05R\x16\x64\x61tabricksSparkVersion\x12\x31\n\x11\x65mr_spark_version\x18\x02 \x01(\tB\x05\x92M\x02\x18\x05R\x0f\x65mrSparkVersion\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xe9\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12+\n\x0btls_enabled\x18\x06 \x01(\x08\x42\n\x92M\x02\x08\x01\x92M\x02\x18\x05R\ntlsEnabled\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail*\xe9\x01\n\x0f\x46\x65\x61tureViewType\x12\x1d\n\x19\x46\x45\x41TURE_VIEW_TYPE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbb\x01\n\x12\x42\x61\x63kfillConfigMode\x12 \n\x1c\x42\x41\x43KFILL_CONFIG_MODE_UNKNOWN\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8b\x01\n\x14StreamProcessingMode\x12\"\n\x1eSTREAM_PROCESSING_MODE_UNKNOWN\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa4\x01\n\x10\x42\x61tchTriggerType\x12\x1e\n\x1a\x42\x41TCH_TRIGGER_TYPE_UNKNOWN\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.args.feature_view_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.argsP\001'
@@ -109,14 +109,16 @@
   _FEATURETABLEARGS.fields_by_name['online_store_config']._serialized_options = b'\202}\002\020\003'
   _FEATURETABLEARGS.fields_by_name['online_store']._options = None
   _FEATURETABLEARGS.fields_by_name['online_store']._serialized_options = b'\202}\002\010\005'
   _FEATURETABLEARGS.fields_by_name['batch_materialization']._options = None
   _FEATURETABLEARGS.fields_by_name['batch_materialization']._serialized_options = b'\202}\002\020\003'
   _FEATURETABLEARGS.fields_by_name['batch_compute']._options = None
   _FEATURETABLEARGS.fields_by_name['batch_compute']._serialized_options = b'\202}\002\010\005'
+  _FEATURETABLEARGS.fields_by_name['monitoring']._options = None
+  _FEATURETABLEARGS.fields_by_name['monitoring']._serialized_options = b'\222M\002\010\001\222M\002\020\001'
   _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._options = None
   _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_options = b'8\001'
   _FEATUREAGGREGATION.fields_by_name['time_windows']._options = None
   _FEATUREAGGREGATION.fields_by_name['time_windows']._serialized_options = b'\202}\002\020\003'
   _FEATUREAGGREGATION.fields_by_name['time_window_strs']._options = None
   _FEATUREAGGREGATION.fields_by_name['time_window_strs']._serialized_options = b'\202}\002\020\003\222M\002\010\005'
   _FEATUREAGGREGATION.fields_by_name['time_window']._options = None
@@ -159,22 +161,22 @@
   _OFFLINEFEATURESTORECONFIG.fields_by_name['subdirectory_override']._serialized_options = b'\222M\002\010\001'
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._serialized_options = b'\202}\002\020\003'
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._serialized_options = b'\202}\002\010\005'
   _MONITORINGCONFIG.fields_by_name['alert_email']._options = None
   _MONITORINGCONFIG.fields_by_name['alert_email']._serialized_options = b'\362\342\002\002\010\001'
-  _FEATUREVIEWTYPE._serialized_start=11073
-  _FEATUREVIEWTYPE._serialized_end=11306
-  _BACKFILLCONFIGMODE._serialized_start=11309
-  _BACKFILLCONFIGMODE._serialized_end=11496
-  _STREAMPROCESSINGMODE._serialized_start=11499
-  _STREAMPROCESSINGMODE._serialized_end=11638
-  _BATCHTRIGGERTYPE._serialized_start=11641
-  _BATCHTRIGGERTYPE._serialized_end=11805
+  _FEATUREVIEWTYPE._serialized_start=11154
+  _FEATUREVIEWTYPE._serialized_end=11387
+  _BACKFILLCONFIGMODE._serialized_start=11390
+  _BACKFILLCONFIGMODE._serialized_end=11577
+  _STREAMPROCESSINGMODE._serialized_start=11580
+  _STREAMPROCESSINGMODE._serialized_end=11719
+  _BATCHTRIGGERTYPE._serialized_start=11722
+  _BATCHTRIGGERTYPE._serialized_end=11886
   _FEATUREVIEWARGS._serialized_start=583
   _FEATUREVIEWARGS._serialized_end=2064
   _ENTITYKEYOVERRIDE._serialized_start=2066
   _ENTITYKEYOVERRIDE._serialized_end=2168
   _BACKFILLCONFIG._serialized_start=2170
   _BACKFILLCONFIG._serialized_end=2245
   _OUTPUTSTREAM._serialized_start=2248
@@ -184,47 +186,47 @@
   _TEMPORALAGGREGATEARGS._serialized_start=3541
   _TEMPORALAGGREGATEARGS._serialized_end=4670
   _MATERIALIZEDFEATUREVIEWARGS._serialized_start=4673
   _MATERIALIZEDFEATUREVIEWARGS._serialized_end=6167
   _ONDEMANDARGS._serialized_start=6170
   _ONDEMANDARGS._serialized_end=6381
   _FEATURETABLEARGS._serialized_start=6384
-  _FEATURETABLEARGS._serialized_end=7139
-  _FEATUREAGGREGATION._serialized_start=7142
-  _FEATUREAGGREGATION._serialized_end=7634
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=7538
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=7634
-  _PARAMVALUE._serialized_start=7636
-  _PARAMVALUE._serialized_end=7729
-  _DATAQUALITYCONFIG._serialized_start=7732
-  _DATAQUALITYCONFIG._serialized_end=7875
-  _CLUSTERCONFIG._serialized_start=7878
-  _CLUSTERCONFIG._serialized_end=8495
-  _JSONCLUSTERCONFIG._serialized_start=8497
-  _JSONCLUSTERCONFIG._serialized_end=8561
-  _EXISTINGCLUSTERCONFIG._serialized_start=8563
-  _EXISTINGCLUSTERCONFIG._serialized_end=8634
-  _NEWCLUSTERCONFIG._serialized_start=8637
-  _NEWCLUSTERCONFIG._serialized_end=9052
-  _DEFAULTCLUSTERCONFIG._serialized_start=9055
-  _DEFAULTCLUSTERCONFIG._serialized_end=9193
-  _SPARKCONFIG._serialized_start=9196
-  _SPARKCONFIG._serialized_end=9583
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=9523
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=9583
-  _ONLINESTORECONFIG._serialized_start=9586
-  _ONLINESTORECONFIG._serialized_end=9816
-  _DYNAMODBONLINESTORE._serialized_start=9819
-  _DYNAMODBONLINESTORE._serialized_end=10108
-  _REDISONLINESTORE._serialized_start=10111
-  _REDISONLINESTORE._serialized_end=10344
-  _BIGTABLEONLINESTORE._serialized_start=10346
-  _BIGTABLEONLINESTORE._serialized_end=10457
-  _OFFLINEFEATURESTORECONFIG._serialized_start=10460
-  _OFFLINEFEATURESTORECONFIG._serialized_end=10679
-  _PARQUETCONFIG._serialized_start=10681
-  _PARQUETCONFIG._serialized_end=10696
-  _DELTACONFIG._serialized_start=10698
-  _DELTACONFIG._serialized_end=10786
-  _MONITORINGCONFIG._serialized_start=10789
-  _MONITORINGCONFIG._serialized_end=11070
+  _FEATURETABLEARGS._serialized_end=7220
+  _FEATUREAGGREGATION._serialized_start=7223
+  _FEATUREAGGREGATION._serialized_end=7715
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=7619
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=7715
+  _PARAMVALUE._serialized_start=7717
+  _PARAMVALUE._serialized_end=7810
+  _DATAQUALITYCONFIG._serialized_start=7813
+  _DATAQUALITYCONFIG._serialized_end=7956
+  _CLUSTERCONFIG._serialized_start=7959
+  _CLUSTERCONFIG._serialized_end=8576
+  _JSONCLUSTERCONFIG._serialized_start=8578
+  _JSONCLUSTERCONFIG._serialized_end=8642
+  _EXISTINGCLUSTERCONFIG._serialized_start=8644
+  _EXISTINGCLUSTERCONFIG._serialized_end=8715
+  _NEWCLUSTERCONFIG._serialized_start=8718
+  _NEWCLUSTERCONFIG._serialized_end=9133
+  _DEFAULTCLUSTERCONFIG._serialized_start=9136
+  _DEFAULTCLUSTERCONFIG._serialized_end=9274
+  _SPARKCONFIG._serialized_start=9277
+  _SPARKCONFIG._serialized_end=9664
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=9604
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=9664
+  _ONLINESTORECONFIG._serialized_start=9667
+  _ONLINESTORECONFIG._serialized_end=9897
+  _DYNAMODBONLINESTORE._serialized_start=9900
+  _DYNAMODBONLINESTORE._serialized_end=10189
+  _REDISONLINESTORE._serialized_start=10192
+  _REDISONLINESTORE._serialized_end=10425
+  _BIGTABLEONLINESTORE._serialized_start=10427
+  _BIGTABLEONLINESTORE._serialized_end=10538
+  _OFFLINEFEATURESTORECONFIG._serialized_start=10541
+  _OFFLINEFEATURESTORECONFIG._serialized_end=10760
+  _PARQUETCONFIG._serialized_start=10762
+  _PARQUETCONFIG._serialized_end=10777
+  _DELTACONFIG._serialized_start=10779
+  _DELTACONFIG._serialized_end=10867
+  _MONITORINGCONFIG._serialized_start=10870
+  _MONITORINGCONFIG._serialized_end=11151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0rc2/tecton_proto/args/pipeline_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/transformation_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.7.0rc3/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/acl_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/principal_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/resource_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/auth/service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/canary/type_pb2.py` & `tecton-0.7.0rc3/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/canary/update_pb2.py` & `tecton-0.7.0rc3/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.7.0rc3/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/column_type_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/container_image_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/data_type_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/framework_version_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/id_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/pair_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/schema_container_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/schema_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/secret_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.7.0rc3/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.7.0rc3/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/data_source_access_config_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/data_source_access_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/entity_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/fco_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/feature_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/feature_store_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/feature_view_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/onboarding_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/principal_group_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/serving_status_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/state_update_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/summary_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/transformation_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/user_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/data/workspace_pb2.py` & `tecton-0.7.0rc3/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.7.0rc3/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/config_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.7.0rc3/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.7.0rc3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materialization/params_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.7.0rc3/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.7.0rc3/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.7.0rc3/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.7.0rc3/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.7.0rc3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/snowflake/location_pb2.py` & `tecton-0.7.0rc3/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/spark_api/error_pb2.py` & `tecton-0.7.0rc3/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.7.0rc3/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.7.0rc3/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.7.0rc3/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_proto/validation/validator_pb2.py` & `tecton-0.7.0rc3/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/pipeline_helper.py` & `tecton-0.7.0rc3/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.7.0rc3/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.7.0rc3/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/sql_helper.py` & `tecton-0.7.0rc3/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/historical_features.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates/time_limit.sql` & `tecton-0.7.0rc3/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_snowflake/templates_utils.py` & `tecton-0.7.0rc3/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/aggregation_plans.py` & `tecton-0.7.0rc3/tecton_spark/aggregation_plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,19 @@
         )
 
     return _approx_percentile_full_aggregation
 
 
 def _make_approx_percentile_continuous_partial() -> Callable[[List[str]], List[Column]]:
     def _approx_percentile_continuous_partial(cols: List[str]) -> List[Column]:
-        msg = "approx_percentile does not support continuous mode"
-        raise NotImplementedError(msg)
+        input_col = F.col(cols[0])
+
+        # The partial aggregate tiles for approx_percentile do not allow nulls, so we replace nulls with NaNs, which will be filtered out of the eventual result.
+        mean_col = F.when(input_col.isNull(), F.lit(float("nan"))).otherwise(input_col)
+        return [F.array(mean_col), F.array(F.lit(1.0))]
 
     return _approx_percentile_continuous_partial
 
 
 def ApproxCountDistinctFullAgg(indices: str, registers: str, precision: int) -> Column:
     sc = SparkContext._active_spark_context
     udf_name = "tecton_approx_count_distinct_full"
@@ -480,15 +483,14 @@
         partial_aggregation_transform=lambda cols: _stddev_var_partial(cols[0]),
         continuous_partial_aggregation_transform=_make_stddev_var_continuous_partial(),
         full_aggregation_transform=_stddev_samp_full_aggregation,
         materialized_column_prefixes=get_materialization_aggregation_column_prefixes(
             afpb.AGGREGATION_FUNCTION_STDDEV_SAMP
         ),
     ),
-    # TODO(TEC-14292): Support continuous mode for approx_count_distinct.
     afpb.AGGREGATION_FUNCTION_APPROX_COUNT_DISTINCT: lambda time_key, params, _: AggregationPlan(
         partial_aggregation_transform=_make_approx_count_distinct_partial_aggregation(),
         continuous_partial_aggregation_transform=_make_approx_count_distinct_continuous_partial(),
         full_aggregation_transform=_make_approx_count_distinct_full_aggregation(params.approx_count_distinct.precision),
         materialized_column_prefixes=get_materialization_aggregation_column_prefixes(
             afpb.AGGREGATION_FUNCTION_APPROX_COUNT_DISTINCT
         ),
```

### Comparing `tecton-0.7.0rc2/tecton_spark/data_observability.py` & `tecton-0.7.0rc3/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/data_source_credentials.py` & `tecton-0.7.0rc3/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/data_source_helper.py` & `tecton-0.7.0rc3/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/feature_view_spark_utils.py` & `tecton-0.7.0rc3/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.7.0rc3/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1604241 bytes, number of entries: 972
+Zip file size: 1600615 bytes, number of entries: 971
 -rw----     2.0 fat        0 bx stor 10-Jan-01 00:00 META-INF/
 -rw----     2.0 fat      111 b- defN 10-Jan-01 00:00 META-INF/MANIFEST.MF
 -rw----     2.0 fat      281 b- defN 10-Jan-01 00:00 build-data.properties
 -rw----     2.0 fat       92 bl defN 10-Jan-01 00:00 META-INF/java_com_tecton_udfs_spark3-tecton-udfs-lib.kotlin_module
 -rw----     1.0 fat        0 b- stor 10-Jan-01 00:00 com/
 -rw----     1.0 fat        0 b- stor 10-Jan-01 00:00 com/tecton/
 -rw----     1.0 fat        0 b- stor 10-Jan-01 00:00 com/tecton/udfs/
@@ -11,38 +11,37 @@
 -rw----     2.0 fat     1233 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/AggUtilsKt$concatDistinct$2.class
 -rw----     2.0 fat     1973 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/AggUtilsKt$fixedSizeMergeList$$inlined$sortBy$1.class
 -rw----     2.0 fat     8651 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/AggUtilsKt.class
 -rw----     2.0 fat     5736 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxCountDistinctFullAgg.class
 -rw----     2.0 fat     2244 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxCountDistinctFullRegister.class
 -rw----     2.0 fat     4516 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxCountDistinctPartialAgg.class
 -rw----     2.0 fat     2170 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxCountDistinctPartialRegister.class
--rw----     2.0 fat     4274 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentileFullAgg.class
+-rw----     2.0 fat     4272 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentileFullAgg.class
 -rw----     2.0 fat     2295 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentileFullRegister.class
--rw----     2.0 fat     4775 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialAgg.class
--rw----     2.0 fat     2223 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialAggKt$process$$inlined$sortedBy$1.class
--rw----     2.0 fat     6492 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialAggKt.class
--rw----     2.0 fat     2290 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialRegister.class
+-rw----     2.0 fat     4352 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialAgg.class
+-rw----     2.0 fat     1863 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialAggKt.class
+-rw----     2.0 fat     2250 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/ApproxPercentilePartialRegister.class
 -rw----     2.0 fat     2393 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/Count.class
 -rw----     2.0 fat     2938 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/FeatureTimestampValidator.class
 -rw----     2.0 fat     5372 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/FirstNAgg.class
 -rw----     2.0 fat     2212 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/FirstNRegister.class
 -rw----     2.0 fat     5394 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/LastNAgg.class
 -rw----     2.0 fat     2207 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/LastNRegister.class
 -rw----     2.0 fat     3994 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/LimitedListConcatAgg.class
 -rw----     2.0 fat     2254 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/LimitedListConcatRegister.class
 -rw----     2.0 fat     3014 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/OrderedOutput.class
 -rw----     2.0 fat     2974 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/Output.class
--rw----     2.0 fat     2472 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/Percentile.class
--rw----     2.0 fat     2650 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/PercentileValue.class
+-rw----     2.0 fat     2561 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/Percentile.class
+-rw----     2.0 fat     2770 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/PercentileValue.class
 -rw----     2.0 fat     1782 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/RegisterFeatureTimestampValidator.class
 -rw----     2.0 fat     4826 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/SparseArray.class
 -rw----     2.0 fat     3296 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/SparseArrayItem.class
--rw----     2.0 fat     9773 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigest.class
--rw----     2.0 fat    10430 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigestFinal.class
--rw----     2.0 fat     3941 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigestProcessed.class
+-rw----     2.0 fat     2094 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigest$process$$inlined$sortedBy$1.class
+-rw----     2.0 fat    15862 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigest.class
+-rw----     2.0 fat     4099 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TDigestProcessed.class
 -rw----     2.0 fat      968 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TectonFeatureValidationException.class
 -rw----     2.0 fat     2960 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/Tile.class
 -rw----     2.0 fat     3962 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TimedTile.class
 -rw----     2.0 fat     3455 bl defN 10-Jan-01 00:00 com/tecton/udfs/spark3/TimedTileValue.class
 drwxr-xr-x  2.0 unx        0 b- defN 10-Jan-01 00:00 kotlin/
 drwxr-xr-x  2.0 unx        0 b- defN 10-Jan-01 00:00 kotlin/collections/
 -rw-r--r--  2.0 unx      596 b- defN 10-Jan-01 00:00 kotlin/collections/ArraysUtilJVM.class
@@ -967,8 +966,8 @@
 -rw-r--r--  2.0 unx      646 b- defN 10-Jan-01 00:00 kotlin/internal/internal.kotlin_builtins
 -rw-r--r--  2.0 unx    16434 b- defN 10-Jan-01 00:00 kotlin/kotlin.kotlin_builtins
 -rw-r--r--  2.0 unx     3305 b- defN 10-Jan-01 00:00 kotlin/ranges/ranges.kotlin_builtins
 -rw-r--r--  2.0 unx     2395 b- defN 10-Jan-01 00:00 kotlin/reflect/reflect.kotlin_builtins
 drwxr-xr-x  2.0 unx        0 b- defN 10-Jan-01 00:00 META-INF/versions/
 drwxr-xr-x  2.0 unx        0 b- defN 10-Jan-01 00:00 META-INF/versions/9/
 -rw-r--r--  2.0 unx     1024 b- defN 10-Jan-01 00:00 META-INF/versions/9/module-info.class
-972 files, 3953450 bytes uncompressed, 1445943 bytes compressed:  63.4%
+971 files, 3944253 bytes uncompressed, 1442533 bytes compressed:  63.4%
```

#### zipnote «TEMP»/diffoscope_j1nw3wul_/tmpobig9tef_.zip

```diff
@@ -51,17 +51,14 @@
 
 Filename: com/tecton/udfs/spark3/ApproxPercentileFullRegister.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/ApproxPercentilePartialAgg.class
 Comment: 
 
-Filename: com/tecton/udfs/spark3/ApproxPercentilePartialAggKt$process$$inlined$sortedBy$1.class
-Comment: 
-
 Filename: com/tecton/udfs/spark3/ApproxPercentilePartialAggKt.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/ApproxPercentilePartialRegister.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/Count.class
@@ -105,18 +102,18 @@
 
 Filename: com/tecton/udfs/spark3/SparseArray.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/SparseArrayItem.class
 Comment: 
 
-Filename: com/tecton/udfs/spark3/TDigest.class
+Filename: com/tecton/udfs/spark3/TDigest$process$$inlined$sortedBy$1.class
 Comment: 
 
-Filename: com/tecton/udfs/spark3/TDigestFinal.class
+Filename: com/tecton/udfs/spark3/TDigest.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/TDigestProcessed.class
 Comment: 
 
 Filename: com/tecton/udfs/spark3/TectonFeatureValidationException.class
 Comment:
```

#### com/tecton/udfs/spark3/ApproxPercentileFullAgg.class

##### procyon -ec {}

```diff
@@ -5,16 +5,16 @@
 import kotlin.jvm.internal.Intrinsics;
 import org.apache.spark.sql.Encoders;
 import org.apache.spark.sql.Encoder;
 import org.jetbrains.annotations.NotNull;
 import kotlin.Metadata;
 import org.apache.spark.sql.expressions.Aggregator;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000,\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u0006\n\u0002\b\u0006\n\u0002\u0018\u0002\n\u0002\b\t\u0018\u00002\u0014\u0012\u0004\u0012\u00020\u0002\u0012\u0004\u0012\u00020\u0003\u0012\u0004\u0012\u00020\u00040\u0001B\u0015\u0012\u0006\u0010\u0005\u001a\u00020\u0006\u0012\u0006\u0010\u0007\u001a\u00020\b¢\u0006\u0002\u0010\tJ\u000e\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00030\u000fH\u0016J\u0010\u0010\u0010\u001a\u00020\u00042\u0006\u0010\u0011\u001a\u00020\u0003H\u0016J\u0018\u0010\u0012\u001a\u00020\u00032\u0006\u0010\u0013\u001a\u00020\u00032\u0006\u0010\u0014\u001a\u00020\u0003H\u0016J\u000e\u0010\u0015\u001a\b\u0012\u0004\u0012\u00020\u00040\u000fH\u0016J\u001a\u0010\u0016\u001a\u00020\u00032\u0006\u0010\u0013\u001a\u00020\u00032\b\u0010\u0014\u001a\u0004\u0018\u00010\u0002H\u0016J\b\u0010\u0017\u001a\u00020\u0003H\u0016R\u0011\u0010\u0005\u001a\u00020\u0006¢\u0006\b\n\u0000\u001a\u0004\b\n\u0010\u000bR\u0011\u0010\u0007\u001a\u00020\b¢\u0006\b\n\u0000\u001a\u0004\b\f\u0010\r¨\u0006\u0018" }, d2 = { "Lcom/tecton/udfs/spark3/ApproxPercentileFullAgg;", "Lorg/apache/spark/sql/expressions/Aggregator;", "Lcom/tecton/udfs/spark3/TDigestProcessed;", "Lcom/tecton/udfs/spark3/TDigestFinal;", "Lcom/tecton/udfs/spark3/Percentile;", "compression", "", "q", "", "(ID)V", "getCompression", "()I", "getQ", "()D", "bufferEncoder", "Lorg/apache/spark/sql/Encoder;", "finish", "tDigest", "merge", "tDigest1", "tDigest2", "outputEncoder", "reduce", "zero", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
-public final class ApproxPercentileFullAgg extends Aggregator<TDigestProcessed, TDigestFinal, Percentile>
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000,\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u0006\n\u0002\b\u0006\n\u0002\u0018\u0002\n\u0002\b\t\u0018\u00002\u0014\u0012\u0004\u0012\u00020\u0002\u0012\u0004\u0012\u00020\u0003\u0012\u0004\u0012\u00020\u00040\u0001B\u0015\u0012\u0006\u0010\u0005\u001a\u00020\u0006\u0012\u0006\u0010\u0007\u001a\u00020\b¢\u0006\u0002\u0010\tJ\u000e\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00030\u000fH\u0016J\u0010\u0010\u0010\u001a\u00020\u00042\u0006\u0010\u0011\u001a\u00020\u0003H\u0016J\u0018\u0010\u0012\u001a\u00020\u00032\u0006\u0010\u0013\u001a\u00020\u00032\u0006\u0010\u0014\u001a\u00020\u0003H\u0016J\u000e\u0010\u0015\u001a\b\u0012\u0004\u0012\u00020\u00040\u000fH\u0016J\u001a\u0010\u0016\u001a\u00020\u00032\u0006\u0010\u0013\u001a\u00020\u00032\b\u0010\u0014\u001a\u0004\u0018\u00010\u0002H\u0016J\b\u0010\u0017\u001a\u00020\u0003H\u0016R\u0011\u0010\u0005\u001a\u00020\u0006¢\u0006\b\n\u0000\u001a\u0004\b\n\u0010\u000bR\u0011\u0010\u0007\u001a\u00020\b¢\u0006\b\n\u0000\u001a\u0004\b\f\u0010\r¨\u0006\u0018" }, d2 = { "Lcom/tecton/udfs/spark3/ApproxPercentileFullAgg;", "Lorg/apache/spark/sql/expressions/Aggregator;", "Lcom/tecton/udfs/spark3/TDigestProcessed;", "Lcom/tecton/udfs/spark3/TDigest;", "Lcom/tecton/udfs/spark3/Percentile;", "compression", "", "q", "", "(ID)V", "getCompression", "()I", "getQ", "()D", "bufferEncoder", "Lorg/apache/spark/sql/Encoder;", "finish", "tDigest", "merge", "tDigest1", "tDigest2", "outputEncoder", "reduce", "zero", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+public final class ApproxPercentileFullAgg extends Aggregator<TDigestProcessed, TDigest, Percentile>
 {
     private final int compression;
     private final double q;
     
     public ApproxPercentileFullAgg(final int compression, final double q) {
         this.compression = compression;
         this.q = q;
@@ -25,47 +25,48 @@
     }
     
     public final double getQ() {
         return this.q;
     }
     
     @NotNull
-    public TDigestFinal zero() {
-        return new TDigestFinal();
+    public TDigest zero() {
+        return new TDigest();
     }
     
     @NotNull
-    public Encoder<TDigestFinal> bufferEncoder() {
-        final Encoder bean = Encoders.bean((Class)TDigestFinal.class);
-        Intrinsics.checkNotNullExpressionValue((Object)bean, "bean(TDigestFinal::class.java)");
-        return (Encoder<TDigestFinal>)bean;
+    public Encoder<TDigest> bufferEncoder() {
+        final Encoder bean = Encoders.bean((Class)TDigest.class);
+        Intrinsics.checkNotNullExpressionValue((Object)bean, "bean(TDigest::class.java)");
+        return (Encoder<TDigest>)bean;
     }
     
     @NotNull
     public Encoder<Percentile> outputEncoder() {
         final Encoder bean = Encoders.bean((Class)Percentile.class);
         Intrinsics.checkNotNullExpressionValue((Object)bean, "bean(Percentile::class.java)");
         return (Encoder<Percentile>)bean;
     }
     
     @NotNull
-    public TDigestFinal reduce(@NotNull final TDigestFinal tDigest1, @Nullable final TDigestProcessed tDigest2) {
+    public TDigest reduce(@NotNull final TDigest tDigest1, @Nullable final TDigestProcessed tDigest2) {
         Intrinsics.checkNotNullParameter((Object)tDigest1, "tDigest1");
         if (tDigest2 == null) {
             return tDigest1;
         }
         return tDigest1.reduce(tDigest2, this.compression);
     }
     
     @NotNull
-    public TDigestFinal merge(@NotNull final TDigestFinal tDigest1, @NotNull final TDigestFinal tDigest2) {
+    public TDigest merge(@NotNull final TDigest tDigest1, @NotNull final TDigest tDigest2) {
         Intrinsics.checkNotNullParameter((Object)tDigest1, "tDigest1");
         Intrinsics.checkNotNullParameter((Object)tDigest2, "tDigest2");
         return tDigest1.merge(tDigest2, this.compression);
     }
     
     @NotNull
-    public Percentile finish(@NotNull final TDigestFinal tDigest) {
+    public Percentile finish(@NotNull final TDigest tDigest) {
         Intrinsics.checkNotNullParameter((Object)tDigest, "tDigest");
+        tDigest.process(this.compression);
         return new Percentile(tDigest.quantile(this.q));
     }
 }
```

#### com/tecton/udfs/spark3/ApproxPercentilePartialAgg.class

##### procyon -ec {}

```diff
@@ -5,33 +5,27 @@
 import kotlin.jvm.internal.Intrinsics;
 import org.apache.spark.sql.Encoders;
 import org.apache.spark.sql.Encoder;
 import org.jetbrains.annotations.NotNull;
 import kotlin.Metadata;
 import org.apache.spark.sql.expressions.Aggregator;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000&\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\b\n\u0002\b\u0006\n\u0002\u0018\u0002\n\u0002\b\n\u0018\u00002\u0014\u0012\u0004\u0012\u00020\u0002\u0012\u0004\u0012\u00020\u0003\u0012\u0004\u0012\u00020\u00040\u0001B\u0015\u0012\u0006\u0010\u0005\u001a\u00020\u0006\u0012\u0006\u0010\u0007\u001a\u00020\u0006¢\u0006\u0002\u0010\bJ\u000e\u0010\f\u001a\b\u0012\u0004\u0012\u00020\u00030\rH\u0016J\u0010\u0010\u000e\u001a\u00020\u00042\u0006\u0010\u000f\u001a\u00020\u0003H\u0016J\u0018\u0010\u0010\u001a\u00020\u00032\u0006\u0010\u0011\u001a\u00020\u00032\u0006\u0010\u0012\u001a\u00020\u0003H\u0016J\u000e\u0010\u0013\u001a\b\u0012\u0004\u0012\u00020\u00040\rH\u0016J\u001a\u0010\u0014\u001a\u00020\u00032\u0006\u0010\u000f\u001a\u00020\u00032\b\u0010\u0015\u001a\u0004\u0018\u00010\u0002H\u0016J\b\u0010\u0016\u001a\u00020\u0003H\u0016R\u0011\u0010\u0005\u001a\u00020\u0006¢\u0006\b\n\u0000\u001a\u0004\b\t\u0010\nR\u0011\u0010\u0007\u001a\u00020\u0006¢\u0006\b\n\u0000\u001a\u0004\b\u000b\u0010\n¨\u0006\u0017" }, d2 = { "Lcom/tecton/udfs/spark3/ApproxPercentilePartialAgg;", "Lorg/apache/spark/sql/expressions/Aggregator;", "Lcom/tecton/udfs/spark3/PercentileValue;", "Lcom/tecton/udfs/spark3/TDigest;", "Lcom/tecton/udfs/spark3/TDigestProcessed;", "compression", "", "maxUnprocessed", "(II)V", "getCompression", "()I", "getMaxUnprocessed", "bufferEncoder", "Lorg/apache/spark/sql/Encoder;", "finish", "tDigest", "merge", "tDigest1", "tDigest2", "outputEncoder", "reduce", "percentileValue", "zero", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000&\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\b\n\u0002\b\u0004\n\u0002\u0018\u0002\n\u0002\b\n\u0018\u00002\u0014\u0012\u0004\u0012\u00020\u0002\u0012\u0004\u0012\u00020\u0003\u0012\u0004\u0012\u00020\u00040\u0001B\r\u0012\u0006\u0010\u0005\u001a\u00020\u0006¢\u0006\u0002\u0010\u0007J\u000e\u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00030\u000bH\u0016J\u0010\u0010\f\u001a\u00020\u00042\u0006\u0010\r\u001a\u00020\u0003H\u0016J\u0018\u0010\u000e\u001a\u00020\u00032\u0006\u0010\u000f\u001a\u00020\u00032\u0006\u0010\u0010\u001a\u00020\u0003H\u0016J\u000e\u0010\u0011\u001a\b\u0012\u0004\u0012\u00020\u00040\u000bH\u0016J\u001a\u0010\u0012\u001a\u00020\u00032\u0006\u0010\r\u001a\u00020\u00032\b\u0010\u0013\u001a\u0004\u0018\u00010\u0002H\u0016J\b\u0010\u0014\u001a\u00020\u0003H\u0016R\u0011\u0010\u0005\u001a\u00020\u0006¢\u0006\b\n\u0000\u001a\u0004\b\b\u0010\t¨\u0006\u0015" }, d2 = { "Lcom/tecton/udfs/spark3/ApproxPercentilePartialAgg;", "Lorg/apache/spark/sql/expressions/Aggregator;", "Lcom/tecton/udfs/spark3/PercentileValue;", "Lcom/tecton/udfs/spark3/TDigest;", "Lcom/tecton/udfs/spark3/TDigestProcessed;", "compression", "", "(I)V", "getCompression", "()I", "bufferEncoder", "Lorg/apache/spark/sql/Encoder;", "finish", "tDigest", "merge", "tDigest1", "tDigest2", "outputEncoder", "reduce", "percentileValue", "zero", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class ApproxPercentilePartialAgg extends Aggregator<PercentileValue, TDigest, TDigestProcessed>
 {
     private final int compression;
-    private final int maxUnprocessed;
     
-    public ApproxPercentilePartialAgg(final int compression, final int maxUnprocessed) {
+    public ApproxPercentilePartialAgg(final int compression) {
         this.compression = compression;
-        this.maxUnprocessed = maxUnprocessed;
     }
     
     public final int getCompression() {
         return this.compression;
     }
     
-    public final int getMaxUnprocessed() {
-        return this.maxUnprocessed;
-    }
-    
     @NotNull
     public TDigest zero() {
         return new TDigest();
     }
     
     @NotNull
     public Encoder<TDigest> bufferEncoder() {
@@ -54,25 +48,25 @@
             return tDigest;
         }
         if (percentileValue.getValue() == null) {
             return tDigest;
         }
         final Double value = percentileValue.getValue();
         Intrinsics.checkNotNull((Object)value);
-        tDigest.addCentroid((double)value, 1.0, this.compression, this.maxUnprocessed);
+        tDigest.addCentroid((double)value, 1.0, this.compression);
         return tDigest;
     }
     
     @NotNull
     public TDigest merge(@NotNull final TDigest tDigest1, @NotNull final TDigest tDigest2) {
         Intrinsics.checkNotNullParameter((Object)tDigest1, "tDigest1");
         Intrinsics.checkNotNullParameter((Object)tDigest2, "tDigest2");
-        return tDigest1.merge(tDigest2, this.compression, this.maxUnprocessed);
+        return tDigest1.merge(tDigest2, this.compression);
     }
     
     @NotNull
     public TDigestProcessed finish(@NotNull final TDigest tDigest) {
         Intrinsics.checkNotNullParameter((Object)tDigest, "tDigest");
         tDigest.process(this.compression);
-        return new TDigestProcessed(tDigest.getUsingTempList() ? tDigest.getTempProcessedMeans() : tDigest.getProcessedMeans(), tDigest.getUsingTempList() ? tDigest.getTempProcessedWeights() : tDigest.getProcessedWeights());
+        return new TDigestProcessed(tDigest.getCurrentProcessedMeans(), tDigest.getCurrentProcessedWeights());
     }
 }
```

#### com/tecton/udfs/spark3/ApproxPercentilePartialAggKt.class

##### procyon -ec {}

```diff
@@ -1,17 +1,13 @@
 
 package com.tecton.udfs.spark3;
 
-import java.util.Comparator;
-import kotlin.collections.CollectionsKt;
-import java.util.Collection;
-import java.util.List;
 import kotlin.Metadata;
 
-@Metadata(mv = { 1, 7, 1 }, k = 2, xi = 48, d1 = { "\u0000\u001e\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u0006\n\u0002\b\u0007\n\u0002\u0010\u0002\n\u0000\n\u0002\u0010!\n\u0002\b\b\u001a\u001e\u0010\u0006\u001a\u00020\u00032\u0006\u0010\u0007\u001a\u00020\u00032\u0006\u0010\b\u001a\u00020\u00012\u0006\u0010\t\u001a\u00020\u0003\u001ad\u0010\n\u001a\u00020\u000b2\u0006\u0010\b\u001a\u00020\u00012\f\u0010\f\u001a\b\u0012\u0004\u0012\u00020\u00030\r2\f\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00030\r2\f\u0010\u000f\u001a\b\u0012\u0004\u0012\u00020\u00030\r2\f\u0010\u0010\u001a\b\u0012\u0004\u0012\u00020\u00030\r2\f\u0010\u0011\u001a\b\u0012\u0004\u0012\u00020\u00030\r2\f\u0010\u0012\u001a\b\u0012\u0004\u0012\u00020\u00030\rH\u0002\u001a\u001e\u0010\u0013\u001a\u00020\u00032\u0006\u0010\u0014\u001a\u00020\u00032\u0006\u0010\b\u001a\u00020\u00012\u0006\u0010\t\u001a\u00020\u0003\"\u000e\u0010\u0000\u001a\u00020\u0001X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0002\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0004\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0005\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000¨\u0006\u0015" }, d2 = { "BUFFER_FACTOR", "", "INCREMENT", "", "SINGLETON_DELTA", "SINGLETON_RADIUS", "k3", "q", "compression", "n", "process", "", "processedMeans", "", "processedWeights", "unprocessedMeans", "unprocessedWeights", "newProcessedMeans", "newProcessedWeights", "q3", "k", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 2, xi = 48, d1 = { "\u0000\u0010\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u0006\n\u0002\b\t\u001a\u001e\u0010\u0006\u001a\u00020\u00032\u0006\u0010\u0007\u001a\u00020\u00032\u0006\u0010\b\u001a\u00020\u00012\u0006\u0010\t\u001a\u00020\u0003\u001a\u001e\u0010\n\u001a\u00020\u00032\u0006\u0010\u000b\u001a\u00020\u00032\u0006\u0010\b\u001a\u00020\u00012\u0006\u0010\t\u001a\u00020\u0003\"\u000e\u0010\u0000\u001a\u00020\u0001X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0002\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0004\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000\"\u000e\u0010\u0005\u001a\u00020\u0003X\u0086T¢\u0006\u0002\n\u0000¨\u0006\f" }, d2 = { "BUFFER_FACTOR", "", "INCREMENT", "", "SINGLETON_DELTA", "SINGLETON_RADIUS", "k3", "q", "compression", "n", "q3", "k", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class ApproxPercentilePartialAggKt
 {
     public static final int BUFFER_FACTOR = 10;
     public static final double INCREMENT = 1.0;
     public static final double SINGLETON_RADIUS = 0.5;
     public static final double SINGLETON_DELTA = 0.5;
     
@@ -31,99 +27,8 @@
     
     public static final double q3(final double k, final int compression, final double n) {
         if (k <= 0.0) {
             return Math.exp(k * (4 * Math.log(n / (double)compression) + 21) / (double)compression) / 2;
         }
         return 1 - q3(-k, compression, n);
     }
-    
-    private static final void process(final int compression, final List<Double> processedMeans, final List<Double> processedWeights, final List<Double> unprocessedMeans, final List<Double> unprocessedWeights, final List<Double> newProcessedMeans, final List<Double> newProcessedWeights) {
-        if (processedMeans.size() != processedWeights.size()) {
-            final int n = 0;
-            throw new IllegalArgumentException("processedMeans and processedWeights must have the same length".toString());
-        }
-        if (unprocessedMeans.size() != unprocessedWeights.size()) {
-            final int n2 = 0;
-            throw new IllegalArgumentException("unprocessedMeans and unprocessedWeights must have the same length".toString());
-        }
-        if (unprocessedMeans.size() <= 0) {
-            final int n3 = 0;
-            throw new IllegalArgumentException("Can only process if there are unprocessed centroids.".toString());
-        }
-        if (!newProcessedMeans.isEmpty()) {
-            final int n4 = 0;
-            throw new IllegalArgumentException("newProcessedMeans must be empty".toString());
-        }
-        if (!newProcessedWeights.isEmpty()) {
-            final int n5 = 0;
-            throw new IllegalArgumentException("newProcessedWeights must be empty".toString());
-        }
-        final Iterable $this$sortedBy$iv = (Iterable)CollectionsKt.getIndices((Collection)unprocessedMeans);
-        final int $i$f$sortedBy = 0;
-        final List unprocessedSortedIndices = CollectionsKt.sortedWith($this$sortedBy$iv, (Comparator)new ApproxPercentilePartialAggKt$process$$inlined$sortedBy$1((List)unprocessedMeans));
-        final double totalWeight = CollectionsKt.sumOfDouble((Iterable)unprocessedWeights) + CollectionsKt.sumOfDouble((Iterable)processedWeights);
-        double processedWeight = 0.0;
-        final double startingValue = k3(0.0, compression, totalWeight);
-        double limit = totalWeight * q3(startingValue + 1.0, compression, totalWeight);
-        int iterProcessed = 0;
-        int iterUnprocessed = 0;
-        double mean = 0.0;
-        double weight = 0.0;
-        while (iterProcessed < processedMeans.size() || iterUnprocessed < unprocessedMeans.size()) {
-            if (iterUnprocessed == unprocessedMeans.size()) {
-                mean = ((Number)processedMeans.get(iterProcessed)).doubleValue();
-                weight = ((Number)processedWeights.get(iterProcessed)).doubleValue();
-                ++iterProcessed;
-            }
-            else {
-                final int sortedIndex = ((Number)unprocessedSortedIndices.get(iterUnprocessed)).intValue();
-                if (iterProcessed == processedMeans.size()) {
-                    mean = ((Number)unprocessedMeans.get(sortedIndex)).doubleValue();
-                    weight = ((Number)unprocessedWeights.get(sortedIndex)).doubleValue();
-                    ++iterUnprocessed;
-                }
-                else if (((Number)processedMeans.get(iterProcessed)).doubleValue() < ((Number)unprocessedMeans.get(sortedIndex)).doubleValue()) {
-                    mean = ((Number)processedMeans.get(iterProcessed)).doubleValue();
-                    weight = ((Number)processedWeights.get(iterProcessed)).doubleValue();
-                    ++iterProcessed;
-                }
-                else {
-                    mean = ((Number)unprocessedMeans.get(sortedIndex)).doubleValue();
-                    weight = ((Number)unprocessedWeights.get(sortedIndex)).doubleValue();
-                    ++iterUnprocessed;
-                }
-            }
-            if (newProcessedMeans.isEmpty()) {
-                newProcessedMeans.add(Double.valueOf(mean));
-                newProcessedWeights.add(Double.valueOf(weight));
-            }
-            else if (processedWeight + weight <= limit) {
-                final double newWeight = ((Number)CollectionsKt.last((List)newProcessedWeights)).doubleValue() + weight;
-                final double newMean = (((Number)CollectionsKt.last((List)newProcessedMeans)).doubleValue() * ((Number)CollectionsKt.last((List)newProcessedWeights)).doubleValue() + mean * weight) / newWeight;
-                newProcessedMeans.set(newProcessedMeans.size() - 1, Double.valueOf(newMean));
-                newProcessedWeights.set(newProcessedWeights.size() - 1, Double.valueOf(newWeight));
-            }
-            else {
-                newProcessedMeans.add(Double.valueOf(mean));
-                newProcessedWeights.add(Double.valueOf(weight));
-                limit = totalWeight * q3(k3(processedWeight / totalWeight, compression, totalWeight) + 1.0, compression, totalWeight);
-            }
-            processedWeight += weight;
-        }
-        if (((Collection)newProcessedWeights).isEmpty()) {
-            final int n6 = 0;
-            throw new IllegalStateException("processing must create new centroids".toString());
-        }
-        if (((Number)newProcessedWeights.get(0)).doubleValue() != 1.0) {
-            final int n7 = 0;
-            throw new IllegalStateException("first centroid must have weight 1.0".toString());
-        }
-        if (((Number)CollectionsKt.last((List)newProcessedWeights)).doubleValue() != 1.0) {
-            final int n8 = 0;
-            throw new IllegalStateException("last centroid must have weight 1.0".toString());
-        }
-        processedMeans.clear();
-        processedWeights.clear();
-        unprocessedMeans.clear();
-        unprocessedWeights.clear();
-    }
 }
```

#### com/tecton/udfs/spark3/ApproxPercentilePartialRegister.class

##### procyon -ec {}

```diff
@@ -15,12 +15,11 @@
 {
     public final void register(@NotNull final String name, final int compression) {
         Intrinsics.checkNotNullParameter((Object)name, "name");
         final Option spark = SparkSession.getActiveSession();
         if (spark.isEmpty()) {
             throw new Exception("No active SparkSession!");
         }
-        final int maxUnprocessed = 10 * compression;
-        final ApproxPercentilePartialAgg aggregator = new ApproxPercentilePartialAgg(compression, maxUnprocessed);
+        final ApproxPercentilePartialAgg aggregator = new ApproxPercentilePartialAgg(compression);
         ((SparkSession)spark.get()).udf().register(name, functions.udaf((Aggregator)aggregator, Encoders.bean((Class)PercentileValue.class)));
     }
 }
```

#### com/tecton/udfs/spark3/Percentile.class

##### procyon -ec {}

```diff
@@ -1,55 +1,54 @@
 
 package com.tecton.udfs.spark3;
 
-import org.jetbrains.annotations.Nullable;
+import kotlin.jvm.internal.Intrinsics;
 import org.jetbrains.annotations.NotNull;
-import kotlin.jvm.internal.DefaultConstructorMarker;
+import org.jetbrains.annotations.Nullable;
 import kotlin.Metadata;
 import java.io.Serializable;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000*\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\u0006\n\u0002\b\u0007\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u000f\u0012\b\b\u0002\u0010\u0002\u001a\u00020\u0003¢\u0006\u0002\u0010\u0004J\t\u0010\b\u001a\u00020\u0003H\u00c6\u0003J\u0013\u0010\t\u001a\u00020\u00002\b\b\u0002\u0010\u0002\u001a\u00020\u0003H\u00c6\u0001J\u0013\u0010\n\u001a\u00020\u000b2\b\u0010\f\u001a\u0004\u0018\u00010\rH\u00d6\u0003J\t\u0010\u000e\u001a\u00020\u000fH\u00d6\u0001J\t\u0010\u0010\u001a\u00020\u0011H\u00d6\u0001R\u001a\u0010\u0002\u001a\u00020\u0003X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u0005\u0010\u0006\"\u0004\b\u0007\u0010\u0004¨\u0006\u0012" }, d2 = { "Lcom/tecton/udfs/spark3/Percentile;", "Ljava/io/Serializable;", "percentile", "", "(D)V", "getPercentile", "()D", "setPercentile", "component1", "copy", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000*\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\u0006\n\u0002\b\t\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u000f\u0012\b\u0010\u0002\u001a\u0004\u0018\u00010\u0003¢\u0006\u0002\u0010\u0004J\u0010\u0010\t\u001a\u0004\u0018\u00010\u0003H\u00c6\u0003¢\u0006\u0002\u0010\u0006J\u001a\u0010\n\u001a\u00020\u00002\n\b\u0002\u0010\u0002\u001a\u0004\u0018\u00010\u0003H\u00c6\u0001¢\u0006\u0002\u0010\u000bJ\u0013\u0010\f\u001a\u00020\r2\b\u0010\u000e\u001a\u0004\u0018\u00010\u000fH\u00d6\u0003J\t\u0010\u0010\u001a\u00020\u0011H\u00d6\u0001J\t\u0010\u0012\u001a\u00020\u0013H\u00d6\u0001R\u001e\u0010\u0002\u001a\u0004\u0018\u00010\u0003X\u0086\u000e¢\u0006\u0010\n\u0002\u0010\b\u001a\u0004\b\u0005\u0010\u0006\"\u0004\b\u0007\u0010\u0004¨\u0006\u0014" }, d2 = { "Lcom/tecton/udfs/spark3/Percentile;", "Ljava/io/Serializable;", "percentile", "", "(Ljava/lang/Double;)V", "getPercentile", "()Ljava/lang/Double;", "setPercentile", "Ljava/lang/Double;", "component1", "copy", "(Ljava/lang/Double;)Lcom/tecton/udfs/spark3/Percentile;", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class Percentile implements Serializable
 {
-    private double percentile;
+    @Nullable
+    private Double percentile;
     
-    public Percentile(final double percentile) {
+    public Percentile(@Nullable final Double percentile) {
         this.percentile = percentile;
     }
     
-    public final double getPercentile() {
+    @Nullable
+    public final Double getPercentile() {
         return this.percentile;
     }
     
-    public final void setPercentile(final double <set-?>) {
+    public final void setPercentile(@Nullable final Double <set-?>) {
         this.percentile = <set-?>;
     }
     
-    public final double component1() {
+    @Nullable
+    public final Double component1() {
         return this.percentile;
     }
     
     @NotNull
-    public final Percentile copy(final double percentile) {
+    public final Percentile copy(@Nullable final Double percentile) {
         return new Percentile(percentile);
     }
     
     @NotNull
     @Override
     public String toString() {
         return "Percentile(percentile=" + this.percentile + ')';
     }
     
     @Override
     public int hashCode() {
-        return Double.hashCode(this.percentile);
+        return (this.percentile == null) ? 0 : this.percentile.hashCode();
     }
     
     @Override
     public boolean equals(@Nullable final Object other) {
-        return this == other || (other instanceof Percentile && Double.compare(this.percentile, ((Percentile)other).percentile) == 0);
-    }
-    
-    public Percentile() {
-        this(0.0, 1, null);
+        return this == other || (other instanceof Percentile && Intrinsics.areEqual((Object)this.percentile, (Object)((Percentile)other).percentile));
     }
 }
```

#### com/tecton/udfs/spark3/PercentileValue.class

##### procyon -ec {}

```diff
@@ -1,17 +1,18 @@
 
 package com.tecton.udfs.spark3;
 
 import kotlin.jvm.internal.Intrinsics;
 import org.jetbrains.annotations.NotNull;
+import kotlin.jvm.internal.DefaultConstructorMarker;
 import org.jetbrains.annotations.Nullable;
 import kotlin.Metadata;
 import java.io.Serializable;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000,\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\b\u0002\n\u0002\u0010\u0006\n\u0002\b\t\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u0007\b\u0016¢\u0006\u0002\u0010\u0002B\u000f\u0012\b\u0010\u0003\u001a\u0004\u0018\u00010\u0004¢\u0006\u0002\u0010\u0005J\u0010\u0010\n\u001a\u0004\u0018\u00010\u0004H\u00c6\u0003¢\u0006\u0002\u0010\u0007J\u001a\u0010\u000b\u001a\u00020\u00002\n\b\u0002\u0010\u0003\u001a\u0004\u0018\u00010\u0004H\u00c6\u0001¢\u0006\u0002\u0010\fJ\u0013\u0010\r\u001a\u00020\u000e2\b\u0010\u000f\u001a\u0004\u0018\u00010\u0010H\u00d6\u0003J\t\u0010\u0011\u001a\u00020\u0012H\u00d6\u0001J\t\u0010\u0013\u001a\u00020\u0014H\u00d6\u0001R\u001e\u0010\u0003\u001a\u0004\u0018\u00010\u0004X\u0086\u000e¢\u0006\u0010\n\u0002\u0010\t\u001a\u0004\b\u0006\u0010\u0007\"\u0004\b\b\u0010\u0005¨\u0006\u0015" }, d2 = { "Lcom/tecton/udfs/spark3/PercentileValue;", "Ljava/io/Serializable;", "()V", "value", "", "(Ljava/lang/Double;)V", "getValue", "()Ljava/lang/Double;", "setValue", "Ljava/lang/Double;", "component1", "copy", "(Ljava/lang/Double;)Lcom/tecton/udfs/spark3/PercentileValue;", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000*\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\u0006\n\u0002\b\t\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u0011\u0012\n\b\u0002\u0010\u0002\u001a\u0004\u0018\u00010\u0003¢\u0006\u0002\u0010\u0004J\u0010\u0010\t\u001a\u0004\u0018\u00010\u0003H\u00c6\u0003¢\u0006\u0002\u0010\u0006J\u001a\u0010\n\u001a\u00020\u00002\n\b\u0002\u0010\u0002\u001a\u0004\u0018\u00010\u0003H\u00c6\u0001¢\u0006\u0002\u0010\u000bJ\u0013\u0010\f\u001a\u00020\r2\b\u0010\u000e\u001a\u0004\u0018\u00010\u000fH\u00d6\u0003J\t\u0010\u0010\u001a\u00020\u0011H\u00d6\u0001J\t\u0010\u0012\u001a\u00020\u0013H\u00d6\u0001R\u001e\u0010\u0002\u001a\u0004\u0018\u00010\u0003X\u0086\u000e¢\u0006\u0010\n\u0002\u0010\b\u001a\u0004\b\u0005\u0010\u0006\"\u0004\b\u0007\u0010\u0004¨\u0006\u0014" }, d2 = { "Lcom/tecton/udfs/spark3/PercentileValue;", "Ljava/io/Serializable;", "value", "", "(Ljava/lang/Double;)V", "getValue", "()Ljava/lang/Double;", "setValue", "Ljava/lang/Double;", "component1", "copy", "(Ljava/lang/Double;)Lcom/tecton/udfs/spark3/PercentileValue;", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class PercentileValue implements Serializable
 {
     @Nullable
     private Double value;
     
     public PercentileValue(@Nullable final Double value) {
         this.value = value;
@@ -22,18 +23,14 @@
         return this.value;
     }
     
     public final void setValue(@Nullable final Double <set-?>) {
         this.value = <set-?>;
     }
     
-    public PercentileValue() {
-        this(null);
-    }
-    
     @Nullable
     public final Double component1() {
         return this.value;
     }
     
     @NotNull
     public final PercentileValue copy(@Nullable final Double value) {
@@ -51,8 +48,12 @@
         return (this.value == null) ? 0 : this.value.hashCode();
     }
     
     @Override
     public boolean equals(@Nullable final Object other) {
         return this == other || (other instanceof PercentileValue && Intrinsics.areEqual((Object)this.value, (Object)((PercentileValue)other).value));
     }
+    
+    public PercentileValue() {
+        this(null, 1, null);
+    }
 }
```

#### com/tecton/udfs/spark3/TDigest.class

##### procyon -ec {}

```diff
@@ -1,20 +1,23 @@
 
 package com.tecton.udfs.spark3;
 
 import org.jetbrains.annotations.Nullable;
+import java.util.Comparator;
+import kotlin.collections.CollectionsKt;
 import java.util.Collection;
 import java.util.ArrayList;
+import kotlin.jvm.internal.DefaultConstructorMarker;
 import kotlin.jvm.internal.Intrinsics;
 import org.jetbrains.annotations.NotNull;
 import java.util.List;
 import kotlin.Metadata;
 import java.io.Serializable;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000>\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\b\u0002\n\u0002\u0010!\n\u0002\u0010\u0006\n\u0002\b\u0006\n\u0002\u0010\u000b\n\u0002\b\u001c\n\u0002\u0010\u0002\n\u0002\b\u0003\n\u0002\u0010\b\n\u0002\b\u000b\n\u0002\u0010\u0000\n\u0002\b\u0004\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u0007\b\u0016¢\u0006\u0002\u0010\u0002Ba\u0012\f\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u0006\u0010\u000b\u001a\u00020\f¢\u0006\u0002\u0010\rJ&\u0010(\u001a\u00020)2\u0006\u0010*\u001a\u00020\u00052\u0006\u0010+\u001a\u00020\u00052\u0006\u0010,\u001a\u00020-2\u0006\u0010.\u001a\u00020-J\u000f\u0010/\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00100\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00101\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00102\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00103\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00104\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\t\u00105\u001a\u00020\fH\u00c6\u0003Js\u00106\u001a\u00020\u00002\u000e\b\u0002\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\b\b\u0002\u0010\u000b\u001a\u00020\fH\u00c6\u0001J\u0013\u00107\u001a\u00020\f2\b\u00108\u001a\u0004\u0018\u000109H\u00d6\u0003J\t\u0010:\u001a\u00020-H\u00d6\u0001J\u001e\u0010;\u001a\u00020\u00002\u0006\u00108\u001a\u00020\u00002\u0006\u0010,\u001a\u00020-2\u0006\u0010.\u001a\u00020-J\u000e\u0010<\u001a\u00020)2\u0006\u0010,\u001a\u00020-J\t\u0010=\u001a\u00020>H\u00d6\u0001R\u0017\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u000f\u0010\u0010R\u0017\u0010\u0011\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u0012\u0010\u0010R\u0017\u0010\u0013\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u0014\u0010\u0010R\u0017\u0010\u0015\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u0016\u0010\u0010R \u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u0017\u0010\u0010\"\u0004\b\u0018\u0010\u0019R \u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u001a\u0010\u0010\"\u0004\b\u001b\u0010\u0019R \u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u001c\u0010\u0010\"\u0004\b\u001d\u0010\u0019R \u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u001e\u0010\u0010\"\u0004\b\u001f\u0010\u0019R \u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b \u0010\u0010\"\u0004\b!\u0010\u0019R \u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\"\u0010\u0010\"\u0004\b#\u0010\u0019R\u001a\u0010\u000b\u001a\u00020\fX\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b$\u0010%\"\u0004\b&\u0010'¨\u0006?" }, d2 = { "Lcom/tecton/udfs/spark3/TDigest;", "Ljava/io/Serializable;", "()V", "processedMeans", "", "", "processedWeights", "tempProcessedMeans", "tempProcessedWeights", "unprocessedMeans", "unprocessedWeights", "usingTempList", "", "(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Z)V", "currentProcessedMeans", "getCurrentProcessedMeans", "()Ljava/util/List;", "currentProcessedWeights", "getCurrentProcessedWeights", "newProcessedMeans", "getNewProcessedMeans", "newProcessedWeights", "getNewProcessedWeights", "getProcessedMeans", "setProcessedMeans", "(Ljava/util/List;)V", "getProcessedWeights", "setProcessedWeights", "getTempProcessedMeans", "setTempProcessedMeans", "getTempProcessedWeights", "setTempProcessedWeights", "getUnprocessedMeans", "setUnprocessedMeans", "getUnprocessedWeights", "setUnprocessedWeights", "getUsingTempList", "()Z", "setUsingTempList", "(Z)V", "addCentroid", "", "mean", "weight", "compression", "", "maxUnprocessed", "component1", "component2", "component3", "component4", "component5", "component6", "component7", "copy", "equals", "other", "", "hashCode", "merge", "process", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000D\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\b\u0002\n\u0002\u0010!\n\u0002\u0010\u0006\n\u0002\b\u0006\n\u0002\u0010\u000b\n\u0002\b!\n\u0002\u0010\u0002\n\u0002\b\u0003\n\u0002\u0010\b\n\u0002\b\n\n\u0002\u0010\u0000\n\u0002\b\u0007\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u0007\b\u0016¢\u0006\u0002\u0010\u0002Bo\u0012\u000e\b\u0002\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u000e\b\u0002\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u000e\b\u0002\u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u000e\b\u0002\u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u000e\b\u0002\u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\u000e\b\u0002\u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\b\b\u0002\u0010\u000b\u001a\u00020\f¢\u0006\u0002\u0010\rJ\u001e\u0010-\u001a\u00020.2\u0006\u0010/\u001a\u00020\u00052\u0006\u00100\u001a\u00020\u00052\u0006\u00101\u001a\u000202J\u000f\u00103\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00104\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00105\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00106\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00107\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u00108\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\t\u00109\u001a\u00020\fH\u00c6\u0003Js\u0010:\u001a\u00020\u00002\u000e\b\u0002\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\b\b\u0002\u0010\u000b\u001a\u00020\fH\u00c6\u0001J\u0013\u0010;\u001a\u00020\f2\b\u0010<\u001a\u0004\u0018\u00010=H\u00d6\u0003J\t\u0010>\u001a\u000202H\u00d6\u0001J\u0016\u0010?\u001a\u00020\u00002\u0006\u0010<\u001a\u00020\u00002\u0006\u00101\u001a\u000202J\u000e\u0010@\u001a\u00020.2\u0006\u00101\u001a\u000202J\u0015\u0010A\u001a\u0004\u0018\u00010\u00052\u0006\u0010B\u001a\u00020\u0005¢\u0006\u0002\u0010CJ\u0016\u0010D\u001a\u00020\u00002\u0006\u0010<\u001a\u00020E2\u0006\u00101\u001a\u000202J\t\u0010F\u001a\u00020GH\u00d6\u0001R\u0017\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u000f\u0010\u0010R\u0017\u0010\u0011\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u0012\u0010\u0010R\u0011\u0010\u0013\u001a\u00020\u00058F¢\u0006\u0006\u001a\u0004\b\u0014\u0010\u0015R\u0011\u0010\u0016\u001a\u00020\u00058F¢\u0006\u0006\u001a\u0004\b\u0017\u0010\u0015R\u0017\u0010\u0018\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u0019\u0010\u0010R\u0017\u0010\u001a\u001a\b\u0012\u0004\u0012\u00020\u00050\u00048F¢\u0006\u0006\u001a\u0004\b\u001b\u0010\u0010R \u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u001c\u0010\u0010\"\u0004\b\u001d\u0010\u001eR \u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u001f\u0010\u0010\"\u0004\b \u0010\u001eR \u0010\u0007\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b!\u0010\u0010\"\u0004\b\"\u0010\u001eR \u0010\b\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b#\u0010\u0010\"\u0004\b$\u0010\u001eR \u0010\t\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b%\u0010\u0010\"\u0004\b&\u0010\u001eR \u0010\n\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b'\u0010\u0010\"\u0004\b(\u0010\u001eR\u001a\u0010\u000b\u001a\u00020\fX\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b)\u0010*\"\u0004\b+\u0010,¨\u0006H" }, d2 = { "Lcom/tecton/udfs/spark3/TDigest;", "Ljava/io/Serializable;", "()V", "processedMeans", "", "", "processedWeights", "tempProcessedMeans", "tempProcessedWeights", "unprocessedMeans", "unprocessedWeights", "usingTempList", "", "(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Z)V", "currentProcessedMeans", "getCurrentProcessedMeans", "()Ljava/util/List;", "currentProcessedWeights", "getCurrentProcessedWeights", "max", "getMax", "()D", "min", "getMin", "newProcessedMeans", "getNewProcessedMeans", "newProcessedWeights", "getNewProcessedWeights", "getProcessedMeans", "setProcessedMeans", "(Ljava/util/List;)V", "getProcessedWeights", "setProcessedWeights", "getTempProcessedMeans", "setTempProcessedMeans", "getTempProcessedWeights", "setTempProcessedWeights", "getUnprocessedMeans", "setUnprocessedMeans", "getUnprocessedWeights", "setUnprocessedWeights", "getUsingTempList", "()Z", "setUsingTempList", "(Z)V", "addCentroid", "", "mean", "weight", "compression", "", "component1", "component2", "component3", "component4", "component5", "component6", "component7", "copy", "equals", "other", "", "hashCode", "merge", "process", "quantile", "q", "(D)Ljava/lang/Double;", "reduce", "Lcom/tecton/udfs/spark3/TDigestProcessed;", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class TDigest implements Serializable
 {
     @NotNull
     private List<Double> processedMeans;
     @NotNull
     private List<Double> processedWeights;
     @NotNull
@@ -111,42 +114,197 @@
         this.usingTempList = <set-?>;
     }
     
     public TDigest() {
         this(new ArrayList<Double>(), new ArrayList<Double>(), new ArrayList<Double>(), new ArrayList<Double>(), new ArrayList<Double>(), new ArrayList<Double>(), false);
     }
     
-    public final void addCentroid(final double mean, final double weight, final int compression, final int maxUnprocessed) {
+    public final void addCentroid(final double mean, final double weight, final int compression) {
+        if (mean == Double.NEGATIVE_INFINITY || mean == Double.POSITIVE_INFINITY || Double.isNaN(mean)) {
+            return;
+        }
         this.unprocessedMeans.add(Double.valueOf(mean));
         this.unprocessedWeights.add(Double.valueOf(weight));
+        final int maxUnprocessed = compression * 10;
         if (this.unprocessedMeans.size() > maxUnprocessed) {
             this.process(compression);
         }
     }
     
-    public final void process(final int compression) {
-        if (this.unprocessedMeans.isEmpty()) {
-            return;
+    @NotNull
+    public final TDigest reduce(@NotNull final TDigestProcessed other, final int compression) {
+        Intrinsics.checkNotNullParameter((Object)other, "other");
+        for (int i = 0; i < other.getProcessedMeans().size(); ++i) {
+            this.addCentroid(((Number)other.getProcessedMeans().get(i)).doubleValue(), ((Number)other.getProcessedWeights().get(i)).doubleValue(), compression);
         }
-        ApproxPercentilePartialAggKt.access$process(compression, (List)this.getCurrentProcessedMeans(), (List)this.getCurrentProcessedWeights(), (List)this.unprocessedMeans, (List)this.unprocessedWeights, (List)this.getNewProcessedMeans(), (List)this.getNewProcessedWeights());
-        this.usingTempList = !this.usingTempList;
+        return this;
     }
     
     @NotNull
-    public final TDigest merge(@NotNull final TDigest other, final int compression, final int maxUnprocessed) {
+    public final TDigest merge(@NotNull final TDigest other, final int compression) {
         Intrinsics.checkNotNullParameter((Object)other, "other");
         if (!((Collection)other.unprocessedMeans).isEmpty()) {
             other.process(compression);
         }
         for (int i = 0; i < other.getCurrentProcessedMeans().size(); ++i) {
-            this.addCentroid(((Number)other.getCurrentProcessedMeans().get(i)).doubleValue(), ((Number)other.getCurrentProcessedWeights().get(i)).doubleValue(), compression, maxUnprocessed);
+            this.addCentroid(((Number)other.getCurrentProcessedMeans().get(i)).doubleValue(), ((Number)other.getCurrentProcessedWeights().get(i)).doubleValue(), compression);
         }
         return this;
     }
     
+    public final void process(final int compression) {
+        if (this.getCurrentProcessedMeans().size() != this.getCurrentProcessedWeights().size()) {
+            final int n = 0;
+            throw new IllegalArgumentException("processedMeans and processedWeights must have the same length".toString());
+        }
+        if (this.unprocessedMeans.size() != this.unprocessedWeights.size()) {
+            final int n2 = 0;
+            throw new IllegalArgumentException("unprocessedMeans and unprocessedWeights must have the same length".toString());
+        }
+        if (!this.getNewProcessedMeans().isEmpty()) {
+            final int n3 = 0;
+            throw new IllegalArgumentException("newProcessedMeans must be empty".toString());
+        }
+        if (!this.getNewProcessedWeights().isEmpty()) {
+            final int n4 = 0;
+            throw new IllegalArgumentException("newProcessedWeights must be empty".toString());
+        }
+        if (this.unprocessedMeans.isEmpty()) {
+            return;
+        }
+        final Iterable $this$sortedBy$iv = (Iterable)CollectionsKt.getIndices((Collection)this.unprocessedMeans);
+        final int $i$f$sortedBy = 0;
+        final List unprocessedSortedIndices = CollectionsKt.sortedWith($this$sortedBy$iv, (Comparator)new TDigest$process$$inlined$sortedBy$1(this));
+        final double totalWeight = CollectionsKt.sumOfDouble((Iterable)this.unprocessedWeights) + CollectionsKt.sumOfDouble((Iterable)this.getCurrentProcessedWeights());
+        double processedWeight = 0.0;
+        final double startingValue = ApproxPercentilePartialAggKt.k3(0.0, compression, totalWeight);
+        double limit = totalWeight * ApproxPercentilePartialAggKt.q3(startingValue + 1.0, compression, totalWeight);
+        int iterProcessed = 0;
+        int iterUnprocessed = 0;
+        double mean = 0.0;
+        double weight = 0.0;
+        while (iterProcessed < this.getCurrentProcessedMeans().size() || iterUnprocessed < this.unprocessedMeans.size()) {
+            if (iterUnprocessed == this.unprocessedMeans.size()) {
+                mean = ((Number)this.getCurrentProcessedMeans().get(iterProcessed)).doubleValue();
+                weight = ((Number)this.getCurrentProcessedWeights().get(iterProcessed)).doubleValue();
+                ++iterProcessed;
+            }
+            else {
+                final int sortedIndex = ((Number)unprocessedSortedIndices.get(iterUnprocessed)).intValue();
+                if (iterProcessed == this.getCurrentProcessedMeans().size()) {
+                    mean = ((Number)this.unprocessedMeans.get(sortedIndex)).doubleValue();
+                    weight = ((Number)this.unprocessedWeights.get(sortedIndex)).doubleValue();
+                    ++iterUnprocessed;
+                }
+                else if (((Number)this.getCurrentProcessedMeans().get(iterProcessed)).doubleValue() < ((Number)this.unprocessedMeans.get(sortedIndex)).doubleValue()) {
+                    mean = ((Number)this.getCurrentProcessedMeans().get(iterProcessed)).doubleValue();
+                    weight = ((Number)this.getCurrentProcessedWeights().get(iterProcessed)).doubleValue();
+                    ++iterProcessed;
+                }
+                else {
+                    mean = ((Number)this.unprocessedMeans.get(sortedIndex)).doubleValue();
+                    weight = ((Number)this.unprocessedWeights.get(sortedIndex)).doubleValue();
+                    ++iterUnprocessed;
+                }
+            }
+            if (this.getNewProcessedMeans().isEmpty()) {
+                this.getNewProcessedMeans().add(Double.valueOf(mean));
+                this.getNewProcessedWeights().add(Double.valueOf(weight));
+            }
+            else if (processedWeight + weight <= limit) {
+                final double newWeight = ((Number)CollectionsKt.last((List)this.getNewProcessedWeights())).doubleValue() + weight;
+                final double newMean = (((Number)CollectionsKt.last((List)this.getNewProcessedMeans())).doubleValue() * ((Number)CollectionsKt.last((List)this.getNewProcessedWeights())).doubleValue() + mean * weight) / newWeight;
+                this.getNewProcessedMeans().set(this.getNewProcessedMeans().size() - 1, Double.valueOf(newMean));
+                this.getNewProcessedWeights().set(this.getNewProcessedWeights().size() - 1, Double.valueOf(newWeight));
+            }
+            else {
+                this.getNewProcessedMeans().add(Double.valueOf(mean));
+                this.getNewProcessedWeights().add(Double.valueOf(weight));
+                limit = totalWeight * ApproxPercentilePartialAggKt.q3(ApproxPercentilePartialAggKt.k3(processedWeight / totalWeight, compression, totalWeight) + 1.0, compression, totalWeight);
+            }
+            processedWeight += weight;
+        }
+        if (((Collection)this.getNewProcessedWeights()).isEmpty()) {
+            final int n5 = 0;
+            throw new IllegalStateException("processing must create new centroids".toString());
+        }
+        if (((Number)this.getNewProcessedWeights().get(0)).doubleValue() != 1.0) {
+            final int n6 = 0;
+            throw new IllegalStateException("first centroid must have weight 1.0".toString());
+        }
+        if (((Number)CollectionsKt.last((List)this.getNewProcessedWeights())).doubleValue() != 1.0) {
+            final int n7 = 0;
+            throw new IllegalStateException("last centroid must have weight 1.0".toString());
+        }
+        this.getCurrentProcessedMeans().clear();
+        this.getCurrentProcessedWeights().clear();
+        this.unprocessedMeans.clear();
+        this.unprocessedWeights.clear();
+        this.usingTempList = !this.usingTempList;
+    }
+    
+    @Nullable
+    public final Double quantile(final double q) {
+        if (q < 0.0 || q > 1.0) {
+            final int n = 0;
+            throw new IllegalArgumentException("q must be in the range [0.0, 1.0]".toString());
+        }
+        if (this.getCurrentProcessedMeans().isEmpty()) {
+            return null;
+        }
+        if (((Number)this.getCurrentProcessedWeights().get(0)).doubleValue() != 1.0 || ((Number)this.getCurrentProcessedWeights().get(this.getCurrentProcessedWeights().size() - 1)).doubleValue() != 1.0) {
+            final int n2 = 0;
+            throw new IllegalArgumentException("The first and last centroids must have weight 1.0".toString());
+        }
+        if (this.getCurrentProcessedMeans().size() == 1) {
+            return Double.valueOf(this.getCurrentProcessedMeans().get(0));
+        }
+        final double processedWeight = CollectionsKt.sumOfDouble((Iterable)this.getCurrentProcessedWeights());
+        final double index = q * processedWeight;
+        if (index < 1.0) {
+            return Double.valueOf(this.getMin());
+        }
+        if (index > processedWeight - 1) {
+            return Double.valueOf(this.getMax());
+        }
+        double weightSoFar = ((Number)this.getCurrentProcessedWeights().get(0)).doubleValue() / 2.0;
+        int i = 0;
+        final int n3 = this.getCurrentProcessedWeights().size() - 2;
+        if (i <= n3) {
+            while (true) {
+                final double dw = (((Number)this.getCurrentProcessedWeights().get(i)).doubleValue() + ((Number)this.getCurrentProcessedWeights().get(i + 1)).doubleValue()) / 2.0;
+                if (weightSoFar + dw > index) {
+                    double leftDelta = 0.0;
+                    if (((Number)this.getCurrentProcessedWeights().get(i)).doubleValue() == 1.0) {
+                        if (index - weightSoFar < 0.5) {
+                            return Double.valueOf(this.getCurrentProcessedMeans().get(i));
+                        }
+                        leftDelta = 0.5;
+                    }
+                    double rightDelta = 0.0;
+                    if (((Number)this.getCurrentProcessedWeights().get(i + 1)).doubleValue() == 1.0) {
+                        if (weightSoFar + dw - index <= 0.5) {
+                            return Double.valueOf(this.getCurrentProcessedMeans().get(i + 1));
+                        }
+                        rightDelta = 0.5;
+                    }
+                    final double z1 = index - weightSoFar - leftDelta;
+                    final double z2 = weightSoFar + dw - index - rightDelta;
+                    return Double.valueOf((((Number)this.getCurrentProcessedMeans().get(i)).doubleValue() * z2 + ((Number)this.getCurrentProcessedMeans().get(i + 1)).doubleValue() * z1) / (z1 + z2));
+                }
+                weightSoFar += dw;
+                if (i == n3) {
+                    break;
+                }
+                ++i;
+            }
+        }
+        throw new IllegalStateException("should never get here");
+    }
+    
     @NotNull
     public final List<Double> getCurrentProcessedMeans() {
         return this.usingTempList ? this.tempProcessedMeans : this.processedMeans;
     }
     
     @NotNull
     public final List<Double> getCurrentProcessedWeights() {
@@ -159,14 +317,30 @@
     }
     
     @NotNull
     public final List<Double> getNewProcessedWeights() {
         return this.usingTempList ? this.processedWeights : this.tempProcessedWeights;
     }
     
+    public final double getMin() {
+        if (((Collection)this.getCurrentProcessedMeans()).isEmpty()) {
+            final int n = 0;
+            throw new IllegalArgumentException("can only get min if there are centroids ".toString());
+        }
+        return ((Number)this.getCurrentProcessedMeans().get(0)).doubleValue();
+    }
+    
+    public final double getMax() {
+        if (((Collection)this.getCurrentProcessedMeans()).isEmpty()) {
+            final int n = 0;
+            throw new IllegalArgumentException("can only get max if there are centroids ".toString());
+        }
+        return ((Number)this.getCurrentProcessedMeans().get(this.getCurrentProcessedMeans().size() - 1)).doubleValue();
+    }
+    
     @NotNull
     public final List<Double> component1() {
         return this.processedMeans;
     }
     
     @NotNull
     public final List<Double> component2() {
```

#### com/tecton/udfs/spark3/TDigestProcessed.class

##### procyon -ec {}

```diff
@@ -1,19 +1,20 @@
 
 package com.tecton.udfs.spark3;
 
 import org.jetbrains.annotations.Nullable;
 import java.util.ArrayList;
+import kotlin.jvm.internal.DefaultConstructorMarker;
 import kotlin.jvm.internal.Intrinsics;
 import org.jetbrains.annotations.NotNull;
 import java.util.List;
 import kotlin.Metadata;
 import java.io.Serializable;
 
-@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u00000\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0002\b\u0002\n\u0002\u0010!\n\u0002\u0010\u0006\n\u0002\b\f\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B\u0007\b\u0016¢\u0006\u0002\u0010\u0002B!\u0012\f\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004\u0012\f\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004¢\u0006\u0002\u0010\u0007J\u000f\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J\u000f\u0010\u000f\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0003J)\u0010\u0010\u001a\u00020\u00002\u000e\b\u0002\u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u00042\u000e\b\u0002\u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004H\u00c6\u0001J\u0013\u0010\u0011\u001a\u00020\u00122\b\u0010\u0013\u001a\u0004\u0018\u00010\u0014H\u00d6\u0003J\t\u0010\u0015\u001a\u00020\u0016H\u00d6\u0001J\t\u0010\u0017\u001a\u00020\u0018H\u00d6\u0001R \u0010\u0003\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\b\u0010\t\"\u0004\b\n\u0010\u000bR \u0010\u0006\u001a\b\u0012\u0004\u0012\u00020\u00050\u0004X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\f\u0010\t\"\u0004\b\r\u0010\u000b¨\u0006\u0019" }, d2 = { "Lcom/tecton/udfs/spark3/TDigestProcessed;", "Ljava/io/Serializable;", "()V", "processedMeans", "", "", "processedWeights", "(Ljava/util/List;Ljava/util/List;)V", "getProcessedMeans", "()Ljava/util/List;", "setProcessedMeans", "(Ljava/util/List;)V", "getProcessedWeights", "setProcessedWeights", "component1", "component2", "copy", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
+@Metadata(mv = { 1, 7, 1 }, k = 1, xi = 48, d1 = { "\u0000.\n\u0002\u0018\u0002\n\u0002\u0018\u0002\n\u0000\n\u0002\u0010!\n\u0002\u0010\u0006\n\u0002\b\f\n\u0002\u0010\u000b\n\u0000\n\u0002\u0010\u0000\n\u0000\n\u0002\u0010\b\n\u0000\n\u0002\u0010\u000e\n\u0000\b\u0086\b\u0018\u00002\u00020\u0001B%\u0012\u000e\b\u0002\u0010\u0002\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003\u0012\u000e\b\u0002\u0010\u0005\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003¢\u0006\u0002\u0010\u0006J\u000f\u0010\r\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003H\u00c6\u0003J\u000f\u0010\u000e\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003H\u00c6\u0003J)\u0010\u000f\u001a\u00020\u00002\u000e\b\u0002\u0010\u0002\u001a\b\u0012\u0004\u0012\u00020\u00040\u00032\u000e\b\u0002\u0010\u0005\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003H\u00c6\u0001J\u0013\u0010\u0010\u001a\u00020\u00112\b\u0010\u0012\u001a\u0004\u0018\u00010\u0013H\u00d6\u0003J\t\u0010\u0014\u001a\u00020\u0015H\u00d6\u0001J\t\u0010\u0016\u001a\u00020\u0017H\u00d6\u0001R \u0010\u0002\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u0007\u0010\b\"\u0004\b\t\u0010\nR \u0010\u0005\u001a\b\u0012\u0004\u0012\u00020\u00040\u0003X\u0086\u000e¢\u0006\u000e\n\u0000\u001a\u0004\b\u000b\u0010\b\"\u0004\b\f\u0010\n¨\u0006\u0018" }, d2 = { "Lcom/tecton/udfs/spark3/TDigestProcessed;", "Ljava/io/Serializable;", "processedMeans", "", "", "processedWeights", "(Ljava/util/List;Ljava/util/List;)V", "getProcessedMeans", "()Ljava/util/List;", "setProcessedMeans", "(Ljava/util/List;)V", "getProcessedWeights", "setProcessedWeights", "component1", "component2", "copy", "equals", "", "other", "", "hashCode", "", "toString", "", "java_com_tecton_udfs_spark3-tecton-udfs-lib" })
 public final class TDigestProcessed implements Serializable
 {
     @NotNull
     private List<Double> processedMeans;
     @NotNull
     private List<Double> processedWeights;
     
@@ -40,18 +41,14 @@
     }
     
     public final void setProcessedWeights(@NotNull final List<Double> <set-?>) {
         Intrinsics.checkNotNullParameter((Object)<set-?>, "<set-?>");
         this.processedWeights = <set-?>;
     }
     
-    public TDigestProcessed() {
-        this(new ArrayList<Double>(), new ArrayList<Double>());
-    }
-    
     @NotNull
     public final List<Double> component1() {
         return this.processedMeans;
     }
     
     @NotNull
     public final List<Double> component2() {
@@ -85,8 +82,12 @@
         }
         if (!(other instanceof TDigestProcessed)) {
             return false;
         }
         final TDigestProcessed tDigestProcessed = (TDigestProcessed)other;
         return Intrinsics.areEqual((Object)this.processedMeans, (Object)tDigestProcessed.processedMeans) && Intrinsics.areEqual((Object)this.processedWeights, (Object)tDigestProcessed.processedWeights);
     }
+    
+    public TDigestProcessed() {
+        this(null, null, 3, null);
+    }
 }
```

### Comparing `tecton-0.7.0rc2/tecton_spark/materialization_plan.py` & `tecton-0.7.0rc3/tecton_spark/materialization_plan.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/offline_store.py` & `tecton-0.7.0rc3/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/partial_aggregations.py` & `tecton-0.7.0rc3/tecton_spark/partial_aggregations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/pipeline_helper.py` & `tecton-0.7.0rc3/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/data_source.py` & `tecton-0.7.0rc3/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/filter.py` & `tecton-0.7.0rc3/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/join.py` & `tecton-0.7.0rc3/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/node.py` & `tecton-0.7.0rc3/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/pipeline.py` & `tecton-0.7.0rc3/tecton_spark/query/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/projection.py` & `tecton-0.7.0rc3/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/query/translate.py` & `tecton-0.7.0rc3/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/schema_derivation_utils.py` & `tecton-0.7.0rc3/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/schema_spark_utils.py` & `tecton-0.7.0rc3/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/spark_helper.py` & `tecton-0.7.0rc3/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/spark_schema_wrapper.py` & `tecton-0.7.0rc3/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/time_utils.py` & `tecton-0.7.0rc3/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc2/tecton_spark/udfs.py` & `tecton-0.7.0rc3/tecton_spark/udfs.py`

 * *Files identical despite different names*

