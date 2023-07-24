# Comparing `tmp/neptune-1.3.3rc0.tar.gz` & `tmp/neptune-1.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-1.3.3rc0.tar", max compression
+gzip compressed data, was "neptune-1.4.0rc0.tar", max compression
```

## Comparing `neptune-1.3.3rc0.tar` & `neptune-1.4.0rc0.tar`

### file list

```diff
@@ -1,327 +1,328 @@
--rw-r--r--   0        0        0    27363 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/LICENSE
--rw-r--r--   0        0        0    13935 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/README.md
--rw-r--r--   0        0        0     5431 2023-07-12 12:33:43.836290 neptune-1.3.3rc0/pyproject.toml
--rw-r--r--   0        0        0     3532 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/api/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/api/exceptions_utils.py
--rw-r--r--   0        0        0      992 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     1218 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2023-07-12 12:33:28.476122 neptune-1.3.3rc0/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3048 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1788 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     1704 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2395 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2658 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     2642 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4583 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     1949 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4292 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3498 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0      866 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/abstract_backend_runner.py
--rw-r--r--   0        0        0     3436 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5574 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/commands.py
--rw-r--r--   0        0        0     2814 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/container_manager.py
--rw-r--r--   0        0        0     1947 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3899 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/status.py
--rw-r--r--   0        0        0     9995 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5028 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     5615 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14676 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2568 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2023-07-12 12:33:28.480122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7335 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7527 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/utils.py
--rw-r--r--   0        0        0     2206 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0      985 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/constants.py
--rw-r--r--   0        0        0     1863 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/envs.py
--rw-r--r--   0        0        0    41967 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/exceptions.py
--rw-r--r--   0        0        0    29698 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3084 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     4017 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7169 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     6700 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6232 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    17136 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    40705 2023-07-12 12:33:28.484122 neptune-1.3.3rc0/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     8506 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    31714 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1942 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4471 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1619 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5184 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0     8765 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1537 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1154 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      350 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0     8543 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/disk_queue.py
--rw-r--r--   0        0        0      689 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2466 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5101 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0      796 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1572 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1831 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17310 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    10682 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     2177 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     2136 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     1253 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1998 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/operation_storage.py
--rw-r--r--   0        0        0     1577 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     2483 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     3724 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      776 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     2023 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3041 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5476 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     1665 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0     4856 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2374 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     5962 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0     9732 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     3053 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/json_file_splitter.py
--rw-r--r--   0        0        0     1633 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     1488 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1042 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2188 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1207 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     1457 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/sync_offset_file.py
--rw-r--r--   0        0        0     1998 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2426 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.488122 neptune-1.3.3rc0/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5334 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     3857 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2023-07-12 12:33:28.492122 neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4454 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    36941 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2063 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    22556 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9194 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    12337 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    11428 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    15433 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    24367 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     2606 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11695 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1727 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2447 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     2553 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2023-07-12 12:33:28.496122 neptune-1.3.3rc0/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0      698 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/typing.py
--rw-r--r--   0        0        0     1755 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2228 2023-07-12 12:33:28.500122 neptune-1.3.3rc0/src/neptune/version.py
--rw-r--r--   0        0        0    18352 1970-01-01 00:00:00.000000 neptune-1.3.3rc0/PKG-INFO
+-rw-r--r--   0        0        0    27959 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/LICENSE
+-rw-r--r--   0        0        0    13935 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/README.md
+-rw-r--r--   0        0        0     5608 2023-07-24 07:09:29.719764 neptune-1.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     3532 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/api/exceptions_utils.py
+-rw-r--r--   0        0        0      992 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     1218 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3048 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1788 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     1704 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2395 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2658 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     2642 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4583 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     1949 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4292 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3498 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1017 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0      866 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/abstract_backend_runner.py
+-rw-r--r--   0        0        0     3436 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5574 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0     2814 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/container_manager.py
+-rw-r--r--   0        0        0     1947 2023-07-24 07:09:10.206738 neptune-1.4.0rc0/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3899 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     9995 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5028 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     5615 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14676 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2568 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7335 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7527 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     2206 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0      985 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/constants.py
+-rw-r--r--   0        0        0     1863 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/envs.py
+-rw-r--r--   0        0        0    41967 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    29698 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.210739 neptune-1.4.0rc0/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3084 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1022 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     4017 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7169 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     6700 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6232 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    17136 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    40705 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     8506 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    31714 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     1942 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4471 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1619 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5184 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0     8765 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1537 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1154 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      350 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2023-07-24 07:09:10.214739 neptune-1.4.0rc0/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0     8543 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/disk_queue.py
+-rw-r--r--   0        0        0      689 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5101 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0      796 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1572 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1831 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17310 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    10721 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     2177 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     2175 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     1253 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1876 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/operation_storage.py
+-rw-r--r--   0        0        0     1577 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     2522 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     3724 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      776 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2023 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3041 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5476 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     1665 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0     4856 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2374 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     5962 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0     9732 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     3053 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/json_file_splitter.py
+-rw-r--r--   0        0        0     1633 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     1488 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1042 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2188 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1207 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     1457 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/sync_offset_file.py
+-rw-r--r--   0        0        0     1998 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2426 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5334 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2023-07-24 07:09:10.218739 neptune-1.4.0rc0/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     3857 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2023-07-24 07:09:10.222739 neptune-1.4.0rc0/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4454 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    36941 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2063 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    22556 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9194 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    12337 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    11428 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    15433 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    24367 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     2606 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11695 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1727 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2447 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     2553 2023-07-24 07:09:10.226740 neptune-1.4.0rc0/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0      698 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/typing.py
+-rw-r--r--   0        0        0     1755 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2228 2023-07-24 07:09:10.230740 neptune-1.4.0rc0/src/neptune/version.py
+-rw-r--r--   0        0        0    18531 1970-01-01 00:00:00.000000 neptune-1.4.0rc0/PKG-INFO
```

### Comparing `neptune-1.3.3rc0/CHANGELOG.md` & `neptune-1.4.0rc0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-##  neptune 1.3.3
+## [UNRELEASED] neptune 1.4.0
+
+### Fixes
+- Fixed operation processor bug if current working directory is different from the script directory ([#1391](https://github.com/neptune-ai/neptune-client/pull/1391))
+
+### Features
+- Added support for `tensorboard` integration ([#1368](https://github.com/neptune-ai/neptune-client/pull/1368))
+- Added support for `mlflow` integration ([#1381](https://github.com/neptune-ai/neptune-client/pull/1381))
+
+
+##  neptune 1.3.3rc0
 
 ### Changes
 - Dependency tracking feature will log an error if a given file path doesn't exist ([#1389](https://github.com/neptune-ai/neptune-client/pull/1389))
-- Use `pip list --format=freeze` instead of `pip freeze` in dependency tracking ([#1389](https://github.com/neptune-ai/neptune-client/pull/1389))
+- Use `importlib` instead of `pip freeze` in dependency tracking ([#1389](https://github.com/neptune-ai/neptune-client/pull/1389))
 - Log both uploaded and inferred requirements to the same namespace ([#1389](https://github.com/neptune-ai/neptune-client/pull/1389))
 
 ### Fixes
+- Fixed operation processor bug if current working directory is different from the script directory ([#1391](https://github.com/neptune-ai/neptune-client/pull/1391))
 - Tracking uncommitted changes and dependencies will be skipped in case of any exception, to not disturb the run initialization ([#1395](https://github.com/neptune-ai/neptune-client/pull/1395))
 
 ## neptune 1.3.2
 
 ### Fixes
 - Fixed GitPython `is_dirty` failing on Windows ([#1371](https://github.com/neptune-ai/neptune-client/pull/1371))
 - Fix SSL errors after forking process ([#1353](https://github.com/neptune-ai/neptune-client/pull/1353))
```

### Comparing `neptune-1.3.3rc0/LICENSE` & `neptune-1.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/README.md` & `neptune-1.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/pyproject.toml` & `neptune-1.4.0rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -74,35 +74,39 @@
 pytorch-lightning = { version = "*", optional = true }
 neptune-optuna = { version = "*", optional = true }
 neptune-prophet = { version = "*", optional = true }
 neptune-pytorch = { version = "*", optional = true }
 neptune-sacred = { version = "*", optional = true }
 neptune-sklearn = { version = "*", optional = true }
 neptune-tensorflow-keras = { version = "*", optional = true }
+neptune-tensorboard = { version = "*", optional = true }
 neptune-xgboost = { version = "*", optional = true }
 transformers = { version = "*", optional = true }
 zenml = { version = "*", optional = true, python = "<3.9" }
 neptune-aws = { version = "*", optional = true }
+mlflow = { version = ">1.30", optional = true }
 
 [tool.poetry.extras]
 aws = ["neptune-aws"]
 detectron2 = ["neptune-detectron2"]
 fastai = ["neptune-fastai"]
 kedro = ["kedro-neptune"]
 lightgbm = ["neptune-lightgbm"]
 optuna = ["neptune-optuna"]
 prophet = ["neptune-prophet"]
 pytorch = ["neptune-pytorch"]
 pytorch-lightning = ["pytorch-lightning"]
 sacred = ["neptune-sacred"]
 sklearn = ["neptune-sklearn"]
 tensorflow-keras = ["neptune-tensorflow-keras"]
+tensorboard = ["neptune-tensorboard"]
 transformers = ["transformers"]
 xgboost = ["neptune-xgboost"]
 zenml = ["zenml"]
+mlflow = ["mlflow"]
 dev = [
     "altair",
     "bokeh",
     "Faker",
     "freezegun",
     "matplotlib",
     "mock",
@@ -124,27 +128,28 @@
     "optuna",
     "pytorch-lightning",
     "scikit-learn",
     "torchvision",
     "transformers",
     "accelerate",
     "zenml",
+    "mlflow",
 ]
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
 description = "Neptune Client"
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "1.3.3-rc.0"
+version = "1.4.0-rc.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-1.3.3rc0/src/neptune/__init__.py` & `neptune-1.4.0rc0/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/api/__init__.py` & `neptune-1.4.0rc0/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/api/exceptions_utils.py` & `neptune-1.4.0rc0/src/neptune/api/exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/api/requests_utils.py` & `neptune-1.4.0rc0/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/__init__.py` & `neptune-1.4.0rc0/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/__init__.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/artifact.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/atom.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/boolean.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/datetime.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/file.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/float.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/git_ref.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/integer.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/run_state.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/atoms/string.py` & `neptune-1.4.0rc0/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/attribute.py` & `neptune-1.4.0rc0/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/constants.py` & `neptune-1.4.0rc0/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/file_set.py` & `neptune-1.4.0rc0/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/namespace.py` & `neptune-1.4.0rc0/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/__init__.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/fetchable_series.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/file_series.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/float_series.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/series.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/series/string_series.py` & `neptune-1.4.0rc0/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/sets/__init__.py` & `neptune-1.4.0rc0/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/sets/set.py` & `neptune-1.4.0rc0/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/sets/string_set.py` & `neptune-1.4.0rc0/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/attributes/utils.py` & `neptune-1.4.0rc0/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/__init__.py` & `neptune-1.4.0rc0/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/__main__.py` & `neptune-1.4.0rc0/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/abstract_backend_runner.py` & `neptune-1.4.0rc0/src/neptune/cli/abstract_backend_runner.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/clear.py` & `neptune-1.4.0rc0/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/commands.py` & `neptune-1.4.0rc0/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/container_manager.py` & `neptune-1.4.0rc0/src/neptune/cli/container_manager.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/path_option.py` & `neptune-1.4.0rc0/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/status.py` & `neptune-1.4.0rc0/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/sync.py` & `neptune-1.4.0rc0/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/cli/utils.py` & `neptune-1.4.0rc0/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/backends/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/backends/api_model.py` & `neptune-1.4.0rc0/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/backends/utils.py` & `neptune-1.4.0rc0/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/envs.py` & `neptune-1.4.0rc0/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/exceptions.py` & `neptune-1.4.0rc0/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/experiments.py` & `neptune-1.4.0rc0/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/git_info.py` & `neptune-1.4.0rc0/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/constants.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/cpu.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/gpu.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gauges/memory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gpu/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metric.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/resources/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/system/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/hardware/system/system_monitor.py` & `neptune-1.4.0rc0/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/oauth.py` & `neptune-1.4.0rc0/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/patches/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/patches/bravado.py` & `neptune-1.4.0rc0/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/patterns.py` & `neptune-1.4.0rc0/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/storage/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/storage/datastream.py` & `neptune-1.4.0rc0/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/storage/storage_utils.py` & `neptune-1.4.0rc0/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/utils.py` & `neptune-1.4.0rc0/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/warnings.py` & `neptune-1.4.0rc0/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/websockets/__init__.py` & `neptune-1.4.0rc0/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune-1.4.0rc0/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune-1.4.0rc0/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/constants.py` & `neptune-1.4.0rc0/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/envs.py` & `neptune-1.4.0rc0/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/exceptions.py` & `neptune-1.4.0rc0/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/handler.py` & `neptune-1.4.0rc0/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/aws/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/detectron2/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/fastai/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/kedro/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/lightgbm/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/optuna/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/prophet/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/python_logger.py` & `neptune-1.4.0rc0/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/pytorch/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/sacred/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/sklearn/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/transformers/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/utils.py` & `neptune-1.4.0rc0/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/integrations/xgboost/__init__.py` & `neptune-1.4.0rc0/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/local.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/file_hasher.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/types.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/artifacts/utils.py` & `neptune-1.4.0rc0/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/api_model.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/factory.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/hosted_client.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/neptune_backend.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/nql.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/project_name_lookup.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backends/utils.py` & `neptune-1.4.0rc0/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/backgroud_job_list.py` & `neptune-1.4.0rc0/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/background_job.py` & `neptune-1.4.0rc0/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/container_structure.py` & `neptune-1.4.0rc0/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/container_type.py` & `neptune-1.4.0rc0/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/credentials.py` & `neptune-1.4.0rc0/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/disk_queue.py` & `neptune-1.4.0rc0/src/neptune/internal/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/exceptions.py` & `neptune-1.4.0rc0/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/hardware/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-1.4.0rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-1.4.0rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/id_formats.py` & `neptune-1.4.0rc0/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/init/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/init/parameters.py` & `neptune-1.4.0rc0/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/notebooks/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/notebooks/comm.py` & `neptune-1.4.0rc0/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/notebooks/notebooks.py` & `neptune-1.4.0rc0/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation.py` & `neptune-1.4.0rc0/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 __all__ = ("AsyncOperationProcessor",)
 
 import logging
 import os
 import threading
 from datetime import datetime
+from pathlib import Path
 from time import (
     monotonic,
     time,
 )
 from typing import (
     List,
     Optional,
@@ -77,20 +78,20 @@
         self._consumed_version = 0
         self._consumer = self.ConsumerThread(self, sleep_time, batch_size)
 
         # Caller is responsible for taking this lock
         self._waiting_cond = threading.Condition(lock=lock)
 
     @staticmethod
-    def _init_data_path(container_id: UniqueId, container_type: ContainerType):
+    def _init_data_path(container_id: UniqueId, container_type: ContainerType) -> Path:
         now = datetime.now()
         container_dir = f"{NEPTUNE_DATA_DIRECTORY}/{ASYNC_DIRECTORY}/{container_type.create_dir_name(container_id)}"
         data_path = f"{container_dir}/exec-{now.timestamp()}-{now.strftime('%Y-%m-%d_%H.%M.%S.%f')}-{os.getpid()}"
         data_path = data_path.replace(" ", "_").replace(":", ".")
-        return data_path
+        return Path(data_path)
 
     def enqueue_operation(self, op: Operation, *, wait: bool) -> None:
         self._last_version = self._queue.put(op)
         if self._queue.size() > self._batch_size / 2:
             self._consumer.wake_up()
         if wait:
             self.wait()
```

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/factory.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ("OfflineOperationProcessor",)
 
 import threading
+from pathlib import Path
 from typing import Optional
 
 from neptune.constants import (
     NEPTUNE_DATA_DIRECTORY,
     OFFLINE_DIRECTORY,
 )
 from neptune.internal.container_type import ContainerType
@@ -38,16 +39,16 @@
             dir_path=self._operation_storage.data_path,
             to_dict=lambda x: x.to_dict(),
             from_dict=Operation.from_dict,
             lock=lock,
         )
 
     @staticmethod
-    def _init_data_path(container_id: UniqueId, container_type: ContainerType):
-        return f"{NEPTUNE_DATA_DIRECTORY}/{OFFLINE_DIRECTORY}/{container_type.create_dir_name(container_id)}"
+    def _init_data_path(container_id: UniqueId, container_type: ContainerType) -> Path:
+        return Path(f"{NEPTUNE_DATA_DIRECTORY}/{OFFLINE_DIRECTORY}/{container_type.create_dir_name(container_id)}")
 
     def enqueue_operation(self, op: Operation, *, wait: bool) -> None:
         self._queue.put(op)
 
     def wait(self):
         self.flush()
```

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ("SyncOperationProcessor",)
 
 from datetime import datetime
+from pathlib import Path
 from typing import Optional
 
 from neptune.constants import (
     NEPTUNE_DATA_DIRECTORY,
     SYNC_DIRECTORY,
 )
 from neptune.internal.backends.neptune_backend import NeptuneBackend
@@ -34,19 +35,19 @@
     def __init__(self, container_id: UniqueId, container_type: ContainerType, backend: NeptuneBackend):
         self._container_id = container_id
         self._container_type = container_type
         self._backend = backend
         self._operation_storage = OperationStorage(self._init_data_path(container_id, container_type))
 
     @staticmethod
-    def _init_data_path(container_id: UniqueId, container_type: ContainerType):
+    def _init_data_path(container_id: UniqueId, container_type: ContainerType) -> Path:
         now = datetime.now()
         container_dir = f"{NEPTUNE_DATA_DIRECTORY}/{SYNC_DIRECTORY}/{container_type.create_dir_name(container_id)}"
         data_path = f"{container_dir}/exec-{now.timestamp()}-{now.strftime('%Y-%m-%d_%H.%M.%S.%f')}"
-        return data_path
+        return Path(data_path)
 
     def enqueue_operation(self, op: Operation, *, wait: bool) -> None:
         _, errors = self._backend.execute_operations(
             container_id=self._container_id,
             container_type=self._container_type,
             operations=[op],
             operation_storage=self._operation_storage,
```

### Comparing `neptune-1.3.3rc0/src/neptune/internal/operation_visitor.py` & `neptune-1.4.0rc0/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/state.py` & `neptune-1.4.0rc0/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/streams/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-1.4.0rc0/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-1.4.0rc0/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/threading/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/threading/daemon.py` & `neptune-1.4.0rc0/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/types/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/types/file_types.py` & `neptune-1.4.0rc0/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/types/stringify_value.py` & `neptune-1.4.0rc0/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/dependency_tracking.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/deprecation.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/git.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/hashing.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/images.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/iteration.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/json_file_splitter.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/limits.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/logger.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/paths.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/ping_background_job.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/process_killer.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/run_state.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/runningmode.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/s3.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/source_code.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/sync_offset_file.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/traceback_job.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-1.4.0rc0/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-1.4.0rc0/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/websockets/__init__.py` & `neptune-1.4.0rc0/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-1.4.0rc0/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/internal/websockets/websockets_factory.py` & `neptune-1.4.0rc0/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/api_exceptions.py` & `neptune-1.4.0rc0/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/backend.py` & `neptune-1.4.0rc0/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/checkpoint.py` & `neptune-1.4.0rc0/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/constants.py` & `neptune-1.4.0rc0/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/envs.py` & `neptune-1.4.0rc0/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/exceptions.py` & `neptune-1.4.0rc0/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/experiments.py` & `neptune-1.4.0rc0/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/git_info.py` & `neptune-1.4.0rc0/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/abort.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/backends/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/channels/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/channels/channels.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/execution/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/execution/execution_context.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/experiments/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/comm.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/streams/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/threads/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/deprecation.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/http.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/http_utils.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/image.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/utils/source_code.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/__init__.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/message.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune-1.4.0rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/model.py` & `neptune-1.4.0rc0/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/notebook.py` & `neptune-1.4.0rc0/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/oauth.py` & `neptune-1.4.0rc0/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/patterns.py` & `neptune-1.4.0rc0/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/projects.py` & `neptune-1.4.0rc0/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/sessions.py` & `neptune-1.4.0rc0/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/legacy/utils.py` & `neptune-1.4.0rc0/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/logging/__init__.py` & `neptune-1.4.0rc0/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/logging/logger.py` & `neptune-1.4.0rc0/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/__init__.py` & `neptune-1.4.0rc0/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/exceptions.py` & `neptune-1.4.0rc0/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/internal/__init__.py` & `neptune-1.4.0rc0/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/internal/api.py` & `neptune-1.4.0rc0/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/internal/dto.py` & `neptune-1.4.0rc0/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/internal/types.py` & `neptune-1.4.0rc0/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/management/internal/utils.py` & `neptune-1.4.0rc0/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/__init__.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/abstract.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/metadata_container.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/metadata_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/model.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/model_version.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/project.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/metadata_containers/run.py` & `neptune-1.4.0rc0/src/neptune/metadata_containers/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/__init__.py` & `neptune-1.4.0rc0/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/_compatibility.py` & `neptune-1.4.0rc0/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/constants.py` & `neptune-1.4.0rc0/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/envs.py` & `neptune-1.4.0rc0/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/exceptions.py` & `neptune-1.4.0rc0/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/handler.py` & `neptune-1.4.0rc0/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/project.py` & `neptune-1.4.0rc0/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/run.py` & `neptune-1.4.0rc0/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/runs_table.py` & `neptune-1.4.0rc0/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/utils.py` & `neptune-1.4.0rc0/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/new/version.py` & `neptune-1.4.0rc0/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/__init__.py` & `neptune-1.4.0rc0/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/__init__.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/artifact.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/atom.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/boolean.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/datetime.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/file.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/float.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/git_ref.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/integer.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/atoms/string.py` & `neptune-1.4.0rc0/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/file_set.py` & `neptune-1.4.0rc0/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/mode.py` & `neptune-1.4.0rc0/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/model_version_stage.py` & `neptune-1.4.0rc0/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/namespace.py` & `neptune-1.4.0rc0/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/__init__.py` & `neptune-1.4.0rc0/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/file_series.py` & `neptune-1.4.0rc0/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/float_series.py` & `neptune-1.4.0rc0/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/series.py` & `neptune-1.4.0rc0/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/series_value.py` & `neptune-1.4.0rc0/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/series/string_series.py` & `neptune-1.4.0rc0/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/sets/__init__.py` & `neptune-1.4.0rc0/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/sets/set.py` & `neptune-1.4.0rc0/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/sets/string_set.py` & `neptune-1.4.0rc0/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/type_casting.py` & `neptune-1.4.0rc0/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/value.py` & `neptune-1.4.0rc0/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/value_copy.py` & `neptune-1.4.0rc0/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/types/value_visitor.py` & `neptune-1.4.0rc0/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/typing.py` & `neptune-1.4.0rc0/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/utils.py` & `neptune-1.4.0rc0/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/vendor/lib_programname.py` & `neptune-1.4.0rc0/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/vendor/pynvml.py` & `neptune-1.4.0rc0/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/src/neptune/version.py` & `neptune-1.4.0rc0/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.3rc0/PKG-INFO` & `neptune-1.4.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 1.3.3rc0
+Version: 1.4.0rc0
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -30,20 +30,22 @@
 Provides-Extra: aws
 Provides-Extra: detectron2
 Provides-Extra: dev
 Provides-Extra: e2e
 Provides-Extra: fastai
 Provides-Extra: kedro
 Provides-Extra: lightgbm
+Provides-Extra: mlflow
 Provides-Extra: optuna
 Provides-Extra: prophet
 Provides-Extra: pytorch
 Provides-Extra: pytorch-lightning
 Provides-Extra: sacred
 Provides-Extra: sklearn
+Provides-Extra: tensorboard
 Provides-Extra: tensorflow-keras
 Provides-Extra: transformers
 Provides-Extra: xgboost
 Provides-Extra: zenml
 Requires-Dist: Faker ; extra == "dev"
 Requires-Dist: GitPython (>=2.0.8)
 Requires-Dist: Pillow (>=1.1.6)
@@ -56,26 +58,28 @@
 Requires-Dist: bravado (>=11.0.0,<12.0.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: freezegun ; extra == "dev"
 Requires-Dist: future (>=0.17.1)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: kedro-neptune ; (python_version < "3.11") and (extra == "kedro")
 Requires-Dist: matplotlib ; extra == "dev"
+Requires-Dist: mlflow (>1.30) ; extra == "mlflow" or extra == "e2e"
 Requires-Dist: mock ; extra == "dev"
 Requires-Dist: moto[s3] ; extra == "dev"
 Requires-Dist: munch ; extra == "dev"
 Requires-Dist: neptune-aws ; extra == "aws"
 Requires-Dist: neptune-detectron2 ; (python_version >= "3.7") and (extra == "detectron2")
 Requires-Dist: neptune-fastai ; extra == "fastai"
 Requires-Dist: neptune-lightgbm ; extra == "lightgbm"
 Requires-Dist: neptune-optuna ; extra == "optuna"
 Requires-Dist: neptune-prophet ; extra == "prophet"
 Requires-Dist: neptune-pytorch ; extra == "pytorch"
 Requires-Dist: neptune-sacred ; extra == "sacred"
 Requires-Dist: neptune-sklearn ; extra == "sklearn"
+Requires-Dist: neptune-tensorboard ; extra == "tensorboard"
 Requires-Dist: neptune-tensorflow-keras ; extra == "tensorflow-keras"
 Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0)
 Requires-Dist: optuna ; extra == "e2e"
 Requires-Dist: packaging
 Requires-Dist: pandas
 Requires-Dist: plotly ; extra == "dev"
```

