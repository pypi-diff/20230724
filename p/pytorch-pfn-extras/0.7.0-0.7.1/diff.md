# Comparing `tmp/pytorch-pfn-extras-0.7.0.tar.gz` & `tmp/pytorch-pfn-extras-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pfn-extras-0.7.0.tar", last modified: Thu Jul 20 05:41:08 2023, max compression
+gzip compressed data, was "pytorch-pfn-extras-0.7.1.tar", last modified: Mon Jul 24 05:49:39 2023, max compression
```

## Comparing `pytorch-pfn-extras-0.7.0.tar` & `pytorch-pfn-extras-0.7.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.124438 pytorch-pfn-extras-0.7.0/
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1068 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/LICENSE
--rw-r--r--   0 linsho    (2621) linsho    (2621)      290 2023-07-20 05:41:08.124438 pytorch-pfn-extras-0.7.0/PKG-INFO
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2355 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/README.md
--rw-r--r--   0 linsho    (2621) linsho    (2621)      445 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pyproject.toml
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.768439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1408 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/__init__.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.784439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_cupy/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      421 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_cupy/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)       24 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_cupy/_cupy_stub.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.796439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/
--rw-r--r--   0 linsho    (2621) linsho    (2621)       64 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     9475 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_compile.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    11323 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_optimizer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5249 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_splitter.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5157 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_tensor.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      259 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_torch_version.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)       22 2023-07-20 05:40:58.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_version.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     9574 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/config.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1111 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/config_types.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.800439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/cuda/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      235 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/cuda/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2126 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/cuda/_allocator.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.808439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataloaders/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      130 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataloaders/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)       84 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataloaders/dataloader.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1099 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataloaders/utils.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.816439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      264 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1909 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/shared_dataset.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.844439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      558 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1056 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_asmode.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4202 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_concat.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2175 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_join.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2039 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_slice.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    10159 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_transform.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2774 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_utils.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      808 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_with_converter.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1735 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5368 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/from_data.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    11143 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.856439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      329 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1686 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_dataset_util.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2440 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2525 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_initialize.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    10020 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/engine.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.868439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      439 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3918 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_code_block.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    16492 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_handler.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    19567 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_logic.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1727 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/logging.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.868439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      756 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/__init__.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.888439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/
--rw-r--r--   0 linsho    (2621) linsho    (2621)        0 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4587 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/ensure_shape.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3935 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/extended_sequential.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     8223 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3142 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2254 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_conv.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1348 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_linear.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.896439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/parallel/
--rw-r--r--   0 linsho    (2621) linsho    (2621)       96 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/parallel/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    13431 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/parallel/distributed.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.932439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      989 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4507 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_as_output.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1021 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_constants.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      951 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_globals.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3568 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_grad.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      659 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_helper.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    21962 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_lax.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    14777 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/annotate.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    19142 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/export_testcase.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1231 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/load.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.940439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/pfto_exporter/
--rw-r--r--   0 linsho    (2621) linsho    (2621)       60 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/pfto_exporter/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    49631 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/pfto_exporter/export.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3470 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/strip_large_tensor.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1129 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/symbolic_registry.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4784 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/unstrip_tensor.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.948439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      360 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2934 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/_record.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    11641 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/_time_summary.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)        0 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/py.typed
--rw-r--r--   0 linsho    (2621) linsho    (2621)    15252 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/reporting.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.968439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      266 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1257 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_autocast.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      380 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_map.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      834 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_registry.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    17981 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_runtime.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2546 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_to.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1363 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/testing.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      518 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/torchscript.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.000439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1060 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     6547 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_evaluator.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1749 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_manager_protocol.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    15637 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_trainer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      456 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_transform_model.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2953 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_trigger_util.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      716 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_util.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    10466 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extension.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.072439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2523 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    19361 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/_snapshot.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4477 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/best_value.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    17529 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/evaluator.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1416 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/fail_on_non_number.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    10600 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/log_report.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2633 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/lr_scheduler.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3693 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/micro_average.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     7595 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/parameter_statistics.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     8512 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/plot_report.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     6804 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/print_report.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2161 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/print_report_notebook.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     6145 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/profile_report.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4151 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/progress_bar.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5366 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    14659 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/slack.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)       82 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/snapshot_writers.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     4412 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/util.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2024 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/value_observation.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    15851 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    28835 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/manager.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1142 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/metrics.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      512 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/trigger.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.096439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      680 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5012 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2891 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/interval_trigger.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2411 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5093 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1663 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/once_trigger.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)      974 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/time_trigger.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.104438 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      110 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2018 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/checkpoint.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    27771 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/comparer.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:08.120438 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      698 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/__init__.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     3011 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_parallel_writer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5428 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_queue_writer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     1556 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_simple_writer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)     2802 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_tensorboard_writer.py
--rw-r--r--   0 linsho    (2621) linsho    (2621)    12880 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_writer_base.py
-drwxr-xr-x   0 linsho    (2621) linsho    (2621)        0 2023-07-20 05:41:07.780439 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/
--rw-r--r--   0 linsho    (2621) linsho    (2621)      290 2023-07-20 05:41:07.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/PKG-INFO
--rw-r--r--   0 linsho    (2621) linsho    (2621)     5795 2023-07-20 05:41:07.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/SOURCES.txt
--rw-r--r--   0 linsho    (2621) linsho    (2621)        1 2023-07-20 05:41:07.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/dependency_links.txt
--rw-r--r--   0 linsho    (2621) linsho    (2621)       98 2023-07-20 05:41:07.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/requires.txt
--rw-r--r--   0 linsho    (2621) linsho    (2621)       19 2023-07-20 05:41:07.000000 pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/top_level.txt
--rw-r--r--   0 linsho    (2621) linsho    (2621)      709 2023-07-20 05:41:08.128439 pytorch-pfn-extras-0.7.0/setup.cfg
--rw-r--r--   0 linsho    (2621) linsho    (2621)      784 2023-07-19 07:10:45.000000 pytorch-pfn-extras-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.626589 pytorch-pfn-extras-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 05:49:39.630589 pytorch-pfn-extras-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_cupy/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_cupy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_cupy/_cupy_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_torch_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/config_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/cuda/_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataloaders/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataloaders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/shared_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_asmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_with_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/from_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_dataset_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_code_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19567 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/ensure_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/extended_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.618589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/parallel/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.622589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_as_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21962 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_lax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/export_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.622589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/pfto_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/pfto_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49631 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/pfto_exporter/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/strip_large_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/symbolic_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/unstrip_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.622589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/_time_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.622589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.622589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_manager_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_transform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_trigger_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.626589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19361 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/best_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/fail_on_non_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/log_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/micro_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/parameter_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/plot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/print_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/print_report_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/profile_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/snapshot_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/value_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28835 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.626589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/interval_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/once_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/time_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.626589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27771 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/comparer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.626589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_parallel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_simple_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_writer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:49:39.614589 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 05:49:39.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-24 05:49:39.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:49:39.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 05:49:39.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 05:49:39.000000 pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 05:49:39.630589 pytorch-pfn-extras-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 05:49:28.000000 pytorch-pfn-extras-0.7.1/setup.py
```

### Comparing `pytorch-pfn-extras-0.7.0/LICENSE` & `pytorch-pfn-extras-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/README.md` & `pytorch-pfn-extras-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_compile.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_compile.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_optimizer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_dynamo/_splitter.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_dynamo/_splitter.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/_tensor.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/config.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/config.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/config_types.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/config_types.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/cuda/_allocator.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/cuda/_allocator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataloaders/utils.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataloaders/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/shared_dataset.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/shared_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_asmode.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_asmode.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_concat.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_concat.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_join.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_join.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_slice.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_slice.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_transform.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_transform.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_utils.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/_with_converter.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/_with_converter.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/from_data.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/from_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_dataset_util.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_dataset_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/distributed/_initialize.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/distributed/_initialize.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/engine.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_code_block.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_code_block.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_handler.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/handler/_logic.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/handler/_logic.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/logging.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/logging.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/ensure_shape.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/ensure_shape.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/extended_sequential.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/extended_sequential.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_conv.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_conv.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/modules/lazy_linear.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/modules/lazy_linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/nn/parallel/distributed.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/nn/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_as_output.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_as_output.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_constants.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_constants.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_globals.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_globals.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_grad.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_grad.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_helper.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_helper.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/_lax.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/_lax.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/annotate.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/annotate.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/export_testcase.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/export_testcase.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/load.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/load.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/pfto_exporter/export.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/pfto_exporter/export.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/strip_large_tensor.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/strip_large_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/symbolic_registry.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/symbolic_registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/onnx/unstrip_tensor.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/onnx/unstrip_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/_record.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/_record.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/profiler/_time_summary.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/profiler/_time_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,15 +124,19 @@
         self._thread_exited = False
 
     def initialize(self) -> None:
         if self._initialized:
             return
         self._queue = queue.Queue(self._max_queue_size)
         self._events = queue.Queue(self._max_queue_size * 2)
-        self._thread = threading.Thread(target=self._worker, daemon=True)
+        self._thread = threading.Thread(
+            target=self._worker,
+            args=(torch.cuda.current_device(),),
+            daemon=True,
+        )
         self._thread.start()
         self._initialized = True
         self._thread_exited = False
 
     def finalize(self) -> None:
         if not self._initialized:
             return
@@ -152,27 +156,30 @@
         name: str,
         events: Tuple[torch.cuda.Event, torch.cuda.Event],
     ) -> None:
         assert self._queue is not None
         assert not self._thread_exited
         self._queue.put((name, events))
 
-    def _worker(self) -> None:
+    def _worker(self, device_id: int) -> None:
         assert self._queue is not None
         assert self._events is not None
+        torch.cuda.set_device(device_id)
         while True:
             try:
                 v = self._queue.get()
             except EOFError:
                 self._thread_exited = True
                 break
             if v is None:
                 self._queue.task_done()
                 break
             name, (begin, end) = v
+            assert begin.device == end.device
+            assert begin.device.index == torch.cuda.current_device()
             end.synchronize()  # type: ignore[no-untyped-call]
             t_ms = begin.elapsed_time(end)  # type: ignore[no-untyped-call]
             self._add(name, t_ms / 1000)
             with self._event_lock:
                 self._events.put(begin)
                 self._events.put(end)
             self._queue.task_done()
```

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/reporting.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/reporting.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_autocast.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_autocast.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_registry.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_runtime.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_runtime.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/runtime/_to.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/runtime/_to.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/testing.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/testing.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/torchscript.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/torchscript.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_evaluator.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_evaluator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_manager_protocol.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_manager_protocol.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_trainer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_trigger_util.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_trigger_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/_util.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extension.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extension.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/_snapshot.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/_snapshot.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/best_value.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/best_value.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/evaluator.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/evaluator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/fail_on_non_number.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/fail_on_non_number.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/log_report.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/log_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/lr_scheduler.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/micro_average.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/micro_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/parameter_statistics.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/parameter_statistics.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/plot_report.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/plot_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/print_report.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/print_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/print_report_notebook.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/print_report_notebook.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/profile_report.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/profile_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/progress_bar.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/slack.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/slack.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/util.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/value_observation.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/value_observation.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/manager.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/manager.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/metrics.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/metrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/interval_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/interval_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/once_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/once_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/training/triggers/time_trigger.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/training/triggers/time_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/checkpoint.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/utils/comparer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/utils/comparer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/__init__.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_parallel_writer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_parallel_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_queue_writer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_queue_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_simple_writer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_simple_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_tensorboard_writer.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras/writing/_writer_base.py` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras/writing/_writer_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/pytorch_pfn_extras.egg-info/SOURCES.txt` & `pytorch-pfn-extras-0.7.1/pytorch_pfn_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/setup.cfg` & `pytorch-pfn-extras-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.7.0/setup.py` & `pytorch-pfn-extras-0.7.1/setup.py`

 * *Files identical despite different names*

