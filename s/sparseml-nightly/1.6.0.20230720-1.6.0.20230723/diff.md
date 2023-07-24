# Comparing `tmp/sparseml_nightly-1.6.0.20230720-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230723-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,378 +1,378 @@
-Zip file size: 970811 bytes, number of entries: 376
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-20 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jul-20 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-20 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-20 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-20 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jul-20 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-20 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-20 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jul-20 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-20 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-20 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-20 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-20 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-20 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-20 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-20 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-20 01:31 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4847 b- defN 23-Jul-20 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     4630 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     6297 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3433 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/propagate_dequant_through_split.py
--rw-rw-r--  2.0 unx     4801 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    30558 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6523 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/configs.py
--rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
--rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-20 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-20 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-20 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-20 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-20 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-20 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jul-20 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-20 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jul-20 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-20 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jul-20 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-20 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jul-20 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-20 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-20 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-20 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-20 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-20 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-20 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-20 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-20 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-20 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-20 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-20 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jul-20 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-20 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jul-20 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-20 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-20 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-20 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-20 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-20 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-20 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-20 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jul-20 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-20 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jul-20 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-20 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-20 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jul-20 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-20 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-20 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-20 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-20 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jul-20 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-20 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-20 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-20 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jul-20 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-20 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-20 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-20 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-20 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-20 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-20 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-20 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jul-20 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    11013 b- defN 23-Jul-20 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4457 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jul-20 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jul-20 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-20 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-20 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jul-20 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-20 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-20 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-20 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-20 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-20 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-20 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-20 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-20 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-20 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-20 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    18014 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-20 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-20 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31241 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    41226 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-20 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jul-20 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-20 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-20 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-20 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-20 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-20 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-20 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-20 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-20 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-20 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-20 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-20 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-20 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-20 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-20 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-20 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-20 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-20 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36976 b- defN 23-Jul-20 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-20 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-20 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-20 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-20 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-20 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-20 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-20 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-20 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-20 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17074 b- defN 23-Jul-20 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jul-20 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jul-20 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-20 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-20 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-20 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-20 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-20 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-20 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-20 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-20 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-20 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-20 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-20 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-20 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-20 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-20 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-20 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     6061 b- defN 23-Jul-20 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-20 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-20 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7394 b- defN 23-Jul-20 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    37320 b- defN 23-Jul-20 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-20 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8459 b- defN 23-Jul-20 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jul-20 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6683 b- defN 23-Jul-20 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-20 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21838 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37503 b- defN 23-Jul-20 01:36 sparseml_nightly-1.6.0.20230720.dist-info/RECORD
-376 files, 3511960 bytes uncompressed, 910059 bytes compressed:  74.1%
+Zip file size: 969880 bytes, number of entries: 376
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-23 01:31 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jul-23 01:31 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-23 01:31 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-23 01:31 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-23 01:31 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jul-23 01:31 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-23 01:31 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-23 01:31 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jul-23 01:31 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-23 01:31 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-23 01:31 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-23 01:31 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-23 01:31 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-23 01:31 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-23 01:31 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-23 01:31 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4847 b- defN 23-Jul-23 01:31 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     4630 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     6297 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3433 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/propagate_dequant_through_split.py
+-rw-rw-r--  2.0 unx     4801 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      909 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    30558 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6523 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/configs.py
+-rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+-rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-23 01:31 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-23 01:31 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-23 01:31 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-23 01:31 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jul-23 01:31 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-23 01:31 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jul-23 01:31 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-23 01:31 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-23 01:31 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-23 01:31 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jul-23 01:31 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-23 01:31 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-23 01:31 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-23 01:31 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-23 01:31 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-23 01:31 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-23 01:31 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jul-23 01:31 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-23 01:31 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jul-23 01:31 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-23 01:31 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-23 01:31 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-23 01:31 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-23 01:31 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-23 01:31 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-23 01:31 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-23 01:31 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jul-23 01:31 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-23 01:31 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jul-23 01:31 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-23 01:31 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jul-23 01:31 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-23 01:31 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-23 01:31 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-23 01:31 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-23 01:31 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-23 01:31 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-23 01:31 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-23 01:31 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jul-23 01:31 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    11013 b- defN 23-Jul-23 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4457 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jul-23 01:31 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-23 01:31 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31241 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    41226 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jul-23 01:31 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-23 01:31 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-23 01:31 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-23 01:31 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-23 01:31 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-23 01:31 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-23 01:31 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-23 01:31 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-23 01:31 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-23 01:31 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-23 01:31 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-23 01:31 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-23 01:31 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36976 b- defN 23-Jul-23 01:31 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-23 01:31 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-23 01:31 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17074 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jul-23 01:31 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jul-23 01:31 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-23 01:31 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-23 01:31 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-23 01:31 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-23 01:31 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-23 01:31 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-23 01:31 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-23 01:31 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-23 01:31 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-23 01:31 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-23 01:31 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-23 01:31 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-23 01:31 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-23 01:31 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jul-23 01:31 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jul-23 01:31 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-23 01:31 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-23 01:31 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jul-23 01:31 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    35999 b- defN 23-Jul-23 01:31 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-23 01:31 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jul-23 01:31 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6247 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21837 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37503 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/RECORD
+376 files, 3509348 bytes uncompressed, 909128 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1101,29 +1101,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230720.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230723.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/pytorch/sparsification/quantization/quantize.py

```diff
@@ -358,15 +358,16 @@
 ) -> Optional[str]:
     # match preferences:
     #   1. match module type name
     #   2. match the submodule prefix (longest first)
     submodule_match = ""
     for name_or_type in names_or_types:
         name_to_compare = submodule_name[:]
-        name_to_compare = _maybe_discard_prefix(name_to_compare)
+        if name_to_compare.startswith("module."):
+            name_to_compare = name_to_compare[7:]
         if name_or_type == submodule.__class__.__name__:
             # type match, return type name
             return name_or_type
         if name_to_compare.startswith(name_or_type) and (
             len(name_or_type) > len(submodule_match)
         ):
             # match to most specific submodule name
@@ -421,15 +422,16 @@
 ):
     def _get_unmatched_types_or_names(types_or_names):
         unmatched = []
         for type_or_name in types_or_names:
             matched = False
             for submodule_name, submodule in model.named_modules():
                 name_to_compare = submodule_name[:]
-                name_to_compare = _maybe_discard_prefix(name_to_compare)
+                if name_to_compare.startswith("module."):
+                    name_to_compare = name_to_compare[7:]
                 if name_to_compare.startswith(type_or_name) or (
                     submodule.__class__.__name__ == type_or_name
                 ):
                     matched = True
                     break
             if not matched:
                 unmatched.append(type_or_name)
@@ -447,14 +449,7 @@
         raise ValueError(
             _build_error_str("scheme_overrides", unmatched_scheme_overrides)
         )
 
     unmatched_ignore = _get_unmatched_types_or_names(ignore)
     if unmatched_ignore:
         raise ValueError(_build_error_str("ignore", unmatched_ignore))
-
-
-def _maybe_discard_prefix(name: str) -> str:
-    for prefix in ["module.", "model."]:
-        if name.startswith(prefix):
-            name = name.replace(prefix, "", 1)
-    return name
```

## sparseml/yolov8/__init__.py

```diff
@@ -20,12 +20,12 @@
     import ultralytics as _ultralytics  # noqa: F401
 except ImportError:
     raise ImportError("Please install sparseml[yolov8] to use this pathway")
 
 
 _analytics.send_event("python__yolov8__init")
 
-if "8.0.124" not in ultralytics.__version__:
+if "8.0.30" not in ultralytics.__version__:
     raise ValueError(
-        f"ultralytics==8.0.124 is required, found {ultralytics.__version__}. "
+        f"ultralytics==8.0.30 is required, found {ultralytics.__version__}. "
         "To fix run `pip install sparseml[ultralytics]`."
     )
```

## sparseml/yolov8/default.yaml

```diff
@@ -29,17 +29,14 @@
 deterministic: True # whether to enable deterministic mode
 single_cls: False # train multi-class data as single-class
 image_weights: False # use weighted image selection for training
 rect: False # support rectangular training
 cos_lr: False # use cosine learning rate scheduler
 close_mosaic: 10 # disable mosaic augmentation for final 10 epochs
 resume: False # resume training from last checkpoint
-amp: True # (bool) Automatic Mixed Precision (AMP) training, choices=[True, False], True runs AMP check
-fraction: 1.0  # (float) dataset fraction to train on (default is 1.0, all images in train set)
-profile: False # (bool) profile ONNX and TensorRT speeds during training for loggers
 min_memory: False  # minimize memory footprint loss function, choices=[False, True, <roll_out_thr>]
 
 # Segmentation
 overlap_mask: True # masks should overlap during training
 mask_ratio: 4 # mask downsample ratio
 # Classification
 dropout: 0.0  # use dropout regularization
@@ -49,27 +46,27 @@
 split: val  # dataset split to use for validation, i.e. 'val', 'test' or 'train'
 save_json: False # save results to JSON file
 save_hybrid: False # save hybrid version of labels (labels + additional predictions)
 conf: null # object confidence threshold for detection (default 0.25 predict, 0.001 val)
 iou: 0.7 # intersection over union (IoU) threshold for NMS
 max_det: 300 # maximum number of detections per image
 half: False # use half precision (FP16)
-dnn: False # use OpenCV DNN for ONNX inferences
+dnn: False # use OpenCV DNN for ONNX inference
 plots: True # show plots during training
 
 # Prediction settings --------------------------------------------------------------------------------------------------
 source: null # source directory for images or videos
 show: False # show results if possible
 save_txt: False # save results as .txt file
 save_conf: False # save results with confidence scores
 save_crop: False # save cropped images with results
-show_labels: True # hide labels
-show_conf: True # hide confidence scores
+hide_labels: False # hide labels
+hide_conf: False # hide confidence scores
 vid_stride: 1 # video frame-rate stride
-line_width: 3 # bounding box thickness (pixels)
+line_thickness: 3 # bounding box thickness (pixels)
 visualize: False # visualize results
 augment: False # apply data augmentation to images
 agnostic_nms: False # class-agnostiic NMS
 classes:  # filter results by class, i.e. class=0, or class=[0,2,3]
 retina_masks: False # use retina masks for object detection
 boxes: True # Show boxes in segmentation predictions
```

## sparseml/yolov8/train.py

```diff
@@ -46,21 +46,21 @@
     type=click.Choice(["detect", "segment", "classify"]),
     help="Specify task to run.",
 )
 @click.option(
     "--model",
     default="yolov8n.yaml",
     type=str,
-    help="i.e. yolov8n.pt, yolov8n.yaml, yolov8n-seg.yaml. Path to model file",
+    help="i.e. yolov8n.pt, yolov8n.yaml. Path to model file",
 )
 @click.option(
     "--data",
     default="coco128.yaml",
     type=str,
-    help="i.e. coco128.yaml, coco128-seg.yaml. Path to data file",
+    help="i.e. coco128.yaml. Path to data file",
 )
 @click.option("--epochs", default=100, type=int, help="number of epochs to train for")
 @click.option(
     "--patience",
     default=50,
     type=int,
     help="epochs to wait for no observable improvement for early stopping of training",
@@ -217,15 +217,13 @@
     help="Path to override default dataset path.",
 )
 def main(**kwargs):
     if kwargs["dataset_path"] is not None:
         kwargs["data"] = data_from_dataset_path(kwargs["data"], kwargs["dataset_path"])
     del kwargs["dataset_path"]
 
-    # NOTE: the task, model, and data kwargs will override the values in default.yaml
-    # They should be provided or default values will be used.
-    model = SparseYOLO(kwargs["model"], kwargs["task"])
+    model = SparseYOLO(kwargs["model"])
     model.train(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/yolov8/trainers.py

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from copy import copy, deepcopy
 from datetime import datetime, timedelta
@@ -48,29 +47,25 @@
 from sparsezoo import Model
 from sparsezoo.utils import validate_onnx
 from ultralytics import __version__
 from ultralytics.nn.modules import Detect, Segment
 from ultralytics.nn.tasks import SegmentationModel, attempt_load_one_weight
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
-from ultralytics.yolo.engine.model import TASK_MAP, YOLO
+from ultralytics.yolo.engine.model import YOLO
 from ultralytics.yolo.engine.trainer import BaseTrainer
 from ultralytics.yolo.utils import LOGGER, IterableSimpleNamespace, yaml_load
 from ultralytics.yolo.utils.checks import check_file, check_imgsz, check_yaml
 from ultralytics.yolo.utils.dist import (
     USER_CONFIG_DIR,
     ddp_cleanup,
     find_free_network_port,
 )
 from ultralytics.yolo.utils.files import get_latest_run
-from ultralytics.yolo.utils.torch_utils import (
-    TORCH_1_9,
-    de_parallel,
-    smart_inference_mode,
-)
+from ultralytics.yolo.utils.torch_utils import de_parallel, smart_inference_mode
 from ultralytics.yolo.v8.classify import ClassificationTrainer, ClassificationValidator
 from ultralytics.yolo.v8.detect import DetectionTrainer, DetectionValidator
 from ultralytics.yolo.v8.segment import SegmentationTrainer, SegmentationValidator
 
 
 class _NullLRScheduler:
     def step(self):
@@ -156,31 +151,23 @@
                 ) from e
         self.resume = resume
 
     def train(self):
         # NOTE: overriden to use our version of `generate_ddp_command`
         world_size = torch.cuda.device_count()
         if world_size > 1 and "LOCAL_RANK" not in os.environ:
-            if self.args.rect:
-                LOGGER.warning(
-                    "WARNING ⚠️ 'rect=True' is incompatible with Multi-GPU training, "
-                    "setting rect=False"
-                )
-                self.args.rect = False
-
-            command, file = generate_ddp_command(world_size, self)
+            command = generate_ddp_command(world_size, self)
             try:
-                LOGGER.info(f"DDP command: {command}")
-                subprocess.run(command, check=True)
+                subprocess.run(command)
             except Exception as e:
-                raise e
+                self.console(e)
             finally:
-                ddp_cleanup(command, str(file))
+                ddp_cleanup(command, self)
         else:
-            self._do_train(world_size)
+            self._do_train(int(os.getenv("RANK", -1)), world_size)
 
     def setup_model(self):
         # NOTE: override to handle pickled checkpoints and our own checkpoints
         if isinstance(self.model, torch.nn.Module):
             LOGGER.info("Received torch.nn.Module, not loading from checkpoint")
             self._build_managers(ckpt=None)
             return
@@ -285,18 +272,16 @@
             try:
                 self.ema.ema.load_state_dict(ema_state_dict)
             except RuntimeError:
                 LOGGER.warning("Unable to load EMA weights - disabling EMA.")
                 self.ema.enabled = False
             self.ema.updates = ckpt["updates"]
 
-    def _setup_train(self, world_size):
-        rank = int(os.getenv("RANK", -1))
-
-        super()._setup_train(world_size)
+    def _setup_train(self, rank, world_size):
+        super()._setup_train(rank, world_size)
         # NOTE: self.resume_training() was called in ^
 
         if rank in {0, -1}:
             self.test_loader = self.get_dataloader(
                 self.testset,
                 batch_size=max(1, self.train_loader.batch_size // 4),
                 rank=-1,
@@ -351,27 +336,26 @@
                 self.optimizer,
                 steps_per_epoch=self.steps_per_epoch,
                 epoch=self.start_epoch,
                 wrap_optim=self.scaler,
                 loggers=self.logger_manager,
                 grad_sampler={
                     "data_loader_builder": self._get_data_loader_builder(),
-                    "loss_function": lambda preds, batch: self.model.loss(
-                        batch=batch, preds=preds
-                    )[0]
+                    "loss_function": lambda preds, batch: self.criterion(preds, batch)[
+                        0
+                    ]
                     / self.train_loader.batch_size,
                 },
             )
         else:
             # initialize steps_per_epoch for logging when there's no recipe
             self.steps_per_epoch = len(self.train_loader)
 
-    def _setup_ddp(self, world_size):
+    def _setup_ddp(self, rank, world_size):
         # increases the timeout for DDP processes
-        rank = int(os.getenv("RANK", -1))
         torch.cuda.set_device(rank)
         self.device = torch.device("cuda", rank)
         LOGGER.info(
             f"DDP settings: RANK {rank}, WORLD_SIZE {world_size}, DEVICE {self.device}"
         )
         torch.distributed.init_process_group(
             "nccl" if torch.distributed.is_nccl_available() else "gloo",
@@ -531,36 +515,40 @@
 
 class SparseDetectionTrainer(SparseTrainer, DetectionTrainer):
     def get_validator(self):
         self.loss_names = "box_loss", "cls_loss", "dfl_loss"
         return SparseDetectionValidator(
             self.test_loader,
             save_dir=self.save_dir,
+            logger=self.console,
             args=copy(self.args),
         )
 
 
 class SparseClassificationTrainer(SparseTrainer, ClassificationTrainer):
     def get_validator(self):
         self.loss_names = ["loss"]
-        return SparseClassificationValidator(self.test_loader, self.save_dir)
+        return SparseClassificationValidator(
+            self.test_loader, self.save_dir, logger=self.console
+        )
 
 
 class SparseSegmentationTrainer(SparseTrainer, SegmentationTrainer):
     def get_validator(self):
         self.loss_names = "box_loss", "seg_loss", "cls_loss", "dfl_loss"
         return SparseSegmentationValidator(
             self.test_loader,
             save_dir=self.save_dir,
+            logger=self.console,
             args=copy(self.args),
         )
 
 
 class SparseYOLO(YOLO):
-    def __init__(self, model="yolov8n.yaml", task="detect") -> None:
+    def __init__(self, model="yolov8n.yaml", type="v8") -> None:
         model_str = str(model)
 
         if model_str.startswith("zoo:"):
             model = download_framework_model_by_recipe_type(
                 Model(model_str), model_suffix="pt"
             )
             model_str = str(model)
@@ -573,20 +561,15 @@
                     "source" in ckpt and ckpt["source"] == "sparseml"
                 )
             else:
                 self.is_sparseml_checkpoint = False
         else:
             self.is_sparseml_checkpoint = False
 
-        super().__init__(model, task)
-
-        self.ModelClass = TASK_MAP[self.task][0]
-        self.TrainerClass = TASK_MAP[self.task][1]
-        self.ValidatorClass = TASK_MAP[self.task][2]
-        self.PredictorClass = TASK_MAP[self.task][3]
+        super().__init__(model, type)
 
         if self.TrainerClass == DetectionTrainer:
             self.TrainerClass = SparseDetectionTrainer
         elif self.TrainerClass == ClassificationTrainer:
             self.TrainerClass = SparseClassificationTrainer
         elif self.TrainerClass == SegmentationTrainer:
             self.TrainerClass = SparseSegmentationTrainer
@@ -594,15 +577,15 @@
         if self.ValidatorClass == DetectionValidator:
             self.ValidatorClass = SparseDetectionValidator
         elif self.ValidatorClass == ClassificationValidator:
             self.ValidatorClass = SparseClassificationValidator
         elif self.ValidatorClass == SegmentationValidator:
             self.ValidatorClass = SparseSegmentationValidator
 
-    def _load(self, weights: str, task=None):
+    def _load(self, weights: str):
         if self.is_sparseml_checkpoint:
             """
             NOTE: the model is given to the trainer class with this snippet
             from YOLO base class:
             ```python
             self.trainer = self.TrainerClass(overrides=overrides)
             if not overrides.get("resume"):  # manually set model only if not resuming
@@ -616,15 +599,20 @@
             self.ckpt = torch.load(weights, map_location="cpu")
             config = dict(self.ckpt["train_args"])
             config.pop("save_dir", None)
             self.ckpt_path = weights
             self.task = config["task"]
             self.overrides = deepcopy(config)
             self._reset_ckpt_args(self.overrides)
-            self.ModelClass = TASK_MAP[self.task][0]
+            (
+                self.ModelClass,
+                self.TrainerClass,
+                self.ValidatorClass,
+                self.PredictorClass,
+            ) = self._assign_ops_from_task(self.task)
 
             if "yaml" in self.ckpt:
                 self.model = self.ModelClass(dict(self.ckpt["yaml"]))
             elif "model_yaml" in self.ckpt:
                 self.model = self.ModelClass(dict(self.ckpt["model_yaml"]))
             else:
                 self.model = self.ModelClass(dict(self.ckpt["model"].yaml))
@@ -646,20 +634,16 @@
 
             if self.ckpt["ema"]:
                 self.model.load_state_dict(self.ckpt["ema"])
             else:
                 self.model.load_state_dict(self.ckpt["model"])
             LOGGER.info("Loaded previous weights from checkpoint")
             assert self.model.yaml == self.ckpt["model_yaml"]
-
-            self.overrides["model"] = weights
-            self.overrides["task"] = self.task
-
         else:
-            super()._load(weights, task)
+            return super()._load(weights)
 
     def export(self, **kwargs):
         """
         Export model.
         Args:
             **kwargs : Any other args accepted by the exporter.
         """
@@ -723,31 +707,21 @@
             )
             recipe = (
                 ScheduledModifierManager.compose_staged(recipe, manager)
                 if recipe
                 else manager
             )
 
-        if args.get("name") and args["name"]:
-            name = args["name"]
-        else:
-            name = f"{type(self.model).__name__}.onnx"
-
+        name = args.get("name", f"{type(self.model).__name__}.onnx")
         save_dir = args["save_dir"]
-        if not os.path.exists(save_dir):
-            os.mkdir(save_dir)
 
         for _, m in self.model.named_modules():
             if isinstance(m, (Detect, Segment)):
                 m.export = True
 
-        # format attribute seems to not exist within this ultralytics update
-        # This is a workaround. Should be one of
-        # ('saved_model', 'pb', 'tflite', 'edgetpu', 'tfjs')
-        self.model.model[-1].format = "saved_model"
         exporter = ModuleExporter(self.model, save_dir)
         if save_one_shot_torch:
             if not one_shot:
                 warnings.warn(
                     "No one-shot recipe detected; "
                     "skipping one-shot model torch export..."
                 )
@@ -844,31 +818,28 @@
             raise AttributeError(
                 "dataset not provided! Please define `data` "
                 "in config.yaml or pass as an argument."
             )
         if overrides.get("resume"):
             overrides["resume"] = self.ckpt_path
 
-        overrides["nbs"] = int(overrides["nbs"])
         self.trainer = self.TrainerClass(overrides=overrides)
         if not overrides.get("resume"):  # manually set model only if not resuming
             self.trainer.model = self.trainer.get_model(
                 weights=self.model if self.ckpt else None, cfg=self.model.yaml
             )
             self.model = self.trainer.model
         self.trainer.train()
 
     @smart_inference_mode()
     def val(self, data=None, **kwargs):
         overrides = self.overrides.copy()
         overrides["rect"] = True  # rect batches as default
         overrides.update(kwargs)
         overrides["mode"] = "val"
-        if overrides.get("nbs"):
-            overrides["nbs"] = int(overrides["nbs"])
         overrides["data"] = data or overrides["data"]
         args = get_cfg(cfg=DEFAULT_CFG, overrides=overrides)
         args.data = data or args.data
         args.task = self.task
         if args.imgsz == DEFAULT_CFG.imgsz:
             # use trained imgsz unless custom value is passed
             args.imgsz = self.ckpt["train_args"]["imgsz"]
@@ -882,45 +853,38 @@
             trainer=self.TrainerClass(overrides=overrides),
             training=False,
         )
 
 
 def generate_ddp_command(world_size, trainer):
     # NOTE: copied from ultralytics.yolo.utils.dist.generate_ddp_command
-    """Generates and returns command for distributed training."""
     import __main__  # noqa local import to avoid https://github.com/Lightning-AI/lightning/issues/15218
 
-    if not trainer.resume:
-        shutil.rmtree(trainer.save_dir)  # remove the save_dir
-    file = str(Path(sys.argv[0]).resolve())
-    safe_pattern = re.compile(
-        r"^[a-zA-Z0-9_. /\\-]{1,128}$"
-    )  # allowed characters and maximum of 100 characters
-    if not (
-        safe_pattern.match(file) and Path(file).exists() and file.endswith(".py")
-    ):  # using CLI
-        file = generate_ddp_file(trainer)
-    dist_cmd = "torch.distributed.run" if TORCH_1_9 else "torch.distributed.launch"
-    port = find_free_network_port()
-    cmd = [
+    file_name = os.path.abspath(sys.argv[0])
+    using_cli = not file_name.endswith(".py")
+    if using_cli:
+        file_name = generate_ddp_file(trainer)
+    return [
         sys.executable,
         "-m",
-        dist_cmd,
+        "torch.distributed.run",
         "--nproc_per_node",
         f"{world_size}",
         "--master_port",
-        f"{port}",
-        file,
-    ]
-    return cmd, file
+        f"{find_free_network_port()}",
+        file_name,
+    ] + sys.argv[1:]
 
 
 def generate_ddp_file(trainer):
     # NOTE: adapted from ultralytics.yolo.utils.dist.generate_ddp_file
 
+    if not trainer.resume:
+        shutil.rmtree(trainer.save_dir)  # remove the save_dir
+
     content = f"""if __name__ == "__main__":
     from sparseml.yolov8.trainers import {trainer.__class__.__name__}
     trainer = {trainer.__class__.__name__}(config={dict(trainer.args)})
     trainer.train()
 """
     (USER_CONFIG_DIR / "DDP").mkdir(exist_ok=True)
     with tempfile.NamedTemporaryFile(
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## sparseml/yolov8/validators.py

```diff
@@ -19,15 +19,15 @@
 import torch
 from tqdm import tqdm
 
 from sparseml.pytorch.utils import detach
 from ultralytics.nn.autobackend import AutoBackend
 from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.yolo.engine.validator import BaseValidator
-from ultralytics.yolo.utils import LOGGER, TQDM_BAR_FORMAT, callbacks, emojis
+from ultralytics.yolo.utils import TQDM_BAR_FORMAT, callbacks, emojis
 from ultralytics.yolo.utils.checks import check_imgsz
 from ultralytics.yolo.utils.ops import Profile
 from ultralytics.yolo.utils.torch_utils import de_parallel, select_device
 from ultralytics.yolo.v8.classify.val import ClassificationValidator
 from ultralytics.yolo.v8.detect.val import DetectionValidator
 from ultralytics.yolo.v8.segment.val import SegmentationValidator
 
@@ -45,66 +45,64 @@
             else:
                 model = trainer.ema.ema or trainer.model
 
             # self.args.half = self.device.type != "cpu"
             model = model.half() if self.args.half else model.float()
             self.model = model
             self.loss = torch.zeros_like(trainer.loss_items, device=trainer.device)
-
             self.args.plots = (
-                trainer.stopper.possible_stop or trainer.epoch == trainer.epochs - 1
+                trainer.epoch == trainer.epochs - 1
             )  # always plot final epoch
-
             model.eval()
         else:
             callbacks.add_integration_callbacks(self)
             self.run_callbacks("on_val_start")
             assert model is not None, "Either trainer or model is needed for validation"
             self.device = select_device(self.args.device, self.args.batch)
             # self.args.half &= self.device.type != "cpu"
             model = AutoBackend(
                 model,
                 device=self.device,
                 dnn=self.args.dnn,
-                data=self.args.data,
                 fp16=self.args.half,
+                fuse=False,
             )
             self.model = model
             stride, pt, jit, engine = model.stride, model.pt, model.jit, model.engine
             imgsz = check_imgsz(self.args.imgsz, stride=stride)
             if engine:
                 self.args.batch = model.batch_size
             else:
                 self.device = model.device
                 if not pt and not jit:
                     self.args.batch = 1  # export.py models default to batch-size 1
-                    LOGGER.info(
+                    self.logger.info(
                         "Forcing --batch-size 1 square inference (1,3,"
                         f"{imgsz},{imgsz}) for non-PyTorch models"
                     )
 
             if isinstance(self.args.data, str) and self.args.data.endswith(".yaml"):
                 self.data = check_det_dataset(self.args.data)
             elif self.args.task == "classify":
-                self.data = check_cls_dataset(self.args.data, split=self.args.split)
+                self.data = check_cls_dataset(self.args.data)
             else:
                 raise FileNotFoundError(
                     emojis(f"Dataset '{self.args.data}' not found ❌")
                 )
             if isinstance(self.data["path"], str):
                 self.data["path"] = Path(self.data["path"])
 
             if self.device.type == "cpu":
                 self.args.workers = (
                     0  # faster CPU val as time dominated by inference, not dataloading
                 )
             if not pt:
                 self.args.rect = False
             self.dataloader = self.dataloader or self.get_dataloader(
-                self.data.get(self.args.split), self.args.batch
+                self.data.get("val") or self.data.set("test"), self.args.batch
             )
 
             model.eval()
             model.warmup(
                 imgsz=(1 if pt else self.args.batch, 3, imgsz, imgsz)
             )  # warmup
             trainer.model = model.model
@@ -127,25 +125,26 @@
             self.batch_i = batch_i
             # pre-process
             with dt[0]:
                 batch = self.preprocess(batch)
 
             # inference
             with dt[1]:
-                preds = model(batch["img"], augment=self.args.augment)
+                preds = model(batch["img"])
 
             # loss
             with dt[2]:
-                if self.training:
-                    self.loss += model.loss(batch=batch, preds=preds)[1]
+                if not hasattr(self, "loss"):
+                    self.loss = trainer.criterion(
+                        preds if self.training else preds[1], batch
+                    )[1]
                 else:
-                    if hasattr(self, "loss"):
-                        self.loss += model.model.loss(batch=batch, preds=preds[1])[1]
-                    else:
-                        self.loss = model.model.loss(batch=batch, preds=preds[1])[1]
+                    self.loss += trainer.criterion(
+                        preds if self.training else preds[1], batch
+                    )[1]
 
             # pre-process predictions
             with dt[3]:
                 preds = self.postprocess(preds)
 
             # During QAT the resulting preds are grad required, breaking
             # the update metrics function.
@@ -155,47 +154,44 @@
             if self.args.plots and batch_i < 3:
                 self.plot_val_samples(batch, batch_i)
                 self.plot_predictions(batch, detached_preds, batch_i)
 
             self.run_callbacks("on_val_batch_end")
         stats = self.get_stats()
         self.check_stats(stats)
-        self.speed = dict(
-            zip(
-                self.speed.keys(),
-                (x.t / len(self.dataloader.dataset) * 1e3 for x in dt),
-            )
-        )
-        self.finalize_metrics()
+        self.print_results()
+        self.speed = tuple(
+            x.t / len(self.dataloader.dataset) * 1e3 for x in dt
+        )  # speeds per image
         self.run_callbacks("on_val_end")
         model.float()
-        results = {
+        stats = {
             **stats,
             **trainer.label_loss_items(
                 self.loss.cpu() / len(self.dataloader), prefix="val"
             ),
         }
         if self.training:
             return {
-                k: round(float(v), 5) for k, v in results.items()
+                k: round(float(v), 5) for k, v in stats.items()
             }  # return results as 5 decimal place floats
         else:
-            LOGGER.info(
-                "Speed: %.1fms preprocess, %.1fms inference, %.1fms loss, %.1fms "
-                "postprocess per image" % tuple(self.speed.values())
+            self.logger.info(
+                (
+                    "Speed: %.1fms pre-process, %.1fms inference, %.1fms loss, %.1fms "
+                    "post-process per image"
+                ),
+                *self.speed,
             )
-            LOGGER.info(f"Validation loss: {results['val/Loss']}")
-            LOGGER.info(f"Metrics: {results}")
+            self.logger.info(f"Validation loss: {stats['val/Loss']}")
             if self.args.save_json and self.jdict:
                 with open(str(self.save_dir / "predictions.json"), "w") as f:
-                    LOGGER.info(f"Saving {f.name}...")
+                    self.logger.info(f"Saving {f.name}...")
                     json.dump(self.jdict, f)  # flatten and save
                 stats = self.eval_json(stats)  # update stats
-            if self.args.plots or self.args.save_json:
-                LOGGER.info(f"Results saved to {self.save_dir}")
             return stats
 
 
 class SparseDetectionValidator(SparseValidator, DetectionValidator):
     ...
```

## sparseml/yolov8/utils/export_samples.py

```diff
@@ -141,51 +141,37 @@
 def _export_torch_outputs(
     image: torch.Tensor, model: torch.nn.Module, sample_out_dir: str, file_idx: str
 ):
 
     # Run model to get torch outputs
     model_out = model(image)
     preds = model_out
-    sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
-    seg_prediction = None
 
     # Move to cpu for exporting
-    # Segmentation currently supports two outputs
-    if isinstance(preds, tuple):
-        preds_out = preds[0].detach().to("cpu")
-        seg_prediction = preds[1].detach().to("cpu")
-    else:
-        preds_out = preds.detach().to("cpu")
+    preds = preds.detach().to("cpu")
 
-    numpy.savez(sample_output_filename, preds_out, seg_prediction=seg_prediction)
+    sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
+    numpy.savez(sample_output_filename, preds)
 
 
 def _export_ort_outputs(
     image: numpy.ndarray,
     session: "onnxruntime.InferenceSession",  # noqa: F821
     sample_out_dir: str,
     file_idx: str,
 ):
 
     # Run model to get onnxruntime outputs
     ort_inputs = {session.get_inputs()[0].name: image}
     ort_outs = session.run(None, ort_inputs)
-    preds = ort_outs
-    seg_prediction = None
-
-    if len(preds) > 1:
-        preds_out = preds[0]
-        seg_prediction = preds[1]
-    else:
-        preds_out = preds[0]
-
-    preds_out = numpy.squeeze(preds_out, axis=0)
+    preds = numpy.squeeze(ort_outs, axis=0)
+    preds = numpy.squeeze(preds, axis=0)
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
-    numpy.savez(sample_output_filename, preds_out, seg_prediction=seg_prediction)
+    numpy.savez(sample_output_filename, preds)
 
 
 def _export_inputs(image: torch.Tensor, sample_in_dir: str, file_idx: str):
 
     sample_in = image.detach().to("cpu").squeeze(0)
 
     sample_input_filename = os.path.join(sample_in_dir, f"inp-{file_idx}.npz")
```

## Comparing `sparseml_nightly-1.6.0.20230720.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230723.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230720.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230723.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230720
+Version: 1.6.0.20230723
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -111,15 +111,15 @@
 Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=2.11) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
 Requires-Dist: einops ; extra == 'transformers'
 Requires-Dist: accelerate (>=0.20.3) ; extra == 'transformers'
 Provides-Extra: ultralytics
-Requires-Dist: ultralytics (==8.0.124) ; extra == 'ultralytics'
+Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
 Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'yolov5'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'yolov5'
 Requires-Dist: nm-yolov5-nightly (~=1.6.0) ; extra == 'yolov5'
```

## Comparing `sparseml_nightly-1.6.0.20230720.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230723.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230720.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230720.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230723.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=LkHNB1IsiFlZugUecB4-LZMjWuoboFYf_PXPx6uPl1g,26778
 sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
-sparseml/pytorch/sparsification/quantization/quantize.py,sha256=5vM57jjD2HuQjsYT7P1ayfpLJbXRthrI_Frlh1BELZQ,18014
+sparseml/pytorch/sparsification/quantization/quantize.py,sha256=bqqH2qBEWYHfea5jzAHmz52uPddfRdmP3TFaCKgQqjM,17905
 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=6JLbd3NUy9J0_pygSypJZsPtfxLlY8ZFJfK7kJSRrSY,76796
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
@@ -352,25 +352,25 @@
 sparseml/yolact/COCO_test.sh,sha256=ZoA_h_68zM8EWF510o24_5xBaQtbJLMHenNjSzldYYc,1418
 sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
 sparseml/yolov5/__init__.py,sha256=LiVvIlHR1FF63Ixm2MabdDH1Ul8sFEUEIb3Sbs4awLI,1440
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
-sparseml/yolov8/__init__.py,sha256=eeK3RbfsXhhjbAlqWgXwmxPFbnBxhOmbYBjKLwChpNE,1117
-sparseml/yolov8/default.yaml,sha256=Mi__Ox_lxhsftLyIJfNtDz7t_ncHYxjMXQd0hxHId78,6061
+sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
+sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
-sparseml/yolov8/train.py,sha256=eetdfCbRQJdBWc7XHb9GYPqMQxZzbKG7FG-4xQeTutk,7394
-sparseml/yolov8/trainers.py,sha256=1ldL_fFAh8Bm8c3k_eQHFa-v7bKy-9_xSWoNXmCtQVk,37320
+sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
+sparseml/yolov8/trainers.py,sha256=6jr1v056lTlZy8DmPstQosAAIq6-Wj39gdHUoQABzQk,35999
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
-sparseml/yolov8/validators.py,sha256=fkEnjRp1day-KY0n7DZ_VI-zmNqKbalh-g6U-lwHmfQ,8459
+sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
-sparseml/yolov8/utils/export_samples.py,sha256=qus5AKOZHxVaSJ2wtawcWZTuZnfHHxEf5KOPNs05AjU,6683
+sparseml/yolov8/utils/export_samples.py,sha256=Zy26etoYraN7k6IInS_i0j3RfoIzeeoK6JD-xFjkRk4,6247
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230720.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230720.dist-info/METADATA,sha256=395nCB_2pST3Wj7WW5psrXxfg4mKpQc3tTo08KEbfjw,21838
-sparseml_nightly-1.6.0.20230720.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230720.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230720.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
-sparseml_nightly-1.6.0.20230720.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230720.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230723.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230723.dist-info/METADATA,sha256=L4xP3fNPXhroNhydDPuhlEZ04jXsplVnHnfCFl9wB2E,21837
+sparseml_nightly-1.6.0.20230723.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230723.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
+sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230723.dist-info/RECORD,,
```

