# Comparing `tmp/starwhale-0.5.6.tar.gz` & `tmp/starwhale-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starwhale-0.5.6.tar", last modified: Wed Jul 19 02:50:15 2023, max compression
+gzip compressed data, was "dist/starwhale-0.5.7.tar", last modified: Mon Jul 24 02:38:14 2023, max compression
```

## Comparing `starwhale-0.5.6.tar` & `starwhale-0.5.7.tar`

### file list

```diff
@@ -1,363 +1,363 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-19 02:50:15.000000 starwhale-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 02:38:58.000000 starwhale-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-19 02:38:58.000000 starwhale-0.5.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8580 2023-07-19 02:38:58.000000 starwhale-0.5.6/scripts/sw-docker-entrypoint
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:50:15.000000 starwhale-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-19 02:38:58.000000 starwhale-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/api/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62504 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/data_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/builder/mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    51602 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/api/_impl/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/hooker.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/syncer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/track/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/_impl/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/api/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/base/blob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/blob/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/blob/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/cloud_blob_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/base/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/scheduler/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/scheduler/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/scheduler/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/base/uri/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/uri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/uri/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/uri/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/uri/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/uri/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/base/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/cli/assistance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/assistance/wait_console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/cli/board/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/board/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/board/project_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/board/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/cli/mngt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/consts/
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/consts/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/dataset/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/instance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/instance/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/job/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/job/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/job/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/job/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23670 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/model/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/project/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/project/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/project/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    77768 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/runtime/template/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/template/Dockerfile.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/runtime/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/core/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/core/track/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/integrations/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/huggingface/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/integrations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/pytorch/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/integrations/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/integrations/tensorflow/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/mngt/
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/mngt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/proto_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/proto_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/proto_gen/model_package_storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/utils/venv_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/web/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale/web/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/BlockLabel-5fb1ba40.js
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Column-32430de0.js
--rw-r--r--   0 runner    (1001) docker     (123)    51834 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/DatasetForm-b1b79ee8.js
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/File-0190a4b6.js
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Image-7d3d0587.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Image2-fef2a6da.js
--rw-r--r--   0 runner    (1001) docker     (123)   222410 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/LogViewer-b5684b3d.css
--rw-r--r--   0 runner    (1001) docker     (123)   132579 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/LogViewer-ead1dacc.js
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Model3D-017f88a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/ModifyUpload-ca14033f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28661 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29148 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32496 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37096 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35980 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    31952 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Tabs-58551549.js
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Upload-5020e3e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    52093 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/Webcam-1d7c84ed.js
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/_commonjsHelpers-23156833.js
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/account2-668f906e.svg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/color-ab3477a6.js
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/csv-17a3ae92.js
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/dsv-62f8cd07.js
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/empty-chart-1e62901a.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/empty-f3091520.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/google-9d1a8b2b.svg
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/iconfont-0a880318.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/iconfont-10b60b11.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index-0a9704a2.js
--rw-r--r--   0 runner    (1001) docker     (123)  3809533 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index-1d08769b.js
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index-4b525ef6.css
--rw-r--r--   0 runner    (1001) docker     (123)  2779485 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index-54aca6e3.js
--rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index-c467f321.css
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index10-42042dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index11-78c7e86b.js
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index12-ab265665.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index13-7c871e80.js
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index14-6c615bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index15-86a0c1f0.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index16-2bdd3a00.js
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index17-f009f53c.js
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index18-b8f18d2d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index19-a472c2fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    33625 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index2-040b1a6e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index20-cea79a56.js
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index21-839b404f.js
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index22-b0a063e3.js
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index23-2546fc23.js
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index24-ee89579d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index25-fb12b103.js
--rw-r--r--   0 runner    (1001) docker     (123)  3544392 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index26-70ba7bd9.js
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index27-202147ca.js
--rw-r--r--   0 runner    (1001) docker     (123)  4615288 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index28-4db56c35.js
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index29-f4b57e8f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index3-3ed81e50.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index30-6cfd7268.js
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index31-feae9916.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index32-efa03b40.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index33-c77eb4e8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index34-74e21fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index35-76158480.js
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index36-051a9d0c.js
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index37-4dd6b1d2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index38-42b4b637.js
--rw-r--r--   0 runner    (1001) docker     (123)    17355 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index39-4548d90a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index4-efddfb05.js
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index5-a485e343.js
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index6-c4dad8b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index7-c30707d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index8-1ed9ba9d.js
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/index9-1a9ea67c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/invalid-file-82d62dec.svg
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/left-8c88a49a.svg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/left-shadow-e0fdfe32.png
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/linear-8d973619.js
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
--rw-r--r--   0 runner    (1001) docker     (123)   117896 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/main-6cf1adbb.js
--rw-r--r--   0 runner    (1001) docker     (123)    94147 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/module-ddaca3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/module2-74df381a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/module3-49e9a615.js
--rw-r--r--   0 runner    (1001) docker     (123)    42104 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-452a631f.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37252 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45068 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41368 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    33808 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36660 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    42532 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35056 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36800 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37972 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45720 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37368 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45240 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-italic-b81a6146.woff
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-3f8151f4.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34472 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    44372 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36580 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    51572 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    65060 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff
--rw-r--r--   0 runner    (1001) docker     (123)    50112 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63324 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff
--rw-r--r--   0 runner    (1001) docker     (123)    65036 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51524 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    64944 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    51308 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-regular-16b63547.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44728 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36904 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40860 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    33696 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35900 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   276435 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    67491 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   195594 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   116699 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   362032 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   588571 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pficon-0a333dac.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/pficon-86c74539.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/project-863f66b0.svg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/right-aefe3c24.svg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/right-shadow-58dd9abc.png
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/search-empty-13cbde15.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/setting-6d098443.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/utils-de54785e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/web-vitals-d4fac006.js
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/assets/wechat-cffee157.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-19 02:50:04.000000 starwhale-0.5.6/starwhale/web/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-19 02:50:04.000000 starwhale-0.5.6/starwhale/web/ui/favicon_white.ico
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-19 02:50:04.000000 starwhale-0.5.6/starwhale/web/ui/iconfont.js
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    45165 2023-07-19 02:50:13.000000 starwhale-0.5.6/starwhale/web/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 02:50:04.000000 starwhale-0.5.6/starwhale/web/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-19 02:38:58.000000 starwhale-0.5.6/starwhale/web/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-19 02:50:14.000000 starwhale-0.5.6/starwhale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-19 02:50:15.000000 starwhale-0.5.6/starwhale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:50:14.000000 starwhale-0.5.6/starwhale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 02:50:14.000000 starwhale-0.5.6/starwhale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:39:33.000000 starwhale-0.5.6/starwhale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-19 02:50:14.000000 starwhale-0.5.6/starwhale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 02:50:14.000000 starwhale-0.5.6/starwhale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-24 02:38:14.000000 starwhale-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-24 02:24:44.000000 starwhale-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-24 02:24:44.000000 starwhale-0.5.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8580 2023-07-24 02:24:44.000000 starwhale-0.5.7/scripts/sw-docker-entrypoint
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:38:14.000000 starwhale-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-24 02:24:44.000000 starwhale-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/api/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62504 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/data_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/builder/mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51602 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/api/_impl/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/hooker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/syncer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/track/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/_impl/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/api/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/base/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/blob/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/blob/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/cloud_blob_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/base/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/scheduler/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/scheduler/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/scheduler/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/base/uri/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/uri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/uri/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/uri/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/uri/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/uri/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/base/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/cli/assistance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/assistance/wait_console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/cli/board/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/board/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/board/project_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/board/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/cli/mngt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/consts/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/dataset/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/instance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/instance/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/job/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/job/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/job/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/job/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23670 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33266 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/model/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/project/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77768 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/runtime/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/template/Dockerfile.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/runtime/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/core/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/core/track/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/integrations/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/huggingface/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/integrations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/pytorch/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/integrations/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/integrations/tensorflow/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/mngt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/mngt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/proto_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/proto_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/proto_gen/model_package_storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26882 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/utils/venv_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/web/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale/web/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/BlockLabel-fe080bcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Column-958ed910.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51849 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/DatasetForm-45360b60.js
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/File-d0f0778c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Image-953a3e24.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Image2-08f40595.js
+-rw-r--r--   0 runner    (1001) docker     (123)   132579 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/LogViewer-1215be01.js
+-rw-r--r--   0 runner    (1001) docker     (123)   222410 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/LogViewer-b5684b3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Model3D-ff19b927.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/ModifyUpload-972867fe.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28661 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29148 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32496 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37096 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29049 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35980 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25768 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    31952 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Tabs-0edcf972.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Upload-699ac090.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52093 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/Webcam-77a82fdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/_commonjsHelpers-23156833.js
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/account2-668f906e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/color-de3304e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/csv-17a3ae92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/dsv-62f8cd07.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/empty-chart-1e62901a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/empty-f3091520.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/google-9d1a8b2b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/iconfont-0a880318.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/iconfont-10b60b11.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  2779471 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index-00cfa2a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index-0ebd961e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index-4b525ef6.css
+-rw-r--r--   0 runner    (1001) docker     (123)    50329 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index-c467f321.css
+-rw-r--r--   0 runner    (1001) docker     (123)  3809533 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index-fa288f1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index10-6962b31b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index11-6a6faac8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index12-d5dc887c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index13-6dafecb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index14-8c46ae7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index15-7940e50b.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index16-583cafad.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index17-e0f03f64.js
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index18-85c307e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index19-46ac23c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33625 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index2-4608846d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index20-61594d37.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index21-976d330c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index22-ccb7efe7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index23-680c92d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index24-597a8e3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index25-88e85639.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3544392 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index26-36e22149.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index27-dee2bd12.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4615288 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index28-a52d95a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index29-dd39a343.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index3-f722b477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index30-edf8c102.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index31-2a9aa647.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index32-1efd457e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index33-988b470f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index34-e9d05f99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index35-d013c15c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index36-640baba3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index37-675e963b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index38-8ed1f571.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17355 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index39-2e025855.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index4-0bc63b4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index5-f4812d85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index6-aa6ede7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index7-644441a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index8-dfa6b4d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/index9-74c82f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/invalid-file-82d62dec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/left-8c88a49a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/left-shadow-e0fdfe32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/linear-8d973619.js
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   117896 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/main-2ed4d8ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94147 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/module-ddaca3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/module2-74df381a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/module3-49e9a615.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42104 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-452a631f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34752 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37252 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45068 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41368 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33808 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36660 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    42532 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35056 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36800 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37972 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45720 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37368 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45240 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-italic-b81a6146.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-3f8151f4.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34472 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    44372 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36580 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    51572 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    65060 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    50112 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63324 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    65036 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51524 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    64944 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    51308 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-regular-16b63547.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33416 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44728 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36904 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40860 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33696 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43504 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35900 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   276435 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    67491 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   195594 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   116699 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   362032 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   588571 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pficon-0a333dac.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/pficon-86c74539.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/project-863f66b0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/right-aefe3c24.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/right-shadow-58dd9abc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/search-empty-13cbde15.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/setting-6d098443.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/utils-de54785e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/web-vitals-d4fac006.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/assets/wechat-cffee157.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 02:38:00.000000 starwhale-0.5.7/starwhale/web/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 02:38:00.000000 starwhale-0.5.7/starwhale/web/ui/favicon_white.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-24 02:38:00.000000 starwhale-0.5.7/starwhale/web/ui/iconfont.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45165 2023-07-24 02:38:11.000000 starwhale-0.5.7/starwhale/web/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 02:38:00.000000 starwhale-0.5.7/starwhale/web/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 02:24:44.000000 starwhale-0.5.7/starwhale/web/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:38:14.000000 starwhale-0.5.7/starwhale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:26:02.000000 starwhale-0.5.7/starwhale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 02:38:13.000000 starwhale-0.5.7/starwhale.egg-info/top_level.txt
```

### Comparing `starwhale-0.5.6/PKG-INFO` & `starwhale-0.5.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.5.6
+Version: 0.5.7
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,50 +86,50 @@
     <img src='https://github.com/star-whale/starwhale/actions/workflows/e2e-test.yml/badge.svg' alt='Starwhale E2E Test'>
 </a>
 
 </p>
 
 ## What is Starwhale
 
-Starwhale is an MLOps platform. It provides **Instance**, **Project**, **Runtime**, **Model**, and **Dataset**.
+Starwhale is an MLOps/LLMOps platform. It provides **Instance**, **Project**, **Runtime**, **Model**, and **Dataset**.
 
 - **Instance**: Each installation of Starwhale is called an instance.
-  - 👻 **Standalone Instance**: The simplest form that requires only the Starwhale Client(`swcli`). `swcli` is written by pure python3.
-  - 🎍 **On-Premises Instance**: Cloud form, we call it **private cloud instance**. Kubernetes and BareMetal both meet the basic environmental requirements.
-  - ☁️ **Cloud Hosted Instance**: Cloud form, we call it **public cloud instance**. Starwhale team maintains the web service.
+  - 👻 **Starwhale Standalone**:  Rather than a running service, Starwhale Standalone is actually a repository that resides in your local file system. It is created and managed by the Starwhale Client (SWCLI). You only need to install SWCLI to use it. Currently, each user on a single machine can have only ONE Starwhale Standalone instance. We recommend you use the Starwhale Standalone to build and test your datasets, runtime, and models before pushing them to Starwhale Server/Cloud instances.
+  - 🎍 **Starwhale Server**:  Starwhale Server is a service deployed on your local server. Besides text-only results from the Starwhale Client (SWCLI), Starwhale Server provides Web UI for you to manage your datasets and models, evaluate your models in your local Kubernetes cluster, and review the evaluation results.
+  - ☁️ **Starwhale Cloud**: Starwhale Cloud is a managed service hosted on public clouds. By registering an account on https://cloud.starwhale.cn , you are ready to use Starwhale without needing to install, operate, and maintain your own instances. Starwhale Cloud also provides public resources for you to download, like datasets, runtimes, and models. Check the "starwhale/public" project on Starwhale Cloud for more details.
 
   **Starwhale tries to keep concepts consistent across different types of instances. In this way, people can easily exchange data and migrate between them.**
 
 - **Project**: The basic unit for organizing different resources.
 
 - **ML Basic Elements**: The Machine Learning/Deep Learning running environments or artifacts. Starwhale empowers the ML/DL essential elements with packaging, versioning, reproducibility, and shareability.
-  - 🐌 **Runtime**: Software dependencies description to "run" a model, which includes python libraries, native libraries, native binaries, etc.
+  - 🐌 **Runtime**: Software dependencies description to "run" a model, which includes Python libraries, native libraries, native binaries, etc.
   - 🐇 **Model**: The standard model format used in model delivery.
   - 🐫 **Dataset**: A unified description of how the data and labels are stored and organized. Starwhale datasets can be loaded efficiently.
 
 - **Running Fundamentals**: Starwhale uses **Job**, **Step**, and **Task** to execute ML/DL actions like model training， evaluation, and serving. Starwhale's **Controller-Agents** structure scales out easily.
   - 🥕 **Job**: A set of programs to do specific work. Each job consists of one or more steps.
   - 🌵 **Step**: Represents distinct stages of the work. Each step consists of one or more tasks.
   - 🥑 **Task**: Operation entity. Tasks are in some specific steps.
 
 - **Scenarios**: Starwhale provides the best practice and out-of-the-box for different ML/DL scenarios.
   - 🚝 **Model Training(WIP)**: Use Starwhale Python SDK to record experiment meta, metric, log, and artifact.
-  - 🛥️ **Model Evaluation**: `PipelineHandler` and some report decorators can give you complete, helpful, and user-friendly evaluation reports with only a few lines of codes.
+  - 🛥️ **Model Evaluation**: `PipelineHandler` and some report decorators can give you complete, helpful, and user-friendly evaluation reports with only a few lines of code.
   - 🛫 **Model Serving(TBD)**: Starwhale Model can be deployed as a web service or stream service in production with deployment capability, observability, and scalability. Data scientists do not need to write ML/DL irrelevant codes.
 
-## MNIST Quick Tour for the standalone instance
+## MNIST Quick Tour for the Starwhale Standalone Instance
 
 ### Use Notebook
 
-- You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/mnist/notebook.ipynb)
-- Or run [example/mnist/notebook.ipynb](example/mnist/notebook.ipynb) locally using [vscode](https://code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/jupyterlab)
+- You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/quickstart-standalone.ipynb)
+- Or run [quickstart example](example/notebooks/quickstart-standalone.ipynb) locally using [vscode](https://code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/jupyterlab)
 
-### Use your own python env
+### Use your own Python env
 
-![Core Job Workflow](docs/docs/img/standalone-core-workflow.gif)
+![Core Job Workflow](https://doc.starwhale.ai/assets/images/standalone-core-workflow-270ac0f0cb5b20dbe5ccd11727e2620b.gif)
 
 - 🍰 **STEP1**: Installing Starwhale
 
     ```bash
     python3 -m pip install starwhale
     ```
 
@@ -147,22 +147,22 @@
     > When you first build runtime, creating an isolated python environment and downloading python dependencies will take a lot of time. The command execution time is related to the network environment of the machine and the number of packages in the runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/pip.conf` file is a recommended practice.
     >
     > For users in the mainland of China, the following conf file is an option:
     >
     > ```conf
     > [global]
     > cache-dir = ~/.cache/pip
-    > index-url = https://mirrors.aliyun.com/pypi/simple/
-    > extra-index-url = https://pypi.doubanio.com/simple
+    > index-url = https://pypi.tuna.tsinghua.edu.cn/simple
+    > extra-index-url = https://mirrors.aliyun.com/pypi/simple/
     > ```
 
     ```bash
-    swcli runtime build example/runtime/pytorch
+    swcli runtime build --yaml example/runtime/pytorch/runtime.yaml
     swcli runtime list
-    swcli runtime info pytorch/version/latest
+    swcli runtime info pytorch
     ```
 
 - 🍞 **STEP4**: Building a model
 
   - Download pre-trained model file:
 
     ```bash
@@ -225,17 +225,17 @@
     run:
         handler: mnist.evaluator:MNISTInference
     ```
 
   - Run one command to build the model.
 
     ```bash
-    swcli model build example/mnist --runtime pytorch/version/latest
+    swcli model build example/mnist --runtime pytorch
     swcli model list
-    swcli model info mnist/version/latest
+    swcli model info mnist
     ```
 
 - 🍺 **STEP5**: Building a dataset
 
   - Download MNIST RAW data files.
 
     ```bash
@@ -278,34 +278,34 @@
                     "label": _label,
                 }
     ```
 
   - Run one command to build the dataset.
 
     ```bash
-    swcli dataset build example/mnist --handler mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest
-    swcli dataset info mnist/version/latest
-    swcli dataset head mnist/version/latest
+    swcli dataset build --yaml example/mnist/dataset.yaml
+    swcli dataset info mnist
+    swcli dataset head mnist
     ```
 
-  Starwhale also supports build dataset with pure python sdk. You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/dataset-sdk.ipynb).
+  Starwhale also supports building datasets with pure Python SDK. You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/dataset-sdk.ipynb).
 
 - 🍖 **STEP6**: Running an evaluation job
 
     ```bash
-    swcli eval run --model mnist/version/latest --dataset mnist/version/latest --runtime pytorch/version/latest
-    swcli eval list
-    swcli eval info $(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
+    swcli -vvv model run --uri mnist --dataset mnist --runtime pytorch
+    swcli job list
+    swcli job info $(swcli job list | grep mnist | grep success | awk '{print $1}' | head -n 1)
     ```
 
 **👏 Now, you have completed the fundamental steps for Starwhale standalone. Let's go ahead and finish the tutorial on the on-premises instance.**
 
-## MNIST Quick Tour for on-premises instance
+## MNIST Quick Tour for Starwhale Server Instance
 
-![Create Job Workflow](docs/docs/img/console-create-job.gif)
+![Create Job Workflow](https://doc.starwhale.ai/assets/images/console-artifacts-fd7bf6e54d06dc37d234019e769031e6.gif)
 
 - 🍰 **STEP1**: Install minikube and helm
 
   - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+
   - [Helm](https://helm.sh/docs/intro/install/) 3.2.0+
 
 - 🍵 **STEP2**: Start minikube
@@ -364,41 +364,66 @@
         - web visit: http://minio.starwhale.svc
         - admin visit: http://minio-admin.starwhale.svc
     MySQL:
         - port-forward:
         - run: kubectl port-forward --namespace starwhale svc/mysql 3306:3306
         - visit: mysql -h 127.0.0.1 -P 3306 -ustarwhale -pstarwhale
     Please run the following command for the domains searching:
-        echo "$(minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
+        echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
     ******************************************
     Login Info:
     - starwhale: u:starwhale, p:abcd1234
     - minio admin: u:minioadmin, p:minioadmin
 
     *_* Enjoy to use Starwhale Platform. *_*
     ```
 
-    Then keep checking the minikube service status until all deployments are running.
+    Then keep checking the minikube service status until all deployments are running(waiting for 3~5 mins).
 
     ```bash
     kubectl get deployments -n starwhale
     ```
 
     | NAME       | READY | UP-TO-DATE | AVAILABLE | AGE |
     | ---------- | ----- | ---------- | --------- | --- |
     | controller | 1/1   | 1          | 1         | 5m  |
     | minio      | 1/1   | 1          | 1         | 5m  |
     | mysql      | 1/1   | 1          | 1         | 5m  |
 
     Make the Starwhale controller accessible locally with the following command:
 
     ```bash
-    kubectl port-forward --namespace starwhale svc/controller 8082:8082
+    echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
     ```
 
+    Then you can visit http://controller.starwhale.svc in your local web browser.
+
+    If other users also want to access Starwhale Server Instance, the following commands maybe help you:
+
+    - in your machine(Linux, Starwhale Server Instance machine):
+
+        for temporary use with socat command:
+
+        ```bash
+        # install socat at first, ref: https://howtoinstall.co/en/socat
+        sudo socat TCP4-LISTEN:80,fork,reuseaddr,bind=0.0.0.0 TCP4:`minikube ip`:80
+        ```
+
+      When you kill the socat process, the share access will be blocked. `iptables` maybe a better choice for long-term use.
+
+    - in other users' machines:
+
+        ```bash
+        # for macOSX or Linux environment, run the command in the shell.
+        echo ${your_machine_ip} controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
+
+        # for Windows environment, run the command in the PowerShell with administrator permission.
+        Add-Content -Path C:\Windows\System32\drivers\etc\hosts -Value "`n${your_machine_ip} controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc"
+        ```
+
 - ☕ **STEP4**: Upload the artifacts to the cloud instance
 
     > **pre-prepared artifacts**
     > Before starting this tutorial, the following three artifacts should already exist on your machine：
     >
     > - a starwhale model named mnist
     > - a starwhale dataset named mnist
@@ -406,41 +431,31 @@
     >
     > The above three artifacts are what we built on our machine using starwhale.
 
     1. Use swcli to operate the remote server
         First, log in to the server:
 
         ```bash
-        swcli instance login --username starwhale --password abcd1234 --alias dev http://localhost:8082
+        swcli instance login --username starwhale --password abcd1234 --alias dev http://controller.starwhale.svc
         ```
 
     2. Start copying the model, dataset, and runtime that we constructed earlier:
 
         ```bash
-        swcli model copy mnist/version/latest dev/project/starwhale
-        swcli dataset copy mnist/version/latest dev/project/starwhale
-        swcli runtime copy pytorch/version/latest dev/project/starwhale
+        swcli model copy mnist cloud://dev/project/starwhale
+        swcli dataset copy mnist cloud://dev/project/starwhale
+        swcli runtime copy pytorch cloud://dev/project/starwhale
         ```
 
 - 🍞 **STEP5**: Use the web UI to run an evaluation
 
-    1. Log in Starwhale instance: let's use the username(starwhale) and password(abcd1234) to open the server web UI(<http://localhost:8082/>).
-
-    2. Then, we will see the project named 'project_for_mnist' that we created earlier with swcli. Click the project name, you will see the model, runtime, and dataset uploaded in the previous step.
-        <details>
-            <summary>Show the uploaded artifacts screenshots</summary>
-
-        ![Console Artifacts](docs/docs/img/console-artifacts.gif)
-        </details>
-    3. Create and view an evaluation job
-        <details>
-            <summary>Show create job screenshot</summary>
+    1. Log in Starwhale instance: let's use the username(starwhale) and password(abcd1234) to open the server web UI(<http://controller.starwhale.svc>).
 
-        ![Console Create Job](docs/docs/img/console-create-job.gif)
-        </details>
+    2. Then, we will see the project named 'starwhale/starwhale' that we created earlier with swcli. Click the project name, you will see the model, runtime, and dataset uploaded in the previous step.
+    3. Create and view an evaluation job.
 
 **👏 Congratulations! You have completed the evaluation process for a model.**
 
 ## Documentation, Community, and Support
 
 - Visit [Starwhale HomePage](https://starwhale.ai).
 - More information in the [official documentation](https://doc.starwhale.ai).
@@ -453,12 +468,12 @@
   - Helm Charts on [Artifacthub](https://artifacthub.io/packages/helm/starwhale/starwhale).
   - Docker Images on [Docker Hub](https://hub.docker.com/u/starwhaleai), [Github Packages](https://github.com/orgs/star-whale/packages) and [Starwhale Registry](https://docker-registry.starwhale.cn/).
 
 - Additionally, you can always find us at *developer@starwhale.ai*.
 
 ## Contributing
 
-🌼👏**PRs are always welcomed** 👍🍺. See [Contribution to Starwhale](https://doc.starwhale.ai/docs/community/contribute) for more details.
+🌼👏**PRs are always welcomed** 👍🍺. See [Contribution to Starwhale](https://doc.starwhale.ai/community/contribute) for more details.
 
 ## License
 
 Starwhale is licensed under the [Apache License 2.0](https://github.com/star-whale/starwhale/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.5.6 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.5.7 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -23,68 +23,81 @@
   img.shields.io/pypi/v/starwhale?style=flat] [https://img.shields.io/github/
   license/star-whale/starwhale?style=flat] [PyPI_-_Python_Version] [https://
    github.com/star-whale/starwhale/actions/workflows/client.yaml/badge.svg]
      [https://github.com/star-whale/starwhale/actions/workflows/server-ut-
     report.yml/badge.svg] [https://github.com/star-whale/starwhale/actions/
 workflows/console.yml/badge.svg] [Codecov] [Codecov] [Artifact_Hub] [Starwhale
                                    E2E_Test]
-## What is Starwhale Starwhale is an MLOps platform. It provides **Instance**,
-**Project**, **Runtime**, **Model**, and **Dataset**. - **Instance**: Each
-installation of Starwhale is called an instance. - ð» **Standalone
-Instance**: The simplest form that requires only the Starwhale Client(`swcli`).
-`swcli` is written by pure python3. - ð **On-Premises Instance**: Cloud
-form, we call it **private cloud instance**. Kubernetes and BareMetal both meet
-the basic environmental requirements. - âï¸ **Cloud Hosted Instance**: Cloud
-form, we call it **public cloud instance**. Starwhale team maintains the web
-service. **Starwhale tries to keep concepts consistent across different types
+## What is Starwhale Starwhale is an MLOps/LLMOps platform. It provides
+**Instance**, **Project**, **Runtime**, **Model**, and **Dataset**. -
+**Instance**: Each installation of Starwhale is called an instance. - ð»
+**Starwhale Standalone**: Rather than a running service, Starwhale Standalone
+is actually a repository that resides in your local file system. It is created
+and managed by the Starwhale Client (SWCLI). You only need to install SWCLI to
+use it. Currently, each user on a single machine can have only ONE Starwhale
+Standalone instance. We recommend you use the Starwhale Standalone to build and
+test your datasets, runtime, and models before pushing them to Starwhale
+Server/Cloud instances. - ð **Starwhale Server**: Starwhale Server is a
+service deployed on your local server. Besides text-only results from the
+Starwhale Client (SWCLI), Starwhale Server provides Web UI for you to manage
+your datasets and models, evaluate your models in your local Kubernetes
+cluster, and review the evaluation results. - âï¸ **Starwhale Cloud**:
+Starwhale Cloud is a managed service hosted on public clouds. By registering an
+account on https://cloud.starwhale.cn , you are ready to use Starwhale without
+needing to install, operate, and maintain your own instances. Starwhale Cloud
+also provides public resources for you to download, like datasets, runtimes,
+and models. Check the "starwhale/public" project on Starwhale Cloud for more
+details. **Starwhale tries to keep concepts consistent across different types
 of instances. In this way, people can easily exchange data and migrate between
 them.** - **Project**: The basic unit for organizing different resources. -
 **ML Basic Elements**: The Machine Learning/Deep Learning running environments
 or artifacts. Starwhale empowers the ML/DL essential elements with packaging,
 versioning, reproducibility, and shareability. - ð **Runtime**: Software
-dependencies description to "run" a model, which includes python libraries,
+dependencies description to "run" a model, which includes Python libraries,
 native libraries, native binaries, etc. - ð **Model**: The standard model
 format used in model delivery. - ð« **Dataset**: A unified description of how
 the data and labels are stored and organized. Starwhale datasets can be loaded
 efficiently. - **Running Fundamentals**: Starwhale uses **Job**, **Step**, and
 **Task** to execute ML/DL actions like model trainingï¼ evaluation, and
 serving. Starwhale's **Controller-Agents** structure scales out easily. - ð¥
 **Job**: A set of programs to do specific work. Each job consists of one or
 more steps. - ðµ **Step**: Represents distinct stages of the work. Each step
 consists of one or more tasks. - ð¥ **Task**: Operation entity. Tasks are in
 some specific steps. - **Scenarios**: Starwhale provides the best practice and
 out-of-the-box for different ML/DL scenarios. - ð **Model Training(WIP)**:
 Use Starwhale Python SDK to record experiment meta, metric, log, and artifact.
 - ð¥ï¸ **Model Evaluation**: `PipelineHandler` and some report decorators
 can give you complete, helpful, and user-friendly evaluation reports with only
-a few lines of codes. - ð« **Model Serving(TBD)**: Starwhale Model can be
+a few lines of code. - ð« **Model Serving(TBD)**: Starwhale Model can be
 deployed as a web service or stream service in production with deployment
 capability, observability, and scalability. Data scientists do not need to
-write ML/DL irrelevant codes. ## MNIST Quick Tour for the standalone instance
-### Use Notebook - You can try it in [Google Colab](https://
-colab.research.google.com/github/star-whale/starwhale/blob/main/example/mnist/
-notebook.ipynb) - Or run [example/mnist/notebook.ipynb](example/mnist/
-notebook.ipynb) locally using [vscode](https://code.visualstudio.com/) or
-[jupyterlab](https://github.com/jupyterlab/jupyterlab) ### Use your own python
-env ![Core Job Workflow](docs/docs/img/standalone-core-workflow.gif) - ð°
-**STEP1**: Installing Starwhale ```bash python3 -m pip install starwhale ``` -
-ðµ **STEP2**: Downloading the MNIST example > To save time in the example
-downloading, we skip git-lfs and other commits info. ```bash
-GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/star-whale/starwhale.git --
-depth 1 cd starwhale ``` - â **STEP3**: Building a runtime > When you first
-build runtime, creating an isolated python environment and downloading python
-dependencies will take a lot of time. The command execution time is related to
-the network environment of the machine and the number of packages in the
-runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/
-pip.conf` file is a recommended practice. > > For users in the mainland of
-China, the following conf file is an option: > > ```conf > [global] > cache-dir
-= ~/.cache/pip > index-url = https://mirrors.aliyun.com/pypi/simple/ > extra-
-index-url = https://pypi.doubanio.com/simple > ``` ```bash swcli runtime build
-example/runtime/pytorch swcli runtime list swcli runtime info pytorch/version/
-latest ``` - ð **STEP4**: Building a model - Download pre-trained model
+write ML/DL irrelevant codes. ## MNIST Quick Tour for the Starwhale Standalone
+Instance ### Use Notebook - You can try it in [Google Colab](https://
+colab.research.google.com/github/star-whale/starwhale/blob/main/example/
+notebooks/quickstart-standalone.ipynb) - Or run [quickstart example](example/
+notebooks/quickstart-standalone.ipynb) locally using [vscode](https://
+code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/
+jupyterlab) ### Use your own Python env ![Core Job Workflow](https://
+doc.starwhale.ai/assets/images/standalone-core-workflow-
+270ac0f0cb5b20dbe5ccd11727e2620b.gif) - ð° **STEP1**: Installing Starwhale
+```bash python3 -m pip install starwhale ``` - ðµ **STEP2**: Downloading the
+MNIST example > To save time in the example downloading, we skip git-lfs and
+other commits info. ```bash GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/
+star-whale/starwhale.git --depth 1 cd starwhale ``` - â **STEP3**: Building a
+runtime > When you first build runtime, creating an isolated python environment
+and downloading python dependencies will take a lot of time. The command
+execution time is related to the network environment of the machine and the
+number of packages in the runtime.yaml. Using the befitting pypi mirror and
+cache config in the `~/.pip/pip.conf` file is a recommended practice. > > For
+users in the mainland of China, the following conf file is an option: > >
+```conf > [global] > cache-dir = ~/.cache/pip > index-url = https://
+pypi.tuna.tsinghua.edu.cn/simple > extra-index-url = https://
+mirrors.aliyun.com/pypi/simple/ > ``` ```bash swcli runtime build --yaml
+example/runtime/pytorch/runtime.yaml swcli runtime list swcli runtime info
+pytorch ``` - ð **STEP4**: Building a model - Download pre-trained model
 file: ```bash cd example/mnist make download-model # For users in the mainland
 of China, please add `CN=1` environment for make command: # CN=1 make download-
 model cd - ``` - [Code Example]Write some code with Starwhale Python SDK.
 Complete code is [here](https://github.com/star-whale/starwhale/blob/main/
 example/mnist/mnist/evaluator.py). ```python import typing as t import torch
 from starwhale import Image, PipelineHandler, multi_classification class
 MNISTInference(PipelineHandler): def __init__(self) -> None: super().__init__()
@@ -99,55 +112,54 @@
 [] for _data in ppl_result: label.append(_data["input"]["label"]) result.append
 (_data["output"][0]) pr.append(_data["output"][1]) return label, result, pr def
 _pre(self, input:bytes): """write some mnist preprocessing code""" def _post
 (self, input:bytes): """write some mnist post-processing code""" def
 _load_model(): """load your pre trained model""" ``` - [Code Example]Define
 `model.yaml`. ```yaml name: mnist run: handler: mnist.evaluator:MNISTInference
 ``` - Run one command to build the model. ```bash swcli model build example/
-mnist --runtime pytorch/version/latest swcli model list swcli model info mnist/
-version/latest ``` - ðº **STEP5**: Building a dataset - Download MNIST RAW
-data files. ```bash cd example/mnist make download-data # For users in the
-mainland of China, please add `CN=1` environment for make command: # CN=1 make
-download-data cd - ``` - [Code Example]Write some code with Starwhale Python
-SDK. Full code is [here](https://github.com/star-whale/starwhale/blob/main/
-example/mnist/mnist/dataset.py). ```python import struct from pathlib import
-Path from starwhale import GrayscaleImage def iter_swds_bin_item(): root_dir =
-Path(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
+mnist --runtime pytorch swcli model list swcli model info mnist ``` - ðº
+**STEP5**: Building a dataset - Download MNIST RAW data files. ```bash cd
+example/mnist make download-data # For users in the mainland of China, please
+add `CN=1` environment for make command: # CN=1 make download-data cd - ``` -
+[Code Example]Write some code with Starwhale Python SDK. Full code is [here]
+(https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/
+dataset.py). ```python import struct from pathlib import Path from starwhale
+import GrayscaleImage def iter_swds_bin_item(): root_dir = Path
+(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
 ubyte").open("rb") as data_file, ( root_dir / "t10k-labels-idx1-ubyte" ).open
 ("rb") as label_file: _, data_number, height, width = struct.unpack(">IIII",
 data_file.read(16)) _, label_number = struct.unpack(">II", label_file.read(8))
 print( f">data({data_file.name}) split data:{data_number}, label:{label_number}
 group" ) image_size = height * width for i in range(0, min(data_number,
 label_number)): _data = data_file.read(image_size) _label = struct.unpack(">B",
 label_file.read(1))[0] yield { "img": GrayscaleImage( _data, display_name=f"
 {i}", shape=(height, width, 1), ), "label": _label, } ``` - Run one command to
-build the dataset. ```bash swcli dataset build example/mnist --handler
-mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest swcli dataset
-info mnist/version/latest swcli dataset head mnist/version/latest ``` Starwhale
-also supports build dataset with pure python sdk. You can try it in [Google
+build the dataset. ```bash swcli dataset build --yaml example/mnist/
+dataset.yaml swcli dataset info mnist swcli dataset head mnist ``` Starwhale
+also supports building datasets with pure Python SDK. You can try it in [Google
 Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/
 example/notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation
-job ```bash swcli eval run --model mnist/version/latest --dataset mnist/
-version/latest --runtime pytorch/version/latest swcli eval list swcli eval info
-$(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
-``` **ð Now, you have completed the fundamental steps for Starwhale
-standalone. Let's go ahead and finish the tutorial on the on-premises
-instance.** ## MNIST Quick Tour for on-premises instance ![Create Job Workflow]
-(docs/docs/img/console-create-job.gif) - ð° **STEP1**: Install minikube and
-helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm]
-(https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube
-```bash minikube start --addons ingress ``` > For users in the mainland of
-China, please add some external parameters. The following command was well
-tested; you may also try another kubernetes version. > > ```bash > minikube
-start --addons ingress --image-mirror-country=cn --kubernetes-version=1.25.3 >
-``` If there is no kubectl bin in your machine, you may use `minikube kubectl`
-or `alias kubectl="minikube kubectl --"` alias command. - ðµ **STEP3**:
-Installing Starwhale ```bash helm repo add starwhale https://star-
-whale.github.io/charts helm repo update helm pull starwhale/starwhale --untar -
--untardir ./charts helm upgrade --install starwhale ./charts/starwhale -
+job ```bash swcli -vvv model run --uri mnist --dataset mnist --runtime pytorch
+swcli job list swcli job info $(swcli job list | grep mnist | grep success |
+awk '{print $1}' | head -n 1) ``` **ð Now, you have completed the
+fundamental steps for Starwhale standalone. Let's go ahead and finish the
+tutorial on the on-premises instance.** ## MNIST Quick Tour for Starwhale
+Server Instance ![Create Job Workflow](https://doc.starwhale.ai/assets/images/
+console-artifacts-fd7bf6e54d06dc37d234019e769031e6.gif) - ð° **STEP1**:
+Install minikube and helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/
+) 1.25+ - [Helm](https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**:
+Start minikube ```bash minikube start --addons ingress ``` > For users in the
+mainland of China, please add some external parameters. The following command
+was well tested; you may also try another kubernetes version. > > ```bash >
+minikube start --addons ingress --image-mirror-country=cn --kubernetes-
+version=1.25.3 > ``` If there is no kubectl bin in your machine, you may use
+`minikube kubectl` or `alias kubectl="minikube kubectl --"` alias command. -
+ðµ **STEP3**: Installing Starwhale ```bash helm repo add starwhale https://
+star-whale.github.io/charts helm repo update helm pull starwhale/starwhale --
+untar --untardir ./charts helm upgrade --install starwhale ./charts/starwhale -
 n starwhale --create-namespace -f ./charts/starwhale/
 values.minikube.global.yaml ``` > For users in the mainland of China, use
 `values.minikube.global.yaml`. ```bash helm upgrade --install starwhale ./
 charts/starwhale -n starwhale --create-namespace -f ./charts/starwhale/
 values.minikube.cn.yaml ``` After the installation is successful, the following
 prompt message appears: ```bash Release "starwhale" has been upgraded. Happy
 Helming! NAME: starwhale LAST DEPLOYED: Tue Feb 14 16:25:03 2023 NAMESPACE:
@@ -156,55 +168,66 @@
 0.1.0 App Version: latest Starwhale Image: - server: ghcr.io/star-whale/server:
 latest Runtime default Image: - runtime image: ghcr.io/star-whale/starwhale:
 latest ****************************************** Controller: - visit: http://
 controller.starwhale.svc Minio: - web visit: http://minio.starwhale.svc - admin
 visit: http://minio-admin.starwhale.svc MySQL: - port-forward: - run: kubectl
 port-forward --namespace starwhale svc/mysql 3306:3306 - visit: mysql -
 h 127.0.0.1 -P 3306 -ustarwhale -pstarwhale Please run the following command
-for the domains searching: echo "$(minikube ip) controller.starwhale.svc
+for the domains searching: echo "$(sudo minikube ip) controller.starwhale.svc
 minio.starwhale.svc minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
 ****************************************** Login Info: - starwhale: u:
 starwhale, p:abcd1234 - minio admin: u:minioadmin, p:minioadmin *_* Enjoy to
 use Starwhale Platform. *_* ``` Then keep checking the minikube service status
-until all deployments are running. ```bash kubectl get deployments -n starwhale
-``` | NAME | READY | UP-TO-DATE | AVAILABLE | AGE | | ---------- | ----- | ----
------- | --------- | --- | | controller | 1/1 | 1 | 1 | 5m | | minio | 1/1 | 1
-| 1 | 5m | | mysql | 1/1 | 1 | 1 | 5m | Make the Starwhale controller
-accessible locally with the following command: ```bash kubectl port-forward --
-namespace starwhale svc/controller 8082:8082 ``` - â **STEP4**: Upload the
-artifacts to the cloud instance > **pre-prepared artifacts** > Before starting
-this tutorial, the following three artifacts should already exist on your
-machineï¼ > > - a starwhale model named mnist > - a starwhale dataset named
-mnist > - a starwhale runtime named pytorch > > The above three artifacts are
-what we built on our machine using starwhale. 1. Use swcli to operate the
-remote server First, log in to the server: ```bash swcli instance login --
-username starwhale --password abcd1234 --alias dev http://localhost:8082 ``` 2.
-Start copying the model, dataset, and runtime that we constructed earlier:
-```bash swcli model copy mnist/version/latest dev/project/starwhale swcli
-dataset copy mnist/version/latest dev/project/starwhale swcli runtime copy
-pytorch/version/latest dev/project/starwhale ``` - ð **STEP5**: Use the web
-UI to run an evaluation 1. Log in Starwhale instance: let's use the username
-(starwhale) and password(abcd1234) to open the server web UI(
-localhost:8082/>). 2. Then, we will see the project named 'project_for_mnist'
-that we created earlier with swcli. Click the project name, you will see the
-model, runtime, and dataset uploaded in the previous step.  Show the uploaded
-artifacts screenshots ![Console Artifacts](docs/docs/img/console-artifacts.gif)
-3. Create and view an evaluation job  Show create job screenshot ![Console
-Create Job](docs/docs/img/console-create-job.gif)  **ð Congratulations! You
-have completed the evaluation process for a model.** ## Documentation,
-Community, and Support - Visit [Starwhale HomePage](https://starwhale.ai). -
-More information in the [official documentation](https://doc.starwhale.ai). -
-For general questions and support, join the [Slack](https://
-starwhale.slack.com/). - For bug reports and feature requests, please use
-[Github Issue](https://github.com/star-whale/starwhale/issues). - To get
-community updates, follow [@starwhaleai](https://twitter.com/starwhaleai) on
-Twitter. - For Starwhale artifacts, please visit: - Python Package on [Pypi]
-(https://pypi.org/project/starwhale/). - Helm Charts on [Artifacthub](https://
-artifacthub.io/packages/helm/starwhale/starwhale). - Docker Images on [Docker
-Hub](https://hub.docker.com/u/starwhaleai), [Github Packages](https://
-github.com/orgs/star-whale/packages) and [Starwhale Registry](https://docker-
-registry.starwhale.cn/). - Additionally, you can always find us at
-*developer@starwhale.ai*. ## Contributing ð¼ð**PRs are always welcomed**
-ððº. See [Contribution to Starwhale](https://doc.starwhale.ai/docs/
+until all deployments are running(waiting for 3~5 mins). ```bash kubectl get
+deployments -n starwhale ``` | NAME | READY | UP-TO-DATE | AVAILABLE | AGE | |
+---------- | ----- | ---------- | --------- | --- | | controller | 1/1 | 1 | 1
+| 5m | | minio | 1/1 | 1 | 1 | 5m | | mysql | 1/1 | 1 | 1 | 5m | Make the
+Starwhale controller accessible locally with the following command: ```bash
+echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc minio-
+admin.starwhale.svc " | sudo tee -a /etc/hosts ``` Then you can visit http://
+controller.starwhale.svc in your local web browser. If other users also want to
+access Starwhale Server Instance, the following commands maybe help you: - in
+your machine(Linux, Starwhale Server Instance machine): for temporary use with
+socat command: ```bash # install socat at first, ref: https://howtoinstall.co/
+en/socat sudo socat TCP4-LISTEN:80,fork,reuseaddr,bind=0.0.0.0 TCP4:`minikube
+ip`:80 ``` When you kill the socat process, the share access will be blocked.
+`iptables` maybe a better choice for long-term use. - in other users' machines:
+```bash # for macOSX or Linux environment, run the command in the shell. echo $
+{your_machine_ip} controller.starwhale.svc minio.starwhale.svc minio-
+admin.starwhale.svc " | sudo tee -a /etc/hosts # for Windows environment, run
+the command in the PowerShell with administrator permission. Add-Content -Path
+C:\Windows\System32\drivers\etc\hosts -Value "`n${your_machine_ip}
+controller.starwhale.svc minio.starwhale.svc minio-admin.starwhale.svc" ``` -
+â **STEP4**: Upload the artifacts to the cloud instance > **pre-prepared
+artifacts** > Before starting this tutorial, the following three artifacts
+should already exist on your machineï¼ > > - a starwhale model named mnist > -
+a starwhale dataset named mnist > - a starwhale runtime named pytorch > > The
+above three artifacts are what we built on our machine using starwhale. 1. Use
+swcli to operate the remote server First, log in to the server: ```bash swcli
+instance login --username starwhale --password abcd1234 --alias dev http://
+controller.starwhale.svc ``` 2. Start copying the model, dataset, and runtime
+that we constructed earlier: ```bash swcli model copy mnist cloud://dev/
+project/starwhale swcli dataset copy mnist cloud://dev/project/starwhale swcli
+runtime copy pytorch cloud://dev/project/starwhale ``` - ð **STEP5**: Use
+the web UI to run an evaluation 1. Log in Starwhale instance: let's use the
+username(starwhale) and password(abcd1234) to open the server web UI(
+controller.starwhale.svc>). 2. Then, we will see the project named 'starwhale/
+starwhale' that we created earlier with swcli. Click the project name, you will
+see the model, runtime, and dataset uploaded in the previous step. 3. Create
+and view an evaluation job. **ð Congratulations! You have completed the
+evaluation process for a model.** ## Documentation, Community, and Support -
+Visit [Starwhale HomePage](https://starwhale.ai). - More information in the
+[official documentation](https://doc.starwhale.ai). - For general questions and
+support, join the [Slack](https://starwhale.slack.com/). - For bug reports and
+feature requests, please use [Github Issue](https://github.com/star-whale/
+starwhale/issues). - To get community updates, follow [@starwhaleai](https://
+twitter.com/starwhaleai) on Twitter. - For Starwhale artifacts, please visit: -
+Python Package on [Pypi](https://pypi.org/project/starwhale/). - Helm Charts on
+[Artifacthub](https://artifacthub.io/packages/helm/starwhale/starwhale). -
+Docker Images on [Docker Hub](https://hub.docker.com/u/starwhaleai), [Github
+Packages](https://github.com/orgs/star-whale/packages) and [Starwhale Registry]
+(https://docker-registry.starwhale.cn/). - Additionally, you can always find us
+at *developer@starwhale.ai*. ## Contributing ð¼ð**PRs are always
+welcomed** ððº. See [Contribution to Starwhale](https://doc.starwhale.ai/
 community/contribute) for more details. ## License Starwhale is licensed under
 the [Apache License 2.0](https://github.com/star-whale/starwhale/blob/main/
 LICENSE).
```

### Comparing `starwhale-0.5.6/pyproject.toml` & `starwhale-0.5.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     | \.venv
     | __pycache__
     | venv
     | build
     | dist
     | \.history
     | example/LLM/belle-bloom/BELLE
+    | example/LLM/llama2/llama
     | starwhale/proto_gen
   )/
 )
 '''
 
 [tool.mypy]
 exclude = [
@@ -49,8 +50,8 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 length_sort = true
 order_by_type = true
 force_alphabetical_sort_within_sections = true
-extend_skip_glob="../example/LLM/belle-bloom/BELLE/*,starwhale/proto_gen/*"
+extend_skip_glob="*/example/LLM/llama2/llama/*,*/example/LLM/belle-bloom/BELLE/*,starwhale/proto_gen/*,"
```

### Comparing `starwhale-0.5.6/scripts/sw-docker-entrypoint` & `starwhale-0.5.7/scripts/sw-docker-entrypoint`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/setup.py` & `starwhale-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/__init__.py` & `starwhale-0.5.7/starwhale/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/data_store.py` & `starwhale-0.5.7/starwhale/api/_impl/data_store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/dataset/__init__.py` & `starwhale-0.5.7/starwhale/api/_impl/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/dataset/builder/mapping_builder.py` & `starwhale-0.5.7/starwhale/api/_impl/dataset/builder/mapping_builder.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/dataset/loader.py` & `starwhale-0.5.7/starwhale/api/_impl/dataset/loader.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/dataset/model.py` & `starwhale-0.5.7/starwhale/api/_impl/dataset/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/evaluation.py` & `starwhale-0.5.7/starwhale/api/_impl/evaluation.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/experiment.py` & `starwhale-0.5.7/starwhale/api/_impl/experiment.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/job.py` & `starwhale-0.5.7/starwhale/api/_impl/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,17 @@
                     inspect.isclass(v)
                     and issubclass(v, PipelineHandler)
                     and v != PipelineHandler
                 ):
                     # compatible with old version: ppl and cmp function are renamed to predict and evaluate
                     predict_func = getattr(v, "predict", None) or getattr(v, "ppl")
                     evaluate_func = getattr(v, "evaluate", None) or getattr(v, "cmp")
-                    Handler.register(replicas=1, name="predict")(predict_func)
+                    Handler.register(replicas=1, name="predict", require_dataset=True)(
+                        predict_func
+                    )
                     Handler.register(
                         replicas=1,
                         needs=[predict_func],
                         name="evaluate",
                     )(evaluate_func)
 
     @classmethod
```

### Comparing `starwhale-0.5.6/starwhale/api/_impl/metric.py` & `starwhale-0.5.7/starwhale/api/_impl/metric.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/model.py` & `starwhale-0.5.7/starwhale/api/_impl/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/service.py` & `starwhale-0.5.7/starwhale/api/_impl/service.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/track/base.py` & `starwhale-0.5.7/starwhale/api/_impl/track/base.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/track/collector.py` & `starwhale-0.5.7/starwhale/api/_impl/track/collector.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/track/handler.py` & `starwhale-0.5.7/starwhale/api/_impl/track/handler.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/track/hooker.py` & `starwhale-0.5.7/starwhale/api/_impl/track/hooker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/track/tracker.py` & `starwhale-0.5.7/starwhale/api/_impl/track/tracker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/_impl/wrapper.py` & `starwhale-0.5.7/starwhale/api/_impl/wrapper.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/api/dataset.py` & `starwhale-0.5.7/starwhale/api/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/blob/file.py` & `starwhale-0.5.7/starwhale/base/blob/file.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/blob/store.py` & `starwhale-0.5.7/starwhale/base/blob/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/bundle.py` & `starwhale-0.5.7/starwhale/base/bundle.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/bundle_copy.py` & `starwhale-0.5.7/starwhale/base/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/cloud.py` & `starwhale-0.5.7/starwhale/base/cloud.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/cloud_blob_cache.py` & `starwhale-0.5.7/starwhale/base/cloud_blob_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,26 @@
                 _Server(ip) for ip in socket.gethostbyname_ex(_pseudo_host_name)[2]
             ]
             random.shuffle(_servers)
         except Exception:
             _servers = []
 
 
+_index = 0
+
+
 # This module is not thread safe. This function should be invoked by async
 # funtions in the same event loop.
 def replace_url(url: str, replace: bool) -> t.Generator[str, None, None]:
     assert _servers is not None
     result = urlparse(url)
     if len(_servers) == 0 or not replace:
         while True:
             yield url
     else:
         result = result._replace(scheme="http")
-        index = 0
         while True:
+            global _index
+            _index += 1
             yield result._replace(
-                netloc=f"{_servers[index % len(_servers)].ip}:{_cache_server_port}"
+                netloc=f"{_servers[_index % len(_servers)].ip}:{_cache_server_port}"
             ).geturl()
-            index += 1
```

### Comparing `starwhale-0.5.6/starwhale/base/context.py` & `starwhale-0.5.7/starwhale/base/context.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/mixin.py` & `starwhale-0.5.7/starwhale/base/mixin.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/scheduler/__init__.py` & `starwhale-0.5.7/starwhale/base/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/scheduler/dag.py` & `starwhale-0.5.7/starwhale/base/scheduler/dag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/scheduler/step.py` & `starwhale-0.5.7/starwhale/base/scheduler/step.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/scheduler/task.py` & `starwhale-0.5.7/starwhale/base/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/store.py` & `starwhale-0.5.7/starwhale/base/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/tag.py` & `starwhale-0.5.7/starwhale/base/tag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/type.py` & `starwhale-0.5.7/starwhale/base/type.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/uri/exceptions.py` & `starwhale-0.5.7/starwhale/base/uri/exceptions.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/uri/instance.py` & `starwhale-0.5.7/starwhale/base/uri/instance.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/uri/project.py` & `starwhale-0.5.7/starwhale/base/uri/project.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/uri/resource.py` & `starwhale-0.5.7/starwhale/base/uri/resource.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/base/view.py` & `starwhale-0.5.7/starwhale/base/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/__init__.py` & `starwhale-0.5.7/starwhale/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/broker.py` & `starwhale-0.5.7/starwhale/cli/assistance/broker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/cli.py` & `starwhale-0.5.7/starwhale/cli/assistance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/common.py` & `starwhale-0.5.7/starwhale/cli/assistance/common.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/host.py` & `starwhale-0.5.7/starwhale/cli/assistance/host.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/remote.py` & `starwhale-0.5.7/starwhale/cli/assistance/remote.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/assistance/wait_console.py` & `starwhale-0.5.7/starwhale/cli/assistance/wait_console.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/board/board.py` & `starwhale-0.5.7/starwhale/cli/board/board.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/board/project_tree.py` & `starwhale-0.5.7/starwhale/cli/board/project_tree.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/board/widgets.py` & `starwhale-0.5.7/starwhale/cli/board/widgets.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/completion.py` & `starwhale-0.5.7/starwhale/cli/completion.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/cli/mngt.py` & `starwhale-0.5.7/starwhale/cli/mngt.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/consts/__init__.py` & `starwhale-0.5.7/starwhale/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/cli.py` & `starwhale-0.5.7/starwhale/core/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/copy.py` & `starwhale-0.5.7/starwhale/core/dataset/copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/model.py` & `starwhale-0.5.7/starwhale/core/dataset/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/store.py` & `starwhale-0.5.7/starwhale/core/dataset/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/tabular.py` & `starwhale-0.5.7/starwhale/core/dataset/tabular.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/type.py` & `starwhale-0.5.7/starwhale/core/dataset/type.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/dataset/view.py` & `starwhale-0.5.7/starwhale/core/dataset/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/instance/cli.py` & `starwhale-0.5.7/starwhale/core/instance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/instance/view.py` & `starwhale-0.5.7/starwhale/core/instance/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/job/cli.py` & `starwhale-0.5.7/starwhale/core/job/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/job/model.py` & `starwhale-0.5.7/starwhale/core/job/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/job/store.py` & `starwhale-0.5.7/starwhale/core/job/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/job/view.py` & `starwhale-0.5.7/starwhale/core/job/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/model/cli.py` & `starwhale-0.5.7/starwhale/core/model/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/model/copy.py` & `starwhale-0.5.7/starwhale/core/model/copy.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/model/model.py` & `starwhale-0.5.7/starwhale/core/model/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/model/store.py` & `starwhale-0.5.7/starwhale/core/model/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/model/view.py` & `starwhale-0.5.7/starwhale/core/model/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/project/cli.py` & `starwhale-0.5.7/starwhale/core/project/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/project/model.py` & `starwhale-0.5.7/starwhale/core/project/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/project/view.py` & `starwhale-0.5.7/starwhale/core/project/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/cli.py` & `starwhale-0.5.7/starwhale/core/runtime/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/model.py` & `starwhale-0.5.7/starwhale/core/runtime/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/process.py` & `starwhale-0.5.7/starwhale/core/runtime/process.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/store.py` & `starwhale-0.5.7/starwhale/core/runtime/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/template/Dockerfile.tmpl` & `starwhale-0.5.7/starwhale/core/runtime/template/Dockerfile.tmpl`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/core/runtime/view.py` & `starwhale-0.5.7/starwhale/core/runtime/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/integrations/huggingface/dataset.py` & `starwhale-0.5.7/starwhale/integrations/huggingface/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/integrations/pytorch/dataset.py` & `starwhale-0.5.7/starwhale/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/integrations/tensorflow/dataset.py` & `starwhale-0.5.7/starwhale/integrations/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/mngt/__init__.py` & `starwhale-0.5.7/starwhale/mngt/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/proto_gen/model_package_storage_pb2.py` & `starwhale-0.5.7/starwhale/proto_gen/model_package_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/__init__.py` & `starwhale-0.5.7/starwhale/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/cli.py` & `starwhale-0.5.7/starwhale/utils/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/config.py` & `starwhale-0.5.7/starwhale/utils/config.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/console.py` & `starwhale-0.5.7/starwhale/utils/console.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/debug.py` & `starwhale-0.5.7/starwhale/utils/debug.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/dict_util.py` & `starwhale-0.5.7/starwhale/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/docker.py` & `starwhale-0.5.7/starwhale/utils/docker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/error.py` & `starwhale-0.5.7/starwhale/utils/error.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/fs.py` & `starwhale-0.5.7/starwhale/utils/fs.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/http.py` & `starwhale-0.5.7/starwhale/utils/http.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/load.py` & `starwhale-0.5.7/starwhale/utils/load.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/log.py` & `starwhale-0.5.7/starwhale/utils/log.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/process.py` & `starwhale-0.5.7/starwhale/utils/process.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/progress.py` & `starwhale-0.5.7/starwhale/utils/progress.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/retry.py` & `starwhale-0.5.7/starwhale/utils/retry.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/venv.py` & `starwhale-0.5.7/starwhale/utils/venv.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/utils/venv_pack.py` & `starwhale-0.5.7/starwhale/utils/venv_pack.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/data_store.py` & `starwhale-0.5.7/starwhale/web/data_store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/panel.py` & `starwhale-0.5.7/starwhale/web/panel.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/project.py` & `starwhale-0.5.7/starwhale/web/project.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/server.py` & `starwhale-0.5.7/starwhale/web/server.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/BlockLabel-5fb1ba40.js` & `starwhale-0.5.7/starwhale/web/ui/assets/BlockLabel-fe080bcf.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     a6 as p,
     a8 as I,
     a9 as k,
     aa as v,
     ab as z,
     ac as B,
     aI as q
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function C(t) {
     let a, n, s, b, o, r, l;
     return s = new t[1]({}), {
         c() {
             a = u("div"), n = u("span"), h(s.$$.fragment), b = y(), o = w(t[0]), f(n, "class", "mr-2 h-[12px] w-[12px] opacity-80"), f(a, "class", r = "absolute left-0 top-0 py-1 px-2 rounded-br-lg shadow-sm text-xs text-gray-500 flex items-center pointer-events-none bg-white z-20 border-b border-r border-gray-100 dark:bg-gray-900 " + t[3]), c(a, "h-0", !t[2]), c(a, "sr-only", !t[2])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js` & `starwhale-0.5.7/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     ab as X,
     aA as Y,
     ak as Z,
     ai as E,
     aK as y,
     aL as z,
     aM as H
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function F(a) {
     let t, o, e, u, L, f, m = a[2] + 1 + "",
         v, p, d = a[3].length + "",
         _, b, i, r, x, l;
     const w = a[9].default,
         n = D(w, a, a[8], null);
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Column-32430de0.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Column-958ed910.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
     a4 as C,
     ae as q,
     af as S,
     ag as W,
     a9 as X,
     aa as Y,
     ab as Z
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function j(a) {
     let e, t, m, f;
     const o = a[7].default,
         i = w(o, a, a[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/DatasetForm-b1b79ee8.js` & `starwhale-0.5.7/starwhale/web/ui/assets/DatasetForm-45360b60.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,15 @@
     C as Lr,
     D as Br,
     U as zr,
     F as Mr,
     G as Nr,
     H as Ur,
     J as Vr
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 var Ht = {
         onUnhandledError: null,
         onStoppedNotification: null,
         Promise: void 0,
         useDeprecatedSynchronousErrorHandling: !1,
         useDeprecatedNextContext: !1
     },
@@ -2640,15 +2640,15 @@
                 return d(b => [...b, {
                     ...Qe(p.file),
                     status: "uploading"
                 }]), m({
                     method: "PUT",
                     url: p.oss,
                     headers: {
-                        "Content-Type": p.file.type,
+                        "Content-Type": "application/octet-stream",
                         "X-Requested-With": "XMLHttpRequest"
                     },
                     data: p.file,
                     onUploadProgress: b => (d(P => {
                         const F = P.findIndex(re => re.path === p.file.path);
                         if (F === -1) return [...P];
                         const fe = {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/File-0190a4b6.js` & `starwhale-0.5.7/starwhale/web/ui/assets/File-d0f0778c.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     Y as d,
     aw as o,
     a2 as t,
     a4 as f,
     a5 as l,
     ax as r,
     ab as u
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function w(i) {
     let e, a, s;
     return {
         c() {
             e = o("svg"), a = o("path"), s = o("polyline"), t(a, "d", "M13 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V9z"), t(s, "points", "13 2 13 9 20 9"), t(e, "xmlns", "http://www.w3.org/2000/svg"), t(e, "width", "100%"), t(e, "height", "100%"), t(e, "viewBox", "0 0 24 24"), t(e, "fill", "none"), t(e, "stroke", "currentColor"), t(e, "stroke-width", "1.5"), t(e, "stroke-linecap", "round"), t(e, "stroke-linejoin", "round"), t(e, "class", "feather feather-file")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Image-7d3d0587.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Image-953a3e24.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     Y as o,
     Z as _,
     a2 as l,
     ay as n,
     a4 as f,
     ax as c,
     ab as g
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function d(i) {
     let e, s;
     return {
         c() {
             e = _("img"), l(e, "class", "gr-sample-image object-contain h-20 w-20"), n(e.src, s = i[0]) || l(e, "src", s)
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Image2-fef2a6da.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Image2-08f40595.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     Y as d,
     aw as s,
     a2 as e,
     a4 as m,
     a5 as i,
     ax as l,
     ab as u
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function w(c) {
     let t, r, a, n;
     return {
         c() {
             t = s("svg"), r = s("rect"), a = s("circle"), n = s("polyline"), e(r, "x", "3"), e(r, "y", "3"), e(r, "width", "18"), e(r, "height", "18"), e(r, "rx", "2"), e(r, "ry", "2"), e(a, "cx", "8.5"), e(a, "cy", "8.5"), e(a, "r", "1.5"), e(n, "points", "21 15 16 10 5 21"), e(t, "xmlns", "http://www.w3.org/2000/svg"), e(t, "width", "100%"), e(t, "height", "100%"), e(t, "viewBox", "0 0 24 24"), e(t, "fill", "none"), e(t, "stroke", "currentColor"), e(t, "stroke-width", "1.5"), e(t, "stroke-linecap", "round"), e(t, "stroke-linejoin", "round"), e(t, "class", "feather feather-image")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/LogViewer-b5684b3d.css` & `starwhale-0.5.7/starwhale/web/ui/assets/LogViewer-b5684b3d.css`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/LogViewer-ead1dacc.js` & `starwhale-0.5.7/starwhale/web/ui/assets/LogViewer-1215be01.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     M as D,
     N as Xt,
     R as J,
     O as un,
     x as wr,
     v as Or,
     Q as Sr
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 const dn = x.createContext(null),
     ys = x.createContext(null);
 
 function w(...e) {
     const t = [],
         n = {}.hasOwnProperty;
     return e.filter(Boolean).forEach(s => {
@@ -5807,15 +5807,15 @@
     onClose: n,
     onMessage: s
 }) {
     const r = x.useRef(void 0),
         i = x.useRef(void 0);
     x.useEffect(() => {
         const l = {
-            GIT_COMMIT_HASH: '"7c7ff4faabd947e430e924cfeeb8a0c17e57afb8"'
+            GIT_COMMIT_HASH: '"e3eeb75dd0ede013451252d6f333084f0c3b14fc"'
         }.DEBUG ? wr.bind(console.log, console, "[useWebSocket]") : (...m) => {};
         if (l("use effect", e), !e) return;
         i.current && (l("prev closed", i.current), i.current.close());
         const o = new WebSocket(e);
         i.current = o;
         const a = () => {
                 o?.readyState === o?.OPEN && o?.send("ping"), r.current = window.setTimeout(a, 2e3)
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/ModifyUpload-ca14033f.js` & `starwhale-0.5.7/starwhale/web/ui/assets/ModifyUpload-972867fe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     ac as C,
     ak as B,
     ax as f,
     a7 as E,
     aw as g,
     aY as u,
     as as q
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function Y(o) {
     let e, a, t, l, n, r;
     return t = new o[0]({}), {
         c() {
             e = x("button"), a = x("div"), y(t.$$.fragment), s(a, "class", "m-t-1 w-[60%] h-[60%] opacity-80 dark:text-white"), s(e, "class", "text-gray-500 bg-white/90 h-5 w-5 flex items-center justify-center rounded shadow-sm hover:shadow-xl hover:ring-1 ring-inset ring-gray-200 z-10 dark:bg-gray-900 dark:ring-gray-600"), s(e, "aria-label", o[1])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Medium-da0621a9.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplay-updated-Regular-d0b90ff3.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplayVF-updated-ItalicModified-8483eece.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatDisplayVFModified-updated-3a6592a3.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatMono-updated-Regular-1686cd5c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatMonoVF-updated-4cca9c27.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatMonoVF-updated-Italic-ca135ebd.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Medium-702e86ff.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Medium-eb14b046.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Tabs-58551549.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Tabs-0edcf972.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
     an as S,
     bb as G,
     aM as H,
     aL as J,
     $ as B,
     a7 as O,
     a8 as D
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function q(n, e, a) {
     const t = n.slice();
     return t[11] = e[a], t
 }
 
 function P(n) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Upload-5020e3e5.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Upload-699ac090.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     a9 as x,
     aa as $,
     ab as ee,
     aA as le,
     ak as ae,
     as as y,
     av as te
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function ie(a) {
     let l, i, n, m, h, c, o, d, k, w;
     const _ = a[14].default,
         r = K(_, a, a[13], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/Webcam-1d7c84ed.js` & `starwhale-0.5.7/starwhale/web/ui/assets/Webcam-77a82fdc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     av as Ze,
     aw as W,
     ax as I,
     a1 as Gt,
     a6 as qt,
     ac as Ft,
     an as Ke
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function Qe(a) {
     let t, e, i;
     return {
         c() {
             t = W("svg"), e = W("path"), i = W("circle"), p(e, "d", "M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"), p(i, "cx", "12"), p(i, "cy", "13"), p(i, "r", "4"), p(t, "xmlns", "http://www.w3.org/2000/svg"), p(t, "width", "100%"), p(t, "height", "100%"), p(t, "viewBox", "0 0 24 24"), p(t, "fill", "none"), p(t, "stroke", "currentColor"), p(t, "stroke-width", "1.5"), p(t, "stroke-linecap", "round"), p(t, "stroke-linejoin", "round"), p(t, "class", "feather feather-camera")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/account2-668f906e.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/account2-668f906e.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/dsv-62f8cd07.js` & `starwhale-0.5.7/starwhale/web/ui/assets/dsv-62f8cd07.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/empty-chart-1e62901a.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/empty-chart-1e62901a.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/empty-f3091520.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/empty-f3091520.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/google-9d1a8b2b.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/google-9d1a8b2b.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index-0a9704a2.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index-0ebd961e.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -17,18 +17,18 @@
     aa as k,
     ab as Y,
     ac as Z,
     ad as z,
     ae as D,
     af as E,
     ag as F
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     C as G
-} from "./Column-32430de0.js";
+} from "./Column-958ed910.js";
 
 function H(n) {
     let e;
     const a = n[6].default,
         t = z(a, n, n[7], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index-1d08769b.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index-fa288f1e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     m as Mu,
     bf as F0,
     bg as O0,
     bh as B0,
     V as To,
     L as N0,
     x as U0
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function H0({
     style: Ps = {},
     isLoading: Gl = !1,
     className: d = "",
     children: re,
     loaderType: ne = "spinner",
@@ -9221,15 +9221,15 @@
                             }
                             return J
                         };
                         var T = {},
                             e;
                         ne.debuglog = function(F) {
                             if (c(e) && (e = {
-                                    GIT_COMMIT_HASH: '"7c7ff4faabd947e430e924cfeeb8a0c17e57afb8"'
+                                    GIT_COMMIT_HASH: '"e3eeb75dd0ede013451252d6f333084f0c3b14fc"'
                                 }.NODE_DEBUG || ""), F = F.toUpperCase(), !T[F])
                                 if (new RegExp("\\b" + F + "\\b", "i").test(e)) {
                                     var H = w.pid;
                                     T[F] = function() {
                                         var G = ne.format.apply(ne, arguments);
                                         console.error("%s %d: %s", F, H, G)
                                     }
@@ -61523,15 +61523,15 @@
 
                         function a() {
                             var r;
                             try {
                                 r = ne.storage.debug
                             } catch {}
                             return !r && typeof w < "u" && "env" in w && (r = {
-                                GIT_COMMIT_HASH: '"7c7ff4faabd947e430e924cfeeb8a0c17e57afb8"'
+                                GIT_COMMIT_HASH: '"e3eeb75dd0ede013451252d6f333084f0c3b14fc"'
                             }.DEBUG), r
                         }
                         ne.enable(a());
 
                         function n() {
                             try {
                                 return window.localStorage
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index-54aca6e3.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index-00cfa2a7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -37960,16 +37960,16 @@
         label: "English",
         id: "en"
     }, {
         label: "简体中文",
         id: "zh"
     }],
     dj = "http://127.0.0.1:8007",
-    kUe = "https://doc.starwhale.ai/zh/docs/",
-    zUe = "https://doc.starwhale.ai/docs/",
+    kUe = "https://starwhale.cn/docs",
+    zUe = "https://doc.starwhale.ai",
     jUe = rr({
         mainWrapper: {
             display: "flex",
             flexFlow: "row nowrap",
             justifyContent: "space-between",
             position: "relative",
             flex: "1",
@@ -92516,15 +92516,15 @@
             options: Vne,
             style: {
                 height: "100px"
             }
         })
     })
 }
-const eDt = R.lazy(() => Nt(() => import("./main-6cf1adbb.js").then(e => e.m), []));
+const eDt = R.lazy(() => Nt(() => import("./main-2ed4d8ce.js").then(e => e.m), []));
 
 function C2({
     data: e,
     collapsed: t = 1,
     collapseStringsAfterLength: r = 10,
     style: n = {}
 }) {
@@ -95529,15 +95529,15 @@
             type: "heatmap"
         }],
         layout: {
             ...i
         }
     }
 }
-const IFt = R.lazy(() => Nt(() => import("./index-1d08769b.js"), ["assets/index-1d08769b.js", "assets/index-4b525ef6.css"])),
+const IFt = R.lazy(() => Nt(() => import("./index-fa288f1e.js"), ["assets/index-fa288f1e.js", "assets/index-4b525ef6.css"])),
     RFt = {
         type: "ui:panel:rocauc",
         group: wp.PANEL,
         name: "Roc Auc",
         fieldConfig: {
             schema: {
                 tableName: {},
@@ -95583,15 +95583,15 @@
         children: f.jsx(IFt, {
             data: c
         })
     })
 }
 const FFt = new Iw(DFt, RFt),
     BFt = FFt,
-    WFt = R.lazy(() => Nt(() => import("./index-1d08769b.js"), ["assets/index-1d08769b.js", "assets/index-4b525ef6.css"])),
+    WFt = R.lazy(() => Nt(() => import("./index-fa288f1e.js"), ["assets/index-fa288f1e.js", "assets/index-4b525ef6.css"])),
     qFt = {
         type: "ui:panel:confusion_matrix",
         group: wp.PANEL,
         name: "Confusion Matrix"
     };
 
 function UFt(e) {
@@ -103370,15 +103370,15 @@
     return f.jsx(pn, {
         title: t("Run Model"),
         children: f.jsx(gq, {
             onSubmit: r
         })
     })
 }
-const HUt = R.lazy(() => Nt(() => import("./DatasetForm-b1b79ee8.js"), []));
+const HUt = R.lazy(() => Nt(() => import("./DatasetForm-45360b60.js"), []));
 
 function VUt() {
     const {
         projectId: e,
         datasetId: t
     } = Dr(), {
         query: r
@@ -103619,15 +103619,15 @@
                     job: n,
                     task: c
                 })
             })]
         })]
     })
 }
-const JUt = R.lazy(() => Nt(() => import("./LogViewer-ead1dacc.js"), ["assets/LogViewer-ead1dacc.js", "assets/LogViewer-b5684b3d.css"]));
+const JUt = R.lazy(() => Nt(() => import("./LogViewer-1215be01.js"), ["assets/LogViewer-1215be01.js", "assets/LogViewer-b5684b3d.css"]));
 
 function Hie() {
     const [e] = Ne(), [t, r] = C.useState(void 0), [, n] = C.useState(!1), [i, o] = C.useState({}), a = C.useCallback(async (c, u) => {
         r(u);
         const d = {};
         if ([lA.RUNNING].includes(u.taskStatus)) {
             const m = [u?.stepName, u?.id].join("@");
@@ -113680,53 +113680,53 @@
     mYt = (e, t = gf()) => vwe(e, t),
     bJt = Xg([Gg, Qw], () => dYt);
 Xg([Gg], () => fYt);
 Xg([Gg], () => pYt);
 Xg([Gg], () => hYt);
 Xg([Gg, Qw], () => mYt);
 const gYt = {
-    accordion: () => Nt(() => import("./index-0a9704a2.js"), ["assets/index-0a9704a2.js", "assets/Column-32430de0.js"]),
-    audio: () => Nt(() => import("./index2-040b1a6e.js"), ["assets/index2-040b1a6e.js", "assets/Upload-5020e3e5.js", "assets/ModifyUpload-ca14033f.js", "assets/BlockLabel-5fb1ba40.js", "assets/utils-de54785e.js"]),
-    box: () => Nt(() => import("./index3-3ed81e50.js"), []),
-    button: () => Nt(() => import("./index4-efddfb05.js"), []),
-    carousel: () => Nt(() => import("./index5-a485e343.js"), ["assets/index5-a485e343.js", "assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js"]),
-    carouselitem: () => Nt(() => import("./index6-c4dad8b6.js"), ["assets/index6-c4dad8b6.js", "assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js"]),
-    chatbot: () => Nt(() => import("./index7-c30707d3.js"), ["assets/index7-c30707d3.js", "assets/BlockLabel-5fb1ba40.js"]),
-    checkbox: () => Nt(() => import("./index8-1ed9ba9d.js"), []),
-    checkboxgroup: () => Nt(() => import("./index9-1a9ea67c.js"), []),
-    colorpicker: () => Nt(() => import("./index10-42042dc4.js"), []),
-    column: () => Nt(() => import("./index11-78c7e86b.js"), ["assets/index11-78c7e86b.js", "assets/Column-32430de0.js"]),
-    dataframe: () => Nt(() => import("./index12-ab265665.js"), ["assets/index12-ab265665.js", "assets/Upload-5020e3e5.js", "assets/dsv-62f8cd07.js"]),
-    dataset: () => Nt(() => import("./index13-7c871e80.js"), ["assets/index13-7c871e80.js", "assets/Image-7d3d0587.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js", "assets/Model3D-017f88a9.js"]),
-    dropdown: () => Nt(() => import("./index14-6c615bf9.js"), []),
-    file: () => Nt(() => import("./index15-86a0c1f0.js"), ["assets/index15-86a0c1f0.js", "assets/BlockLabel-5fb1ba40.js", "assets/File-0190a4b6.js", "assets/Upload-5020e3e5.js", "assets/ModifyUpload-ca14033f.js", "assets/utils-de54785e.js"]),
-    form: () => Nt(() => import("./index16-2bdd3a00.js"), []),
-    gallery: () => Nt(() => import("./index17-f009f53c.js"), ["assets/index17-f009f53c.js", "assets/BlockLabel-5fb1ba40.js", "assets/ModifyUpload-ca14033f.js", "assets/utils-de54785e.js", "assets/Image2-fef2a6da.js"]),
-    group: () => Nt(() => import("./index18-b8f18d2d.js"), []),
-    highlightedtext: () => Nt(() => import("./index19-a472c2fd.js"), ["assets/index19-a472c2fd.js", "assets/color-ab3477a6.js", "assets/BlockLabel-5fb1ba40.js"]),
-    html: () => Nt(() => import("./index20-cea79a56.js"), []),
-    image: () => Nt(() => import("./index21-839b404f.js"), ["assets/index21-839b404f.js", "assets/BlockLabel-5fb1ba40.js", "assets/Image2-fef2a6da.js", "assets/Webcam-1d7c84ed.js", "assets/ModifyUpload-ca14033f.js", "assets/Upload-5020e3e5.js", "assets/Image-7d3d0587.js"]),
-    interpretation: () => Nt(() => import("./index22-b0a063e3.js"), []),
-    json: () => Nt(() => import("./index23-2546fc23.js"), ["assets/index23-2546fc23.js", "assets/BlockLabel-5fb1ba40.js"]),
-    label: () => Nt(() => import("./index24-ee89579d.js"), ["assets/index24-ee89579d.js", "assets/BlockLabel-5fb1ba40.js"]),
-    markdown: () => Nt(() => import("./index25-fb12b103.js"), []),
-    model3d: () => Nt(() => import("./index26-70ba7bd9.js"), ["assets/index26-70ba7bd9.js", "assets/utils-de54785e.js", "assets/BlockLabel-5fb1ba40.js", "assets/File-0190a4b6.js", "assets/_commonjsHelpers-23156833.js", "assets/Upload-5020e3e5.js", "assets/ModifyUpload-ca14033f.js", "assets/Model3D-017f88a9.js"]),
-    number: () => Nt(() => import("./index27-202147ca.js"), []),
-    plot: () => Nt(() => import("./index28-4db56c35.js"), ["assets/index28-4db56c35.js", "assets/_commonjsHelpers-23156833.js", "assets/color-ab3477a6.js", "assets/linear-8d973619.js", "assets/dsv-62f8cd07.js", "assets/BlockLabel-5fb1ba40.js"]),
-    radio: () => Nt(() => import("./index29-f4b57e8f.js"), []),
-    row: () => Nt(() => import("./index30-6cfd7268.js"), []),
-    slider: () => Nt(() => import("./index31-feae9916.js"), []),
-    state: () => Nt(() => import("./index32-efa03b40.js"), []),
-    statustracker: () => Nt(() => import("./index33-c77eb4e8.js"), []),
-    tabs: () => Nt(() => import("./index34-74e21fbb.js"), ["assets/index34-74e21fbb.js", "assets/Tabs-58551549.js"]),
-    tabitem: () => Nt(() => import("./index35-76158480.js"), ["assets/index35-76158480.js", "assets/Tabs-58551549.js", "assets/Column-32430de0.js"]),
-    textbox: () => Nt(() => import("./index36-051a9d0c.js"), []),
-    timeseries: () => Nt(() => import("./index37-4dd6b1d2.js"), ["assets/index37-4dd6b1d2.js", "assets/Upload-5020e3e5.js", "assets/ModifyUpload-ca14033f.js", "assets/BlockLabel-5fb1ba40.js", "assets/color-ab3477a6.js", "assets/linear-8d973619.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js"]),
-    uploadbutton: () => Nt(() => import("./index38-42b4b637.js"), []),
-    video: () => Nt(() => import("./index39-4548d90a.js"), ["assets/index39-4548d90a.js", "assets/utils-de54785e.js", "assets/Upload-5020e3e5.js", "assets/ModifyUpload-ca14033f.js", "assets/BlockLabel-5fb1ba40.js", "assets/Webcam-1d7c84ed.js"])
+    accordion: () => Nt(() => import("./index-0ebd961e.js"), ["assets/index-0ebd961e.js", "assets/Column-958ed910.js"]),
+    audio: () => Nt(() => import("./index2-4608846d.js"), ["assets/index2-4608846d.js", "assets/Upload-699ac090.js", "assets/ModifyUpload-972867fe.js", "assets/BlockLabel-fe080bcf.js", "assets/utils-de54785e.js"]),
+    box: () => Nt(() => import("./index3-f722b477.js"), []),
+    button: () => Nt(() => import("./index4-0bc63b4d.js"), []),
+    carousel: () => Nt(() => import("./index5-f4812d85.js"), ["assets/index5-f4812d85.js", "assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js"]),
+    carouselitem: () => Nt(() => import("./index6-aa6ede7c.js"), ["assets/index6-aa6ede7c.js", "assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js"]),
+    chatbot: () => Nt(() => import("./index7-644441a2.js"), ["assets/index7-644441a2.js", "assets/BlockLabel-fe080bcf.js"]),
+    checkbox: () => Nt(() => import("./index8-dfa6b4d6.js"), []),
+    checkboxgroup: () => Nt(() => import("./index9-74c82f9d.js"), []),
+    colorpicker: () => Nt(() => import("./index10-6962b31b.js"), []),
+    column: () => Nt(() => import("./index11-6a6faac8.js"), ["assets/index11-6a6faac8.js", "assets/Column-958ed910.js"]),
+    dataframe: () => Nt(() => import("./index12-d5dc887c.js"), ["assets/index12-d5dc887c.js", "assets/Upload-699ac090.js", "assets/dsv-62f8cd07.js"]),
+    dataset: () => Nt(() => import("./index13-6dafecb5.js"), ["assets/index13-6dafecb5.js", "assets/Image-953a3e24.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js", "assets/Model3D-ff19b927.js"]),
+    dropdown: () => Nt(() => import("./index14-8c46ae7f.js"), []),
+    file: () => Nt(() => import("./index15-7940e50b.js"), ["assets/index15-7940e50b.js", "assets/BlockLabel-fe080bcf.js", "assets/File-d0f0778c.js", "assets/Upload-699ac090.js", "assets/ModifyUpload-972867fe.js", "assets/utils-de54785e.js"]),
+    form: () => Nt(() => import("./index16-583cafad.js"), []),
+    gallery: () => Nt(() => import("./index17-e0f03f64.js"), ["assets/index17-e0f03f64.js", "assets/BlockLabel-fe080bcf.js", "assets/ModifyUpload-972867fe.js", "assets/utils-de54785e.js", "assets/Image2-08f40595.js"]),
+    group: () => Nt(() => import("./index18-85c307e0.js"), []),
+    highlightedtext: () => Nt(() => import("./index19-46ac23c8.js"), ["assets/index19-46ac23c8.js", "assets/color-de3304e0.js", "assets/BlockLabel-fe080bcf.js"]),
+    html: () => Nt(() => import("./index20-61594d37.js"), []),
+    image: () => Nt(() => import("./index21-976d330c.js"), ["assets/index21-976d330c.js", "assets/BlockLabel-fe080bcf.js", "assets/Image2-08f40595.js", "assets/Webcam-77a82fdc.js", "assets/ModifyUpload-972867fe.js", "assets/Upload-699ac090.js", "assets/Image-953a3e24.js"]),
+    interpretation: () => Nt(() => import("./index22-ccb7efe7.js"), []),
+    json: () => Nt(() => import("./index23-680c92d8.js"), ["assets/index23-680c92d8.js", "assets/BlockLabel-fe080bcf.js"]),
+    label: () => Nt(() => import("./index24-597a8e3c.js"), ["assets/index24-597a8e3c.js", "assets/BlockLabel-fe080bcf.js"]),
+    markdown: () => Nt(() => import("./index25-88e85639.js"), []),
+    model3d: () => Nt(() => import("./index26-36e22149.js"), ["assets/index26-36e22149.js", "assets/utils-de54785e.js", "assets/BlockLabel-fe080bcf.js", "assets/File-d0f0778c.js", "assets/_commonjsHelpers-23156833.js", "assets/Upload-699ac090.js", "assets/ModifyUpload-972867fe.js", "assets/Model3D-ff19b927.js"]),
+    number: () => Nt(() => import("./index27-dee2bd12.js"), []),
+    plot: () => Nt(() => import("./index28-a52d95a5.js"), ["assets/index28-a52d95a5.js", "assets/_commonjsHelpers-23156833.js", "assets/color-de3304e0.js", "assets/linear-8d973619.js", "assets/dsv-62f8cd07.js", "assets/BlockLabel-fe080bcf.js"]),
+    radio: () => Nt(() => import("./index29-dd39a343.js"), []),
+    row: () => Nt(() => import("./index30-edf8c102.js"), []),
+    slider: () => Nt(() => import("./index31-2a9aa647.js"), []),
+    state: () => Nt(() => import("./index32-1efd457e.js"), []),
+    statustracker: () => Nt(() => import("./index33-988b470f.js"), []),
+    tabs: () => Nt(() => import("./index34-e9d05f99.js"), ["assets/index34-e9d05f99.js", "assets/Tabs-0edcf972.js"]),
+    tabitem: () => Nt(() => import("./index35-d013c15c.js"), ["assets/index35-d013c15c.js", "assets/Tabs-0edcf972.js", "assets/Column-958ed910.js"]),
+    textbox: () => Nt(() => import("./index36-640baba3.js"), []),
+    timeseries: () => Nt(() => import("./index37-675e963b.js"), ["assets/index37-675e963b.js", "assets/Upload-699ac090.js", "assets/ModifyUpload-972867fe.js", "assets/BlockLabel-fe080bcf.js", "assets/color-de3304e0.js", "assets/linear-8d973619.js", "assets/csv-17a3ae92.js", "assets/dsv-62f8cd07.js"]),
+    uploadbutton: () => Nt(() => import("./index38-8ed1f571.js"), []),
+    video: () => Nt(() => import("./index39-2e025855.js"), ["assets/index39-2e025855.js", "assets/utils-de54785e.js", "assets/Upload-699ac090.js", "assets/ModifyUpload-972867fe.js", "assets/BlockLabel-fe080bcf.js", "assets/Webcam-77a82fdc.js"])
 };
 
 function vYt() {
     const e = $p({}),
         t = [],
         r = [],
         n = new Map,
@@ -118467,15 +118467,15 @@
                     task: u
                 })
             })]
         })]
     })
 }
 var aSe = (e => (e.CREATED = "CREATED", e.UPLOADING = "UPLOADING", e.BUILDING = "BUILDING", e.SUCCESS = "SUCCESS", e.FAILED = "FAILED", e))(aSe || {});
-const jZt = R.lazy(() => Nt(() => import("./LogViewer-ead1dacc.js"), ["assets/LogViewer-ead1dacc.js", "assets/LogViewer-b5684b3d.css"]));
+const jZt = R.lazy(() => Nt(() => import("./LogViewer-1215be01.js"), ["assets/LogViewer-1215be01.js", "assets/LogViewer-b5684b3d.css"]));
 
 function NZt() {
     const [e] = Ne(), [t, r] = C.useState(void 0), [, n] = C.useState(!1), [i, o] = C.useState({}), a = C.useCallback(async (c, u) => {
         r(u);
         const d = {},
             p = [u?.datasetName, u?.id].join("@");
         if ([aSe.BUILDING].includes(u.status)) d[p] = "ws";
@@ -118957,15 +118957,15 @@
                 })
             })
         })
     })
 }
 window.g = null;
 window.i = null;
-console.log('"7c7ff4faabd947e430e924cfeeb8a0c17e57afb8"');
+console.log('"e3eeb75dd0ede013451252d6f333084f0c3b14fc"');
 async function XZt() {
     return {}
 }
 async function GZt() {
     const {
         authed: e,
         unauthed: t,
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index-c467f321.css` & `starwhale-0.5.7/starwhale/web/ui/assets/index-c467f321.css`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index10-42042dc4.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index10-6962b31b.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
     a2 as y,
     a5 as T,
     aT as j,
     a7 as I,
     ak as J,
     $ as K,
     a8 as L
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function M(a) {
     let e;
     return {
         c() {
             e = K(a[1])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index12-ab265665.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index12-d5dc887c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -33,18 +33,18 @@
     aW as oe,
     ar as fe,
     aw as ve,
     aT as Ae,
     as as De,
     an as ol,
     aP as fl
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     U as dl
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     d as cl
 } from "./dsv-62f8cd07.js";
 var Le = Object.prototype.hasOwnProperty;
 
 function te(r, e) {
     var l, t;
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index13-7c871e80.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index13-6dafecb5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26,27 +26,27 @@
     a1 as X,
     a6 as Z,
     ac as G,
     av as Me,
     aA as ge,
     ay as Q,
     aH as U
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     E as je
-} from "./Image-7d3d0587.js";
+} from "./Image-953a3e24.js";
 import {
     c as Ae
 } from "./csv-17a3ae92.js";
 import {
     d as Ce
 } from "./dsv-62f8cd07.js";
 import {
     E as Ee
-} from "./Model3D-017f88a9.js";
+} from "./Model3D-ff19b927.js";
 var Te = Ce("	"),
     ze = Te.parseRows;
 
 function Le(r) {
     let e, t;
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index14-6c615bf9.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index14-8c46ae7f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     a_ as E,
     a7 as O,
     aE as P,
     ak as Q,
     $ as W,
     a8 as X,
     a$ as U
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function S(t, l, a) {
     const n = t.slice();
     return n[7] = l[a], n
 }
 
 function V(t) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index15-86a0c1f0.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index15-7940e50b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -29,27 +29,27 @@
     ax as T,
     av as Q,
     aB as R,
     aC as V,
     $ as y,
     a8 as E,
     aE as x
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as $
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     F as Y
-} from "./File-0190a4b6.js";
+} from "./File-d0f0778c.js";
 import {
     U as ee
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     M as de
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     n as be
 } from "./utils-de54785e.js";
 const me = f => {
         let e = ["B", "KB", "MB", "GB", "PB"],
             i = 0;
         for (; f > 1024;) f /= 1024, i++;
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index17-f009f53c.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index17-e0f03f64.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -31,27 +31,27 @@
     ax as V,
     ay as R,
     aY as K,
     aE as ae,
     aA as qe,
     $ as oe,
     a8 as se
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as De
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     M as Le
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     n as O
 } from "./utils-de54785e.js";
 import {
     I as X
-} from "./Image2-fef2a6da.js";
+} from "./Image2-08f40595.js";
 
 function P(t, e, l) {
     const i = t.slice();
     return i[30] = e[l][0], i[31] = e[l][1], i[33] = l, i
 }
 
 function Q(t, e, l) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index18-b8f18d2d.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index18-85c307e0.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     a4 as g,
     ae as v,
     af as b,
     ag as h,
     a9 as C,
     aa as G,
     ab as p
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function q(l) {
     let s, a;
     const o = l[3].default,
         t = m(o, l, l[2], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index19-a472c2fd.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index19-46ac23c8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -28,21 +28,21 @@
     aE as Q,
     aY as N,
     $ as B,
     a8 as S,
     a7 as E,
     aA as de,
     a3 as R
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     g as me
-} from "./color-ab3477a6.js";
+} from "./color-de3304e0.js";
 import {
     B as ge
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 
 function he(r) {
     let e, n, l;
     return {
         c() {
             e = q("svg"), n = q("path"), l = q("path"), c(n, "fill", "currentColor"), c(n, "d", "M12 15H5a3 3 0 0 1-3-3v-2a3 3 0 0 1 3-3h5V5a1 1 0 0 0-1-1H3V2h6a3 3 0 0 1 3 3zM5 9a1 1 0 0 0-1 1v2a1 1 0 0 0 1 1h5V9zm15 14v2a1 1 0 0 0 1 1h5v-4h-5a1 1 0 0 0-1 1z"), c(l, "fill", "currentColor"), c(l, "d", "M2 30h28V2Zm26-2h-7a3 3 0 0 1-3-3v-2a3 3 0 0 1 3-3h5v-2a1 1 0 0 0-1-1h-6v-2h6a3 3 0 0 1 3 3Z"), c(e, "xmlns", "http://www.w3.org/2000/svg"), c(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), c(e, "aria-hidden", "true"), c(e, "role", "img"), c(e, "class", "iconify iconify--carbon"), c(e, "width", "100%"), c(e, "height", "100%"), c(e, "preserveAspectRatio", "xMidYMid meet"), c(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index2-040b1a6e.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index2-4608846d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,24 +40,24 @@
     aD as Ve,
     aE as _l,
     aF as Nl,
     $ as U,
     a8 as N,
     aG as Ol,
     aH as de
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     U as Kl
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     M as Yl
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     B as dl
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     n as jl
 } from "./utils-de54785e.js";
 
 function zl(l) {
     let e, i, a, n;
     return {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index20-cea79a56.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index20-61594d37.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     a3 as o,
     a4 as k,
     ao as Y,
     ap as Z,
     ab as T,
     as as z,
     ax as M
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function A(i) {
     let e;
     return {
         c() {
             e = q("div"), c(e, "class", "output-html"), c(e, "id", i[0]), o(e, "min-h-[6rem]", i[3]), o(e, "!hidden", !i[2])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index21-839b404f.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index21-976d330c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -44,38 +44,38 @@
     b2 as Ke,
     aY as Je,
     b3 as St,
     aA as pt,
     aT as Re,
     b4 as Rt,
     b5 as $e
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as wt
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     I as Ee
-} from "./Image2-fef2a6da.js";
+} from "./Image2-08f40595.js";
 import {
     W as Et,
     C as Dt,
     i as Lt,
     U as Ut
-} from "./Webcam-1d7c84ed.js";
+} from "./Webcam-77a82fdc.js";
 import {
     M as Le,
     I as De,
     C as Nt
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     U as qt
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     E as Wn
-} from "./Image-7d3d0587.js";
+} from "./Image-953a3e24.js";
 
 function Ft(t) {
     let e, n, i;
     return {
         c() {
             e = J("svg"), n = J("path"), i = J("path"), d(n, "d", "M28.828 3.172a4.094 4.094 0 0 0-5.656 0L4.05 22.292A6.954 6.954 0 0 0 2 27.242V30h2.756a6.952 6.952 0 0 0 4.95-2.05L28.828 8.829a3.999 3.999 0 0 0 0-5.657zM10.91 18.26l2.829 2.829l-2.122 2.121l-2.828-2.828zm-2.619 8.276A4.966 4.966 0 0 1 4.756 28H4v-.759a4.967 4.967 0 0 1 1.464-3.535l1.91-1.91l2.829 2.828zM27.415 7.414l-12.261 12.26l-2.829-2.828l12.262-12.26a2.047 2.047 0 0 1 2.828 0a2 2 0 0 1 0 2.828z"), d(n, "fill", "currentColor"), d(i, "d", "M6.5 15a3.5 3.5 0 0 1-2.475-5.974l3.5-3.5a1.502 1.502 0 0 0 0-2.121a1.537 1.537 0 0 0-2.121 0L3.415 5.394L2 3.98l1.99-1.988a3.585 3.585 0 0 1 4.95 0a3.504 3.504 0 0 1 0 4.949L5.439 10.44a1.502 1.502 0 0 0 0 2.121a1.537 1.537 0 0 0 2.122 0l4.024-4.024L13 9.95l-4.025 4.024A3.475 3.475 0 0 1 6.5 15z"), d(i, "fill", "currentColor"), d(e, "width", "100%"), d(e, "height", "100%"), d(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index22-b0a063e3.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index22-ccb7efe7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     aw as z,
     a3 as O,
     $ as j,
     a8 as S,
     ay as U,
     aO as ge,
     av as W
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 const w = i => {
         var e = null;
         return i < 0 ? e = [52, 152, 219] : e = [231, 76, 60], _e(de(Math.abs(i), [255, 255, 255], e))
     },
     de = (i, e, t) => {
         i > 1 && (i = 1), i = Math.sqrt(i);
         var n = [0, 0, 0],
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index23-2546fc23.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index23-680c92d8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,18 +32,18 @@
     at as ae,
     aZ as se,
     b6 as ce,
     b5 as I,
     b7 as fe,
     a3 as X,
     aE as Q
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as ue
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 
 function _e(c) {
     let e, t;
     return {
         c() {
             e = q("svg"), t = q("path"), d(t, "fill", "currentColor"), d(t, "d", "M5 3h2v2H5v5a2 2 0 0 1-2 2a2 2 0 0 1 2 2v5h2v2H5c-1.07-.27-2-.9-2-2v-4a2 2 0 0 0-2-2H0v-2h1a2 2 0 0 0 2-2V5a2 2 0 0 1 2-2m14 0a2 2 0 0 1 2 2v4a2 2 0 0 0 2 2h1v2h-1a2 2 0 0 0-2 2v4a2 2 0 0 1-2 2h-2v-2h2v-5a2 2 0 0 1 2-2a2 2 0 0 1-2-2V5h-2V3h2m-7 12a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1m-4 0a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1m8 0a1 1 0 0 1 1 1a1 1 0 0 1-1 1a1 1 0 0 1-1-1a1 1 0 0 1 1-1Z"), d(e, "xmlns", "http://www.w3.org/2000/svg"), d(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), d(e, "aria-hidden", "true"), d(e, "role", "img"), d(e, "class", "iconify iconify--mdi"), d(e, "width", "100%"), d(e, "height", "100%"), d(e, "preserveAspectRatio", "xMidYMid meet"), d(e, "viewBox", "0 0 24 24")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index24-ee89579d.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index24-597a8e3c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -25,18 +25,18 @@
     ax as H,
     aw as I,
     $ as Z,
     a3 as C,
     aY as N,
     a8 as S,
     aE as $
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as ee
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 
 function le(i) {
     let e, n;
     return {
         c() {
             e = I("svg"), n = I("path"), _(n, "fill", "currentColor"), _(n, "d", "M4 2H2v26a2 2 0 0 0 2 2h26v-2H4v-3h22v-8H4v-4h14V5H4Zm20 17v4H4v-4ZM16 7v4H4V7Z"), _(e, "xmlns", "http://www.w3.org/2000/svg"), _(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), _(e, "aria-hidden", "true"), _(e, "role", "img"), _(e, "class", "iconify iconify--carbon"), _(e, "width", "100%"), _(e, "height", "100%"), _(e, "preserveAspectRatio", "xMidYMid meet"), _(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index25-fb12b103.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index25-88e85639.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
     ao as E,
     ap as W,
     ab as w,
     as as X,
     aY as Z,
     ax as M,
     av as z
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function A(n) {
     let e;
     return {
         c() {
             e = S("div"), c(e, "id", n[0]), c(e, "class", "output-markdown gr-prose"), Z(e, "max-width", "100%"), f(e, "min-h-[6rem]", n[3]), f(e, "hidden", !n[1])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index26-70ba7bd9.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index26-36e22149.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -30,36 +30,36 @@
     a2 as Lo,
     a5 as ou,
     ax as Do,
     aB as wv,
     aC as Fv,
     $ as Io,
     a8 as iu
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     n as Bv
 } from "./utils-de54785e.js";
 import {
     B as Od
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     F as du
-} from "./File-0190a4b6.js";
+} from "./File-d0f0778c.js";
 import {
     c as Qi
 } from "./_commonjsHelpers-23156833.js";
 import {
     U as Uv
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     M as Vv
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     E as _b
-} from "./Model3D-017f88a9.js";
+} from "./Model3D-ff19b927.js";
 var Gr = {
     exports: {}
 };
 (function(dt, Ze) {
     (function(Ie, y) {
         dt.exports = y()
     })(typeof self < "u" ? self : typeof Qi < "u" ? Qi : Qi, function() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index27-202147ca.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index27-dee2bd12.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     a7 as y,
     b4 as R,
     aA as J,
     ak as K,
     $ as L,
     a8 as M,
     aU as O
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function P(l) {
     let e;
     return {
         c() {
             e = L(l[2])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index28-4db56c35.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index28-a52d95a5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -31,23 +31,23 @@
     Z as Gh,
     ay as wD,
     $ as FZ,
     a8 as NZ,
     aB as BZ,
     aC as jZ,
     ak as UZ
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     c as Ro,
     a as Qx,
     g as VZ
 } from "./_commonjsHelpers-23156833.js";
 import {
     g as qZ
-} from "./color-ab3477a6.js";
+} from "./color-de3304e0.js";
 import {
     d as yC,
     e as xC,
     _ as VN,
     b as Hw,
     f as eS,
     p as HZ,
@@ -104,15 +104,15 @@
     a2 as dJ
 } from "./linear-8d973619.js";
 import {
     d as pJ
 } from "./dsv-62f8cd07.js";
 import {
     B as gJ
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 var mJ = Object.defineProperty,
     vJ = Object.defineProperties,
     yJ = Object.getOwnPropertyDescriptors,
     SD = Object.getOwnPropertySymbols,
     xJ = Object.prototype.hasOwnProperty,
     bJ = Object.prototype.propertyIsEnumerable,
     ED = (t, n, e) => n in t ? mJ(t, n, {
@@ -188970,15 +188970,15 @@
     YL = {
         SEMVER_SPEC_VERSION: rTe,
         MAX_LENGTH: iTe,
         MAX_SAFE_INTEGER: aTe,
         MAX_SAFE_COMPONENT_LENGTH: oTe
     },
     sTe = typeof process == "object" && {
-        GIT_COMMIT_HASH: '"7c7ff4faabd947e430e924cfeeb8a0c17e57afb8"'
+        GIT_COMMIT_HASH: '"e3eeb75dd0ede013451252d6f333084f0c3b14fc"'
     } && {}.NODE_DEBUG && /\bsemver\b/i.test({}.NODE_DEBUG) ? function() {
         for (var t = arguments.length, n = new Array(t), e = 0; e < t; e++) n[e] = arguments[e];
         return console.error("SEMVER", ...n)
     } : () => {},
     qT = sTe;
 (function(t, n) {
     var e = YL.MAX_SAFE_COMPONENT_LENGTH,
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index29-f4b57e8f.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index29-dd39a343.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     ak as L,
     aI as N,
     $ as M,
     a8 as O,
     a3 as T,
     a5 as k,
     a7 as P
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function j(n, e, t) {
     const l = n.slice();
     return l[11] = e[t], l[13] = t, l
 }
 
 function Q(n) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index3-3ed81e50.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index3-f722b477.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     a9 as f,
     aa as c,
     ac as g,
     ad as p,
     ae as v,
     af as $,
     ag as h
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function k(n) {
     let s;
     const a = n[2].default,
         e = p(a, n, n[3], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index30-6cfd7268.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index30-edf8c102.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     a4 as v,
     ae as q,
     af as b,
     ag as w,
     a9 as C,
     aa as R,
     ab as S
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function W(s) {
     let e, t;
     const u = s[5].default,
         l = c(u, s, s[4], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index31-feae9916.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index31-2a9aa647.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     aT as S,
     a7 as B,
     b4 as D,
     aA as N,
     ak as O,
     $ as P,
     a8 as Q
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function U(a) {
     let e;
     return {
         c() {
             e = P(a[5])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index34-74e21fbb.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index34-e9d05f99.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -12,18 +12,18 @@
     ac as C,
     ak as q,
     ad as w,
     ae as B,
     af as D,
     ag as E,
     as as S
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     T as W
-} from "./Tabs-58551549.js";
+} from "./Tabs-0edcf972.js";
 
 function X(s) {
     let e;
     const l = s[3].default,
         t = w(l, s, s[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index35-76158480.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index35-d013c15c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,21 +18,21 @@
     a4 as E,
     ab as I,
     ak as J,
     aJ as M,
     ai as U,
     aX as W,
     aU as Z
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     a as j
-} from "./Tabs-58551549.js";
+} from "./Tabs-0edcf972.js";
 import {
     C as z
-} from "./Column-32430de0.js";
+} from "./Column-958ed910.js";
 
 function F(s) {
     let a;
     const n = s[5].default,
         t = w(n, s, s[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index37-4dd6b1d2.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index37-675e963b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,27 +32,27 @@
     aX as Se,
     aY as X,
     aQ as G,
     az as Be,
     aH as Te,
     aZ as Ne,
     b1 as Xe
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     U as Fe
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     M as Ue
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     B as Ye
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     g as De
-} from "./color-ab3477a6.js";
+} from "./color-de3304e0.js";
 import {
     l as J,
     _ as K,
     o as x
 } from "./linear-8d973619.js";
 import {
     a as He
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index38-42b4b637.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index38-8ed1f571.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     a7 as R,
     ae as V,
     af as p,
     ag as x,
     aA as $,
     aI as ee,
     av as te
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function le(l) {
     let e, i, n, u, c, o, r, f, b, m;
     const y = l[13].default,
         _ = N(y, l, l[12], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index39-4548d90a.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index39-2e025855.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -39,31 +39,31 @@
     a7 as C,
     aD as fe,
     b3 as Ve,
     aA as Ce,
     bd as Me,
     be as Ue,
     aU as Xe
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     n as qe
 } from "./utils-de54785e.js";
 import {
     U as ze
-} from "./Upload-5020e3e5.js";
+} from "./Upload-699ac090.js";
 import {
     M as Fe
-} from "./ModifyUpload-ca14033f.js";
+} from "./ModifyUpload-972867fe.js";
 import {
     B as be
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 import {
     W as Pe,
     U as De
-} from "./Webcam-1d7c84ed.js";
+} from "./Webcam-77a82fdc.js";
 
 function Se(n) {
     let e, l;
     return {
         c() {
             e = R("svg"), l = R("path"), c(l, "d", "M8 3H5a2 2 0 0 0-2 2v3m18 0V5a2 2 0 0 0-2-2h-3m0 18h3a2 2 0 0 0 2-2v-3M3 16v3a2 2 0 0 0 2 2h3"), c(e, "xmlns", "http://www.w3.org/2000/svg"), c(e, "width", "100%"), c(e, "height", "100%"), c(e, "viewBox", "0 0 24 24"), c(e, "fill", "none"), c(e, "stroke", "currentColor"), c(e, "stroke-width", "1.5"), c(e, "stroke-linecap", "round"), c(e, "stroke-linejoin", "round")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index4-efddfb05.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index4-0bc63b4d.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
     a2 as c,
     a3 as m,
     a7 as Y,
     ae as Z,
     af as A,
     ag as D,
     aI as E
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function F(n) {
     let e, a, t, i, f;
     const r = n[7].default,
         s = S(r, n, n[6], null);
     return {
         c() {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index5-a485e343.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index5-f4812d85.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -15,18 +15,18 @@
     ao as S,
     ap as j,
     ae as q,
     af as T,
     ag as W,
     ab as X,
     as as Y
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     C as z
-} from "./CarouselItem.svelte_svelte_type_style_lang-1aa90835.js";
+} from "./CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js";
 
 function A(l) {
     let s, o, t;
     const i = [l[2]];
     let r = {};
     for (let e = 0; e < i.length; e += 1) r = v(r, i[e]);
     s = new C({
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index6-c4dad8b6.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index6-aa6ede7c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,18 +19,18 @@
     a5 as q,
     ab as y,
     aJ as J,
     ai as L,
     at as O,
     $ as R,
     a8 as U
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     a as W
-} from "./CarouselItem.svelte_svelte_type_style_lang-1aa90835.js";
+} from "./CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js";
 
 function p(a) {
     let t, n;
     return {
         c() {
             t = w("div"), n = R(a[0]), I(t, "class", "absolute left-0 top-0 py-1 px-2 rounded-br-lg shadow-sm text-xs text-gray-500 flex items-center pointer-events-none bg-white z-20 dark:bg-gray-800")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index7-c30707d3.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index7-644441a2.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -26,18 +26,18 @@
     ak as D,
     aN as I,
     aO as P,
     aw as M,
     av as Q,
     aP as W,
     aQ as j
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 import {
     B as X
-} from "./BlockLabel-5fb1ba40.js";
+} from "./BlockLabel-fe080bcf.js";
 
 function F(n) {
     let e, s, t;
     return {
         c() {
             e = M("svg"), s = M("path"), t = M("path"), _(s, "fill", "currentColor"), _(s, "d", "M17.74 30L16 29l4-7h6a2 2 0 0 0 2-2V8a2 2 0 0 0-2-2H6a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h9v2H6a4 4 0 0 1-4-4V8a4 4 0 0 1 4-4h20a4 4 0 0 1 4 4v12a4 4 0 0 1-4 4h-4.84Z"), _(t, "fill", "currentColor"), _(t, "d", "M8 10h16v2H8zm0 6h10v2H8z"), _(e, "xmlns", "http://www.w3.org/2000/svg"), _(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), _(e, "aria-hidden", "true"), _(e, "role", "img"), _(e, "class", "iconify iconify--carbon"), _(e, "width", "100%"), _(e, "height", "100%"), _(e, "preserveAspectRatio", "xMidYMid meet"), _(e, "viewBox", "0 0 32 32")
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index8-1ed9ba9d.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index8-dfa6b4d6.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     a2 as d,
     a3 as B,
     a5 as m,
     a7 as J,
     a8 as K,
     ax as S,
     ak as L
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function M(n) {
     let e, t, a, i, c, r, f;
     return {
         c() {
             e = g("label"), t = g("input"), a = y(), i = g("span"), c = I(n[2]), t.disabled = n[1], t.checked = n[0], d(t, "type", "checkbox"), d(t, "name", "test"), d(t, "class", "gr-check-radio gr-checkbox"), d(i, "class", "ml-2"), d(e, "class", "flex items-center text-gray-700 text-sm space-x-2 rounded-lg cursor-pointer dark:bg-transparent "), B(e, "!cursor-not-allowed", n[1])
         },
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/index9-1a9ea67c.js` & `starwhale-0.5.7/starwhale/web/ui/assets/index9-74c82f9d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     ak as M,
     aI as N,
     $ as I,
     a8 as O,
     a3 as S,
     a5 as k,
     a7 as P
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function T(l, e, t) {
     const a = l.slice();
     return a[10] = e[t], a
 }
 
 function Q(l) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/invalid-file-82d62dec.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/invalid-file-82d62dec.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/left-8c88a49a.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/left-8c88a49a.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/linear-8d973619.js` & `starwhale-0.5.7/starwhale/web/ui/assets/linear-8d973619.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/logo_small_en_white-782559aa.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/main-6cf1adbb.js` & `starwhale-0.5.7/starwhale/web/ui/assets/main-2ed4d8ce.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     L as Ct,
     r as St,
     V as wt
-} from "./index-54aca6e3.js";
+} from "./index-00cfa2a7.js";
 
 function At(rt, pt) {
     for (var Ye = 0; Ye < pt.length; Ye++) {
         const o = pt[Ye];
         if (typeof o != "string" && !Array.isArray(o)) {
             for (const n in o)
                 if (n !== "default" && !(n in rt)) {
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/module-ddaca3b9.js` & `starwhale-0.5.7/starwhale/web/ui/assets/module-ddaca3b9.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/module2-74df381a.js` & `starwhale-0.5.7/starwhale/web/ui/assets/module2-74df381a.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/module3-49e9a615.js` & `starwhale-0.5.7/starwhale/web/ui/assets/module3-49e9a615.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-452a631f.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-452a631f.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-613313c8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-648ba0e7.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-italic-33533562.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extrabold-italic-a258578a.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-64fbbd3d.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-f053be7c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-italic-6cbe5597.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-extralight-italic-d23afde2.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-5e0869ee.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-c7e67c68.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-italic-8f5fbf20.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-heavy-italic-c702fef1.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-italic-34df3d81.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-italic-b81a6146.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-italic-b81a6146.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-3f8151f4.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-3f8151f4.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-9db6ab0a.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-italic-a1454ca5.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-light-italic-ec333948.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-bold-2bf715ff.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-bold-9b29c79a.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-light-5bae063c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-light-7fbe3706.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-regular-95881615.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-regular-a13dec50.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-semibold-085fb4a8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-mono-semibold-b39c5174.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-regular-16b63547.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-regular-16b63547.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-regular-8e2261df.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-3d06895e.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-ec5809e8.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-italic-1935eb14.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-semibold-italic-ae706d8c.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-6feca5dc.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-e85966f1.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-italic-2dffa092.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/overpass-thin-italic-44db8e3d.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_2000-1f17de55.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_576-1d76d6cc.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_576@2x-4942ea78.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_768-8bc3cc8a.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_768@2x-037bce76.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg` & `starwhale-0.5.7/starwhale/web/ui/assets/pfbg_992@2x-9dfd9687.jpg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pficon-0a333dac.woff` & `starwhale-0.5.7/starwhale/web/ui/assets/pficon-0a333dac.woff`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/pficon-86c74539.woff2` & `starwhale-0.5.7/starwhale/web/ui/assets/pficon-86c74539.woff2`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/project-863f66b0.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/project-863f66b0.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/right-aefe3c24.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/right-aefe3c24.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/search-empty-13cbde15.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/search-empty-13cbde15.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/setting-6d098443.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/setting-6d098443.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/status-icon-sprite-bc89cb14.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/web-vitals-d4fac006.js` & `starwhale-0.5.7/starwhale/web/ui/assets/web-vitals-d4fac006.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/assets/wechat-cffee157.svg` & `starwhale-0.5.7/starwhale/web/ui/assets/wechat-cffee157.svg`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/favicon.ico` & `starwhale-0.5.7/starwhale/web/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/favicon_white.ico` & `starwhale-0.5.7/starwhale/web/ui/favicon_white.ico`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/iconfont.js` & `starwhale-0.5.7/starwhale/web/ui/iconfont.js`

 * *Files identical despite different names*

### Comparing `starwhale-0.5.6/starwhale/web/ui/index.html` & `starwhale-0.5.7/starwhale/web/ui/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       Only files inside the `public` folder can be referenced from the HTML.
 
       Unlike "/favicon.ico" or "favicon.ico", "%PUBLIC_URL%/favicon.ico" will
       work correctly both with client-side routing and a non-root public URL.
       Learn how to configure a non-root public URL by running `npm run build`.
     -->
         <title>Starwhale Console</title>
-      <script type="module" crossorigin src="/assets/index-54aca6e3.js"></script>
+      <script type="module" crossorigin src="/assets/index-00cfa2a7.js"></script>
       <link rel="stylesheet" href="/assets/index-c467f321.css">
     </head>
     <body>
         <noscript>You need to enable JavaScript to run this app.</noscript>
         <div id="root"></div>
         <!--
       This HTML file is a template.
```

### Comparing `starwhale-0.5.6/starwhale/web/ui/manifest.json` & `starwhale-0.5.7/starwhale/web/ui/manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8324661085257824%*

 * *Differences: {"'_BlockLabel-fe080bcf.js'": "OrderedDict([('file', 'assets/BlockLabel-fe080bcf.js'), ('imports', "*

 * *                              "['index.html'])])",*

 * * "'_CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js'": "OrderedDict([('file', "*

 * *                                                              "'assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js'), "*

 * *                                                              "('imports', ['index.html'])])",*

 * * "'_Column-958ed910.js'": "OrderedDict([('file' […]*

```diff
@@ -1,79 +1,79 @@
 {
-    "_BlockLabel-5fb1ba40.js": {
-        "file": "assets/BlockLabel-5fb1ba40.js",
+    "_BlockLabel-fe080bcf.js": {
+        "file": "assets/BlockLabel-fe080bcf.js",
         "imports": [
             "index.html"
         ]
     },
-    "_CarouselItem.svelte_svelte_type_style_lang-1aa90835.js": {
-        "file": "assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js",
+    "_CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js": {
+        "file": "assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Column-32430de0.js": {
-        "file": "assets/Column-32430de0.js",
+    "_Column-958ed910.js": {
+        "file": "assets/Column-958ed910.js",
         "imports": [
             "index.html"
         ]
     },
-    "_File-0190a4b6.js": {
-        "file": "assets/File-0190a4b6.js",
+    "_File-d0f0778c.js": {
+        "file": "assets/File-d0f0778c.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Image-7d3d0587.js": {
-        "file": "assets/Image-7d3d0587.js",
+    "_Image-953a3e24.js": {
+        "file": "assets/Image-953a3e24.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Image2-fef2a6da.js": {
-        "file": "assets/Image2-fef2a6da.js",
+    "_Image2-08f40595.js": {
+        "file": "assets/Image2-08f40595.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Model3D-017f88a9.js": {
-        "file": "assets/Model3D-017f88a9.js",
+    "_Model3D-ff19b927.js": {
+        "file": "assets/Model3D-ff19b927.js",
         "imports": [
             "index.html"
         ]
     },
-    "_ModifyUpload-ca14033f.js": {
-        "file": "assets/ModifyUpload-ca14033f.js",
+    "_ModifyUpload-972867fe.js": {
+        "file": "assets/ModifyUpload-972867fe.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Tabs-58551549.js": {
-        "file": "assets/Tabs-58551549.js",
+    "_Tabs-0edcf972.js": {
+        "file": "assets/Tabs-0edcf972.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Upload-5020e3e5.js": {
-        "file": "assets/Upload-5020e3e5.js",
+    "_Upload-699ac090.js": {
+        "file": "assets/Upload-699ac090.js",
         "imports": [
             "index.html"
         ]
     },
-    "_Webcam-1d7c84ed.js": {
-        "file": "assets/Webcam-1d7c84ed.js",
+    "_Webcam-77a82fdc.js": {
+        "file": "assets/Webcam-77a82fdc.js",
         "imports": [
             "index.html"
         ]
     },
     "__commonjsHelpers-23156833.js": {
         "file": "assets/_commonjsHelpers-23156833.js"
     },
-    "_color-ab3477a6.js": {
-        "file": "assets/color-ab3477a6.js",
+    "_color-de3304e0.js": {
+        "file": "assets/color-de3304e0.js",
         "imports": [
             "index.html"
         ]
     },
     "_csv-17a3ae92.js": {
         "file": "assets/csv-17a3ae92.js",
         "imports": [
@@ -82,16 +82,16 @@
     },
     "_dsv-62f8cd07.js": {
         "file": "assets/dsv-62f8cd07.js"
     },
     "_linear-8d973619.js": {
         "file": "assets/linear-8d973619.js"
     },
-    "_main-6cf1adbb.js": {
-        "file": "assets/main-6cf1adbb.js",
+    "_main-2ed4d8ce.js": {
+        "file": "assets/main-2ed4d8ce.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true
     },
     "_module2-74df381a.js": {
         "file": "assets/module2-74df381a.js"
@@ -131,15 +131,15 @@
             "assets/iconfont-10b60b11.ttf"
         ],
         "css": [
             "assets/index-c467f321.css"
         ],
         "dynamicImports": [
             "node_modules/web-vitals/dist/web-vitals.js",
-            "_main-6cf1adbb.js",
+            "_main-2ed4d8ce.js",
             "packages/starwhale-ui/src/Plotly/index.ts",
             "packages/starwhale-ui/src/Plotly/index.ts",
             "src/domain/dataset/components/DatasetForm.tsx",
             "src/components/LogViewer/LogViewer.tsx",
             "src/assets/GradioWidget/es/index.js",
             "src/assets/GradioWidget/es/index2.js",
             "src/assets/GradioWidget/es/index3.js",
@@ -177,15 +177,15 @@
             "src/assets/GradioWidget/es/index35.js",
             "src/assets/GradioWidget/es/index36.js",
             "src/assets/GradioWidget/es/index37.js",
             "src/assets/GradioWidget/es/index38.js",
             "src/assets/GradioWidget/es/index39.js",
             "src/components/LogViewer/LogViewer.tsx"
         ],
-        "file": "assets/index-54aca6e3.js",
+        "file": "assets/index-00cfa2a7.js",
         "isEntry": true,
         "src": "index.html"
     },
     "node_modules/@patternfly/react-core/dist/styles/assets/fonts/RedHatDisplay/RedHatDisplay-Bold.woff": {
         "file": "assets/RedHatDisplay-Bold-44214a55.woff",
         "src": "node_modules/@patternfly/react-core/dist/styles/assets/fonts/RedHatDisplay/RedHatDisplay-Bold.woff"
     },
@@ -526,392 +526,392 @@
         "file": "assets/index-4b525ef6.css",
         "src": "packages/starwhale-ui/src/Plotly/index.css"
     },
     "packages/starwhale-ui/src/Plotly/index.ts": {
         "css": [
             "assets/index-4b525ef6.css"
         ],
-        "file": "assets/index-1d08769b.js",
+        "file": "assets/index-fa288f1e.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "packages/starwhale-ui/src/Plotly/index.ts"
     },
     "src/assets/GradioWidget/es/index.js": {
-        "file": "assets/index-0a9704a2.js",
+        "file": "assets/index-0ebd961e.js",
         "imports": [
             "index.html",
-            "_Column-32430de0.js"
+            "_Column-958ed910.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index.js"
     },
     "src/assets/GradioWidget/es/index10.js": {
-        "file": "assets/index10-42042dc4.js",
+        "file": "assets/index10-6962b31b.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index10.js"
     },
     "src/assets/GradioWidget/es/index11.js": {
-        "file": "assets/index11-78c7e86b.js",
+        "file": "assets/index11-6a6faac8.js",
         "imports": [
-            "_Column-32430de0.js",
+            "_Column-958ed910.js",
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index11.js"
     },
     "src/assets/GradioWidget/es/index12.js": {
-        "file": "assets/index12-ab265665.js",
+        "file": "assets/index12-d5dc887c.js",
         "imports": [
             "index.html",
-            "_Upload-5020e3e5.js",
+            "_Upload-699ac090.js",
             "_dsv-62f8cd07.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index12.js"
     },
     "src/assets/GradioWidget/es/index13.js": {
-        "file": "assets/index13-7c871e80.js",
+        "file": "assets/index13-6dafecb5.js",
         "imports": [
             "index.html",
-            "_Image-7d3d0587.js",
+            "_Image-953a3e24.js",
             "_csv-17a3ae92.js",
             "_dsv-62f8cd07.js",
-            "_Model3D-017f88a9.js"
+            "_Model3D-ff19b927.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index13.js"
     },
     "src/assets/GradioWidget/es/index14.js": {
-        "file": "assets/index14-6c615bf9.js",
+        "file": "assets/index14-8c46ae7f.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index14.js"
     },
     "src/assets/GradioWidget/es/index15.js": {
-        "file": "assets/index15-86a0c1f0.js",
+        "file": "assets/index15-7940e50b.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js",
-            "_File-0190a4b6.js",
-            "_Upload-5020e3e5.js",
-            "_ModifyUpload-ca14033f.js",
+            "_BlockLabel-fe080bcf.js",
+            "_File-d0f0778c.js",
+            "_Upload-699ac090.js",
+            "_ModifyUpload-972867fe.js",
             "_utils-de54785e.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index15.js"
     },
     "src/assets/GradioWidget/es/index16.js": {
-        "file": "assets/index16-2bdd3a00.js",
+        "file": "assets/index16-583cafad.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index16.js"
     },
     "src/assets/GradioWidget/es/index17.js": {
-        "file": "assets/index17-f009f53c.js",
+        "file": "assets/index17-e0f03f64.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js",
-            "_ModifyUpload-ca14033f.js",
+            "_BlockLabel-fe080bcf.js",
+            "_ModifyUpload-972867fe.js",
             "_utils-de54785e.js",
-            "_Image2-fef2a6da.js"
+            "_Image2-08f40595.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index17.js"
     },
     "src/assets/GradioWidget/es/index18.js": {
-        "file": "assets/index18-b8f18d2d.js",
+        "file": "assets/index18-85c307e0.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index18.js"
     },
     "src/assets/GradioWidget/es/index19.js": {
-        "file": "assets/index19-a472c2fd.js",
+        "file": "assets/index19-46ac23c8.js",
         "imports": [
             "index.html",
-            "_color-ab3477a6.js",
-            "_BlockLabel-5fb1ba40.js"
+            "_color-de3304e0.js",
+            "_BlockLabel-fe080bcf.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index19.js"
     },
     "src/assets/GradioWidget/es/index2.js": {
         "dynamicImports": [
             "src/assets/GradioWidget/es/module.js",
             "src/assets/GradioWidget/es/module3.js"
         ],
-        "file": "assets/index2-040b1a6e.js",
+        "file": "assets/index2-4608846d.js",
         "imports": [
             "index.html",
-            "_Upload-5020e3e5.js",
-            "_ModifyUpload-ca14033f.js",
-            "_BlockLabel-5fb1ba40.js",
+            "_Upload-699ac090.js",
+            "_ModifyUpload-972867fe.js",
+            "_BlockLabel-fe080bcf.js",
             "_utils-de54785e.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index2.js"
     },
     "src/assets/GradioWidget/es/index20.js": {
-        "file": "assets/index20-cea79a56.js",
+        "file": "assets/index20-61594d37.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index20.js"
     },
     "src/assets/GradioWidget/es/index21.js": {
-        "file": "assets/index21-839b404f.js",
+        "file": "assets/index21-976d330c.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js",
-            "_Image2-fef2a6da.js",
-            "_Webcam-1d7c84ed.js",
-            "_ModifyUpload-ca14033f.js",
-            "_Upload-5020e3e5.js",
-            "_Image-7d3d0587.js"
+            "_BlockLabel-fe080bcf.js",
+            "_Image2-08f40595.js",
+            "_Webcam-77a82fdc.js",
+            "_ModifyUpload-972867fe.js",
+            "_Upload-699ac090.js",
+            "_Image-953a3e24.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index21.js"
     },
     "src/assets/GradioWidget/es/index22.js": {
-        "file": "assets/index22-b0a063e3.js",
+        "file": "assets/index22-ccb7efe7.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index22.js"
     },
     "src/assets/GradioWidget/es/index23.js": {
-        "file": "assets/index23-2546fc23.js",
+        "file": "assets/index23-680c92d8.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js"
+            "_BlockLabel-fe080bcf.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index23.js"
     },
     "src/assets/GradioWidget/es/index24.js": {
-        "file": "assets/index24-ee89579d.js",
+        "file": "assets/index24-597a8e3c.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js"
+            "_BlockLabel-fe080bcf.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index24.js"
     },
     "src/assets/GradioWidget/es/index25.js": {
-        "file": "assets/index25-fb12b103.js",
+        "file": "assets/index25-88e85639.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index25.js"
     },
     "src/assets/GradioWidget/es/index26.js": {
-        "file": "assets/index26-70ba7bd9.js",
+        "file": "assets/index26-36e22149.js",
         "imports": [
             "index.html",
             "_utils-de54785e.js",
-            "_BlockLabel-5fb1ba40.js",
-            "_File-0190a4b6.js",
+            "_BlockLabel-fe080bcf.js",
+            "_File-d0f0778c.js",
             "__commonjsHelpers-23156833.js",
-            "_Upload-5020e3e5.js",
-            "_ModifyUpload-ca14033f.js",
-            "_Model3D-017f88a9.js"
+            "_Upload-699ac090.js",
+            "_ModifyUpload-972867fe.js",
+            "_Model3D-ff19b927.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index26.js"
     },
     "src/assets/GradioWidget/es/index27.js": {
-        "file": "assets/index27-202147ca.js",
+        "file": "assets/index27-dee2bd12.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index27.js"
     },
     "src/assets/GradioWidget/es/index28.js": {
-        "file": "assets/index28-4db56c35.js",
+        "file": "assets/index28-a52d95a5.js",
         "imports": [
             "index.html",
             "__commonjsHelpers-23156833.js",
-            "_color-ab3477a6.js",
+            "_color-de3304e0.js",
             "_linear-8d973619.js",
             "_dsv-62f8cd07.js",
-            "_BlockLabel-5fb1ba40.js"
+            "_BlockLabel-fe080bcf.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index28.js"
     },
     "src/assets/GradioWidget/es/index29.js": {
-        "file": "assets/index29-f4b57e8f.js",
+        "file": "assets/index29-dd39a343.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index29.js"
     },
     "src/assets/GradioWidget/es/index3.js": {
-        "file": "assets/index3-3ed81e50.js",
+        "file": "assets/index3-f722b477.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index3.js"
     },
     "src/assets/GradioWidget/es/index30.js": {
-        "file": "assets/index30-6cfd7268.js",
+        "file": "assets/index30-edf8c102.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index30.js"
     },
     "src/assets/GradioWidget/es/index31.js": {
-        "file": "assets/index31-feae9916.js",
+        "file": "assets/index31-2a9aa647.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index31.js"
     },
     "src/assets/GradioWidget/es/index32.js": {
-        "file": "assets/index32-efa03b40.js",
+        "file": "assets/index32-1efd457e.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index32.js"
     },
     "src/assets/GradioWidget/es/index33.js": {
-        "file": "assets/index33-c77eb4e8.js",
+        "file": "assets/index33-988b470f.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index33.js"
     },
     "src/assets/GradioWidget/es/index34.js": {
-        "file": "assets/index34-74e21fbb.js",
+        "file": "assets/index34-e9d05f99.js",
         "imports": [
             "index.html",
-            "_Tabs-58551549.js"
+            "_Tabs-0edcf972.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index34.js"
     },
     "src/assets/GradioWidget/es/index35.js": {
-        "file": "assets/index35-76158480.js",
+        "file": "assets/index35-d013c15c.js",
         "imports": [
             "index.html",
-            "_Tabs-58551549.js",
-            "_Column-32430de0.js"
+            "_Tabs-0edcf972.js",
+            "_Column-958ed910.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index35.js"
     },
     "src/assets/GradioWidget/es/index36.js": {
-        "file": "assets/index36-051a9d0c.js",
+        "file": "assets/index36-640baba3.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index36.js"
     },
     "src/assets/GradioWidget/es/index37.js": {
-        "file": "assets/index37-4dd6b1d2.js",
+        "file": "assets/index37-675e963b.js",
         "imports": [
             "index.html",
-            "_Upload-5020e3e5.js",
-            "_ModifyUpload-ca14033f.js",
-            "_BlockLabel-5fb1ba40.js",
-            "_color-ab3477a6.js",
+            "_Upload-699ac090.js",
+            "_ModifyUpload-972867fe.js",
+            "_BlockLabel-fe080bcf.js",
+            "_color-de3304e0.js",
             "_linear-8d973619.js",
             "_csv-17a3ae92.js",
             "_dsv-62f8cd07.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index37.js"
     },
     "src/assets/GradioWidget/es/index38.js": {
-        "file": "assets/index38-42b4b637.js",
+        "file": "assets/index38-8ed1f571.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index38.js"
     },
     "src/assets/GradioWidget/es/index39.js": {
-        "file": "assets/index39-4548d90a.js",
+        "file": "assets/index39-2e025855.js",
         "imports": [
             "index.html",
             "_utils-de54785e.js",
-            "_Upload-5020e3e5.js",
-            "_ModifyUpload-ca14033f.js",
-            "_BlockLabel-5fb1ba40.js",
-            "_Webcam-1d7c84ed.js"
+            "_Upload-699ac090.js",
+            "_ModifyUpload-972867fe.js",
+            "_BlockLabel-fe080bcf.js",
+            "_Webcam-77a82fdc.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index39.js"
     },
     "src/assets/GradioWidget/es/index4.js": {
-        "file": "assets/index4-efddfb05.js",
+        "file": "assets/index4-0bc63b4d.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index4.js"
     },
     "src/assets/GradioWidget/es/index5.js": {
-        "file": "assets/index5-a485e343.js",
+        "file": "assets/index5-f4812d85.js",
         "imports": [
             "index.html",
-            "_CarouselItem.svelte_svelte_type_style_lang-1aa90835.js"
+            "_CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index5.js"
     },
     "src/assets/GradioWidget/es/index6.js": {
-        "file": "assets/index6-c4dad8b6.js",
+        "file": "assets/index6-aa6ede7c.js",
         "imports": [
             "index.html",
-            "_CarouselItem.svelte_svelte_type_style_lang-1aa90835.js"
+            "_CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index6.js"
     },
     "src/assets/GradioWidget/es/index7.js": {
-        "file": "assets/index7-c30707d3.js",
+        "file": "assets/index7-644441a2.js",
         "imports": [
             "index.html",
-            "_BlockLabel-5fb1ba40.js"
+            "_BlockLabel-fe080bcf.js"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index7.js"
     },
     "src/assets/GradioWidget/es/index8.js": {
-        "file": "assets/index8-1ed9ba9d.js",
+        "file": "assets/index8-dfa6b4d6.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index8.js"
     },
     "src/assets/GradioWidget/es/index9.js": {
-        "file": "assets/index9-1a9ea67c.js",
+        "file": "assets/index9-74c82f9d.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/assets/GradioWidget/es/index9.js"
     },
     "src/assets/GradioWidget/es/module.js": {
@@ -1049,23 +1049,23 @@
             "assets/pficon-86c74539.woff2",
             "assets/pficon-0a333dac.woff",
             "assets/status-icon-sprite-bc89cb14.svg"
         ],
         "css": [
             "assets/LogViewer-b5684b3d.css"
         ],
-        "file": "assets/LogViewer-ead1dacc.js",
+        "file": "assets/LogViewer-1215be01.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/components/LogViewer/LogViewer.tsx"
     },
     "src/domain/dataset/components/DatasetForm.tsx": {
-        "file": "assets/DatasetForm-b1b79ee8.js",
+        "file": "assets/DatasetForm-45360b60.js",
         "imports": [
             "index.html"
         ],
         "isDynamicEntry": true,
         "src": "src/domain/dataset/components/DatasetForm.tsx"
     }
 }
```

### Comparing `starwhale-0.5.6/starwhale.egg-info/PKG-INFO` & `starwhale-0.5.7/starwhale.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.5.6
+Version: 0.5.7
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,50 +86,50 @@
     <img src='https://github.com/star-whale/starwhale/actions/workflows/e2e-test.yml/badge.svg' alt='Starwhale E2E Test'>
 </a>
 
 </p>
 
 ## What is Starwhale
 
-Starwhale is an MLOps platform. It provides **Instance**, **Project**, **Runtime**, **Model**, and **Dataset**.
+Starwhale is an MLOps/LLMOps platform. It provides **Instance**, **Project**, **Runtime**, **Model**, and **Dataset**.
 
 - **Instance**: Each installation of Starwhale is called an instance.
-  - 👻 **Standalone Instance**: The simplest form that requires only the Starwhale Client(`swcli`). `swcli` is written by pure python3.
-  - 🎍 **On-Premises Instance**: Cloud form, we call it **private cloud instance**. Kubernetes and BareMetal both meet the basic environmental requirements.
-  - ☁️ **Cloud Hosted Instance**: Cloud form, we call it **public cloud instance**. Starwhale team maintains the web service.
+  - 👻 **Starwhale Standalone**:  Rather than a running service, Starwhale Standalone is actually a repository that resides in your local file system. It is created and managed by the Starwhale Client (SWCLI). You only need to install SWCLI to use it. Currently, each user on a single machine can have only ONE Starwhale Standalone instance. We recommend you use the Starwhale Standalone to build and test your datasets, runtime, and models before pushing them to Starwhale Server/Cloud instances.
+  - 🎍 **Starwhale Server**:  Starwhale Server is a service deployed on your local server. Besides text-only results from the Starwhale Client (SWCLI), Starwhale Server provides Web UI for you to manage your datasets and models, evaluate your models in your local Kubernetes cluster, and review the evaluation results.
+  - ☁️ **Starwhale Cloud**: Starwhale Cloud is a managed service hosted on public clouds. By registering an account on https://cloud.starwhale.cn , you are ready to use Starwhale without needing to install, operate, and maintain your own instances. Starwhale Cloud also provides public resources for you to download, like datasets, runtimes, and models. Check the "starwhale/public" project on Starwhale Cloud for more details.
 
   **Starwhale tries to keep concepts consistent across different types of instances. In this way, people can easily exchange data and migrate between them.**
 
 - **Project**: The basic unit for organizing different resources.
 
 - **ML Basic Elements**: The Machine Learning/Deep Learning running environments or artifacts. Starwhale empowers the ML/DL essential elements with packaging, versioning, reproducibility, and shareability.
-  - 🐌 **Runtime**: Software dependencies description to "run" a model, which includes python libraries, native libraries, native binaries, etc.
+  - 🐌 **Runtime**: Software dependencies description to "run" a model, which includes Python libraries, native libraries, native binaries, etc.
   - 🐇 **Model**: The standard model format used in model delivery.
   - 🐫 **Dataset**: A unified description of how the data and labels are stored and organized. Starwhale datasets can be loaded efficiently.
 
 - **Running Fundamentals**: Starwhale uses **Job**, **Step**, and **Task** to execute ML/DL actions like model training， evaluation, and serving. Starwhale's **Controller-Agents** structure scales out easily.
   - 🥕 **Job**: A set of programs to do specific work. Each job consists of one or more steps.
   - 🌵 **Step**: Represents distinct stages of the work. Each step consists of one or more tasks.
   - 🥑 **Task**: Operation entity. Tasks are in some specific steps.
 
 - **Scenarios**: Starwhale provides the best practice and out-of-the-box for different ML/DL scenarios.
   - 🚝 **Model Training(WIP)**: Use Starwhale Python SDK to record experiment meta, metric, log, and artifact.
-  - 🛥️ **Model Evaluation**: `PipelineHandler` and some report decorators can give you complete, helpful, and user-friendly evaluation reports with only a few lines of codes.
+  - 🛥️ **Model Evaluation**: `PipelineHandler` and some report decorators can give you complete, helpful, and user-friendly evaluation reports with only a few lines of code.
   - 🛫 **Model Serving(TBD)**: Starwhale Model can be deployed as a web service or stream service in production with deployment capability, observability, and scalability. Data scientists do not need to write ML/DL irrelevant codes.
 
-## MNIST Quick Tour for the standalone instance
+## MNIST Quick Tour for the Starwhale Standalone Instance
 
 ### Use Notebook
 
-- You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/mnist/notebook.ipynb)
-- Or run [example/mnist/notebook.ipynb](example/mnist/notebook.ipynb) locally using [vscode](https://code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/jupyterlab)
+- You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/quickstart-standalone.ipynb)
+- Or run [quickstart example](example/notebooks/quickstart-standalone.ipynb) locally using [vscode](https://code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/jupyterlab)
 
-### Use your own python env
+### Use your own Python env
 
-![Core Job Workflow](docs/docs/img/standalone-core-workflow.gif)
+![Core Job Workflow](https://doc.starwhale.ai/assets/images/standalone-core-workflow-270ac0f0cb5b20dbe5ccd11727e2620b.gif)
 
 - 🍰 **STEP1**: Installing Starwhale
 
     ```bash
     python3 -m pip install starwhale
     ```
 
@@ -147,22 +147,22 @@
     > When you first build runtime, creating an isolated python environment and downloading python dependencies will take a lot of time. The command execution time is related to the network environment of the machine and the number of packages in the runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/pip.conf` file is a recommended practice.
     >
     > For users in the mainland of China, the following conf file is an option:
     >
     > ```conf
     > [global]
     > cache-dir = ~/.cache/pip
-    > index-url = https://mirrors.aliyun.com/pypi/simple/
-    > extra-index-url = https://pypi.doubanio.com/simple
+    > index-url = https://pypi.tuna.tsinghua.edu.cn/simple
+    > extra-index-url = https://mirrors.aliyun.com/pypi/simple/
     > ```
 
     ```bash
-    swcli runtime build example/runtime/pytorch
+    swcli runtime build --yaml example/runtime/pytorch/runtime.yaml
     swcli runtime list
-    swcli runtime info pytorch/version/latest
+    swcli runtime info pytorch
     ```
 
 - 🍞 **STEP4**: Building a model
 
   - Download pre-trained model file:
 
     ```bash
@@ -225,17 +225,17 @@
     run:
         handler: mnist.evaluator:MNISTInference
     ```
 
   - Run one command to build the model.
 
     ```bash
-    swcli model build example/mnist --runtime pytorch/version/latest
+    swcli model build example/mnist --runtime pytorch
     swcli model list
-    swcli model info mnist/version/latest
+    swcli model info mnist
     ```
 
 - 🍺 **STEP5**: Building a dataset
 
   - Download MNIST RAW data files.
 
     ```bash
@@ -278,34 +278,34 @@
                     "label": _label,
                 }
     ```
 
   - Run one command to build the dataset.
 
     ```bash
-    swcli dataset build example/mnist --handler mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest
-    swcli dataset info mnist/version/latest
-    swcli dataset head mnist/version/latest
+    swcli dataset build --yaml example/mnist/dataset.yaml
+    swcli dataset info mnist
+    swcli dataset head mnist
     ```
 
-  Starwhale also supports build dataset with pure python sdk. You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/dataset-sdk.ipynb).
+  Starwhale also supports building datasets with pure Python SDK. You can try it in [Google Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/example/notebooks/dataset-sdk.ipynb).
 
 - 🍖 **STEP6**: Running an evaluation job
 
     ```bash
-    swcli eval run --model mnist/version/latest --dataset mnist/version/latest --runtime pytorch/version/latest
-    swcli eval list
-    swcli eval info $(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
+    swcli -vvv model run --uri mnist --dataset mnist --runtime pytorch
+    swcli job list
+    swcli job info $(swcli job list | grep mnist | grep success | awk '{print $1}' | head -n 1)
     ```
 
 **👏 Now, you have completed the fundamental steps for Starwhale standalone. Let's go ahead and finish the tutorial on the on-premises instance.**
 
-## MNIST Quick Tour for on-premises instance
+## MNIST Quick Tour for Starwhale Server Instance
 
-![Create Job Workflow](docs/docs/img/console-create-job.gif)
+![Create Job Workflow](https://doc.starwhale.ai/assets/images/console-artifacts-fd7bf6e54d06dc37d234019e769031e6.gif)
 
 - 🍰 **STEP1**: Install minikube and helm
 
   - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+
   - [Helm](https://helm.sh/docs/intro/install/) 3.2.0+
 
 - 🍵 **STEP2**: Start minikube
@@ -364,41 +364,66 @@
         - web visit: http://minio.starwhale.svc
         - admin visit: http://minio-admin.starwhale.svc
     MySQL:
         - port-forward:
         - run: kubectl port-forward --namespace starwhale svc/mysql 3306:3306
         - visit: mysql -h 127.0.0.1 -P 3306 -ustarwhale -pstarwhale
     Please run the following command for the domains searching:
-        echo "$(minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
+        echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
     ******************************************
     Login Info:
     - starwhale: u:starwhale, p:abcd1234
     - minio admin: u:minioadmin, p:minioadmin
 
     *_* Enjoy to use Starwhale Platform. *_*
     ```
 
-    Then keep checking the minikube service status until all deployments are running.
+    Then keep checking the minikube service status until all deployments are running(waiting for 3~5 mins).
 
     ```bash
     kubectl get deployments -n starwhale
     ```
 
     | NAME       | READY | UP-TO-DATE | AVAILABLE | AGE |
     | ---------- | ----- | ---------- | --------- | --- |
     | controller | 1/1   | 1          | 1         | 5m  |
     | minio      | 1/1   | 1          | 1         | 5m  |
     | mysql      | 1/1   | 1          | 1         | 5m  |
 
     Make the Starwhale controller accessible locally with the following command:
 
     ```bash
-    kubectl port-forward --namespace starwhale svc/controller 8082:8082
+    echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
     ```
 
+    Then you can visit http://controller.starwhale.svc in your local web browser.
+
+    If other users also want to access Starwhale Server Instance, the following commands maybe help you:
+
+    - in your machine(Linux, Starwhale Server Instance machine):
+
+        for temporary use with socat command:
+
+        ```bash
+        # install socat at first, ref: https://howtoinstall.co/en/socat
+        sudo socat TCP4-LISTEN:80,fork,reuseaddr,bind=0.0.0.0 TCP4:`minikube ip`:80
+        ```
+
+      When you kill the socat process, the share access will be blocked. `iptables` maybe a better choice for long-term use.
+
+    - in other users' machines:
+
+        ```bash
+        # for macOSX or Linux environment, run the command in the shell.
+        echo ${your_machine_ip} controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
+
+        # for Windows environment, run the command in the PowerShell with administrator permission.
+        Add-Content -Path C:\Windows\System32\drivers\etc\hosts -Value "`n${your_machine_ip} controller.starwhale.svc minio.starwhale.svc  minio-admin.starwhale.svc"
+        ```
+
 - ☕ **STEP4**: Upload the artifacts to the cloud instance
 
     > **pre-prepared artifacts**
     > Before starting this tutorial, the following three artifacts should already exist on your machine：
     >
     > - a starwhale model named mnist
     > - a starwhale dataset named mnist
@@ -406,41 +431,31 @@
     >
     > The above three artifacts are what we built on our machine using starwhale.
 
     1. Use swcli to operate the remote server
         First, log in to the server:
 
         ```bash
-        swcli instance login --username starwhale --password abcd1234 --alias dev http://localhost:8082
+        swcli instance login --username starwhale --password abcd1234 --alias dev http://controller.starwhale.svc
         ```
 
     2. Start copying the model, dataset, and runtime that we constructed earlier:
 
         ```bash
-        swcli model copy mnist/version/latest dev/project/starwhale
-        swcli dataset copy mnist/version/latest dev/project/starwhale
-        swcli runtime copy pytorch/version/latest dev/project/starwhale
+        swcli model copy mnist cloud://dev/project/starwhale
+        swcli dataset copy mnist cloud://dev/project/starwhale
+        swcli runtime copy pytorch cloud://dev/project/starwhale
         ```
 
 - 🍞 **STEP5**: Use the web UI to run an evaluation
 
-    1. Log in Starwhale instance: let's use the username(starwhale) and password(abcd1234) to open the server web UI(<http://localhost:8082/>).
-
-    2. Then, we will see the project named 'project_for_mnist' that we created earlier with swcli. Click the project name, you will see the model, runtime, and dataset uploaded in the previous step.
-        <details>
-            <summary>Show the uploaded artifacts screenshots</summary>
-
-        ![Console Artifacts](docs/docs/img/console-artifacts.gif)
-        </details>
-    3. Create and view an evaluation job
-        <details>
-            <summary>Show create job screenshot</summary>
+    1. Log in Starwhale instance: let's use the username(starwhale) and password(abcd1234) to open the server web UI(<http://controller.starwhale.svc>).
 
-        ![Console Create Job](docs/docs/img/console-create-job.gif)
-        </details>
+    2. Then, we will see the project named 'starwhale/starwhale' that we created earlier with swcli. Click the project name, you will see the model, runtime, and dataset uploaded in the previous step.
+    3. Create and view an evaluation job.
 
 **👏 Congratulations! You have completed the evaluation process for a model.**
 
 ## Documentation, Community, and Support
 
 - Visit [Starwhale HomePage](https://starwhale.ai).
 - More information in the [official documentation](https://doc.starwhale.ai).
@@ -453,12 +468,12 @@
   - Helm Charts on [Artifacthub](https://artifacthub.io/packages/helm/starwhale/starwhale).
   - Docker Images on [Docker Hub](https://hub.docker.com/u/starwhaleai), [Github Packages](https://github.com/orgs/star-whale/packages) and [Starwhale Registry](https://docker-registry.starwhale.cn/).
 
 - Additionally, you can always find us at *developer@starwhale.ai*.
 
 ## Contributing
 
-🌼👏**PRs are always welcomed** 👍🍺. See [Contribution to Starwhale](https://doc.starwhale.ai/docs/community/contribute) for more details.
+🌼👏**PRs are always welcomed** 👍🍺. See [Contribution to Starwhale](https://doc.starwhale.ai/community/contribute) for more details.
 
 ## License
 
 Starwhale is licensed under the [Apache License 2.0](https://github.com/star-whale/starwhale/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.5.6 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.5.7 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -23,68 +23,81 @@
   img.shields.io/pypi/v/starwhale?style=flat] [https://img.shields.io/github/
   license/star-whale/starwhale?style=flat] [PyPI_-_Python_Version] [https://
    github.com/star-whale/starwhale/actions/workflows/client.yaml/badge.svg]
      [https://github.com/star-whale/starwhale/actions/workflows/server-ut-
     report.yml/badge.svg] [https://github.com/star-whale/starwhale/actions/
 workflows/console.yml/badge.svg] [Codecov] [Codecov] [Artifact_Hub] [Starwhale
                                    E2E_Test]
-## What is Starwhale Starwhale is an MLOps platform. It provides **Instance**,
-**Project**, **Runtime**, **Model**, and **Dataset**. - **Instance**: Each
-installation of Starwhale is called an instance. - ð» **Standalone
-Instance**: The simplest form that requires only the Starwhale Client(`swcli`).
-`swcli` is written by pure python3. - ð **On-Premises Instance**: Cloud
-form, we call it **private cloud instance**. Kubernetes and BareMetal both meet
-the basic environmental requirements. - âï¸ **Cloud Hosted Instance**: Cloud
-form, we call it **public cloud instance**. Starwhale team maintains the web
-service. **Starwhale tries to keep concepts consistent across different types
+## What is Starwhale Starwhale is an MLOps/LLMOps platform. It provides
+**Instance**, **Project**, **Runtime**, **Model**, and **Dataset**. -
+**Instance**: Each installation of Starwhale is called an instance. - ð»
+**Starwhale Standalone**: Rather than a running service, Starwhale Standalone
+is actually a repository that resides in your local file system. It is created
+and managed by the Starwhale Client (SWCLI). You only need to install SWCLI to
+use it. Currently, each user on a single machine can have only ONE Starwhale
+Standalone instance. We recommend you use the Starwhale Standalone to build and
+test your datasets, runtime, and models before pushing them to Starwhale
+Server/Cloud instances. - ð **Starwhale Server**: Starwhale Server is a
+service deployed on your local server. Besides text-only results from the
+Starwhale Client (SWCLI), Starwhale Server provides Web UI for you to manage
+your datasets and models, evaluate your models in your local Kubernetes
+cluster, and review the evaluation results. - âï¸ **Starwhale Cloud**:
+Starwhale Cloud is a managed service hosted on public clouds. By registering an
+account on https://cloud.starwhale.cn , you are ready to use Starwhale without
+needing to install, operate, and maintain your own instances. Starwhale Cloud
+also provides public resources for you to download, like datasets, runtimes,
+and models. Check the "starwhale/public" project on Starwhale Cloud for more
+details. **Starwhale tries to keep concepts consistent across different types
 of instances. In this way, people can easily exchange data and migrate between
 them.** - **Project**: The basic unit for organizing different resources. -
 **ML Basic Elements**: The Machine Learning/Deep Learning running environments
 or artifacts. Starwhale empowers the ML/DL essential elements with packaging,
 versioning, reproducibility, and shareability. - ð **Runtime**: Software
-dependencies description to "run" a model, which includes python libraries,
+dependencies description to "run" a model, which includes Python libraries,
 native libraries, native binaries, etc. - ð **Model**: The standard model
 format used in model delivery. - ð« **Dataset**: A unified description of how
 the data and labels are stored and organized. Starwhale datasets can be loaded
 efficiently. - **Running Fundamentals**: Starwhale uses **Job**, **Step**, and
 **Task** to execute ML/DL actions like model trainingï¼ evaluation, and
 serving. Starwhale's **Controller-Agents** structure scales out easily. - ð¥
 **Job**: A set of programs to do specific work. Each job consists of one or
 more steps. - ðµ **Step**: Represents distinct stages of the work. Each step
 consists of one or more tasks. - ð¥ **Task**: Operation entity. Tasks are in
 some specific steps. - **Scenarios**: Starwhale provides the best practice and
 out-of-the-box for different ML/DL scenarios. - ð **Model Training(WIP)**:
 Use Starwhale Python SDK to record experiment meta, metric, log, and artifact.
 - ð¥ï¸ **Model Evaluation**: `PipelineHandler` and some report decorators
 can give you complete, helpful, and user-friendly evaluation reports with only
-a few lines of codes. - ð« **Model Serving(TBD)**: Starwhale Model can be
+a few lines of code. - ð« **Model Serving(TBD)**: Starwhale Model can be
 deployed as a web service or stream service in production with deployment
 capability, observability, and scalability. Data scientists do not need to
-write ML/DL irrelevant codes. ## MNIST Quick Tour for the standalone instance
-### Use Notebook - You can try it in [Google Colab](https://
-colab.research.google.com/github/star-whale/starwhale/blob/main/example/mnist/
-notebook.ipynb) - Or run [example/mnist/notebook.ipynb](example/mnist/
-notebook.ipynb) locally using [vscode](https://code.visualstudio.com/) or
-[jupyterlab](https://github.com/jupyterlab/jupyterlab) ### Use your own python
-env ![Core Job Workflow](docs/docs/img/standalone-core-workflow.gif) - ð°
-**STEP1**: Installing Starwhale ```bash python3 -m pip install starwhale ``` -
-ðµ **STEP2**: Downloading the MNIST example > To save time in the example
-downloading, we skip git-lfs and other commits info. ```bash
-GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/star-whale/starwhale.git --
-depth 1 cd starwhale ``` - â **STEP3**: Building a runtime > When you first
-build runtime, creating an isolated python environment and downloading python
-dependencies will take a lot of time. The command execution time is related to
-the network environment of the machine and the number of packages in the
-runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/
-pip.conf` file is a recommended practice. > > For users in the mainland of
-China, the following conf file is an option: > > ```conf > [global] > cache-dir
-= ~/.cache/pip > index-url = https://mirrors.aliyun.com/pypi/simple/ > extra-
-index-url = https://pypi.doubanio.com/simple > ``` ```bash swcli runtime build
-example/runtime/pytorch swcli runtime list swcli runtime info pytorch/version/
-latest ``` - ð **STEP4**: Building a model - Download pre-trained model
+write ML/DL irrelevant codes. ## MNIST Quick Tour for the Starwhale Standalone
+Instance ### Use Notebook - You can try it in [Google Colab](https://
+colab.research.google.com/github/star-whale/starwhale/blob/main/example/
+notebooks/quickstart-standalone.ipynb) - Or run [quickstart example](example/
+notebooks/quickstart-standalone.ipynb) locally using [vscode](https://
+code.visualstudio.com/) or [jupyterlab](https://github.com/jupyterlab/
+jupyterlab) ### Use your own Python env ![Core Job Workflow](https://
+doc.starwhale.ai/assets/images/standalone-core-workflow-
+270ac0f0cb5b20dbe5ccd11727e2620b.gif) - ð° **STEP1**: Installing Starwhale
+```bash python3 -m pip install starwhale ``` - ðµ **STEP2**: Downloading the
+MNIST example > To save time in the example downloading, we skip git-lfs and
+other commits info. ```bash GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/
+star-whale/starwhale.git --depth 1 cd starwhale ``` - â **STEP3**: Building a
+runtime > When you first build runtime, creating an isolated python environment
+and downloading python dependencies will take a lot of time. The command
+execution time is related to the network environment of the machine and the
+number of packages in the runtime.yaml. Using the befitting pypi mirror and
+cache config in the `~/.pip/pip.conf` file is a recommended practice. > > For
+users in the mainland of China, the following conf file is an option: > >
+```conf > [global] > cache-dir = ~/.cache/pip > index-url = https://
+pypi.tuna.tsinghua.edu.cn/simple > extra-index-url = https://
+mirrors.aliyun.com/pypi/simple/ > ``` ```bash swcli runtime build --yaml
+example/runtime/pytorch/runtime.yaml swcli runtime list swcli runtime info
+pytorch ``` - ð **STEP4**: Building a model - Download pre-trained model
 file: ```bash cd example/mnist make download-model # For users in the mainland
 of China, please add `CN=1` environment for make command: # CN=1 make download-
 model cd - ``` - [Code Example]Write some code with Starwhale Python SDK.
 Complete code is [here](https://github.com/star-whale/starwhale/blob/main/
 example/mnist/mnist/evaluator.py). ```python import typing as t import torch
 from starwhale import Image, PipelineHandler, multi_classification class
 MNISTInference(PipelineHandler): def __init__(self) -> None: super().__init__()
@@ -99,55 +112,54 @@
 [] for _data in ppl_result: label.append(_data["input"]["label"]) result.append
 (_data["output"][0]) pr.append(_data["output"][1]) return label, result, pr def
 _pre(self, input:bytes): """write some mnist preprocessing code""" def _post
 (self, input:bytes): """write some mnist post-processing code""" def
 _load_model(): """load your pre trained model""" ``` - [Code Example]Define
 `model.yaml`. ```yaml name: mnist run: handler: mnist.evaluator:MNISTInference
 ``` - Run one command to build the model. ```bash swcli model build example/
-mnist --runtime pytorch/version/latest swcli model list swcli model info mnist/
-version/latest ``` - ðº **STEP5**: Building a dataset - Download MNIST RAW
-data files. ```bash cd example/mnist make download-data # For users in the
-mainland of China, please add `CN=1` environment for make command: # CN=1 make
-download-data cd - ``` - [Code Example]Write some code with Starwhale Python
-SDK. Full code is [here](https://github.com/star-whale/starwhale/blob/main/
-example/mnist/mnist/dataset.py). ```python import struct from pathlib import
-Path from starwhale import GrayscaleImage def iter_swds_bin_item(): root_dir =
-Path(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
+mnist --runtime pytorch swcli model list swcli model info mnist ``` - ðº
+**STEP5**: Building a dataset - Download MNIST RAW data files. ```bash cd
+example/mnist make download-data # For users in the mainland of China, please
+add `CN=1` environment for make command: # CN=1 make download-data cd - ``` -
+[Code Example]Write some code with Starwhale Python SDK. Full code is [here]
+(https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/
+dataset.py). ```python import struct from pathlib import Path from starwhale
+import GrayscaleImage def iter_swds_bin_item(): root_dir = Path
+(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
 ubyte").open("rb") as data_file, ( root_dir / "t10k-labels-idx1-ubyte" ).open
 ("rb") as label_file: _, data_number, height, width = struct.unpack(">IIII",
 data_file.read(16)) _, label_number = struct.unpack(">II", label_file.read(8))
 print( f">data({data_file.name}) split data:{data_number}, label:{label_number}
 group" ) image_size = height * width for i in range(0, min(data_number,
 label_number)): _data = data_file.read(image_size) _label = struct.unpack(">B",
 label_file.read(1))[0] yield { "img": GrayscaleImage( _data, display_name=f"
 {i}", shape=(height, width, 1), ), "label": _label, } ``` - Run one command to
-build the dataset. ```bash swcli dataset build example/mnist --handler
-mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest swcli dataset
-info mnist/version/latest swcli dataset head mnist/version/latest ``` Starwhale
-also supports build dataset with pure python sdk. You can try it in [Google
+build the dataset. ```bash swcli dataset build --yaml example/mnist/
+dataset.yaml swcli dataset info mnist swcli dataset head mnist ``` Starwhale
+also supports building datasets with pure Python SDK. You can try it in [Google
 Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/
 example/notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation
-job ```bash swcli eval run --model mnist/version/latest --dataset mnist/
-version/latest --runtime pytorch/version/latest swcli eval list swcli eval info
-$(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
-``` **ð Now, you have completed the fundamental steps for Starwhale
-standalone. Let's go ahead and finish the tutorial on the on-premises
-instance.** ## MNIST Quick Tour for on-premises instance ![Create Job Workflow]
-(docs/docs/img/console-create-job.gif) - ð° **STEP1**: Install minikube and
-helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm]
-(https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube
-```bash minikube start --addons ingress ``` > For users in the mainland of
-China, please add some external parameters. The following command was well
-tested; you may also try another kubernetes version. > > ```bash > minikube
-start --addons ingress --image-mirror-country=cn --kubernetes-version=1.25.3 >
-``` If there is no kubectl bin in your machine, you may use `minikube kubectl`
-or `alias kubectl="minikube kubectl --"` alias command. - ðµ **STEP3**:
-Installing Starwhale ```bash helm repo add starwhale https://star-
-whale.github.io/charts helm repo update helm pull starwhale/starwhale --untar -
--untardir ./charts helm upgrade --install starwhale ./charts/starwhale -
+job ```bash swcli -vvv model run --uri mnist --dataset mnist --runtime pytorch
+swcli job list swcli job info $(swcli job list | grep mnist | grep success |
+awk '{print $1}' | head -n 1) ``` **ð Now, you have completed the
+fundamental steps for Starwhale standalone. Let's go ahead and finish the
+tutorial on the on-premises instance.** ## MNIST Quick Tour for Starwhale
+Server Instance ![Create Job Workflow](https://doc.starwhale.ai/assets/images/
+console-artifacts-fd7bf6e54d06dc37d234019e769031e6.gif) - ð° **STEP1**:
+Install minikube and helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/
+) 1.25+ - [Helm](https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**:
+Start minikube ```bash minikube start --addons ingress ``` > For users in the
+mainland of China, please add some external parameters. The following command
+was well tested; you may also try another kubernetes version. > > ```bash >
+minikube start --addons ingress --image-mirror-country=cn --kubernetes-
+version=1.25.3 > ``` If there is no kubectl bin in your machine, you may use
+`minikube kubectl` or `alias kubectl="minikube kubectl --"` alias command. -
+ðµ **STEP3**: Installing Starwhale ```bash helm repo add starwhale https://
+star-whale.github.io/charts helm repo update helm pull starwhale/starwhale --
+untar --untardir ./charts helm upgrade --install starwhale ./charts/starwhale -
 n starwhale --create-namespace -f ./charts/starwhale/
 values.minikube.global.yaml ``` > For users in the mainland of China, use
 `values.minikube.global.yaml`. ```bash helm upgrade --install starwhale ./
 charts/starwhale -n starwhale --create-namespace -f ./charts/starwhale/
 values.minikube.cn.yaml ``` After the installation is successful, the following
 prompt message appears: ```bash Release "starwhale" has been upgraded. Happy
 Helming! NAME: starwhale LAST DEPLOYED: Tue Feb 14 16:25:03 2023 NAMESPACE:
@@ -156,55 +168,66 @@
 0.1.0 App Version: latest Starwhale Image: - server: ghcr.io/star-whale/server:
 latest Runtime default Image: - runtime image: ghcr.io/star-whale/starwhale:
 latest ****************************************** Controller: - visit: http://
 controller.starwhale.svc Minio: - web visit: http://minio.starwhale.svc - admin
 visit: http://minio-admin.starwhale.svc MySQL: - port-forward: - run: kubectl
 port-forward --namespace starwhale svc/mysql 3306:3306 - visit: mysql -
 h 127.0.0.1 -P 3306 -ustarwhale -pstarwhale Please run the following command
-for the domains searching: echo "$(minikube ip) controller.starwhale.svc
+for the domains searching: echo "$(sudo minikube ip) controller.starwhale.svc
 minio.starwhale.svc minio-admin.starwhale.svc " | sudo tee -a /etc/hosts
 ****************************************** Login Info: - starwhale: u:
 starwhale, p:abcd1234 - minio admin: u:minioadmin, p:minioadmin *_* Enjoy to
 use Starwhale Platform. *_* ``` Then keep checking the minikube service status
-until all deployments are running. ```bash kubectl get deployments -n starwhale
-``` | NAME | READY | UP-TO-DATE | AVAILABLE | AGE | | ---------- | ----- | ----
------- | --------- | --- | | controller | 1/1 | 1 | 1 | 5m | | minio | 1/1 | 1
-| 1 | 5m | | mysql | 1/1 | 1 | 1 | 5m | Make the Starwhale controller
-accessible locally with the following command: ```bash kubectl port-forward --
-namespace starwhale svc/controller 8082:8082 ``` - â **STEP4**: Upload the
-artifacts to the cloud instance > **pre-prepared artifacts** > Before starting
-this tutorial, the following three artifacts should already exist on your
-machineï¼ > > - a starwhale model named mnist > - a starwhale dataset named
-mnist > - a starwhale runtime named pytorch > > The above three artifacts are
-what we built on our machine using starwhale. 1. Use swcli to operate the
-remote server First, log in to the server: ```bash swcli instance login --
-username starwhale --password abcd1234 --alias dev http://localhost:8082 ``` 2.
-Start copying the model, dataset, and runtime that we constructed earlier:
-```bash swcli model copy mnist/version/latest dev/project/starwhale swcli
-dataset copy mnist/version/latest dev/project/starwhale swcli runtime copy
-pytorch/version/latest dev/project/starwhale ``` - ð **STEP5**: Use the web
-UI to run an evaluation 1. Log in Starwhale instance: let's use the username
-(starwhale) and password(abcd1234) to open the server web UI(
-localhost:8082/>). 2. Then, we will see the project named 'project_for_mnist'
-that we created earlier with swcli. Click the project name, you will see the
-model, runtime, and dataset uploaded in the previous step.  Show the uploaded
-artifacts screenshots ![Console Artifacts](docs/docs/img/console-artifacts.gif)
-3. Create and view an evaluation job  Show create job screenshot ![Console
-Create Job](docs/docs/img/console-create-job.gif)  **ð Congratulations! You
-have completed the evaluation process for a model.** ## Documentation,
-Community, and Support - Visit [Starwhale HomePage](https://starwhale.ai). -
-More information in the [official documentation](https://doc.starwhale.ai). -
-For general questions and support, join the [Slack](https://
-starwhale.slack.com/). - For bug reports and feature requests, please use
-[Github Issue](https://github.com/star-whale/starwhale/issues). - To get
-community updates, follow [@starwhaleai](https://twitter.com/starwhaleai) on
-Twitter. - For Starwhale artifacts, please visit: - Python Package on [Pypi]
-(https://pypi.org/project/starwhale/). - Helm Charts on [Artifacthub](https://
-artifacthub.io/packages/helm/starwhale/starwhale). - Docker Images on [Docker
-Hub](https://hub.docker.com/u/starwhaleai), [Github Packages](https://
-github.com/orgs/star-whale/packages) and [Starwhale Registry](https://docker-
-registry.starwhale.cn/). - Additionally, you can always find us at
-*developer@starwhale.ai*. ## Contributing ð¼ð**PRs are always welcomed**
-ððº. See [Contribution to Starwhale](https://doc.starwhale.ai/docs/
+until all deployments are running(waiting for 3~5 mins). ```bash kubectl get
+deployments -n starwhale ``` | NAME | READY | UP-TO-DATE | AVAILABLE | AGE | |
+---------- | ----- | ---------- | --------- | --- | | controller | 1/1 | 1 | 1
+| 5m | | minio | 1/1 | 1 | 1 | 5m | | mysql | 1/1 | 1 | 1 | 5m | Make the
+Starwhale controller accessible locally with the following command: ```bash
+echo "$(sudo minikube ip) controller.starwhale.svc minio.starwhale.svc minio-
+admin.starwhale.svc " | sudo tee -a /etc/hosts ``` Then you can visit http://
+controller.starwhale.svc in your local web browser. If other users also want to
+access Starwhale Server Instance, the following commands maybe help you: - in
+your machine(Linux, Starwhale Server Instance machine): for temporary use with
+socat command: ```bash # install socat at first, ref: https://howtoinstall.co/
+en/socat sudo socat TCP4-LISTEN:80,fork,reuseaddr,bind=0.0.0.0 TCP4:`minikube
+ip`:80 ``` When you kill the socat process, the share access will be blocked.
+`iptables` maybe a better choice for long-term use. - in other users' machines:
+```bash # for macOSX or Linux environment, run the command in the shell. echo $
+{your_machine_ip} controller.starwhale.svc minio.starwhale.svc minio-
+admin.starwhale.svc " | sudo tee -a /etc/hosts # for Windows environment, run
+the command in the PowerShell with administrator permission. Add-Content -Path
+C:\Windows\System32\drivers\etc\hosts -Value "`n${your_machine_ip}
+controller.starwhale.svc minio.starwhale.svc minio-admin.starwhale.svc" ``` -
+â **STEP4**: Upload the artifacts to the cloud instance > **pre-prepared
+artifacts** > Before starting this tutorial, the following three artifacts
+should already exist on your machineï¼ > > - a starwhale model named mnist > -
+a starwhale dataset named mnist > - a starwhale runtime named pytorch > > The
+above three artifacts are what we built on our machine using starwhale. 1. Use
+swcli to operate the remote server First, log in to the server: ```bash swcli
+instance login --username starwhale --password abcd1234 --alias dev http://
+controller.starwhale.svc ``` 2. Start copying the model, dataset, and runtime
+that we constructed earlier: ```bash swcli model copy mnist cloud://dev/
+project/starwhale swcli dataset copy mnist cloud://dev/project/starwhale swcli
+runtime copy pytorch cloud://dev/project/starwhale ``` - ð **STEP5**: Use
+the web UI to run an evaluation 1. Log in Starwhale instance: let's use the
+username(starwhale) and password(abcd1234) to open the server web UI(
+controller.starwhale.svc>). 2. Then, we will see the project named 'starwhale/
+starwhale' that we created earlier with swcli. Click the project name, you will
+see the model, runtime, and dataset uploaded in the previous step. 3. Create
+and view an evaluation job. **ð Congratulations! You have completed the
+evaluation process for a model.** ## Documentation, Community, and Support -
+Visit [Starwhale HomePage](https://starwhale.ai). - More information in the
+[official documentation](https://doc.starwhale.ai). - For general questions and
+support, join the [Slack](https://starwhale.slack.com/). - For bug reports and
+feature requests, please use [Github Issue](https://github.com/star-whale/
+starwhale/issues). - To get community updates, follow [@starwhaleai](https://
+twitter.com/starwhaleai) on Twitter. - For Starwhale artifacts, please visit: -
+Python Package on [Pypi](https://pypi.org/project/starwhale/). - Helm Charts on
+[Artifacthub](https://artifacthub.io/packages/helm/starwhale/starwhale). -
+Docker Images on [Docker Hub](https://hub.docker.com/u/starwhaleai), [Github
+Packages](https://github.com/orgs/star-whale/packages) and [Starwhale Registry]
+(https://docker-registry.starwhale.cn/). - Additionally, you can always find us
+at *developer@starwhale.ai*. ## Contributing ð¼ð**PRs are always
+welcomed** ððº. See [Contribution to Starwhale](https://doc.starwhale.ai/
 community/contribute) for more details. ## License Starwhale is licensed under
 the [Apache License 2.0](https://github.com/star-whale/starwhale/blob/main/
 LICENSE).
```

### Comparing `starwhale-0.5.6/starwhale.egg-info/SOURCES.txt` & `starwhale-0.5.7/starwhale.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -156,25 +156,25 @@
 starwhale/web/user.py
 starwhale/web/ui/favicon.ico
 starwhale/web/ui/favicon_white.ico
 starwhale/web/ui/iconfont.js
 starwhale/web/ui/index.html
 starwhale/web/ui/manifest.json
 starwhale/web/ui/robots.txt
-starwhale/web/ui/assets/BlockLabel-5fb1ba40.js
-starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-1aa90835.js
-starwhale/web/ui/assets/Column-32430de0.js
-starwhale/web/ui/assets/DatasetForm-b1b79ee8.js
-starwhale/web/ui/assets/File-0190a4b6.js
-starwhale/web/ui/assets/Image-7d3d0587.js
-starwhale/web/ui/assets/Image2-fef2a6da.js
+starwhale/web/ui/assets/BlockLabel-fe080bcf.js
+starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang-3c98ad87.js
+starwhale/web/ui/assets/Column-958ed910.js
+starwhale/web/ui/assets/DatasetForm-45360b60.js
+starwhale/web/ui/assets/File-d0f0778c.js
+starwhale/web/ui/assets/Image-953a3e24.js
+starwhale/web/ui/assets/Image2-08f40595.js
+starwhale/web/ui/assets/LogViewer-1215be01.js
 starwhale/web/ui/assets/LogViewer-b5684b3d.css
-starwhale/web/ui/assets/LogViewer-ead1dacc.js
-starwhale/web/ui/assets/Model3D-017f88a9.js
-starwhale/web/ui/assets/ModifyUpload-ca14033f.js
+starwhale/web/ui/assets/Model3D-ff19b927.js
+starwhale/web/ui/assets/ModifyUpload-972867fe.js
 starwhale/web/ui/assets/RedHatDisplay-Bold-44214a55.woff
 starwhale/web/ui/assets/RedHatDisplay-Bold-ca18645c.woff2
 starwhale/web/ui/assets/RedHatDisplay-Medium-6ccf2158.woff
 starwhale/web/ui/assets/RedHatDisplay-Medium-6d3ccc0f.woff2
 starwhale/web/ui/assets/RedHatDisplay-Regular-1b99a560.woff
 starwhale/web/ui/assets/RedHatDisplay-Regular-e6fb83d9.woff2
 starwhale/web/ui/assets/RedHatDisplay-updated-Bold-66d1fc26.woff2
@@ -190,83 +190,83 @@
 starwhale/web/ui/assets/RedHatText-Regular-542423d0.woff2
 starwhale/web/ui/assets/RedHatText-Regular-df36d7d0.woff
 starwhale/web/ui/assets/RedHatText-updated-Medium-721ddd64.woff2
 starwhale/web/ui/assets/RedHatText-updated-Regular-2e08dbe8.woff2
 starwhale/web/ui/assets/RedHatTextVF-updated-ItalicModified-9e1c1004.woff2
 starwhale/web/ui/assets/RedHatTextVFModified-updated-942d38f7.woff2
 starwhale/web/ui/assets/RobotoMono-Regular-5c4ca672.ttf
-starwhale/web/ui/assets/Tabs-58551549.js
-starwhale/web/ui/assets/Upload-5020e3e5.js
-starwhale/web/ui/assets/Webcam-1d7c84ed.js
+starwhale/web/ui/assets/Tabs-0edcf972.js
+starwhale/web/ui/assets/Upload-699ac090.js
+starwhale/web/ui/assets/Webcam-77a82fdc.js
 starwhale/web/ui/assets/_commonjsHelpers-23156833.js
 starwhale/web/ui/assets/account2-668f906e.svg
 starwhale/web/ui/assets/bg-1920x1080-8b0d8feb.jpg
 starwhale/web/ui/assets/bg-2560x1440-c97cffa5.jpg
 starwhale/web/ui/assets/bg-3840x2160-f974f4b1.jpg
-starwhale/web/ui/assets/color-ab3477a6.js
+starwhale/web/ui/assets/color-de3304e0.js
 starwhale/web/ui/assets/csv-17a3ae92.js
 starwhale/web/ui/assets/dsv-62f8cd07.js
 starwhale/web/ui/assets/empty-chart-1e62901a.svg
 starwhale/web/ui/assets/empty-f3091520.svg
 starwhale/web/ui/assets/google-9d1a8b2b.svg
 starwhale/web/ui/assets/iconfont-0a880318.woff2
 starwhale/web/ui/assets/iconfont-10b60b11.ttf
 starwhale/web/ui/assets/iconfont-4c4e9d6d.woff
-starwhale/web/ui/assets/index-0a9704a2.js
-starwhale/web/ui/assets/index-1d08769b.js
+starwhale/web/ui/assets/index-00cfa2a7.js
+starwhale/web/ui/assets/index-0ebd961e.js
 starwhale/web/ui/assets/index-4b525ef6.css
-starwhale/web/ui/assets/index-54aca6e3.js
 starwhale/web/ui/assets/index-c467f321.css
-starwhale/web/ui/assets/index10-42042dc4.js
-starwhale/web/ui/assets/index11-78c7e86b.js
-starwhale/web/ui/assets/index12-ab265665.js
-starwhale/web/ui/assets/index13-7c871e80.js
-starwhale/web/ui/assets/index14-6c615bf9.js
-starwhale/web/ui/assets/index15-86a0c1f0.js
-starwhale/web/ui/assets/index16-2bdd3a00.js
-starwhale/web/ui/assets/index17-f009f53c.js
-starwhale/web/ui/assets/index18-b8f18d2d.js
-starwhale/web/ui/assets/index19-a472c2fd.js
-starwhale/web/ui/assets/index2-040b1a6e.js
-starwhale/web/ui/assets/index20-cea79a56.js
-starwhale/web/ui/assets/index21-839b404f.js
-starwhale/web/ui/assets/index22-b0a063e3.js
-starwhale/web/ui/assets/index23-2546fc23.js
-starwhale/web/ui/assets/index24-ee89579d.js
-starwhale/web/ui/assets/index25-fb12b103.js
-starwhale/web/ui/assets/index26-70ba7bd9.js
-starwhale/web/ui/assets/index27-202147ca.js
-starwhale/web/ui/assets/index28-4db56c35.js
-starwhale/web/ui/assets/index29-f4b57e8f.js
-starwhale/web/ui/assets/index3-3ed81e50.js
-starwhale/web/ui/assets/index30-6cfd7268.js
-starwhale/web/ui/assets/index31-feae9916.js
-starwhale/web/ui/assets/index32-efa03b40.js
-starwhale/web/ui/assets/index33-c77eb4e8.js
-starwhale/web/ui/assets/index34-74e21fbb.js
-starwhale/web/ui/assets/index35-76158480.js
-starwhale/web/ui/assets/index36-051a9d0c.js
-starwhale/web/ui/assets/index37-4dd6b1d2.js
-starwhale/web/ui/assets/index38-42b4b637.js
-starwhale/web/ui/assets/index39-4548d90a.js
-starwhale/web/ui/assets/index4-efddfb05.js
-starwhale/web/ui/assets/index5-a485e343.js
-starwhale/web/ui/assets/index6-c4dad8b6.js
-starwhale/web/ui/assets/index7-c30707d3.js
-starwhale/web/ui/assets/index8-1ed9ba9d.js
-starwhale/web/ui/assets/index9-1a9ea67c.js
+starwhale/web/ui/assets/index-fa288f1e.js
+starwhale/web/ui/assets/index10-6962b31b.js
+starwhale/web/ui/assets/index11-6a6faac8.js
+starwhale/web/ui/assets/index12-d5dc887c.js
+starwhale/web/ui/assets/index13-6dafecb5.js
+starwhale/web/ui/assets/index14-8c46ae7f.js
+starwhale/web/ui/assets/index15-7940e50b.js
+starwhale/web/ui/assets/index16-583cafad.js
+starwhale/web/ui/assets/index17-e0f03f64.js
+starwhale/web/ui/assets/index18-85c307e0.js
+starwhale/web/ui/assets/index19-46ac23c8.js
+starwhale/web/ui/assets/index2-4608846d.js
+starwhale/web/ui/assets/index20-61594d37.js
+starwhale/web/ui/assets/index21-976d330c.js
+starwhale/web/ui/assets/index22-ccb7efe7.js
+starwhale/web/ui/assets/index23-680c92d8.js
+starwhale/web/ui/assets/index24-597a8e3c.js
+starwhale/web/ui/assets/index25-88e85639.js
+starwhale/web/ui/assets/index26-36e22149.js
+starwhale/web/ui/assets/index27-dee2bd12.js
+starwhale/web/ui/assets/index28-a52d95a5.js
+starwhale/web/ui/assets/index29-dd39a343.js
+starwhale/web/ui/assets/index3-f722b477.js
+starwhale/web/ui/assets/index30-edf8c102.js
+starwhale/web/ui/assets/index31-2a9aa647.js
+starwhale/web/ui/assets/index32-1efd457e.js
+starwhale/web/ui/assets/index33-988b470f.js
+starwhale/web/ui/assets/index34-e9d05f99.js
+starwhale/web/ui/assets/index35-d013c15c.js
+starwhale/web/ui/assets/index36-640baba3.js
+starwhale/web/ui/assets/index37-675e963b.js
+starwhale/web/ui/assets/index38-8ed1f571.js
+starwhale/web/ui/assets/index39-2e025855.js
+starwhale/web/ui/assets/index4-0bc63b4d.js
+starwhale/web/ui/assets/index5-f4812d85.js
+starwhale/web/ui/assets/index6-aa6ede7c.js
+starwhale/web/ui/assets/index7-644441a2.js
+starwhale/web/ui/assets/index8-dfa6b4d6.js
+starwhale/web/ui/assets/index9-74c82f9d.js
 starwhale/web/ui/assets/invalid-file-82d62dec.svg
 starwhale/web/ui/assets/left-8c88a49a.svg
 starwhale/web/ui/assets/left-shadow-e0fdfe32.png
 starwhale/web/ui/assets/linear-8d973619.js
 starwhale/web/ui/assets/logo_normal_en_blue-18b013e7.png
 starwhale/web/ui/assets/logo_normal_en_gray-163de1a0.svg
 starwhale/web/ui/assets/logo_normal_en_white-ec11283c.svg
 starwhale/web/ui/assets/logo_small_en_white-782559aa.svg
-starwhale/web/ui/assets/main-6cf1adbb.js
+starwhale/web/ui/assets/main-2ed4d8ce.js
 starwhale/web/ui/assets/module-ddaca3b9.js
 starwhale/web/ui/assets/module2-74df381a.js
 starwhale/web/ui/assets/module3-49e9a615.js
 starwhale/web/ui/assets/overpass-bold-452a631f.woff
 starwhale/web/ui/assets/overpass-bold-5c4ed5bb.woff2
 starwhale/web/ui/assets/overpass-bold-italic-16cda7ef.woff2
 starwhale/web/ui/assets/overpass-bold-italic-4926428e.woff
```

