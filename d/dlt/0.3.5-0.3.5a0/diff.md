# Comparing `tmp/dlt-0.3.5.tar.gz` & `tmp/dlt-0.3.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.5.tar", max compression
+gzip compressed data, was "dlt-0.3.5a0.tar", max compression
```

## Comparing `dlt-0.3.5.tar` & `dlt-0.3.5a0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0     4196 2023-07-21 12:57:39.118978 dlt-0.3.5/README.md
--rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17127 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15046 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2308 2023-07-20 14:41:03.294283 dlt-0.3.5/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.5/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.5/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20347 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-07-23 19:50:04.055755 dlt-0.3.5/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-07-21 12:45:34.138978 dlt-0.3.5/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6559 2023-07-20 23:10:47.941211 dlt-0.3.5/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.5/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     8426 2023-07-20 16:41:36.924283 dlt-0.3.5/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    12397 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.5/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19564 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5032 2023-07-21 13:08:23.348978 dlt-0.3.5/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7234 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2798 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25222 2023-07-23 14:19:47.065755 dlt-0.3.5/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-07-20 16:42:01.694283 dlt-0.3.5/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    15192 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0     2019 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     2300 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     4284 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     5105 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.5/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2935 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     6445 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1390 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5216 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    19525 2023-07-23 14:19:47.065755 dlt-0.3.5/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     2244 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/motherduck/__init__.py
--rw-r--r--   0        0        0     2070 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/motherduck/configuration.py
--rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/motherduck/motherduck.py
--rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/motherduck/sql_client.py
--rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     4490 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     5781 2023-07-20 16:42:13.474283 dlt-0.3.5/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      894 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     9085 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/destinations/snowflake/__init__.py
--rw-r--r--   0        0        0     4347 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/destinations/snowflake/configuration.py
--rw-r--r--   0        0        0    10402 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/snowflake/snowflake.py
--rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/destinations/snowflake/sql_client.py
--rw-r--r--   0        0        0     8045 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    12311 2023-07-21 12:58:04.898978 dlt-0.3.5/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.5/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/extract.py
--rw-r--r--   0        0        0    19337 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35424 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.5/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13867 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13214 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/load/exceptions.py
--rw-r--r--   0        0        0    22500 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.5/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16488 2023-07-20 16:42:34.194283 dlt-0.3.5/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.5/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8753 2023-07-21 12:58:04.908978 dlt-0.3.5/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    65184 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     9132 2023-07-20 14:41:03.304283 dlt-0.3.5/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5060 2023-07-23 22:00:45.675755 dlt-0.3.5/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.5/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.5/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.5/dlt/version.py
--rw-r--r--   0        0        0     4459 2023-07-23 22:00:45.675755 dlt-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     7815 1970-01-01 00:00:00.000000 dlt-0.3.5/setup.py
--rw-r--r--   0        0        0     7800 1970-01-01 00:00:00.000000 dlt-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.5a0/LICENSE.txt
+-rw-r--r--   0        0        0     4144 2023-07-08 12:23:15.759697 dlt-0.3.5a0/README.md
+-rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17127 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15046 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2308 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.5a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6559 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.5a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8426 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3158 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11909 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.5a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19531 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7234 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2798 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    14030 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     2257 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4135 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2260 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     5918 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5046 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    17153 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     2201 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/motherduck/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/configuration.py
+-rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/sql_client.py
+-rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-13 15:13:56.520313 dlt-0.3.5a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3176 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     5781 2023-07-15 10:59:55.545022 dlt-0.3.5a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     8620 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4075 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0     9021 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     7776 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10489 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.5a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    19337 2023-07-18 12:05:27.467911 dlt-0.3.5a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35424 2023-07-18 12:05:27.467911 dlt-0.3.5a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.5a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13867 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13214 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    22228 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16488 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8711 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    64550 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     9132 2023-07-18 11:51:55.337911 dlt-0.3.5a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4894 2023-07-18 11:51:55.337911 dlt-0.3.5a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.5a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/version.py
+-rw-r--r--   0        0        0     4461 2023-07-18 12:05:37.647911 dlt-0.3.5a0/pyproject.toml
+-rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 dlt-0.3.5a0/setup.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 dlt-0.3.5a0/PKG-INFO
```

### Comparing `dlt-0.3.5/LICENSE.txt` & `dlt-0.3.5a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/README.md` & `dlt-0.3.5a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,32 +27,29 @@
 
 ## Quick Start
 
 Load chess game data from chess.com API and save it in DuckDB:
 
 ```python
 import dlt
-import requests
-# Create a dlt pipeline that will load
-# chess player data to the DuckDB destination
+from chess import chess # a utility function that grabs data from the chess.com API
+
+# create a dlt pipeline that will load chess game data to the DuckDB destination
 pipeline = dlt.pipeline(
     pipeline_name='chess_pipeline',
     destination='duckdb',
-    dataset_name='player_data'
+    dataset_name='games_data'
 )
-# Grab some player data from Chess.com API
-data = []
-for player in ['magnuscarlsen', 'rpragchess']:
-    response = requests.get(f'https://api.chess.com/pub/player/{player}')
-    response.raise_for_status()
-    data.append(response.json())
-# Extract, normalize, and load the data
-pipeline.run(data, table_name='player')
-```
 
+# use chess.com API to grab data about a few players
+data = chess(['magnuscarlsen', 'rpragchess'], start_month='2022/11', end_month='2022/12')
+
+# extract, normalize, and load the data
+pipeline.run(data)
+```
 
 Try it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
 
 ## Features
 
 - **Automatic Schema:** Data structure inspection and schema creation for the destination.
 - **Data Normalization:** Consistent and verified data before loading.
```

### Comparing `dlt-0.3.5/dlt/__init__.py` & `dlt-0.3.5a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/_dlt.py` & `dlt-0.3.5a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/config_toml_writer.py` & `dlt-0.3.5a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/deploy_command.py` & `dlt-0.3.5a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.5a0/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/echo.py` & `dlt-0.3.5a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/init_command.py` & `dlt-0.3.5a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/pipeline_command.py` & `dlt-0.3.5a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/pipeline_files.py` & `dlt-0.3.5a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/source_detection.py` & `dlt-0.3.5a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/telemetry_command.py` & `dlt-0.3.5a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/cli/utils.py` & `dlt-0.3.5a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/arithmetics.py` & `dlt-0.3.5a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/accessors.py` & `dlt-0.3.5a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/container.py` & `dlt-0.3.5a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/exceptions.py` & `dlt-0.3.5a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/inject.py` & `dlt-0.3.5a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/paths.py` & `dlt-0.3.5a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/context.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/environ.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/provider.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/providers/toml.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/resolve.py` & `dlt-0.3.5a0/dlt/common/configuration/resolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from typing import Any, Dict, ContextManager, List, Optional, Sequence, Tuple, Type, TypeVar
 
 from dlt.common.configuration.providers.provider import ConfigProvider
 from dlt.common.typing import AnyType, StrAny, TSecretValue, get_all_types_of_class_in_union, is_final_type, is_optional_type, is_union
 
 from dlt.common.configuration.specs.base_configuration import BaseConfiguration, CredentialsConfiguration, is_secret_hint, extract_inner_hint, is_context_inner_hint, is_base_configuration_inner_hint, is_valid_hint
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
-from dlt.common.configuration.specs.exceptions import NativeValueError
-from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
 from dlt.common.configuration.container import Container
+from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
 from dlt.common.configuration.utils import log_traces, deserialize_value
 from dlt.common.configuration.exceptions import (
     FinalConfigFieldException, LookupTrace, ConfigFieldMissingException, ConfigurationWrongTypeException,
     ValueNotSecretException, InvalidNativeValue, UnmatchedConfigHintResolversException)
 
 TConfiguration = TypeVar("TConfiguration", bound=BaseConfiguration)
 
@@ -32,41 +31,14 @@
             explicit_value = None
         else:
             log_traces(None, config.__section__, type(config), explicit_value, None, traces)
 
     return _resolve_configuration(config, sections, (), explicit_value, accept_partial)
 
 
-def initialize_credentials(hint: Any, initial_value: Any) -> CredentialsConfiguration:
-    """Instantiate credentials of type `hint` with `initial_value`. The initial value must be a native representation (typically string)
-    or a dictionary corresponding to credential's fields. In case of union of credentials, the first configuration in the union fully resolved by
-    initial value will be instantiated."""
-    # use passed credentials as initial value. initial value may resolve credentials
-    if is_union(hint):
-        specs_in_union = get_all_types_of_class_in_union(hint, CredentialsConfiguration)
-        assert len(specs_in_union) > 0
-        first_credentials: CredentialsConfiguration = None
-        for idx, spec in enumerate(specs_in_union):
-            try:
-                # print(spec)
-                credentials = spec(initial_value)
-                if credentials.is_resolved():
-                    return credentials
-                # keep first credentials in the union to return in case all of the match but not resolve
-                first_credentials = first_credentials or credentials
-            except (NativeValueError, NotImplementedError):
-                # if none of specs in union parsed
-                if idx == len(specs_in_union) - 1 and first_credentials is None:
-                    raise
-        return first_credentials
-    else:
-        assert issubclass(hint, CredentialsConfiguration)
-        return hint(initial_value)  # type: ignore
-
-
 def inject_section(section_context: ConfigSectionContext, merge_existing: bool = True) -> ContextManager[ConfigSectionContext]:
     """Context manager that sets section specified in `section_context` to be used during configuration resolution. Optionally merges the context already in the container with the one provided
 
     Args:
         section_context (ConfigSectionContext): Instance providing a pipeline name and section context
         merge_existing (bool, optional): Merges existing section context with `section_context` in the arguments by executing `merge_style` function on `section_context`. Defaults to True.
```

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/configuration/utils.py` & `dlt-0.3.5a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/data_types/type_helpers.py` & `dlt-0.3.5a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/data_writers/buffered.py` & `dlt-0.3.5a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/data_writers/escape.py` & `dlt-0.3.5a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/data_writers/exceptions.py` & `dlt-0.3.5a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/data_writers/writers.py` & `dlt-0.3.5a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/destination/capabilities.py` & `dlt-0.3.5a0/dlt/common/destination/capabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     max_query_length: int
     is_max_query_length_in_bytes: bool
     max_text_data_type_length: int
     is_max_text_data_type_length_in_bytes: bool
     supports_ddl_transactions: bool
     naming_convention: str = "snake_case"
     alter_add_multi_column: bool = True
-    supports_truncate_command: bool = True
 
     # do not allow to create default value, destination caps must be always explicitly inserted into container
     can_create_default: ClassVar[bool] = False
 
     @staticmethod
     def generic_capabilities(preferred_loader_file_format: TLoaderFileFormat = None) -> "DestinationCapabilitiesContext":
         caps = DestinationCapabilitiesContext()
```

### Comparing `dlt-0.3.5/dlt/common/destination/reference.py` & `dlt-0.3.5a0/dlt/common/destination/reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 from abc import ABC, abstractmethod
 from importlib import import_module
 from types import TracebackType, ModuleType
-from typing import ClassVar, Final, Optional, Literal, Sequence, Iterable, Type, Protocol, Union, TYPE_CHECKING, cast, List, ContextManager
-from contextlib import contextmanager
+from typing import ClassVar, Final, Optional, Literal, Sequence, Iterable, Type, Protocol, Union, TYPE_CHECKING, cast, List
 
 from dlt.common import logger
 from dlt.common.exceptions import IdentifierTooLongException, InvalidDestinationReference, UnknownDestinationModule
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
-from dlt.common.schema.typing import TWriteDisposition
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration, CredentialsConfiguration
 from dlt.common.configuration.accessors import config
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.common.schema.utils import is_complete_column
 from dlt.common.storages import FileStorage
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
 from dlt.common.utils import get_module_name
 from dlt.common.configuration.specs import GcpCredentials, AwsCredentialsWithoutDefaults
 
-TLoaderReplaceStrategy = Literal["truncate-and-insert", "insert-from-staging", "staging-optimized"]
 
 @configspec(init=True)
 class DestinationClientConfiguration(BaseConfiguration):
     destination_name: str = None  # which destination to load data to
     credentials: Optional[CredentialsConfiguration]
 
-    def fingerprint(self) -> str:
-        """Returns a destination fingerprint which is a hash of selected configuration fields. ie. host in case of connection string"""
-        return ""
-
     def __str__(self) -> str:
         """Return displayable destination location"""
         return str(self.credentials)
 
     if TYPE_CHECKING:
         def __init__(self, destination_name: str = None, credentials: Optional[CredentialsConfiguration] = None
 ) -> None:
@@ -44,16 +37,14 @@
 class DestinationClientDwhConfiguration(DestinationClientConfiguration):
     # keep default/initial value if present
     dataset_name: Final[str] = None
     """dataset name in the destination to load data to, for schemas that are not default schema, it is used as dataset prefix"""
     default_schema_name: Optional[str] = None
     """name of default schema to be used to name effective dataset to load data to"""
     staging_credentials: Optional[CredentialsConfiguration] = None
-    """How to handle replace disposition for this destination, can be classic or staging"""
-    replace_strategy: TLoaderReplaceStrategy = "truncate-and-insert"
 
     if TYPE_CHECKING:
         def __init__(
             self,
             destination_name: str = None,
             credentials: Optional[CredentialsConfiguration] = None,
             dataset_name: str = None,
@@ -142,31 +133,32 @@
     capabilities: ClassVar[DestinationCapabilitiesContext] = None
 
     def __init__(self, schema: Schema, config: DestinationClientConfiguration) -> None:
         self.schema = schema
         self.config = config
 
     @abstractmethod
-    def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
-        """Prepares storage to be used ie. creates database schema or file system folder. Truncates requested tables.
+    def initialize_storage(self, staging: bool = False, truncate_tables: Iterable[str] = None) -> None:
+        """Prepares storage to be used ie. creates database schema or file system folder. Creates a staging storage if `staging` flag is true. Truncates requested tables.
         """
         pass
 
     @abstractmethod
-    def is_storage_initialized(self) -> bool:
-        """Returns if storage is ready to be read/written."""
+    def is_storage_initialized(self, staging: bool = False) -> bool:
+        """Returns if storage is ready to be read/written. Checks staging storage if `staging` flag is true"""
         pass
 
-    def update_storage_schema(self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
+    def update_storage_schema(self, staging: bool = False, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
         """Updates storage to the current schema.
 
         Implementations should not assume that `expected_update` is the exact difference between destination state and the self.schema. This is only the case if
         destination has single writer and no other processes modify the schema.
 
         Args:
+            staging (bool, optional): Updates the staging if True. Defaults to False.
             only_tables (Sequence[str], optional): Updates only listed tables. Defaults to None.
             expected_update (TSchemaTables, optional): Update that is expected to be applied to the destination
         Returns:
             Optional[TSchemaTables]: Returns an update that was applied at the destination.
         """
         self._verify_schema()
         return expected_update
@@ -177,17 +169,19 @@
         pass
 
     @abstractmethod
     def restore_file_load(self, file_path: str) -> LoadJob:
         pass
 
     @abstractmethod
-    def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
-        """Creates a list of followup jobs that should be executed after a table chain is completed"""
-        return []
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+        """Creates a table merge job without executing it. The `table_chain` contains a list of tables, ordered by ancestry, that should be merged.
+        Clients that cannot merge should return None
+        """
+        pass
 
     @abstractmethod
     def complete_load(self, load_id: str) -> None:
         pass
 
     @abstractmethod
     def __enter__(self) -> "JobClientBase":
@@ -232,24 +226,14 @@
             raise InvalidDatasetName(dataset_name, norm_name)
         # if default schema is None then suffix is not added
         if default_schema_name is not None and schema.name != default_schema_name:
             norm_name += "_" + schema.name
 
         return norm_name
 
-class StagingJobClientBase(JobClientBase):
-
-    @abstractmethod
-    def get_stage_dispositions(self) -> List[TWriteDisposition]:
-        return []
-
-    @abstractmethod
-    def with_staging_dataset(self)-> ContextManager["JobClientBase"]:
-        return self
-
 
 TDestinationReferenceArg = Union["DestinationReference", ModuleType, None, str]
 
 
 class DestinationReference(Protocol):
     __name__: str
```

### Comparing `dlt-0.3.5/dlt/common/exceptions.py` & `dlt-0.3.5a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/git.py` & `dlt-0.3.5a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/json/__init__.py` & `dlt-0.3.5a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/json/_orjson.py` & `dlt-0.3.5a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/json/_simplejson.py` & `dlt-0.3.5a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/jsonpath.py` & `dlt-0.3.5a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/libs/pyarrow.py` & `dlt-0.3.5a0/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/configuration.py` & `dlt-0.3.5a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.5a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/json/relational.py` & `dlt-0.3.5a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/normalizers/utils.py` & `dlt-0.3.5a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/pipeline.py` & `dlt-0.3.5a0/dlt/common/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 class LoadInfo(NamedTuple):
     """A tuple holding the information on recently loaded packages. Returned by pipeline `run` and `load` methods"""
     pipeline: "SupportsPipeline"
     destination_name: str
     destination_displayable_credentials: str
     staging_name: str
     staging_displayable_credentials: str
-    destination_fingerprint: str
     dataset_name: str
     loads_ids: List[str]
     """ids of the loaded packages"""
     load_packages: List[LoadPackageInfo]
     """Information on loaded packages"""
     started_at: datetime.datetime
     first_run: bool
```

### Comparing `dlt-0.3.5/dlt/common/reflection/spec.py` & `dlt-0.3.5a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/reflection/utils.py` & `dlt-0.3.5a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/configuration.py` & `dlt-0.3.5a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/pool_runner.py` & `dlt-0.3.5a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/runnable.py` & `dlt-0.3.5a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/stdout.py` & `dlt-0.3.5a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/synth_pickle.py` & `dlt-0.3.5a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runners/venv.py` & `dlt-0.3.5a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/collector.py` & `dlt-0.3.5a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/exec_info.py` & `dlt-0.3.5a0/dlt/common/runtime/exec_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 
 from dlt.common.typing import StrStr, StrAny, Literal, List
 from dlt.common.utils import filter_env_vars
 from dlt.version import __version__
 
 
-TExecInfoNames = Literal["kubernetes", "docker", "codespaces", "github_actions", "airflow", "notebook", "colab","aws_lambda","gcp_cloud_function"]
+TExecInfoNames = Literal["kubernetes", "docker", "codespaces", "github_actions", "airflow", "notebook", "colab"]
 # if one of these environment variables is set, we assume to be running in CI env
 CI_ENVIRONMENT_TELL = [
     "bamboo.buildKey",
     "BUILD_ID",
     "BUILD_NUMBER",
     "BUILDKITE",
     "CI",
@@ -41,18 +41,14 @@
         names.append("github_actions")
     if is_notebook():
         names.append("notebook")
     if is_colab():
         names.append("colab")
     if airflow_info():
         names.append("airflow")
-    if is_aws_lambda():
-        names.append("aws_lambda")
-    if is_gcp_cloud_function():
-        names.append("gcp_cloud_function")
     return names
 
 
 def is_codespaces() -> bool:
     return "CODESPACES" in os.environ
 
 
@@ -150,17 +146,7 @@
 
     # if that didn't work, try to use proc information
     try:
         with open("/proc/self/cgroup", mode="r", encoding="utf-8") as f:
             return "docker" in f.read()
     except Exception:
         return False
-
-
-def is_aws_lambda() -> bool:
-    "Return True if the process is running in the serverless platform AWS Lambda"
-    return os.environ.get("AWS_LAMBDA_FUNCTION_NAME") is not None
-
-
-def is_gcp_cloud_function() -> bool:
-    "Return True if the process is running in the serverless platform GCP Cloud Functions"
-    return os.environ.get("FUNCTION_NAME") is not None
```

### Comparing `dlt-0.3.5/dlt/common/runtime/init.py` & `dlt-0.3.5a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/logger.py` & `dlt-0.3.5a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/prometheus.py` & `dlt-0.3.5a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/segment.py` & `dlt-0.3.5a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/sentry.py` & `dlt-0.3.5a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/signals.py` & `dlt-0.3.5a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/slack.py` & `dlt-0.3.5a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/runtime/telemetry.py` & `dlt-0.3.5a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/schema/detections.py` & `dlt-0.3.5a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/schema/exceptions.py` & `dlt-0.3.5a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/schema/schema.py` & `dlt-0.3.5a0/dlt/common/schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,17 +261,17 @@
     def get_table_columns(self, table_name: str, only_complete: bool = False) -> TTableSchemaColumns:
         """Gets columns of `table_name`"""
         if only_complete:
             return {k:v for k, v in self._schema_tables[table_name]["columns"].items() if utils.is_complete_column(v)}
         else:
             return self._schema_tables[table_name]["columns"]
 
-    def data_tables(self, include_incomplete: bool = False) -> List[TTableSchema]:
+    def data_tables(self) -> List[TTableSchema]:
         """Gets list of all tables, that hold the loaded data. Excludes dlt tables. Excludes incomplete tables (ie. without columns)"""
-        return [t for t in self._schema_tables.values() if not t["name"].startswith("_dlt") and (len(t["columns"]) > 0 or include_incomplete)]
+        return [t for t in self._schema_tables.values() if not t["name"].startswith("_dlt") and len(t["columns"]) > 0]
 
     def dlt_tables(self) -> List[TTableSchema]:
         """Gets dlt tables"""
         return [t for t in self._schema_tables.values() if t["name"].startswith("_dlt")]
 
     def get_preferred_type(self, col_name: str) -> Optional[TDataType]:
         return next((m[1] for m in self._compiled_preferred_types if m[0].search(col_name)), None)
```

### Comparing `dlt-0.3.5/dlt/common/schema/typing.py` & `dlt-0.3.5a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/schema/utils.py` & `dlt-0.3.5a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/source.py` & `dlt-0.3.5a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/__init__.py` & `dlt-0.3.5a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/configuration.py` & `dlt-0.3.5a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/data_item_storage.py` & `dlt-0.3.5a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/exceptions.py` & `dlt-0.3.5a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/file_storage.py` & `dlt-0.3.5a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.5a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/load_storage.py` & `dlt-0.3.5a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/normalize_storage.py` & `dlt-0.3.5a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/schema_storage.py` & `dlt-0.3.5a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/transactional_file.py` & `dlt-0.3.5a0/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/storages/versioned_storage.py` & `dlt-0.3.5a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/time.py` & `dlt-0.3.5a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/typing.py` & `dlt-0.3.5a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/utils.py` & `dlt-0.3.5a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/validation.py` & `dlt-0.3.5a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/common/wei.py` & `dlt-0.3.5a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/bigquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast, Type, Any
+from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast, Type
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud import exceptions as gcp_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
 from dlt.common import json, logger
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob
@@ -15,17 +15,16 @@
 
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.destinations.exceptions import DestinationSchemaWillNotUpdate, DestinationTransientException, LoadJobNotExistsException, LoadJobTerminalException, LoadJobUnknownTableException
 
 from dlt.destinations.bigquery import capabilities
 from dlt.destinations.bigquery.configuration import BigQueryClientConfiguration
 from dlt.destinations.bigquery.sql_client import BigQuerySqlClient, BQ_TERMINAL_REASONS
-from dlt.destinations.sql_jobs import SqlMergeJob, SqlStagingCopyJob
+from dlt.destinations.sql_merge_job import SqlMergeJob
 from dlt.destinations.job_impl import NewReferenceJob
-from dlt.destinations.sql_client import SqlClientBase
 
 from dlt.common.schema.utils import table_schema_has_type
 
 SCT_TO_BQT: Dict[TDataType, str] = {
     "complex": "JSON",
     "text": "STRING",
     "double": "FLOAT64",
@@ -110,28 +109,14 @@
     def gen_key_table_clauses(cls, root_table_name: str, staging_root_table_name: str, key_clauses: Sequence[str], for_delete: bool) -> List[str]:
         # generate several clauses: BigQuery does not support OR nor unions
         sql: List[str] = []
         for clause in key_clauses:
             sql.append(f"FROM {root_table_name} AS d WHERE EXISTS (SELECT 1 FROM {staging_root_table_name} AS s WHERE {clause.format(d='d', s='s')})")
         return sql
 
-class BigqueryStagingCopyJob(SqlStagingCopyJob):
-
-    @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        sql: List[str] = []
-        for table in table_chain:
-            with sql_client.with_staging_dataset(staging=True):
-                staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            table_name = sql_client.make_qualified_table_name(table["name"])
-            # drop destination table
-            sql.append(f"DROP TABLE IF EXISTS {table_name};")
-            # recreate destination table with data cloned from staging table
-            sql.append(f"CREATE TABLE {table_name} CLONE {staging_table_name};")
-        return sql
 
 class BigQueryClient(SqlJobClientBase):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: BigQueryClientConfiguration) -> None:
         sql_client = BigQuerySqlClient(
@@ -141,20 +126,17 @@
             config.http_timeout,
             config.retry_deadline
         )
         super().__init__(schema, config, sql_client)
         self.config: BigQueryClientConfiguration = config
         self.sql_client: BigQuerySqlClient = sql_client  # type: ignore
 
-    def _create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return BigQueryMergeJob.from_table_chain(table_chain, self.sql_client)
 
-    def _create_optimized_replace_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
-        return BigqueryStagingCopyJob.from_table_chain(table_chain, self.sql_client)
-
     def restore_file_load(self, file_path: str) -> LoadJob:
         """Returns a completed SqlLoadJob or restored BigQueryLoadJob
 
         See base class for details on SqlLoadJob. BigQueryLoadJob is restored with job id derived from `file_path`
 
         Args:
             file_path (str): a path to a job file
@@ -182,18 +164,17 @@
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
             try:
-                disposition = table["write_disposition"]
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
-                    self._create_load_job(table, disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path),
+                    self._create_load_job(table, file_path),
                     self.config.http_timeout,
                     self.config.retry_deadline
                 )
             except api_core_exceptions.GoogleAPICallError as gace:
                 reason = BigQuerySqlClient._get_reason_from_errors(gace)
                 if reason == "notFound":
                     # google.api_core.exceptions.NotFound: 404 - table not found
@@ -252,18 +233,19 @@
                     "partition": c.name == partition_field
                 }
                 schema_table[c.name] = schema_c
             return True, schema_table
         except gcp_exceptions.NotFound:
             return False, schema_table
 
-    def _create_load_job(self, table: TTableSchema, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str) -> bigquery.LoadJob:
-        # append to table for merge loads (append to stage) and regular appends
-        bq_wd = bigquery.WriteDisposition.WRITE_TRUNCATE if _should_truncate_destination_table else bigquery.WriteDisposition.WRITE_APPEND
+    def _create_load_job(self, table: TTableSchema, file_path: str) -> bigquery.LoadJob:
         table_name = table["name"]
+        write_disposition = table["write_disposition"]
+        # append to table for merge loads (append to stage) and regular appends
+        bq_wd = bigquery.WriteDisposition.WRITE_TRUNCATE if write_disposition == "replace" else bigquery.WriteDisposition.WRITE_APPEND
 
         # determine wether we load from local or uri
         bucket_path = None
         ext: str = os.path.splitext(file_path)[1][1:]
         if NewReferenceJob.is_reference_job(file_path):
             bucket_path = NewReferenceJob.resolve_reference(file_path)
             ext = os.path.splitext(bucket_path)[1][1:]
@@ -276,15 +258,15 @@
             if table_schema_has_type(table, "complex"):
                 raise LoadJobTerminalException(file_path, "Bigquery cannot load into JSON data type from parquet. Use jsonl instead.")
             source_format = bigquery.SourceFormat.PARQUET
             # parquet needs NUMERIC type autodetection
             decimal_target_types = ["NUMERIC", "BIGNUMERIC"]
 
         # if merge then load to staging
-        with self.sql_client.with_staging_dataset(use_staging_table):
+        with self.sql_client.with_staging_dataset(write_disposition == "merge"):
             job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
             job_config = bigquery.LoadJobConfig(
                 autodetect=False,
                 write_disposition=bq_wd,
                 create_disposition=bigquery.CreateDisposition.CREATE_NEVER,
                 source_format=source_format,
                 decimal_target_types=decimal_target_types,
```

### Comparing `dlt-0.3.5/dlt/destinations/bigquery/configuration.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import warnings
 from typing import TYPE_CHECKING, ClassVar, List, Optional
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import GcpServiceAccountCredentials
-from dlt.common.utils import digest128
-
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
 
 
 @configspec(init=True)
 class BigQueryClientConfiguration(DestinationClientDwhConfiguration):
     destination_name: str = "bigquery"
     credentials: GcpServiceAccountCredentials = None
@@ -24,20 +22,14 @@
         if self.location != "US":
             return self.location
         # default was changed in credentials, emit deprecation message
         if self.credentials.location != "US":
             warnings.warn("Setting BigQuery location in the credentials is deprecated. Please set the location directly in bigquery section ie. destinations.bigquery.location='EU'")
         return self.credentials.location
 
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of project_id"""
-        if self.credentials and self.credentials.project_id:
-            return digest128(self.credentials.project_id)
-        return ""
-
     if TYPE_CHECKING:
         def __init__(
             self,
             destination_name: str = None,
             credentials: Optional[GcpServiceAccountCredentials] = None,
             dataset_name: str = None,
             default_schema_name: Optional[str] = None,
```

### Comparing `dlt-0.3.5/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     caps.naming_convention = "duck_case"
     caps.max_query_length = 32 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = True
     caps.alter_add_multi_column = False
-    caps.supports_truncate_command = False
 
     return caps
 
 
 def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
     # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
     from dlt.destinations.duckdb.duck import DuckDbClient
```

### Comparing `dlt-0.3.5/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/duckdb/duck.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/duck.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 
 HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {
     "unique": "UNIQUE"
 }
 
 
 class DuckDbCopyJob(LoadJob, FollowupJob):
-    def __init__(self, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str, sql_client: DuckDbSqlClient) -> None:
+    def __init__(self, table_name: str, write_disposition: TWriteDisposition, file_path: str, sql_client: DuckDbSqlClient) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
 
-        with sql_client.with_staging_dataset(use_staging_table):
+        with sql_client.with_staging_dataset(write_disposition=="merge"):
             qualified_table_name = sql_client.make_qualified_table_name(table_name)
             with sql_client.begin_transaction():
-                if _should_truncate_destination_table:
+                if write_disposition == "replace":
                     sql_client.execute_sql(f"TRUNCATE TABLE {qualified_table_name}")
                 sql_client.execute_sql(f"COPY {qualified_table_name} FROM '{file_path}' ( FORMAT PARQUET );")
 
 
     def state(self) -> TLoadJobState:
         return "completed"
 
@@ -73,16 +73,15 @@
         super().__init__(schema, config, sql_client)
         self.config: DuckDbClientConfiguration = config
         self.sql_client: DuckDbSqlClient = sql_client  # type: ignore
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         if file_path.endswith("parquet"):
-            disposition = table["write_disposition"]
-            return DuckDbCopyJob(table["name"], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path, self.sql_client)
+            return DuckDbCopyJob(table["name"], table["write_disposition"], file_path, self.sql_client)
         return super().start_file_load(table, file_path, load_id)
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
```

### Comparing `dlt-0.3.5/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/dummy/__init__.py` & `dlt-0.3.5a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/dummy/configuration.py` & `dlt-0.3.5a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/dummy/dummy.py` & `dlt-0.3.5a0/dlt/destinations/dummy/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 from copy import copy
 from types import TracebackType
-from typing import ClassVar, Dict, Optional, Sequence, Type, Iterable, List
+from typing import ClassVar, Dict, Optional, Sequence, Type, Iterable
 
 from dlt.common import pendulum
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
-from dlt.common.schema.typing import TWriteDisposition
 from dlt.common.storages import FileStorage
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob, JobClientBase
 
 from dlt.destinations.exceptions import (LoadJobNotExistsException, LoadJobInvalidStateTransitionException,
                                             DestinationTerminalException, DestinationTransientException)
 
@@ -74,22 +73,22 @@
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: DummyClientConfiguration) -> None:
         super().__init__(schema, config)
         self.config: DummyClientConfiguration = config
 
-    def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
+    def initialize_storage(self, staging: bool = False, truncate_tables: Iterable[str] = None) -> None:
         pass
 
-    def is_storage_initialized(self) -> bool:
+    def is_storage_initialized(self, staging: bool = False) -> bool:
         return True
 
-    def update_storage_schema(self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
-        applied_update = super().update_storage_schema(only_tables, expected_update)
+    def update_storage_schema(self, staging: bool = False, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
+        applied_update = super().update_storage_schema(staging, only_tables, expected_update)
         if self.config.fail_schema_update:
             raise DestinationTransientException("Raise on schema update due to fail_schema_update config flag")
         return applied_update
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job_id = FileStorage.get_file_name_from_file_path(file_path)
         file_name = FileStorage.get_file_name_from_file_path(file_path)
@@ -105,17 +104,16 @@
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         job_id = FileStorage.get_file_name_from_file_path(file_path)
         if job_id not in JOBS:
             raise LoadJobNotExistsException(job_id)
         return JOBS[job_id]
 
-    def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
-        """Creates a list of followup jobs that should be executed after a table chain is completed"""
-        return []
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+        return None
 
     def complete_load(self, load_id: str) -> None:
         pass
 
     def __enter__(self) -> "DummyClient":
         return self
```

### Comparing `dlt-0.3.5/dlt/destinations/exceptions.py` & `dlt-0.3.5a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from urllib.parse import urlparse
 
-from typing import Final, Type, Optional, Union, TYPE_CHECKING
+from typing import Final, Type, Optional, Union
 
 from dlt.common.configuration import configspec, resolve_type
 from dlt.common.destination.reference import CredentialsConfiguration, DestinationClientStagingConfiguration
-from dlt.common.configuration.specs import GcpServiceAccountCredentials, AwsCredentials, GcpOAuthCredentials
-from dlt.common.utils import digest128
+from dlt.common.configuration.specs import GcpCredentials, GcpServiceAccountCredentials, AwsCredentials, GcpOAuthCredentials
+
 from dlt.common.configuration.exceptions import ConfigurationValueError
 
 
 PROTOCOL_CREDENTIALS = {
     "gs": Union[GcpServiceAccountCredentials, GcpOAuthCredentials],
     "gcs": Union[GcpServiceAccountCredentials, GcpOAuthCredentials],
     "gdrive": GcpOAuthCredentials,
     "s3": AwsCredentials
 }
 
 
 @configspec(init=True)
 class FilesystemClientConfiguration(DestinationClientStagingConfiguration):
     destination_name: Final[str] = "filesystem"  # type: ignore
-    # should be an union of all possible credentials as found in PROTOCOL_CREDENTIALS
-    credentials: Union[AwsCredentials, GcpServiceAccountCredentials, GcpOAuthCredentials]
+    credentials: Union[AwsCredentials, GcpCredentials]
     bucket_url: str
 
     @property
     def protocol(self) -> str:
         url = urlparse(self.bucket_url)
         return url.scheme or "file"
 
@@ -40,34 +39,17 @@
             self.bucket_url = url.geturl()
 
     @resolve_type('credentials')
     def resolve_credentials_type(self) -> Type[CredentialsConfiguration]:
         # use known credentials or empty credentials for unknown protocol
         return PROTOCOL_CREDENTIALS.get(self.protocol) or Optional[CredentialsConfiguration]  # type: ignore[return-value]
 
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of bucket_url"""
-        if self.bucket_url:
-            return digest128(self.bucket_url)
-        return ""
-
     def __str__(self) -> str:
         """Return displayable destination location"""
         url = urlparse(self.bucket_url)
         # do not show passwords
         if url.password:
             new_netloc = f"{url.username}:****@{url.hostname}"
             if url.port:
                 new_netloc += f":{url.port}"
             return url._replace(netloc=new_netloc).geturl()
         return self.bucket_url
-
-    if TYPE_CHECKING:
-        def __init__(
-            self,
-            destination_name: str = None,
-            credentials: Optional[GcpServiceAccountCredentials] = None,
-            dataset_name: str = None,
-            default_schema_name: Optional[str] = None,
-            bucket_url: str = None
-        ) -> None:
-            ...
```

### Comparing `dlt-0.3.5/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,43 +30,36 @@
             has_merge_keys: bool,
             schema_name: str,
             load_id: str
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(local_path)
         self.config = config
         self.dataset_path = dataset_path
-        self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
 
         super().__init__(file_name)
         fs_client, _ = client_from_config(config)
 
         # fallback to replace for merge without any merge keys
         if write_disposition == 'merge':
             write_disposition = 'append' if has_merge_keys else 'replace'
 
         # replace existing files. also check if dir exists for bucket storages that cannot create dirs
         if write_disposition == 'replace' and fs_client.isdir(dataset_path):
             job_info = LoadStorage.parse_job_file_name(file_name)
-            # remove those files
             search_prefix = posixpath.join(dataset_path, f"{schema_name}.{job_info.table_name}.")
-            # but leave actual load id - files may be loaded from other threads
-            ignore_prefix = posixpath.join(dataset_path, f"{schema_name}.{job_info.table_name}.{load_id}.")
             # NOTE: glob implementation in fsspec does not look thread safe, way better is to use ls and then filter
             all_files: List[str] = fs_client.ls(dataset_path, detail=False, refresh=True)
-            items = [item for item in all_files if item.startswith(search_prefix) and not item.startswith(ignore_prefix)]
+            items = [item for item in all_files if item.startswith(search_prefix)]
             # NOTE: deleting in chunks on s3 does not raise on access denied, file non existing and probably other errors
             # if items:
             #     fs_client.rm(items[0])
             for item in items:
-                # ignore file not found as we can have races from other deleting threads
-                try:
-                    fs_client.rm_file(item)
-                except FileNotFoundError:
-                    pass
+                fs_client.rm_file(item)
 
+        self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
         fs_client.put_file(local_path, self.make_remote_path())
 
     @staticmethod
     def make_destination_filename(file_name: str, schema_name: str, load_id: str) -> str:
         job_info = LoadStorage.parse_job_file_name(file_name)
         return f"{schema_name}.{job_info.table_name}.{load_id}.{job_info.file_id}.{job_info.file_format}"
 
@@ -101,18 +94,18 @@
         self.fs_client, self.fs_path = client_from_config(config)
         self.config: FilesystemClientConfiguration = config
 
     @property
     def dataset_path(self) -> str:
         return posixpath.join(self.fs_path, self.config.dataset_name)
 
-    def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
+    def initialize_storage(self, staging: bool = False, truncate_tables: Iterable[str] = None) -> None:
         self.fs_client.makedirs(self.dataset_path, exist_ok=True)
 
-    def is_storage_initialized(self) -> bool:
+    def is_storage_initialized(self, staging: bool = False) -> bool:
         return self.fs_client.isdir(self.dataset_path)  # type: ignore[no-any-return]
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         cls = FollowupFilesystemJob if self.config.as_staging else LoadFilesystemJob
         has_merge_keys = any(col['merge_key'] or col['primary_key'] for col in table['columns'].values())
         return cls(
             file_path,
@@ -123,17 +116,17 @@
             schema_name=self.schema.name,
             load_id=load_id
         )
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
-    def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
-        """Creates a list of followup jobs that should be executed after a table chain is completed"""
-        return []
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+        return None
+
 
     def complete_load(self, load_id: str) -> None:
         schema_name = self.schema.name
         table_name = LOADS_TABLE_NAME
         file_name = f"{schema_name}.{table_name}.{load_id}"
         self.fs_client.touch(posixpath.join(self.dataset_path, file_name))
```

### Comparing `dlt-0.3.5/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/filesystem_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import cast, Tuple
 
 from fsspec.core import url_to_fs
 from fsspec import AbstractFileSystem
 
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import DictStrAny
-from dlt.common.configuration.specs import CredentialsWithDefault, GcpCredentials,  AwsCredentials
-
-from dlt.destinations.filesystem.configuration import FilesystemClientConfiguration
+from dlt.common.configuration.specs import CredentialsWithDefault
+from dlt.destinations.filesystem.configuration import FilesystemClientConfiguration, GcpCredentials, GcpServiceAccountCredentials,  AwsCredentials
 
 from dlt import version
 
 
 def client_from_config(config: FilesystemClientConfiguration) -> Tuple[AbstractFileSystem, str]:
     proto = config.protocol
     fs_kwargs: DictStrAny = {}
```

### Comparing `dlt-0.3.5/dlt/destinations/insert_job_client.py` & `dlt-0.3.5a0/dlt/destinations/insert_job_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.job_client_impl import SqlJobClientBase
 
 
 class InsertValuesLoadJob(LoadJob, FollowupJob):
-    def __init__(self, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str, sql_client: SqlClientBase[Any]) -> None:
+    def __init__(self, table_name: str, write_disposition: TWriteDisposition, file_path: str, sql_client: SqlClientBase[Any]) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
         self._sql_client = sql_client
         # insert file content immediately
-        with self._sql_client.with_staging_dataset(use_staging_table):
+        with self._sql_client.with_staging_dataset(write_disposition=="merge"):
             with self._sql_client.begin_transaction():
-                for fragments in self._insert(sql_client.make_qualified_table_name(table_name), _should_truncate_destination_table, file_path):
+                for fragments in self._insert(sql_client.make_qualified_table_name(table_name), write_disposition, file_path):
                     self._sql_client.execute_fragments(fragments)
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
 
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
-    def _insert(self, qualified_table_name: str, _should_truncate_destination_table: bool, file_path: str) -> Iterator[List[str]]:
+    def _insert(self, qualified_table_name: str, write_disposition: TWriteDisposition, file_path: str) -> Iterator[List[str]]:
         # WARNING: maximum redshift statement is 16MB https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-sql.html
         # the procedure below will split the inserts into max_query_length // 2 packs
         with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             header = f.readline()
             values_mark = f.readline()
             # properly formatted file has a values marker at the beginning
             assert values_mark == "VALUES\n"
 
             insert_sql = []
-            if _should_truncate_destination_table:
+            if write_disposition == "replace":
                 insert_sql.append("DELETE FROM {};".format(qualified_table_name))
             while content := f.read(self._sql_client.capabilities.max_query_length // 2):
                 # write INSERT
                 insert_sql.extend([header.format(qualified_table_name), values_mark, content])
                 # read one more line in order to
                 # 1. complete the content which ends at "random" position, not an end line
                 # 2. to modify its ending without a need to re-allocating the 8MB of "content"
@@ -88,16 +88,15 @@
             job = EmptyLoadJob.from_file_path(file_path, "completed")
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
         if not job:
             # this is using sql_client internally and will raise a right exception
-            disposition = table["write_disposition"]
-            job = InsertValuesLoadJob(table["name"], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path, self.sql_client)
+            job = InsertValuesLoadJob(table["name"], table["write_disposition"], file_path, self.sql_client)
         return job
 
     # TODO: implement indexes and primary keys for postgres
     def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
         # get primary key
         pass
```

### Comparing `dlt-0.3.5/dlt/destinations/job_client_impl.py` & `dlt-0.3.5a0/dlt/destinations/job_client_impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,79 +2,62 @@
 from abc import abstractmethod
 import base64
 import binascii
 import contextlib
 from copy import copy
 import datetime  # noqa: 251
 from types import TracebackType
-from typing import Any, ClassVar, List, NamedTuple, Optional, Sequence, Tuple, Type, Iterable, Iterator, ContextManager
+from typing import Any, ClassVar, List, NamedTuple, Optional, Sequence, Tuple, Type, Iterable, Iterator
 import zlib
-import re
 
 from dlt.common import json, pendulum, logger
 from dlt.common.data_types import TDataType
-from dlt.common.schema.typing import COLUMN_HINTS, LOADS_TABLE_NAME, VERSION_TABLE_NAME, TColumnSchemaBase, TTableSchema, TWriteDisposition
+from dlt.common.schema.typing import COLUMN_HINTS, LOADS_TABLE_NAME, VERSION_TABLE_NAME, TColumnSchemaBase, TTableSchema
 from dlt.common.schema.utils import add_missing_hints
 from dlt.common.storages import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns, TSchemaTables
-from dlt.common.destination.reference import DestinationClientConfiguration, DestinationClientDwhConfiguration, NewLoadJob, TLoadJobState, LoadJob, StagingJobClientBase, FollowupJob, DestinationClientStagingConfiguration, CredentialsConfiguration
+from dlt.common.destination.reference import DestinationClientConfiguration, DestinationClientDwhConfiguration, NewLoadJob, TLoadJobState, LoadJob, JobClientBase, FollowupJob, DestinationClientStagingConfiguration, CredentialsConfiguration
 from dlt.common.utils import concat_strings_with_limit
 from dlt.destinations.exceptions import DatabaseUndefinedRelation, DestinationSchemaWillNotUpdate
 from dlt.destinations.job_impl import EmptyLoadJobWithoutFollowup, NewReferenceJob
-from dlt.destinations.sql_jobs import SqlMergeJob, SqlStagingCopyJob
+from dlt.destinations.sql_merge_job import SqlMergeJob
 
 from dlt.destinations.typing import TNativeConn
 from dlt.destinations.sql_client import SqlClientBase
+from dlt.common.configuration import with_config, known_sections
 
 
 class StorageSchemaInfo(NamedTuple):
     version_hash: str
     schema_name: str
     version: int
     engine_version: str
     inserted_at: datetime.datetime
     schema: str
 
-# this should suffice for now
-DDL_COMMANDS = [
-    "ALTER",
-    "CREATE",
-    "DROP"
-]
 
 class SqlLoadJob(LoadJob):
     """A job executing sql statement, without followup trait"""
 
     def __init__(self, file_path: str, sql_client: SqlClientBase[Any]) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
         # execute immediately if client present
         with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             sql = f.read()
-
-        # if we detect ddl transactions, only execute transaction if supported by client
-        if not self._string_containts_ddl_queries(sql) or sql_client.capabilities.supports_ddl_transactions:
-            # with sql_client.begin_transaction():
-            sql_client.execute_sql(sql)
-        else:
+        with sql_client.begin_transaction():
             sql_client.execute_sql(sql)
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
 
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
-    def _string_containts_ddl_queries(self, sql: str) -> bool:
-        for cmd in DDL_COMMANDS:
-            if re.search(cmd, sql, re.IGNORECASE):
-                return True
-        return False
-
     @staticmethod
     def is_sql_job(file_path: str) -> bool:
         return os.path.splitext(file_path)[1][1:] == "sql"
 
 
 class CopyRemoteFileLoadJob(LoadJob, FollowupJob):
     def __init__(self, table: TTableSchema, file_path: str, sql_client: SqlClientBase[Any], staging_credentials: Optional[CredentialsConfiguration] = None) -> None:
@@ -89,105 +72,72 @@
         raise NotImplementedError()
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
 
 
-class SqlJobClientBase(StagingJobClientBase):
+class SqlJobClientBase(JobClientBase):
 
     VERSION_TABLE_SCHEMA_COLUMNS: ClassVar[str] = "version_hash, schema_name, version, engine_version, inserted_at, schema"
 
     def __init__(self, schema: Schema, config: DestinationClientConfiguration,  sql_client: SqlClientBase[TNativeConn]) -> None:
         super().__init__(schema, config)
         self.sql_client = sql_client
         assert isinstance(config, DestinationClientDwhConfiguration)
         self.config: DestinationClientDwhConfiguration = config
 
-    def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
-        if not self.is_storage_initialized():
-            self.sql_client.create_dataset()
-        else:
-            # truncate requested tables
-            if truncate_tables:
-                self.sql_client.truncate_tables(*truncate_tables)
-
-
-    def is_storage_initialized(self) -> bool:
-        return self.sql_client.has_dataset()
-
-    def update_storage_schema(self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
-        super().update_storage_schema(only_tables, expected_update)
-        applied_update: TSchemaTables = {}
-        schema_info = self.get_schema_by_hash(self.schema.stored_version_hash)
-        if schema_info is None:
-            logger.info(f"Schema with hash {self.schema.stored_version_hash} not found in the storage. upgrading")
+    def initialize_storage(self, staging: bool = False, truncate_tables: Iterable[str] = None) -> None:
+        # use regular or staging dataset name
+        with self.sql_client.with_staging_dataset(staging):
+            if not self.is_storage_initialized():
+                self.sql_client.create_dataset()
+            else:
+                # truncate requested tables
+                if truncate_tables:
+                    self.sql_client.truncate_tables(*truncate_tables)
+
+
+    def is_storage_initialized(self, staging: bool = False) -> bool:
+        with self.sql_client.with_staging_dataset(staging):
+            return self.sql_client.has_dataset()
+
+    def update_storage_schema(self, staging: bool = False, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
+        with self.sql_client.with_staging_dataset(staging):
+            super().update_storage_schema(staging, only_tables, expected_update)
+            applied_update: TSchemaTables = {}
+            schema_info = self.get_schema_by_hash(self.schema.stored_version_hash)
+            if schema_info is None:
+                logger.info(f"Schema with hash {self.schema.stored_version_hash} not found in the storage. upgrading")
 
-            with self.maybe_ddl_transaction():
-                applied_update = self._execute_schema_update_sql(only_tables)
-        else:
-            logger.info(f"Schema with hash {self.schema.stored_version_hash} inserted at {schema_info.inserted_at} found in storage, no upgrade required")
-        return applied_update
+                with self.maybe_ddl_transaction():
+                    applied_update = self._execute_schema_update_sql(only_tables)
+            else:
+                logger.info(f"Schema with hash {self.schema.stored_version_hash} inserted at {schema_info.inserted_at} found in storage, no upgrade required")
+            return applied_update
 
-    def drop_tables(self, *tables: str, replace_schema: bool = True) -> None:
+    def drop_tables(self, *tables: str, staging: bool = False, replace_schema: bool = True) -> None:
         with self.maybe_ddl_transaction():
-            self.sql_client.drop_tables(*tables)
-            if replace_schema:
-                self._replace_schema_in_storage(self.schema)
+            with self.sql_client.with_staging_dataset(staging):
+                self.sql_client.drop_tables(*tables)
+                if replace_schema:
+                    self._replace_schema_in_storage(self.schema)
 
     @contextlib.contextmanager
     def maybe_ddl_transaction(self) -> Iterator[None]:
         """Begins a transaction if sql client supports it, otherwise works in auto commit"""
         if self.capabilities.supports_ddl_transactions:
             with self.sql_client.begin_transaction():
                 yield
         else:
             yield
 
-    @contextlib.contextmanager
-    def with_staging_dataset(self)-> Iterator["SqlJobClientBase"]:
-        with self.sql_client.with_staging_dataset(True):
-            yield self
-
-    def get_stage_dispositions(self) -> List[TWriteDisposition]:
-        """Returns a list of dispositions that require staging tables to be populated"""
-        dispositions: List[TWriteDisposition] = ["merge"]
-        # if we have anything but the truncate-and-insert replace strategy, we need staging tables
-        if self.config.replace_strategy in ["insert-from-staging", "staging-optimized"]:
-            dispositions.append("replace")
-        return dispositions
-
-    def _should_truncate_destination_table(self, disposition: TWriteDisposition) -> bool:
-        return disposition == "replace" and self.config.replace_strategy == "truncate-and-insert"
-
-    def _create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlMergeJob.from_table_chain(table_chain, self.sql_client)
 
-    # update destination tables from staging tables
-    def _create_staging_copy_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
-        return SqlStagingCopyJob.from_table_chain(table_chain, self.sql_client)
-
-    # optimized replace strategy, defaults to _create_staging_copy_job for the basic client
-    # for some destinations there are much faster destination updates at the cost of
-    # dropping tables possible
-    def _create_optimized_replace_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
-        return self._create_staging_copy_job(table_chain)
-
-    def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
-        jobs = super().create_table_chain_completed_followup_jobs(table_chain)
-        """Creates a list of followup jobs that should be executed after a table chain is completed"""
-        write_disposition = table_chain[0]["write_disposition"]
-        if write_disposition == "merge":
-            jobs.append(self._create_merge_job(table_chain))
-        elif write_disposition == "replace" and self.config.replace_strategy == "insert-from-staging":
-            jobs.append(self._create_staging_copy_job(table_chain))
-        elif write_disposition == "replace" and self.config.replace_strategy == "staging-optimized":
-            jobs.append(self._create_optimized_replace_job(table_chain))
-        return jobs
-
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
         if SqlLoadJob.is_sql_job(file_path):
             # execute sql load job
             return SqlLoadJob(file_path, self.sql_client)
         return None
 
@@ -369,20 +319,19 @@
             with self.sql_client.execute_query(query, *args) as cur:
                 row = cur.fetchone()
         if not row:
             return None
 
         # get schema as string
         # TODO: Re-use decompress/compress_state() implementation from dlt.pipeline.state_sync
-        schema_str: str = row[5]
+        schema_str = row[5]
         try:
             schema_bytes = base64.b64decode(schema_str, validate=True)
             schema_str = zlib.decompress(schema_bytes).decode("utf-8")
-        except ValueError:
-            # not a base64 string
+        except binascii.Error:
             pass
 
         # make utc datetime
         inserted_at = pendulum.instance(row[4])
 
         return StorageSchemaInfo(row[0], row[1], row[2], row[3], inserted_at, schema_str)
```

### Comparing `dlt-0.3.5/dlt/destinations/job_impl.py` & `dlt-0.3.5a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/motherduck/__init__.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     caps.naming_convention = "duck_case"
     caps.max_query_length = 512 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = False
     caps.alter_add_multi_column = False
-    caps.supports_truncate_command = False
 
     return caps
 
 
 def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
     # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
     from dlt.destinations.motherduck.motherduck import MotherDuckClient
```

### Comparing `dlt-0.3.5/dlt/destinations/motherduck/configuration.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, ClassVar, Final, List
 
 from dlt.common.configuration import configspec
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
 from dlt.common.typing import TSecretValue
-from dlt.common.utils import digest128
 from dlt.common.configuration.exceptions import ConfigurationValueError
 
 from dlt.destinations.duckdb.configuration import DuckDbBaseCredentials
 
 MOTHERDUCK_DRIVERNAME = "md"
 
 
@@ -40,13 +39,7 @@
 
 @configspec(init=True)
 class MotherDuckClientConfiguration(DestinationClientDwhConfiguration):
     destination_name: Final[str] = "motherduck"  # type: ignore
     credentials: MotherDuckCredentials
 
     create_indexes: bool = False  # should unique indexes be created, this slows loading down massively
-
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of user access token"""
-        if self.credentials and self.credentials.password:
-            return digest128(self.credentials.password)
-        return ""
```

### Comparing `dlt-0.3.5/dlt/destinations/motherduck/motherduck.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/motherduck/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/postgres/__init__.py` & `dlt-0.3.5a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/postgres/configuration.py` & `dlt-0.3.5a0/dlt/destinations/postgres/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Final, ClassVar, Any, List
 from sqlalchemy.engine import URL
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ConnectionStringCredentials
-from dlt.common.utils import digest128
-from dlt.common.typing import TSecretValue
-
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
+from dlt.common.typing import TSecretValue
 
 
 @configspec
 class PostgresCredentials(ConnectionStringCredentials):
     drivername: Final[str] = "postgresql"  # type: ignore
     password: TSecretValue
     host: str
@@ -36,13 +34,7 @@
 
 @configspec(init=True)
 class PostgresClientConfiguration(DestinationClientDwhConfiguration):
     destination_name: Final[str] = "postgres"  # type: ignore
     credentials: PostgresCredentials
 
     create_indexes: bool = True
-
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of host part of a connection string"""
-        if self.credentials and self.credentials.host:
-            return digest128(self.credentials.host)
-        return ""
```

### Comparing `dlt-0.3.5/dlt/destinations/postgres/postgres.py` & `dlt-0.3.5a0/dlt/destinations/postgres/postgres.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,31 +5,26 @@
     import psycopg2cffi as psycopg2
     from psycopg2cffi.sql import SQL, Composed
 else:
     import psycopg2
     from psycopg2.sql import SQL, Composed
 
 
-from typing import ClassVar, Dict, Optional, Sequence, List, Any
+from typing import ClassVar, Dict, Optional
 
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
-from dlt.common.destination.reference import NewLoadJob
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
-from dlt.common.schema.typing import TTableSchema
-
-from dlt.destinations.sql_jobs import SqlStagingCopyJob
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
 
 from dlt.destinations.postgres import capabilities
 from dlt.destinations.postgres.sql_client import Psycopg2SqlClient
 from dlt.destinations.postgres.configuration import PostgresClientConfiguration
-from dlt.destinations.sql_client import SqlClientBase
 
 
 SCT_TO_PGT: Dict[TDataType, str] = {
     "complex": "jsonb",
     "text": "varchar",
     "double": "double precision",
     "bool": "boolean",
@@ -52,31 +47,14 @@
     "numeric": "decimal"
 }
 
 HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {
     "unique": "UNIQUE"
 }
 
-class PostgresStagingCopyJob(SqlStagingCopyJob):
-
-    @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        sql: List[str] = []
-        for table in table_chain:
-            with sql_client.with_staging_dataset(staging=True):
-                staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            table_name = sql_client.make_qualified_table_name(table["name"])
-            # drop destination table
-            sql.append(f"DROP TABLE IF EXISTS {table_name};")
-            # moving staging table to destination schema
-            sql.append(f"ALTER TABLE {staging_table_name} SET SCHEMA {sql_client.fully_qualified_dataset_name()};")
-            # recreate staging table
-            sql.append(f"CREATE TABLE {staging_table_name} (like {table_name} including all);")
-        return sql
-
 class PostgresClient(InsertValuesJobClient):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: PostgresClientConfiguration) -> None:
         sql_client = Psycopg2SqlClient(
             self.make_dataset_name(schema, config.dataset_name, config.default_schema_name),
@@ -88,17 +66,14 @@
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
-    def _create_optimized_replace_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
-        return PostgresStagingCopyJob.from_table_chain(table_chain, self.sql_client)
-
     @classmethod
     def _to_db_type(cls, sc_t: TDataType) -> str:
         if sc_t == "wei":
             return SCT_TO_PGT["decimal"] % cls.capabilities.wei_precision
         if sc_t == "decimal":
             return SCT_TO_PGT["decimal"] % cls.capabilities.decimal_precision
 
@@ -108,8 +83,7 @@
 
     @classmethod
     def _from_db_type(cls, pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         if pq_t == "numeric":
             if (precision, scale) == cls.capabilities.wei_precision:
                 return "wei"
         return PGT_TO_SCT.get(pq_t, "text")
-
```

### Comparing `dlt-0.3.5/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/redshift/README.md` & `dlt-0.3.5a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/redshift/__init__.py` & `dlt-0.3.5a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/redshift/configuration.py` & `dlt-0.3.5a0/dlt/destinations/redshift/configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Final, Optional
 
 from dlt.common.typing import TSecretValue
 from dlt.common.configuration import configspec
-from dlt.common.utils import digest128
 
 from dlt.destinations.postgres.configuration import PostgresCredentials, PostgresClientConfiguration
 
 
 @configspec
 class RedshiftCredentials(PostgresCredentials):
     port: int = 5439
@@ -16,13 +15,7 @@
 
 
 @configspec(init=True)
 class RedshiftClientConfiguration(PostgresClientConfiguration):
     destination_name: Final[str] = "redshift"  # type: ignore
     credentials: RedshiftCredentials
     staging_iam_role: Optional[str] = None
-
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of host part of a connection string"""
-        if self.credentials and self.credentials.host:
-            return digest128(self.credentials.host)
-        return ""
```

### Comparing `dlt-0.3.5/dlt/destinations/redshift/redshift.py` & `dlt-0.3.5a0/dlt/destinations/redshift/redshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dlt.common.destination.reference import NewLoadJob, CredentialsConfiguration
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 from dlt.common.schema.typing import TTableSchema
 from dlt.common.configuration.specs import AwsCredentialsWithoutDefaults
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
-from dlt.destinations.sql_jobs import SqlMergeJob, SqlStagingCopyJob
+from dlt.destinations.sql_merge_job import SqlMergeJob
 from dlt.destinations.exceptions import DatabaseTerminalException, LoadJobTerminalException
 from dlt.destinations.job_client_impl import CopyRemoteFileLoadJob, LoadJob
 
 from dlt.destinations.redshift import capabilities
 from dlt.destinations.redshift.configuration import RedshiftClientConfiguration
 from dlt.destinations.job_impl import NewReferenceJob
 from dlt.destinations.sql_client import SqlClientBase
@@ -77,24 +77,16 @@
             return DatabaseTerminalException(pg_ex)
         if "Precision exceeds maximum" in pg_ex.pgerror:
             return DatabaseTerminalException(pg_ex)
         return None
 
 class RedshiftCopyFileLoadJob(CopyRemoteFileLoadJob):
 
-    def __init__(self, table: TTableSchema,
-                 file_path: str,
-                 sql_client: SqlClientBase[Any],
-                 use_staging_table: bool,
-                 should_truncate_destination_table: bool,
-                 staging_credentials: Optional[CredentialsConfiguration] = None,
-                 staging_iam_role: str = None) -> None:
+    def __init__(self, table: TTableSchema, file_path: str, sql_client: SqlClientBase[Any], staging_credentials: Optional[CredentialsConfiguration] = None, staging_iam_role: str = None) -> None:
         self._staging_iam_role = staging_iam_role
-        self._use_staging_table = use_staging_table
-        self._should_truncate_destination_table = should_truncate_destination_table
         super().__init__(table, file_path, sql_client, staging_credentials)
 
     def execute(self, table: TTableSchema, bucket_path: str) -> None:
 
         # we assume s3 credentials where provided for the staging
         credentials = ""
         if self._staging_iam_role:
@@ -121,31 +113,28 @@
             # if table contains complex types then SUPER field will be used.
             # https://docs.aws.amazon.com/redshift/latest/dg/ingest-super.html
             if table_schema_has_type(table, "complex"):
                 file_type += " SERIALIZETOJSON"
         else:
             raise ValueError(f"Unsupported file type {ext} for Redshift.")
 
-        with self._sql_client.with_staging_dataset(self._use_staging_table):
+        with self._sql_client.with_staging_dataset(table["write_disposition"]=="merge"):
             with self._sql_client.begin_transaction():
-                dataset_name = self._sql_client.dataset_name
-                if self._should_truncate_destination_table:
+                if table["write_disposition"]=="replace":
                     self._sql_client.execute_sql(f"""TRUNCATE TABLE {table_name}""")
+                dataset_name = self._sql_client.dataset_name
                 # TODO: if we ever support csv here remember to add column names to COPY
                 self._sql_client.execute_sql(f"""
                     COPY {dataset_name}.{table_name}
                     FROM '{bucket_path}'
                     {file_type}
                     {dateformat}
                     {compression}
                     {credentials} MAXERROR 0;""")
 
-
-
-
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
 class RedshiftMergeJob(SqlMergeJob):
 
     @classmethod
@@ -168,27 +157,26 @@
             self.make_dataset_name(schema, config.dataset_name, config.default_schema_name),
             config.credentials
         )
         super().__init__(schema, config, sql_client)
         self.sql_client = sql_client
         self.config: RedshiftClientConfiguration = config
 
-    def _create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
+    def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return RedshiftMergeJob.from_table_chain(table_chain, self.sql_client)
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(HINT_TO_REDSHIFT_ATTR.get(h, "") for h in HINT_TO_REDSHIFT_ATTR.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
         if NewReferenceJob.is_reference_job(file_path):
-            disposition = table["write_disposition"]
-            return RedshiftCopyFileLoadJob(table, file_path, self.sql_client, disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), staging_credentials=self.config.staging_credentials, staging_iam_role=self.config.staging_iam_role)
+            return RedshiftCopyFileLoadJob(table, file_path, self.sql_client, staging_credentials=self.config.staging_credentials, staging_iam_role=self.config.staging_iam_role)
         return super().start_file_load(table, file_path, load_id)
 
     @classmethod
     def _to_db_type(cls, sc_t: TDataType) -> str:
         if sc_t == "wei":
             return SCT_TO_PGT["decimal"] % cls.capabilities.wei_precision
         if sc_t == "decimal":
```

### Comparing `dlt-0.3.5/dlt/destinations/snowflake/__init__.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/snowflake/configuration.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from dlt import version
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import TSecretStrValue
 from dlt.common.configuration.specs import ConnectionStringCredentials
 from dlt.common.configuration.exceptions import ConfigurationValueError
 from dlt.common.configuration import configspec
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
-from dlt.common.utils import digest128
 
 
 def _read_private_key(private_key: str, password: Optional[str] = None) -> bytes:
     """Load an encrypted or unencrypted private key from string.
     """
     try:
         from cryptography.hazmat.backends import default_backend
@@ -87,14 +86,8 @@
 class SnowflakeClientConfiguration(DestinationClientDwhConfiguration):
     destination_name: Final[str] = "snowflake"  # type: ignore[misc]
     credentials: SnowflakeCredentials
 
     stage_name: Optional[str] = None
     """Use an existing named stage instead of the default. Default uses the implicit table stage per table"""
     keep_staged_files: bool = True
-    """Whether to keep or delete the staged files after COPY INTO succeeds"""
-
-    def fingerprint(self) -> str:
-        """Returns a fingerprint of host part of a connection string"""
-        if self.credentials and self.credentials.host:
-            return digest128(self.credentials.host)
-        return ""
+    """Whether to keep or delete the staged files after COPY INTO succeeds"""
```

### Comparing `dlt-0.3.5/dlt/destinations/snowflake/snowflake.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/snowflake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, Any
+from typing import ClassVar, Dict, Optional, Sequence, Tuple, List
 from urllib.parse import urlparse
 
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob, CredentialsConfiguration
+from dlt.common.destination.reference import FollowupJob, TLoadJobState, LoadJob, CredentialsConfiguration
 from dlt.common.configuration.specs import AwsCredentialsWithoutDefaults
 from dlt.common.data_types import TDataType
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
 
 
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.exceptions import LoadJobTerminalException
 
 from dlt.destinations.snowflake import capabilities
 from dlt.destinations.snowflake.configuration import SnowflakeClientConfiguration
 from dlt.destinations.snowflake.sql_client import SnowflakeSqlClient
-from dlt.destinations.sql_jobs import SqlStagingCopyJob
 from dlt.destinations.snowflake.sql_client import SnowflakeSqlClient
 from dlt.destinations.job_impl import NewReferenceJob
-from dlt.destinations.sql_client import SqlClientBase
 
 BIGINT_PRECISION = 19
 MAX_NUMERIC_PRECISION = 38
 
 
 SCT_TO_SNOW: Dict[TDataType, str] = {
     "complex": "VARIANT",
@@ -48,21 +46,21 @@
     "BINARY": "binary",
     "VARIANT": "complex"
 }
 
 
 class SnowflakeLoadJob(LoadJob, FollowupJob):
     def __init__(
-            self, file_path: str, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, load_id: str, client: SnowflakeSqlClient,
+            self, file_path: str, table_name: str, write_disposition: TWriteDisposition, load_id: str, client: SnowflakeSqlClient,
             stage_name: Optional[str] = None, keep_staged_files: bool = True, staging_credentials: Optional[CredentialsConfiguration] = None
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(file_path)
         super().__init__(file_name)
 
-        with client.with_staging_dataset(use_staging_table):
+        with client.with_staging_dataset(write_disposition == "merge"):
             qualified_table_name = client.make_qualified_table_name(table_name)
 
             # extract and prepare some vars
             bucket_path = NewReferenceJob.resolve_reference(file_path) if NewReferenceJob.is_reference_job(file_path) else ""
             file_name = FileStorage.get_file_name_from_file_path(bucket_path) if bucket_path else file_name
             from_clause = ""
             credentials_clause = ""
@@ -71,16 +69,14 @@
 
             if bucket_path:
                 # s3 credentials case
                 if bucket_path.startswith("s3://") and staging_credentials and isinstance(staging_credentials, AwsCredentialsWithoutDefaults):
                     credentials_clause = f"""CREDENTIALS=(AWS_KEY_ID='{staging_credentials.aws_access_key_id}' AWS_SECRET_KEY='{staging_credentials.aws_secret_access_key}')"""
                     from_clause = f"FROM '{bucket_path}'"
                 else:
-                    # ensure that gcs bucket path starts with gcs://, this is a requirement of snowflake
-                    bucket_path = bucket_path.replace("gs://", "gcs://")
                     if not stage_name:
                         # when loading from bucket stage must be given
                         raise LoadJobTerminalException(file_path, f"Cannot load from bucket path {bucket_path} without a stage name. See https://dlthub.com/docs/dlt-ecosystem/destinations/snowflake for instructions on setting up the `stage_name`")
                     from_clause = f"FROM @{stage_name}/"
                     files_clause = f"FILES = ('{urlparse(bucket_path).path.lstrip('/')}')"
             else:
                 # this means we have a local file
@@ -92,15 +88,15 @@
 
             # decide on source format, stage_file_path will either be a local file or a bucket path
             source_format = "( TYPE = 'JSON', BINARY_FORMAT = 'BASE64' )"
             if file_name.endswith("parquet"):
                 source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE)"
 
             with client.begin_transaction():
-                if _should_truncate_destination_table:
+                if write_disposition == "replace":
                     client.execute_sql(f"TRUNCATE TABLE IF EXISTS {qualified_table_name}")
                 # PUT and COPY in one tx if local file, otherwise only copy
                 if not bucket_path:
                     client.execute_sql(f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE, AUTO_COMPRESS = FALSE')
                 client.execute_sql(
                     f"""COPY INTO {qualified_table_name}
                     {from_clause}
@@ -116,29 +112,14 @@
 
     def state(self) -> TLoadJobState:
         return "completed"
 
     def exception(self) -> str:
         raise NotImplementedError()
 
-class SnowflakeStagingCopyJob(SqlStagingCopyJob):
-
-    @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        sql: List[str] = []
-        for table in table_chain:
-            with sql_client.with_staging_dataset(staging=True):
-                staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            table_name = sql_client.make_qualified_table_name(table["name"])
-            # drop destination table
-            sql.append(f"DROP TABLE IF EXISTS {table_name};")
-            # recreate destination table with data cloned from staging table
-            sql.append(f"CREATE TABLE {table_name} CLONE {staging_table_name};")
-        return sql
-
 
 class SnowflakeClient(SqlJobClientBase):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: SnowflakeClientConfiguration) -> None:
         sql_client = SnowflakeSqlClient(
@@ -149,32 +130,28 @@
         self.config: SnowflakeClientConfiguration = config
         self.sql_client: SnowflakeSqlClient = sql_client  # type: ignore
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
-            disposition = table['write_disposition']
             job = SnowflakeLoadJob(
-                file_path, table['name'], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), load_id, self.sql_client,
+                file_path, table['name'], table['write_disposition'], load_id, self.sql_client,
                 stage_name=self.config.stage_name, keep_staged_files=self.config.keep_staged_files,
                 staging_credentials=self.config.staging_credentials
             )
         return job
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
     def _make_add_column_sql(self, new_columns: Sequence[TColumnSchema]) -> List[str]:
         # Override because snowflake requires multiple columns in a single ADD COLUMN clause
         return ["ADD COLUMN\n" + ",\n".join(self._get_column_def_sql(c) for c in new_columns)]
 
-    def _create_optimized_replace_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
-        return SnowflakeStagingCopyJob.from_table_chain(table_chain, self.sql_client)
-
     def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool, separate_alters: bool = False) -> List[str]:
         sql = super()._get_table_update_sql(table_name, new_columns, generate_alter)
 
         cluster_list = [self.capabilities.escape_identifier(c['name']) for c in new_columns if c.get('cluster')]
 
         if cluster_list:
             sql[0] = sql[0] + "\nCLUSTER BY (" + ",".join(cluster_list) + ")"
```

### Comparing `dlt-0.3.5/dlt/destinations/snowflake/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/destinations/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,22 +142,14 @@
         mro = type.mro(type(ex))
         return any(t.__name__ in ("DatabaseError", "DataError") for t in mro)
 
     @staticmethod
     def make_staging_dataset_name(dataset_name: str) -> str:
         return dataset_name + "_staging"
 
-    #
-    # generate sql statements
-    #
-    def truncate_table_sql(self, table_name: str) -> str:
-        if self.capabilities.supports_truncate_command:
-            return f"TRUNCATE TABLE {table_name};"
-        else:
-            return f"DELETE FROM {table_name};"
 
 
 class DBApiCursorImpl(DBApiCursor):
     """A DBApi Cursor wrapper with dataframes reading functionality"""
     def __init__(self, curr: DBApiCursor) -> None:
         self.native_cursor = curr
```

### Comparing `dlt-0.3.5/dlt/destinations/sql_jobs.py` & `dlt-0.3.5a0/dlt/destinations/sql_merge_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,79 +8,45 @@
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
 from dlt.common.utils import uniq_id
 from dlt.destinations.exceptions import MergeDispositionException
 from dlt.destinations.job_impl import NewLoadJobImpl
 from dlt.destinations.sql_client import SqlClientBase
 
 
-class SqlBaseJob(NewLoadJobImpl):
-    """Sql base job for jobs that rely on the whole tablechain"""
-    failed_text: str = ""
+
+class SqlMergeJob(NewLoadJobImpl):
 
     @classmethod
     def from_table_chain(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> NewLoadJobImpl:
-        """Generates a list of sql statements, that will be executed by the sql client when the job is executed in the loader.
+        """Generates a list of sql statements that merge the data in staging dataset with the data in destination dataset.
 
         The `table_chain` contains a list schemas of a tables with parent-child relationship, ordered by the ancestry (the root of the tree is first on the list).
-        """
+        The root table is merged using primary_key and merge_key hints which can be compound and be both specified. In that case the OR clause is generated.
+        The child tables are merged based on propagated `root_key` which is a type of foreign key but always leading to a root table.
 
+        First we store the root_keys of root table elements to be deleted in the temp table. Then we use the temp table to delete records from root and all child tables in the destination dataset.
+        At the end we copy the data from the staging dataset into destination dataset.
+        """
         top_table = table_chain[0]
         file_info = ParsedLoadJobFileName(top_table["name"], uniq_id()[:10], 0, "sql")
         try:
             # Remove line breaks from multiline statements and write one SQL statement per line in output file
             # to support clients that need to execute one statement at a time (i.e. snowflake)
-            sql = [' '.join(stmt.splitlines()) for stmt in cls.generate_sql(table_chain, sql_client)]
+            sql = [' '.join(stmt.splitlines()) for stmt in cls.gen_merge_sql(table_chain, sql_client)]
             job = cls(file_info.job_id(), "running")
             job._save_text_file("\n".join(sql))
         except Exception:
             # return failed job
+            failed_text = "Tried to generate a merge sql job for the following tables:"
             tables_str = yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False)
             job = cls(file_info.job_id(), "failed", pretty_format_exception())
-            job._save_text_file("\n".join([cls.failed_text, tables_str]))
+            job._save_text_file("\n".join([failed_text, tables_str]))
         return job
 
     @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        pass
-
-
-class SqlStagingCopyJob(SqlBaseJob):
-    """Generates a list of sql statements that copy the data from staging dataset into destination dataset."""
-    failed_text: str = "Tried to generate a staging copy sql job for the following tables:"
-
-    @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        sql: List[str] = []
-        for table in table_chain:
-            with sql_client.with_staging_dataset(staging=True):
-                staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            table_name = sql_client.make_qualified_table_name(table["name"])
-            columns = ", ".join(map(sql_client.capabilities.escape_identifier, table["columns"].keys()))
-            sql.append(sql_client.truncate_table_sql(table_name))
-            sql.append(f"INSERT INTO {table_name}({columns}) SELECT {columns} FROM {staging_table_name};")
-        return sql
-
-class SqlMergeJob(SqlBaseJob):
-    """Generates a list of sql statements that merge the data from staging dataset into destination dataset."""
-    failed_text: str = "Tried to generate a merge sql job for the following tables:"
-
-    @classmethod
-    def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
-        """Generates a list of sql statements that merge the data in staging dataset with the data in destination dataset.
-
-        The `table_chain` contains a list schemas of a tables with parent-child relationship, ordered by the ancestry (the root of the tree is first on the list).
-        The root table is merged using primary_key and merge_key hints which can be compound and be both specified. In that case the OR clause is generated.
-        The child tables are merged based on propagated `root_key` which is a type of foreign key but always leading to a root table.
-
-        First we store the root_keys of root table elements to be deleted in the temp table. Then we use the temp table to delete records from root and all child tables in the destination dataset.
-        At the end we copy the data from the staging dataset into destination dataset.
-        """
-        return cls.gen_merge_sql(table_chain, sql_client)
-
-    @classmethod
     def _gen_key_table_clauses(cls, primary_keys: Sequence[str], merge_keys: Sequence[str])-> List[str]:
         """Generate sql clauses to select rows to delete via merge and primary key. Return select all clause if no keys defined."""
         clauses: List[str] = []
         if primary_keys or merge_keys:
             if primary_keys:
                 clauses.append(" AND ".join(["%s.%s = %s.%s" % ("{d}", c, "{s}", c) for c in primary_keys]))
             if merge_keys:
@@ -134,15 +100,14 @@
         merge_keys = list(map(sql_client.capabilities.escape_identifier, get_columns_names_with_prop(root_table, "merge_key")))
         key_clauses = cls._gen_key_table_clauses(primary_keys, merge_keys)
 
         unique_column: str = None
         root_key_column: str = None
         insert_temp_table_sql: str = None
 
-
         if len(table_chain) == 1:
             key_table_clauses = cls.gen_key_table_clauses(root_table_name, staging_root_table_name, key_clauses, for_delete=True)
             # if no child tables, just delete data from top table
             for clause in key_table_clauses:
                 sql.append(f"DELETE {clause};")
         else:
             key_table_clauses = cls.gen_key_table_clauses(root_table_name, staging_root_table_name, key_clauses, for_delete=False)
```

### Comparing `dlt-0.3.5/dlt/destinations/typing.py` & `dlt-0.3.5a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/decorators.py` & `dlt-0.3.5a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/exceptions.py` & `dlt-0.3.5a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/extract.py` & `dlt-0.3.5a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/incremental.py` & `dlt-0.3.5a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/pipe.py` & `dlt-0.3.5a0/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/schema.py` & `dlt-0.3.5a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/source.py` & `dlt-0.3.5a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/typing.py` & `dlt-0.3.5a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/extract/utils.py` & `dlt-0.3.5a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/airflow_helper.py` & `dlt-0.3.5a0/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/__init__.py` & `dlt-0.3.5a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/configuration.py` & `dlt-0.3.5a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.5a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.5a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.5a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/dbt/runner.py` & `dlt-0.3.5a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/pandas_helper.py` & `dlt-0.3.5a0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/helpers/streamlit_helper.py` & `dlt-0.3.5a0/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/load/configuration.py` & `dlt-0.3.5a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/load/exceptions.py` & `dlt-0.3.5a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/load/load.py` & `dlt-0.3.5a0/dlt/load/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from dlt.common.runners import TRunMetrics, Runnable, workermethod
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.runtime.logger import pretty_format_exception
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import VERSION_TABLE_NAME, TTableSchema, TWriteDisposition
 from dlt.common.storages import LoadStorage
-from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, StagingJobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration, DestinationClientStagingConfiguration
+from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration, DestinationClientStagingConfiguration
 from dlt.destinations.filesystem.filesystem import LoadFilesystemJob
 
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.exceptions import DestinationTerminalException, DestinationTransientException, LoadJobUnknownTableException
 
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load.exceptions import LoadClientJobFailed, LoadClientJobRetry, LoadClientUnsupportedWriteDisposition, LoadClientUnsupportedFileFormats
@@ -148,19 +148,19 @@
             except (DestinationTransientException, Exception):
                 # raise on all temporary exceptions, typically network / server problems
                 raise
             jobs.append(job)
 
         return len(jobs), jobs
 
-    def get_new_jobs_info(self, load_id: str, schema: Schema, dispositions: List[TWriteDisposition] = None) -> List[ParsedLoadJobFileName]:
+    def get_new_jobs_info(self, load_id: str, schema: Schema, disposition: TWriteDisposition = None) -> List[ParsedLoadJobFileName]:
         jobs_info: List[ParsedLoadJobFileName] = []
         new_job_files = self.load_storage.list_new_jobs(load_id)
         for job_file in new_job_files:
-            if not dispositions or self.get_load_table(schema, job_file)["write_disposition"] in dispositions:
+            if not disposition or self.get_load_table(schema, job_file)["write_disposition"] == disposition:
                 jobs_info.append(LoadStorage.parse_job_file_name(job_file))
         return jobs_info
 
     def get_completed_table_chain(self, load_id: str, schema: Schema, top_merged_table: TTableSchema, starting_job_id: str) -> List[TTableSchema]:
         """Gets a table chain starting from the `top_merged_table` containing only tables with completed/failed jobs. None is returned if there's any job that is not completed"""
         # returns ordered list of tables from parent to child leaf tables
         table_chain: List[TTableSchema] = []
@@ -181,20 +181,20 @@
 
     def create_followup_jobs(self, load_id: str, state: TLoadJobState, starting_job: LoadJob, schema: Schema) -> List[NewLoadJob]:
         jobs: List[NewLoadJob] = []
         if isinstance(starting_job, FollowupJob):
             # check for merge jobs only for non-staging jobs. we may move that logic to the interface
             starting_job_file_name = starting_job.file_name()
             if state == "completed" and not self.is_staging_job(starting_job_file_name):
-                client = self.destination.client(schema, self.initial_client_config)
                 top_job_table = get_top_level_table(schema.tables, self.get_load_table(schema, starting_job_file_name)["name"])
-                # if all tables of chain completed, create follow  up jobs
-                if table_chain := self.get_completed_table_chain(load_id, schema, top_job_table, starting_job.job_file_info().job_id()):
-                    if follow_up_jobs := client.create_table_chain_completed_followup_jobs(table_chain):
-                        jobs = jobs + follow_up_jobs
+                if top_job_table["write_disposition"] == "merge":
+                    # if all tables completed, create merge sql job on destination client
+                    if table_chain := self.get_completed_table_chain(load_id, schema, top_job_table, starting_job.job_file_info().job_id()):
+                        if job := self.destination.client(schema, self.initial_client_config).create_merge_job(table_chain):
+                            jobs.append(job)
             jobs = jobs + starting_job.create_followup_jobs(state)
         return jobs
 
     def complete_jobs(self, load_id: str, jobs: List[LoadJob], schema: Schema) -> List[LoadJob]:
         remaining_jobs: List[LoadJob] = []
         logger.info(f"Will complete {len(jobs)} for {load_id}")
         for ii in range(len(jobs)):
@@ -263,25 +263,24 @@
                 job_client.initialize_storage()
                 logger.info(f"Client for {job_client.config.destination_name} will update schema to package schema")
                 all_jobs = self.get_new_jobs_info(load_id, schema)
                 all_tables = set(job.table_name for job in all_jobs)
                 dlt_tables = set(t["name"] for t in schema.dlt_tables())
                 # only update tables that are present in the load package
                 applied_update = job_client.update_storage_schema(only_tables=all_tables | dlt_tables, expected_update=expected_update)
-                # update the staging dataset if client supports this
-                if isinstance(job_client, StagingJobClientBase):
-                    if staging_table_jobs := self.get_new_jobs_info(load_id, schema, job_client.get_stage_dispositions()):
-                        with job_client.with_staging_dataset():
-                            logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
-                            job_client.initialize_storage()
-                            logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
-                            staging_tables = set(job.table_name for job in staging_table_jobs)
-                            job_client.update_storage_schema(only_tables=staging_tables | {VERSION_TABLE_NAME}, expected_update=expected_update)
-                            logger.info(f"Client for {job_client.config.destination_name} will TRUNCATE STAGING TABLES: {staging_tables}")
-                            job_client.initialize_storage(truncate_tables=staging_tables)
+                # update the staging dataset
+                merge_jobs = self.get_new_jobs_info(load_id, schema, "merge")
+                if merge_jobs:
+                    logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
+                    job_client.initialize_storage(staging=True)
+                    logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
+                    merge_tables = set(job.table_name for job in merge_jobs)
+                    job_client.update_storage_schema(staging=True, only_tables=merge_tables | {VERSION_TABLE_NAME}, expected_update=expected_update)
+                    logger.info(f"Client for {job_client.config.destination_name} will TRUNCATE STAGING TABLES: {merge_tables}")
+                    job_client.initialize_storage(staging=True, truncate_tables=merge_tables)
                 self.load_storage.commit_schema_update(load_id, applied_update)
             # spool or retrieve unfinished jobs
             if self.staging:
                 with self.get_staging_client(schema) as staging_client:
                     jobs_count, jobs = self.retrieve_jobs(job_client, load_id, staging_client)
             else:
                 jobs_count, jobs = self.retrieve_jobs(job_client, load_id)
@@ -370,14 +369,13 @@
 
         return LoadInfo(
             pipeline,
             self.initial_client_config.destination_name,
             str(self.initial_client_config),
             self.initial_staging_client_config.destination_name if self.initial_staging_client_config else None,
             str(self.initial_staging_client_config) if self.initial_staging_client_config else None,
-            self.initial_client_config.fingerprint(),
             dataset_name,
             list(load_ids),
             load_packages,
             started_at,
             pipeline.first_run
         )
```

### Comparing `dlt-0.3.5/dlt/normalize/configuration.py` & `dlt-0.3.5a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/normalize/normalize.py` & `dlt-0.3.5a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/__init__.py` & `dlt-0.3.5a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/configuration.py` & `dlt-0.3.5a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/dbt.py` & `dlt-0.3.5a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/exceptions.py` & `dlt-0.3.5a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/helpers.py` & `dlt-0.3.5a0/dlt/pipeline/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,15 @@
 
     def _drop_destination_tables(self) -> None:
         table_names = [tbl['name'] for tbl in self.tables_to_drop]
         with self.pipeline._sql_job_client(self.schema) as client:
             client.drop_tables(*table_names)
             # also delete staging but ignore if staging does not exist
             with contextlib.suppress(DatabaseUndefinedRelation):
-                with client.with_staging_dataset():
-                    client.drop_tables(*table_names)
+                client.drop_tables(*table_names, staging=True)
 
     def _delete_pipeline_tables(self) -> None:
         for tbl in self.tables_to_drop:
             del self.schema_tables[tbl['name']]
         self.schema.bump_version()
 
     def _list_state_paths(self, source_state: Dict[str, Any]) -> List[str]:
```

### Comparing `dlt-0.3.5/dlt/pipeline/pipeline.py` & `dlt-0.3.5a0/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from dlt import version
 from dlt.common import json, logger, pendulum
 from dlt.common.configuration import inject_section, known_sections
 from dlt.common.configuration.specs import RunConfiguration, CredentialsConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
-from dlt.common.configuration.resolve import initialize_credentials
-from dlt.common.exceptions import (DestinationLoadingViaStagingNotSupported, DestinationNoStagingMode, MissingDependencyException,
-                                   DestinationIncompatibleLoaderFileFormatException)
+from dlt.common.exceptions import DestinationLoadingViaStagingNotSupported, DestinationNoStagingMode, MissingDependencyException, DestinationIncompatibleLoaderFileFormatException
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TSchemaTables, TWriteDisposition
 from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo
 from dlt.common.typing import TFun, TSecretValue
 from dlt.common.runners import pool_runner as runner
@@ -349,35 +347,25 @@
             return None
 
         # make sure that destination is set and client is importable and can be instantiated
         client = self._get_destination_client(self.default_schema)
         staging_client = None
         if self.staging:
             staging_client = self._get_staging_client(self.default_schema)
-            # inject staging config into destination config,
-            # TODO: Not super clean I think? - DestinationClientDwhConfiguration must be refactored
-            # staging_credentials, dataset name and default schema name are arguments for the loader not parts of configuration
+            # inject staging config into destination config, TODO: Not super clean I think?
             if isinstance(client.config, DestinationClientDwhConfiguration) and not client.config.staging_credentials:
                 client.config.staging_credentials = staging_client.config.credentials
 
         # create default loader config and the loader
         load_config = LoaderConfiguration(
             workers=workers,
             raise_on_failed_jobs=raise_on_failed_jobs,
             _load_storage_config=self._load_storage_config
         )
-        load = Load(
-            self.destination,
-            staging=self.staging,
-            collector=self.collector,
-            is_storage_owner=False,
-            config=load_config,
-            initial_client_config=client.config,
-            initial_staging_client_config=staging_client.config if staging_client else None
-        )
+        load = Load(self.destination, staging=self.staging, collector=self.collector, is_storage_owner=False, config=load_config, initial_client_config=client.config, initial_staging_client_config=staging_client.config if staging_client else None)
         try:
             with signals.delayed_signals():
                 runner.run_pool(load.config, load)
             info = self._get_load_info(load)
             self.first_run = False
             return info
         except Exception as l_ex:
@@ -642,15 +630,14 @@
         """Returns information on normalized/completed package with given load_id, all jobs and their statuses."""
         return self._get_load_storage().get_load_package_info(load_id)
 
     def list_failed_jobs_in_package(self, load_id: str) -> Sequence[LoadJobInfo]:
         """List all failed jobs and associated error messages for a specified `load_id`"""
         return self._get_load_storage().get_load_package_info(load_id).jobs.get("failed_jobs", [])
 
-    @with_schemas_sync
     def sync_schema(self, schema_name: str = None, credentials: Any = None) -> TSchemaTables:
         """Synchronizes the schema `schema_name` with the destination. If no name is provided, the default schema will be synchronized."""
         if not schema_name and not self.default_schema_name:
             raise PipelineConfigMissing(self.pipeline_name, "default_schema_name", "load", "Pipeline contains no schemas. Please extract any data with `extract` or `run` methods.")
 
         schema = self.schemas[schema_name] if schema_name else self.default_schema
         client_config = self._get_destination_client_initial_config(credentials)
@@ -866,15 +853,15 @@
         pipeline_schema = self._schema_storage[source_schema.name]
 
         # initialize import with fully discovered schema
         self._schema_storage.save_import_schema_if_not_exists(source_schema)
 
         # get the current schema and merge tables from source_schema
         # note we are not merging props like max nesting or column propagation
-        for table in source_schema.data_tables(include_incomplete=True):
+        for table in source_schema.data_tables():
             pipeline_schema.update_schema(pipeline_schema.normalize_table_identifiers(table))
 
         return extract_id
 
     def _get_destination_client_initial_config(self, destination: DestinationReference = None, credentials: Any = None, as_staging: bool = False) -> DestinationClientConfiguration:
         destination = destination or self.destination
         if not destination:
@@ -883,23 +870,18 @@
                 "destination",
                 "load",
                 "Please provide `destination` argument to `pipeline`, `run` or `load` method directly or via .dlt config.toml file or environment variable."
             )
         # create initial destination client config
         client_spec = destination.spec()
         # initialize explicit credentials
-        if not as_staging:
-            # explicit credentials passed to dlt.pipeline should not be applied to staging
-            credentials = credentials or self.credentials
+        credentials = credentials or self.credentials
         if credentials is not None and not isinstance(credentials, CredentialsConfiguration):
             # use passed credentials as initial value. initial value may resolve credentials
-            credentials = initialize_credentials(
-                client_spec.get_resolvable_fields()["credentials"],
-                credentials
-            )
+            credentials = client_spec.get_resolvable_fields()["credentials"](credentials)
         # this client support schemas and datasets
         default_schema_name = None if self.config.use_single_dataset else self.default_schema_name
 
         if issubclass(client_spec, DestinationClientStagingConfiguration):
             return client_spec(dataset_name=self.dataset_name, default_schema_name=default_schema_name, credentials=credentials, as_staging=as_staging)
         elif issubclass(client_spec, DestinationClientDwhConfiguration):
             # set default schema name to load all incoming data to a single dataset, no matter what is the current schema name
```

### Comparing `dlt-0.3.5/dlt/pipeline/progress.py` & `dlt-0.3.5a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/state_sync.py` & `dlt-0.3.5a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/trace.py` & `dlt-0.3.5a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/pipeline/track.py` & `dlt-0.3.5a0/dlt/pipeline/track.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,17 +86,14 @@
         "destination_name": DestinationReference.to_name(pipeline.destination) if pipeline.destination else None,
         "transaction_id": trace.transaction_id
     }
     # disable automatic slack messaging until we can configure messages themselves
     if step.step == "extract" and step_info:
         assert isinstance(step_info, ExtractInfo)
         props["extract_data"] = step_info.extract_data_info
-    if step.step == "load" and step_info:
-        assert isinstance(step_info, LoadInfo)
-        props["destination_fingerprint"] = step_info.destination_fingerprint
     dlthub_telemetry_track("pipeline", step.step, props)
 
 
 def on_end_trace(trace: PipelineTrace, pipeline: SupportsPipeline) -> None:
     if pipeline.runtime_config.sentry_dsn:
         # print(f"---END SENTRY TX: {trace.transaction_id} SCOPE: {Hub.current.scope}")
         with contextlib.suppress(Exception):
```

### Comparing `dlt-0.3.5/dlt/reflection/names.py` & `dlt-0.3.5a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/reflection/script_inspector.py` & `dlt-0.3.5a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/reflection/script_visitor.py` & `dlt-0.3.5a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/sources/helpers/requests/session.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/sources/helpers/transform.py` & `dlt-0.3.5a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/dlt/version.py` & `dlt-0.3.5a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.5/pyproject.toml` & `dlt-0.3.5a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.5"
+version = "0.3.5a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.3.5/setup.py` & `dlt-0.3.5a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,17 +101,17 @@
  'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.5',
+    'version': '0.3.5a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
-    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nimport requests\n# Create a dlt pipeline that will load\n# chess player data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'player_data\'\n)\n# Grab some player data from Chess.com API\ndata = []\nfor player in [\'magnuscarlsen\', \'rpragchess\']:\n    response = requests.get(f\'https://api.chess.com/pub/player/{player}\')\n    response.raise_for_status()\n    data.append(response.json())\n# Extract, normalize, and load the data\npipeline.run(data, table_name=\'player\')\n```\n\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
+    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlt-0.3.5/PKG-INFO` & `dlt-0.3.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.5
+Version: 0.3.5a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -109,32 +109,29 @@
 
 ## Quick Start
 
 Load chess game data from chess.com API and save it in DuckDB:
 
 ```python
 import dlt
-import requests
-# Create a dlt pipeline that will load
-# chess player data to the DuckDB destination
+from chess import chess # a utility function that grabs data from the chess.com API
+
+# create a dlt pipeline that will load chess game data to the DuckDB destination
 pipeline = dlt.pipeline(
     pipeline_name='chess_pipeline',
     destination='duckdb',
-    dataset_name='player_data'
+    dataset_name='games_data'
 )
-# Grab some player data from Chess.com API
-data = []
-for player in ['magnuscarlsen', 'rpragchess']:
-    response = requests.get(f'https://api.chess.com/pub/player/{player}')
-    response.raise_for_status()
-    data.append(response.json())
-# Extract, normalize, and load the data
-pipeline.run(data, table_name='player')
-```
 
+# use chess.com API to grab data about a few players
+data = chess(['magnuscarlsen', 'rpragchess'], start_month='2022/11', end_month='2022/12')
+
+# extract, normalize, and load the data
+pipeline.run(data)
+```
 
 Try it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**
 
 ## Features
 
 - **Automatic Schema:** Data structure inspection and schema creation for the destination.
 - **Data Normalization:** Consistent and verified data before loading.
```

