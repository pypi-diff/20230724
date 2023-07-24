# Comparing `tmp/dagshub-0.3.0.post2.tar.gz` & `tmp/dagshub-0.3.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.0.post2.tar", last modified: Mon Jul 24 09:15:41 2023, max compression
+gzip compressed data, was "dagshub-0.3.0.post3.tar", last modified: Mon Jul 24 13:01:32 2023, max compression
```

## Comparing `dagshub-0.3.0.post2.tar` & `dagshub-0.3.0.post3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.239565 dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.231565 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.243566 dagshub-0.3.0.post2/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.235565 dagshub-0.3.0.post2/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 09:15:41.000000 dagshub-0.3.0.post2/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:15:41.247566 dagshub-0.3.0.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 09:15:27.000000 dagshub-0.3.0.post2/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.746530 dagshub-0.3.0.post3/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.750530 dagshub-0.3.0.post3/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.742530 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.750530 dagshub-0.3.0.post3/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_misc.py
```

### Comparing `dagshub-0.3.0.post2/LICENSE` & `dagshub-0.3.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/PKG-INFO` & `dagshub-0.3.0.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post2
+Version: 0.3.0.post3
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
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post2 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post3 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.0.post2/README.md` & `dagshub-0.3.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/auth/oauth.py` & `dagshub-0.3.0.post3/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/auth/token_auth.py` & `dagshub-0.3.0.post3/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/auth/tokens.py` & `dagshub-0.3.0.post3/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/analytics.py` & `dagshub-0.3.0.post3/dagshub/common/analytics.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/api/repo.py` & `dagshub-0.3.0.post3/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/api/responses.py` & `dagshub-0.3.0.post3/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/cli.py` & `dagshub-0.3.0.post3/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/config.py` & `dagshub-0.3.0.post3/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/download.py` & `dagshub-0.3.0.post3/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/helpers.py` & `dagshub-0.3.0.post3/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/init.py` & `dagshub-0.3.0.post3/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/logging_util.py` & `dagshub-0.3.0.post3/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/common/util.py` & `dagshub-0.3.0.post3/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.0.post3/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/data_client.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,22 +30,23 @@
         tensorizers: auto|image|<function>
         savedir: location at which the dataset is stored
         processes: number of parallel processes that download the dataset
         """
         self.metadata_columns = metadata_columns
         self.entries = query_result.entries
         self.tensorizers = [
-                               lambda x: x,
-                           ] * (
-                               len(metadata_columns) + 1
-                           )  # prevent circular calls
+            lambda x: x,
+        ] * (
+            len(metadata_columns) + 1
+        )  # prevent circular calls
         self.datasource = query_result.datasource
         self.repo = self.datasource.source.repoApi
         self.savedir = savedir or self.datasource.default_dataset_location
         self.strategy = strategy
+        self.source = self.datasource.source.path.split("://")[0]
 
         self.datasource_root = Path(
             self.entries[0].path_in_repo.as_posix()[: -len(self.entries[0].path)]
         )
         self.processes = processes
         self.order = None
         self.file_columns = file_columns or self._get_file_columns()
@@ -99,15 +100,15 @@
                 else entry.metadata[column]
             )
 
         return out
 
     def __getitem__(
         self, idx: int
-    ) -> List[Union["torch.Tensor", "tf.Tensor"]]:   # noqa: F821
+    ) -> List[Union["torch.Tensor", "tf.Tensor"]]:  # noqa: F821
         return [
             tensorizer(data)
             for tensorizer, data in zip(self.tensorizers, self.get(idx))
         ]
 
     def pull(self) -> None:
         if self.order is not None:
@@ -125,15 +126,22 @@
             datapoint.path,
             *[datapoint.metadata.get(column) for column in self.file_columns],
         ]
 
         for path in paths:
             (self.savedir / Path(path).parent).mkdir(parents=True, exist_ok=True)
             if not (self.savedir / path).is_file():
-                data = self.repo.get_file(f"{self.datasource_root}/{path}")
+                if self.source == "repo":
+                    data = self.repo.get_file(f"{self.datasource_root}/{path}")
+                else:
+                    data = self.repo.get_storage_file(
+                        f"{'/'.join(list(self.datasource.source.path_parts().values())[:2])}"
+                        f"/{self.datasource_root}/{path}"
+                    )
+
                 filepath = self.savedir / path
                 with open(filepath, "wb") as file:
                     file.write(data)
 
     def _get_tensorizers(
         self, datatypes: Union[str, List[Union[str, FunctionType]]]
     ) -> FunctionType:
```

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/models.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/datasets.py` & `dagshub-0.3.0.post3/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/datasources.py` & `dagshub-0.3.0.post3/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/errors.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/query.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.0.post3/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/fastai/logger.py` & `dagshub-0.3.0.post3/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/keras/logger.py` & `dagshub-0.3.0.post3/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/logger.py` & `dagshub-0.3.0.post3/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/notebook.py` & `dagshub-0.3.0.post3/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.0.post3/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/streaming/dataclasses.py` & `dagshub-0.3.0.post3/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/streaming/filesystem.py` & `dagshub-0.3.0.post3/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/streaming/mount.py` & `dagshub-0.3.0.post3/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/upload/errors.py` & `dagshub-0.3.0.post3/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub/upload/wrapper.py` & `dagshub-0.3.0.post3/dagshub/upload/wrapper.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.0.post3/dagshub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post2
+Version: 0.3.0.post3
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
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post2 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post3 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
```

### Comparing `dagshub-0.3.0.post2/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.0.post3/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/setup.py` & `dagshub-0.3.0.post3/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/tests/test_dagshub_logger.py` & `dagshub-0.3.0.post3/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post2/tests/test_misc.py` & `dagshub-0.3.0.post3/tests/test_misc.py`

 * *Files identical despite different names*

