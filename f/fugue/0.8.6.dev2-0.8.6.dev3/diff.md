# Comparing `tmp/fugue-0.8.6.dev2.tar.gz` & `tmp/fugue-0.8.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.6.dev2.tar", last modified: Sat Jul 22 18:36:12 2023, max compression
+gzip compressed data, was "fugue-0.8.6.dev3.tar", last modified: Mon Jul 24 06:45:03 2023, max compression
```

## Comparing `fugue-0.8.6.dev2.tar` & `fugue-0.8.6.dev3.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.849341 fugue-0.8.6.dev2/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.849341 fugue-0.8.6.dev2/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    78396 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-22 18:36:12.869341 fugue-0.8.6.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-24 06:45:03.000000 fugue-0.8.6.dev3/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78396 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 06:45:03.154468 fugue-0.8.6.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/setup.py
```

### Comparing `fugue-0.8.6.dev2/LICENSE` & `fugue-0.8.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/PKG-INFO` & `fugue-0.8.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev2
+Version: 0.8.6.dev3
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev2/README.md` & `fugue-0.8.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/__init__.py` & `fugue-0.8.6.dev3/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/_utils/display.py` & `fugue-0.8.6.dev3/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/_utils/exception.py` & `fugue-0.8.6.dev3/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/_utils/interfaceless.py` & `fugue-0.8.6.dev3/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/_utils/io.py` & `fugue-0.8.6.dev3/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/_utils/misc.py` & `fugue-0.8.6.dev3/fugue/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/api.py` & `fugue-0.8.6.dev3/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/bag/array_bag.py` & `fugue-0.8.6.dev3/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/bag/bag.py` & `fugue-0.8.6.dev3/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/collections/partition.py` & `fugue-0.8.6.dev3/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/collections/sql.py` & `fugue-0.8.6.dev3/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/collections/yielded.py` & `fugue-0.8.6.dev3/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/column/expressions.py` & `fugue-0.8.6.dev3/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/column/functions.py` & `fugue-0.8.6.dev3/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/column/sql.py` & `fugue-0.8.6.dev3/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/constants.py` & `fugue-0.8.6.dev3/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/__init__.py` & `fugue-0.8.6.dev3/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/api.py` & `fugue-0.8.6.dev3/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/array_dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/dataframes.py` & `fugue-0.8.6.dev3/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/function_wrapper.py` & `fugue-0.8.6.dev3/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.6.dev3/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataframe/utils.py` & `fugue-0.8.6.dev3/fugue/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataset/api.py` & `fugue-0.8.6.dev3/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dataset/dataset.py` & `fugue-0.8.6.dev3/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/dev.py` & `fugue-0.8.6.dev3/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/exceptions.py` & `fugue-0.8.6.dev3/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/execution/api.py` & `fugue-0.8.6.dev3/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/execution/execution_engine.py` & `fugue-0.8.6.dev3/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/execution/factory.py` & `fugue-0.8.6.dev3/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/execution/native_execution_engine.py` & `fugue-0.8.6.dev3/fugue/execution/native_execution_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Type, Union
-
+import numpy as np
 import pandas as pd
 from triad import Schema
 from triad.collections.dict import IndexedOrderedDict
 from triad.collections.fs import FileSystem
 from triad.utils.assertion import assert_or_throw
 from triad.utils.pandas_like import PandasUtils
 
@@ -13,14 +13,15 @@
 from fugue._utils.misc import import_fsql_dependency
 from fugue.collections.partition import (
     PartitionCursor,
     PartitionSpec,
     parse_presort_exp,
 )
 from fugue.collections.sql import StructuredRawSQL
+from fugue.constants import KEYWORD_PARALLELISM, KEYWORD_ROWCOUNT
 from fugue.dataframe import (
     AnyDataFrame,
     DataFrame,
     DataFrames,
     LocalBoundedDataFrame,
     LocalDataFrame,
     PandasDataFrame,
@@ -104,21 +105,45 @@
         ):  # no partition
             if len(partition_spec.presort) > 0:
                 pdf = (
                     df.as_pandas()
                     .sort_values(presort_keys, ascending=presort_asc)
                     .reset_index(drop=True)
                 )
-                input_df = PandasDataFrame(pdf, df.schema, pandas_df_wrapper=True)
-                cursor.set(lambda: input_df.peek_array(), cursor.partition_no + 1, 0)
-                output_df = map_func(cursor, input_df)
+                input_df: LocalDataFrame = PandasDataFrame(
+                    pdf, df.schema, pandas_df_wrapper=True
+                )
             else:
-                df = df.as_local()
-                cursor.set(lambda: df.peek_array(), 0, 0)
-                output_df = map_func(cursor, df)
+                input_df = df.as_local()
+            if (
+                len(partition_spec.partition_by) == 0
+                and partition_spec.num_partitions != "0"
+            ):
+                partitions = partition_spec.get_num_partitions(
+                    **{
+                        KEYWORD_ROWCOUNT: lambda: df.count(),  # type: ignore
+                        KEYWORD_PARALLELISM: lambda: 1,
+                    }
+                )
+                dfs: List[DataFrame] = []
+                for p, subdf in enumerate(
+                    np.array_split(input_df.as_pandas(), partitions)
+                ):
+                    if len(subdf) > 0:
+                        tdf = PandasDataFrame(subdf, df.schema, pandas_df_wrapper=True)
+                        cursor.set(lambda: tdf.peek_array(), p, 0)
+                        dfs.append(map_func(cursor, tdf).as_pandas())
+                output_df: LocalDataFrame = PandasDataFrame(
+                    pd.concat(dfs, ignore_index=True),
+                    schema=output_schema,
+                    pandas_df_wrapper=True,
+                )
+            else:
+                cursor.set(lambda: input_df.peek_array(), 0, 0)
+                output_df = map_func(cursor, input_df)
             if (
                 isinstance(output_df, PandasDataFrame)
                 and output_df.schema != output_schema
             ):
                 output_df = PandasDataFrame(output_df.native, output_schema)
             assert_or_throw(
                 output_df.schema == output_schema,
```

### Comparing `fugue-0.8.6.dev2/fugue/extensions/__init__.py` & `fugue-0.8.6.dev3/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.6.dev3/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/_builtins/creators.py` & `fugue-0.8.6.dev3/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.6.dev3/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/_builtins/processors.py` & `fugue-0.8.6.dev3/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/_utils.py` & `fugue-0.8.6.dev3/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/context.py` & `fugue-0.8.6.dev3/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/creator/convert.py` & `fugue-0.8.6.dev3/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/creator/creator.py` & `fugue-0.8.6.dev3/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/outputter/convert.py` & `fugue-0.8.6.dev3/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/outputter/outputter.py` & `fugue-0.8.6.dev3/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/processor/convert.py` & `fugue-0.8.6.dev3/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/processor/processor.py` & `fugue-0.8.6.dev3/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/transformer/convert.py` & `fugue-0.8.6.dev3/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/extensions/transformer/transformer.py` & `fugue-0.8.6.dev3/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/plugins.py` & `fugue-0.8.6.dev3/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/registry.py` & `fugue-0.8.6.dev3/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/rpc/base.py` & `fugue-0.8.6.dev3/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/rpc/flask.py` & `fugue-0.8.6.dev3/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/sql/_utils.py` & `fugue-0.8.6.dev3/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/sql/_visitors.py` & `fugue-0.8.6.dev3/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/sql/api.py` & `fugue-0.8.6.dev3/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/sql/workflow.py` & `fugue-0.8.6.dev3/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/_checkpoint.py` & `fugue-0.8.6.dev3/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/_tasks.py` & `fugue-0.8.6.dev3/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/_workflow_context.py` & `fugue-0.8.6.dev3/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/api.py` & `fugue-0.8.6.dev3/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/module.py` & `fugue-0.8.6.dev3/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue/workflow/workflow.py` & `fugue-0.8.6.dev3/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue.egg-info/PKG-INFO` & `fugue-0.8.6.dev3/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev2
+Version: 0.8.6.dev3
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev2/fugue.egg-info/SOURCES.txt` & `fugue-0.8.6.dev3/fugue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue.egg-info/requires.txt` & `fugue-0.8.6.dev3/fugue.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.6.dev3/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_contrib/viz/__init__.py` & `fugue-0.8.6.dev3/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_contrib/viz/_ext.py` & `fugue-0.8.6.dev3/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/_io.py` & `fugue-0.8.6.dev3/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/_utils.py` & `fugue-0.8.6.dev3/fugue_dask/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/dataframe.py` & `fugue-0.8.6.dev3/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/execution_engine.py` & `fugue-0.8.6.dev3/fugue_dask/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/ibis_engine.py` & `fugue-0.8.6.dev3/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_dask/registry.py` & `fugue-0.8.6.dev3/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/_io.py` & `fugue-0.8.6.dev3/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/_utils.py` & `fugue-0.8.6.dev3/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/dask.py` & `fugue-0.8.6.dev3/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/dataframe.py` & `fugue-0.8.6.dev3/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/execution_engine.py` & `fugue-0.8.6.dev3/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/ibis_engine.py` & `fugue-0.8.6.dev3/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_duckdb/registry.py` & `fugue-0.8.6.dev3/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/_utils.py` & `fugue-0.8.6.dev3/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/dataframe.py` & `fugue-0.8.6.dev3/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.6.dev3/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.6.dev3/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/execution_engine.py` & `fugue-0.8.6.dev3/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ibis/extensions.py` & `fugue-0.8.6.dev3/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_notebook/__init__.py` & `fugue-0.8.6.dev3/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_notebook/env.py` & `fugue-0.8.6.dev3/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_notebook/nbextension/main.js` & `fugue-0.8.6.dev3/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_polars/polars_dataframe.py` & `fugue-0.8.6.dev3/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_polars/registry.py` & `fugue-0.8.6.dev3/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/_constants.py` & `fugue-0.8.6.dev3/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/_utils/cluster.py` & `fugue-0.8.6.dev3/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/_utils/dataframe.py` & `fugue-0.8.6.dev3/fugue_ray/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/_utils/io.py` & `fugue-0.8.6.dev3/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/dataframe.py` & `fugue-0.8.6.dev3/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/execution_engine.py` & `fugue-0.8.6.dev3/fugue_ray/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_ray/registry.py` & `fugue-0.8.6.dev3/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/_utils/convert.py` & `fugue-0.8.6.dev3/fugue_spark/_utils/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/_utils/io.py` & `fugue-0.8.6.dev3/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/_utils/misc.py` & `fugue-0.8.6.dev3/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/_utils/partition.py` & `fugue-0.8.6.dev3/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/dataframe.py` & `fugue-0.8.6.dev3/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/execution_engine.py` & `fugue-0.8.6.dev3/fugue_spark/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/ibis_engine.py` & `fugue-0.8.6.dev3/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_spark/registry.py` & `fugue-0.8.6.dev3/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_test/bag_suite.py` & `fugue-0.8.6.dev3/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_test/builtin_suite.py` & `fugue-0.8.6.dev3/fugue_test/builtin_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_test/dataframe_suite.py` & `fugue-0.8.6.dev3/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_test/execution_suite.py` & `fugue-0.8.6.dev3/fugue_test/execution_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/fugue_test/ibis_suite.py` & `fugue-0.8.6.dev3/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/setup.cfg` & `fugue-0.8.6.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev2/setup.py` & `fugue-0.8.6.dev3/setup.py`

 * *Files identical despite different names*

