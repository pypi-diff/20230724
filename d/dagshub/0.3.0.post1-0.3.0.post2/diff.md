# Comparing `tmp/dagshub-0.3.0.post1.tar.gz` & `tmp/dagshub-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.0.post1.tar", last modified: Sun Jul 23 15:55:32 2023, max compression
+gzip compressed data, was "dagshub-0.3.0.post2.tar", last modified: Mon Jul 24 09:15:41 2023, max compression
```

## Comparing `dagshub-0.3.0.post1.tar` & `dagshub-0.3.0.post2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.439155 dagshub-0.3.0.post1/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.439155 dagshub-0.3.0.post1/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.439155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.443155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.439155 dagshub-0.3.0.post1/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 15:55:32.000000 dagshub-0.3.0.post1/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:55:32.447155 dagshub-0.3.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-23 15:55:21.000000 dagshub-0.3.0.post1/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.231565 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_misc.py
```

### Comparing `dagshub-0.3.0.post1/LICENSE` & `dagshub-0.3.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/PKG-INFO` & `dagshub-0.3.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post1 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post2 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.0.post1/README.md` & `dagshub-0.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/auth/oauth.py` & `dagshub-0.3.0.post2/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/auth/token_auth.py` & `dagshub-0.3.0.post2/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/auth/tokens.py` & `dagshub-0.3.0.post2/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/analytics.py` & `dagshub-0.3.0.post2/dagshub/common/analytics.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/api/repo.py` & `dagshub-0.3.0.post2/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/api/responses.py` & `dagshub-0.3.0.post2/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/cli.py` & `dagshub-0.3.0.post2/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/config.py` & `dagshub-0.3.0.post2/dagshub/common/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 DAGSHUB_USERNAME_KEY = "DAGSHUB_USERNAME"
 DAGSHUB_PASSWORD_KEY = "DAGSHUB_PASSWORD"
 HTTP_TIMEOUT_KEY = "DAGSHUB_HTTP_TIMEOUT"
 DAGSHUB_QUIET_KEY = "DAGSHUB_QUIET"
 
 parsed_host = urlparse(os.environ.get(HOST_KEY, DEFAULT_HOST))
 hostname = parsed_host.hostname
-host = parsed_host.geturl()
+host = parsed_host.geturl().rstrip("/")
 client_id = os.environ.get(CLIENT_ID_KEY, DEFAULT_CLIENT_ID)
 cache_location = os.environ.get(
     TOKENS_CACHE_LOCATION_KEY, DEFAULT_TOKENS_CACHE_LOCATION
 )
 token = os.environ.get(DAGSHUB_USER_TOKEN_KEY)
 username = os.environ.get(DAGSHUB_USERNAME_KEY)
 password = os.environ.get(DAGSHUB_PASSWORD_KEY)
```

### Comparing `dagshub-0.3.0.post1/dagshub/common/download.py` & `dagshub-0.3.0.post2/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/helpers.py` & `dagshub-0.3.0.post2/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/init.py` & `dagshub-0.3.0.post2/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/logging_util.py` & `dagshub-0.3.0.post2/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/common/util.py` & `dagshub-0.3.0.post2/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.0.post2/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             for res in ann["result"]:
                 try:
                     converted = import_label_studio_annotation(res)
                     annotations.append(converted)
                 except Exception:
                     logger.warning(f"Couldn't convert LS annotation {ann} to voxel annotation")
 
+            if len(annotations) == 0:
+                continue
             # Group the annotations of a similar type together
             # For now assuming there's no mixing and matching
             ann_type = type(annotations[0])
             if ann_type is Detection:
                 labels = Detections()
                 for a in annotations:
                     labels.detections.append(a)
```

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/data_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         has_next_page = True
         after = None
         res = QueryResult([], datasource)
         left = n
 
         progress = get_rich_progress(rich.progress.MofNCompleteColumn())
-        total_task = progress.add_task("Downloading datapoints...", total=left)
+        total_task = progress.add_task("Downloading metadata...", total=left)
 
         with progress:
             while has_next_page and left > 0:
                 take = min(left, self.FULL_LIST_PAGE_SIZE)
                 resp = self._datasource_query(datasource, include_metadata, take, after)
                 has_next_page = resp["pageInfo"]["hasNextPage"]
                 after = resp["pageInfo"]["endCursor"]
@@ -96,15 +96,15 @@
         has_next_page = True
         after = None
         res = QueryResult([], datasource)
         # TODO: smarter batch sizing. Query a constant size at first
         #       On next queries adjust depending on the amount of metadata columns
 
         progress = get_rich_progress(rich.progress.MofNCompleteColumn())
-        total_task = progress.add_task("Downloading datapoints...", total=None)
+        total_task = progress.add_task("Downloading metadata...", total=None)
 
         with progress:
             while has_next_page:
                 resp = self._datasource_query(datasource, include_metadata, self.FULL_LIST_PAGE_SIZE, after)
                 has_next_page = resp["pageInfo"]["hasNextPage"]
                 after = resp["pageInfo"]["endCursor"]
```

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/models.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/datasets.py` & `dagshub-0.3.0.post2/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/datasources.py` & `dagshub-0.3.0.post2/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/errors.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/query.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.0.post2/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/fastai/logger.py` & `dagshub-0.3.0.post2/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/keras/logger.py` & `dagshub-0.3.0.post2/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/logger.py` & `dagshub-0.3.0.post2/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/notebook.py` & `dagshub-0.3.0.post2/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.0.post2/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/streaming/dataclasses.py` & `dagshub-0.3.0.post2/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/streaming/filesystem.py` & `dagshub-0.3.0.post2/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/streaming/mount.py` & `dagshub-0.3.0.post2/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/upload/errors.py` & `dagshub-0.3.0.post2/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub/upload/wrapper.py` & `dagshub-0.3.0.post2/dagshub/upload/wrapper.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.0.post2/dagshub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post1 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post2 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.0.post1/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.0.post2/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/setup.py` & `dagshub-0.3.0.post2/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/tests/test_dagshub_logger.py` & `dagshub-0.3.0.post2/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post1/tests/test_misc.py` & `dagshub-0.3.0.post2/tests/test_misc.py`

 * *Files identical despite different names*

