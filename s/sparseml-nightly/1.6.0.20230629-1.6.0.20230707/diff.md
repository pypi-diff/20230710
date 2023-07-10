# Comparing `tmp/sparseml_nightly-1.6.0.20230629-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230707-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,377 +1,377 @@
-Zip file size: 965532 bytes, number of entries: 375
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-29 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-29 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-29 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-29 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-29 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-29 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17763 b- defN 23-Jun-29 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-29 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-29 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-29 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-29 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-29 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-29 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-29 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-29 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6325 b- defN 23-Jun-29 01:31 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-29 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    26599 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6192 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/configs.py
--rw-rw-r--  2.0 unx     1660 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
--rw-rw-r--  2.0 unx     3377 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-29 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-29 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-29 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-29 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-29 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-29 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-29 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-29 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-29 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-29 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-29 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-29 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-29 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-29 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-29 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-29 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-29 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-29 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-29 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-29 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-29 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-29 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-29 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-29 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-29 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-29 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-29 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-29 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-29 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-29 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-29 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-29 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-29 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-29 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-29 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-29 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    18825 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-29 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-29 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-29 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-29 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-29 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-29 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-29 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-29 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     2190 b- defN 23-Jun-29 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6155 b- defN 23-Jun-29 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-29 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10884 b- defN 23-Jun-29 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-29 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-29 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-29 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-29 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-29 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-29 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-29 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-29 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-29 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-29 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-29 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-29 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-29 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-29 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-29 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-29 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-29 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-29 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-29 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-29 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-29 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-29 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-29 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-29 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-29 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-29 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-29 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-29 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-29 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-29 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-29 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-29 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-29 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-29 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-29 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-29 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-29 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-29 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-29 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-29 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-29 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-29 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-29 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-29 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-29 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-29 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-29 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-29 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-29 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-29 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-29 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-29 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    35106 b- defN 23-Jun-29 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-29 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-29 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-29 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21775 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2326 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37382 b- defN 23-Jun-29 01:33 sparseml_nightly-1.6.0.20230629.dist-info/RECORD
-375 files, 3491114 bytes uncompressed, 904984 bytes compressed:  74.1%
+Zip file size: 966301 bytes, number of entries: 375
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-07 21:17 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jul-07 21:17 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-07 21:17 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-07 21:17 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-07 21:17 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jul-07 21:17 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-07 21:17 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-07 21:17 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jul-07 21:17 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-07 21:17 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-07 21:17 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-07 21:17 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-07 21:17 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-07 21:17 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-07 21:17 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-07 21:17 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jul-07 21:17 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2276 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4866 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      909 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    26599 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6192 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/configs.py
+-rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+-rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-07 21:17 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-07 21:17 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-07 21:17 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-07 21:17 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jul-07 21:17 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-07 21:17 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jul-07 21:17 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-07 21:17 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-07 21:17 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-07 21:17 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jul-07 21:17 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-07 21:17 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-07 21:17 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-07 21:17 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-07 21:17 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-07 21:17 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-07 21:17 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jul-07 21:17 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-07 21:17 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jul-07 21:17 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-07 21:17 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-07 21:17 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-07 21:17 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-07 21:17 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-07 21:17 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-07 21:17 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-07 21:17 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jul-07 21:17 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-07 21:17 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jul-07 21:17 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-07 21:17 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jul-07 21:17 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-07 21:17 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-07 21:17 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-07 21:17 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-07 21:17 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-07 21:17 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-07 21:17 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-07 21:17 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jul-07 21:17 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10884 b- defN 23-Jul-07 21:17 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jul-07 21:17 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-07 21:17 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jul-07 21:17 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-07 21:17 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-07 21:17 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-07 21:17 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-07 21:17 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-07 21:17 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-07 21:17 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-07 21:17 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-07 21:17 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-07 21:17 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-07 21:17 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-07 21:17 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-07 21:17 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jul-07 21:17 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-07 21:17 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-07 21:17 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jul-07 21:17 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jul-07 21:17 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-07 21:17 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-07 21:17 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-07 21:17 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-07 21:17 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-07 21:17 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-07 21:17 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-07 21:17 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-07 21:17 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-07 21:17 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-07 21:17 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-07 21:17 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-07 21:17 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-07 21:17 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jul-07 21:17 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jul-07 21:17 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-07 21:17 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-07 21:17 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jul-07 21:17 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    35999 b- defN 23-Jul-07 21:17 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-07 21:17 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jul-07 21:17 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6172 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21782 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37382 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/RECORD
+375 files, 3494563 bytes uncompressed, 905753 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1098,29 +1098,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230629.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230707.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/pytorch/datasets/registry.py

```diff
@@ -28,14 +28,21 @@
     """
     Registry class for creating datasets
     """
 
     _CONSTRUCTORS = {}
     _ATTRIBUTES = {}
 
+    @classmethod
+    def registered_datasets(cls) -> List[str]:
+        """
+        :return: valid dataset names registered to this registry
+        """
+        return list(cls._CONSTRUCTORS.keys())
+
     @staticmethod
     def create(key: str, *args, **kwargs) -> Dataset:
         """
         Create a new dataset for the given key
 
         :param key: the dataset key (name) to create
         :return: the instantiated model
```

## sparseml/pytorch/image_classification/utils/helpers.py

```diff
@@ -263,22 +263,45 @@
         torch_distributed_zero_first(local_rank)  # only download once locally
         if training
         else nullcontext()
     )
     dataset_kwargs = dataset_kwargs or {}
 
     with download_context:
-        dataset = DatasetRegistry.create(
-            dataset_name,
-            root=dataset_path,
-            train=training,
-            rand_trans=training,
-            image_size=image_size,
-            **dataset_kwargs,
-        )
+        try:
+            dataset = DatasetRegistry.create(
+                key=dataset_name,
+                root=dataset_path,
+                train=training,
+                rand_trans=training,
+                image_size=image_size,
+                **dataset_kwargs,
+            )
+        except Exception as registry_exception:
+            if dataset_name == "imagefolder" and (
+                dataset_path in DatasetRegistry.registered_datasets()
+            ):
+                # user attempting to run imagefolder of pre-supported
+                # dataset, without a local copy,
+                # use the dataset_path as registry key instead to attempt
+                # auto download
+                dataset = DatasetRegistry.create(
+                    key=dataset_path,
+                    train=training,
+                    rand_trans=training,
+                    image_size=image_size,
+                    **dataset_kwargs,
+                )
+                # still treated as image folder dataset, so num_classes attr
+                # should be set at the object level instead of registry
+                dataset.num_classes = DatasetRegistry.attributes(dataset_path).get(
+                    "num_classes"
+                )
+            else:
+                raise registry_exception
 
     sampler = (
         torch.utils.data.distributed.DistributedSampler(dataset)
         if rank != -1 and training  # only run on DDP + training
         else None
     )
     shuffle = sampler is None and not training
```

## sparseml/transformers/export.py

```diff
@@ -113,53 +113,60 @@
 class DeviceCPUTrainingArgs(HFTrainingArgs):
     @property
     def place_model_on_device(self):
         # Ensure model remains in CPU during ONNX export
         return False
 
 
-def load_task_model(task: str, model_path: str, config: Any) -> Module:
+def load_task_model(
+    task: str, model_path: str, config: Any, trust_remote_code: bool = False
+) -> Module:
     if task == "masked-language-modeling" or task == "mlm":
         return SparseAutoModel.masked_language_modeling_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
+            trust_remote_code=trust_remote_code,
         )
 
     if task == "question-answering" or task == "qa":
         return SparseAutoModel.question_answering_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
+            trust_remote_code=trust_remote_code,
         )
 
     if (
         task == "sequence-classification"
         or task == "glue"
         or task == "sentiment-analysis"
         or task == "text-classification"
     ):
         return SparseAutoModel.text_classification_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
+            trust_remote_code=trust_remote_code,
         )
 
     if task == "token-classification" or task == "ner":
         return SparseAutoModel.token_classification_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
+            trust_remote_code=trust_remote_code,
         )
 
     if task == "text-generation":
         return SparseAutoModel.text_generation_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
+            trust_remote_code=trust_remote_code,
         )
 
     raise ValueError(f"unrecognized task given of {task}")
 
 
 def load_task_dataset(
     task: str, tokenizer, data_args: Dict[str, Any], model: Module, config=None
@@ -232,14 +239,15 @@
     task: str,
     model_path: str,
     sequence_length: int = 384,
     convert_qat: bool = True,
     finetuning_task: Optional[str] = None,
     onnx_file_name: str = MODEL_ONNX_NAME,
     num_export_samples: int = 0,
+    trust_remote_code: bool = False,
     data_args: Optional[Union[Dict[str, Any], str]] = None,
     one_shot: Optional[str] = None,
 ) -> str:
     """
     Exports the saved transformers file to ONNX at batch size 1 using
     the given model path weights, config, and tokenizer
 
@@ -251,14 +259,15 @@
         ONNX model. Default is True
     :param finetuning_task: optional string finetuning task for text classification
         and token classification exports
     :param onnx_file_name: name to save the exported ONNX file as. Default
         is model.onnx. Note that when loading a model directory to a deepsparse
         pipeline, it will look only for 'model.onnx'
     :param num_export_samples: number of samples (inputs/outputs) to export
+    :param trust_remote_code: set True to allow custom models in HF-transformers
     :param data_args: additional args to instantiate a `DataTrainingArguments`
         instance for exporting samples
     :param one_shot: one shot recipe to be applied before exporting model
     :return: path to the exported ONNX file
     """
     task = task.replace("_", "-").replace(" ", "-")
 
@@ -276,23 +285,24 @@
         )
     data_args: Dict[str, Any] = _parse_data_args(data_args)
 
     _LOGGER.info(f"Attempting onnx export for model at {model_path} for task {task}")
     config_args = {"finetuning_task": finetuning_task} if finetuning_task else {}
     config = AutoConfig.from_pretrained(
         model_path,
+        trust_remote_code=trust_remote_code,
         **config_args,
     )
     tokenizer = AutoTokenizer.from_pretrained(
         model_path, model_max_length=sequence_length
     )
     if task == "text-generation":
         tokenizer.pad_token = tokenizer.eos_token
 
-    model = load_task_model(task, model_path, config)
+    model = load_task_model(task, model_path, config, trust_remote_code)
     _LOGGER.info(f"loaded model, config, and tokenizer from {model_path}")
 
     eval_dataset = None
     if num_export_samples > 0 and data_args:
         tokenized_dataset = load_task_dataset(
             task=task,
             tokenizer=tokenizer,
@@ -543,37 +553,44 @@
     parser.add_argument(
         "--one_shot",
         type=str,
         default=None,
         help="local path or SparseZoo stub to a recipe that should be applied "
         "in a one-shot manner before exporting",
     )
+    parser.add_argument(
+        "--trust_remote_code",
+        action="store_true",
+        help=("Set flag to allow custom models in HF-transformers"),
+    )
 
     return parser.parse_args()
 
 
 def export(
     task: str,
     model_path: str,
     sequence_length: int,
     no_convert_qat: bool,
     finetuning_task: str,
     onnx_file_name: str,
     num_export_samples: int = 0,
+    trust_remote_code: bool = False,
     data_args: Optional[str] = None,
     one_shot: Optional[str] = None,
 ):
     export_transformer_to_onnx(
         task=task,
         model_path=model_path,
         sequence_length=sequence_length,
         convert_qat=(not no_convert_qat),  # False if flagged
         finetuning_task=finetuning_task,
         onnx_file_name=onnx_file_name,
         num_export_samples=num_export_samples,
+        trust_remote_code=trust_remote_code,
         data_args=data_args,
         one_shot=one_shot,
     )
 
     deployment_folder_dir = create_deployment_folder(
         training_directory=model_path, onnx_file_name=onnx_file_name
     )
@@ -589,14 +606,15 @@
         task=args.task,
         model_path=args.model_path,
         sequence_length=args.sequence_length,
         no_convert_qat=args.no_convert_qat,  # False if flagged
         finetuning_task=args.finetuning_task,
         onnx_file_name=args.onnx_file_name,
         num_export_samples=args.num_export_samples,
+        trust_remote_code=args.trust_remote_code,
         data_args=args.data_args,
         one_shot=args.one_shot,
     )
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/transformers/sparsification/trainer.py

```diff
@@ -29,15 +29,15 @@
 import datasets
 import numpy
 import torch
 from torch import distributed as dist
 from torch.nn import Module
 from transformers import Trainer as HFTransformersTrainer
 from transformers import TrainerCallback, TrainerControl, TrainingArguments
-from transformers.file_utils import WEIGHTS_NAME, PaddingStrategy
+from transformers.file_utils import PaddingStrategy
 from transformers.integrations import TensorBoardCallback
 from transformers.trainer_callback import TrainerState
 from transformers.trainer_pt_utils import reissue_pt_warnings
 from transformers.trainer_utils import ShardedDDPOption, get_last_checkpoint
 
 from sparseml.pytorch.optim import ScheduledModifierManager, ScheduledOptimizer
 from sparseml.pytorch.utils import (
@@ -214,20 +214,21 @@
                 )
                 self.manager_applied = True
                 _LOGGER.info(f"Applied one shot recipe {self.recipe} to the manager")
                 return True
 
         # reload the state dict for the model now that architecture matches expected
         load_path = checkpoint or self.model_state_path
-        self._reload_model_state(load_path, orig_state_dict)
+        if self._reload_model_state(load_path, orig_state_dict):
+            _LOGGER.info(
+                "Reloaded model state after SparseML recipe structure modifications "
+                f"from {load_path}"
+            )
+
         self.manager_applied = True
-        _LOGGER.info(
-            "Reloaded model state after SparseML recipe structure modifications "
-            f"from {load_path}"
-        )
 
         return True
 
     def finalize_manager(self) -> bool:
         """
         Finalize the current recipes to wrap up any held state.
 
@@ -648,40 +649,49 @@
                 f"Overriding num_train_epochs from Recipe to {manager.max_epochs}"
             )
             kwargs["args"].num_train_epochs = manager.max_epochs
 
         return manager, arch_manager
 
     def _reload_model_state(self, load_path: str, orig_state_dict: Dict[str, Any]):
-        if (
-            not load_path
-            or not os.path.isdir(load_path)
-            or not os.path.isfile(os.path.join(load_path, WEIGHTS_NAME))
-        ):
+        """
+        Reload the weights after model arch changes due to recipe application
+        Return True if weights are successfully reloaded; False otherwise
+        """
+        invalid_load_path = not load_path or not os.path.isdir(load_path)
+        files = os.listdir(load_path) if not invalid_load_path else []
+        weight_files = [
+            os.path.join(load_path, f)
+            for f in files
+            if f.startswith("pytorch_model") and f.endswith("bin")
+        ]
+        if not weight_files:
             _LOGGER.warning(
                 "Model state was not reloaded for SparseML: "
-                f"could not find model weights for model_path {load_path}"
+                f"could not find model weights for {load_path}"
             )
-            return
+            return False
 
         current_state_dict = self.model.state_dict()
 
         if set(orig_state_dict.keys()) == set(current_state_dict):
             # no change in keys, ignore reload
-            return
+            return False
 
         # change in keys due to architecture changes, reload statedict
-        loaded_state_dict = torch.load(
-            os.path.join(load_path, WEIGHTS_NAME), map_location="cpu"
-        )
-        _, missing, unexpected, _, _ = self.model._load_pretrained_model(
+        loaded_state_dict = {}
+        for f in weight_files:
+            dd = torch.load(os.path.join(load_path, f), map_location="cpu")
+            loaded_state_dict.update(dd)
+
+        _, missing, unexpected, mismatched, _, _ = self.model._load_pretrained_model(
             model=self.model,
             state_dict=loaded_state_dict,
             loaded_keys=list(loaded_state_dict.keys()),
-            resolved_archive_file=[],
+            resolved_archive_file=None,
             pretrained_model_name_or_path=load_path,
             _fast_init=False,
         )
 
         if missing:
             _LOGGER.warning(
                 "Missing keys found when reloading model state for SparseML recipe:"
@@ -690,24 +700,31 @@
 
         if unexpected:
             _LOGGER.warning(
                 f"Unexpected keys found when reloading model state for SparseML recipe:"
                 f"{unexpected}"
             )
 
+        if mismatched:
+            _LOGGER.warning(
+                f"Mismatched keys found when reloading model state for SparseML recipe:"
+                f"{mismatched}"
+            )
+
         total_loaded = len(current_state_dict) - (len(missing) if len(missing) else 0)
         _LOGGER.info(
             f"Reloaded {total_loaded} model params for SparseML Recipe from {load_path}"
         )
         SparseAutoModel.log_model_load(
             self.model,
             self.model_state_path,
             model_type="student" if self.teacher else "model",
             delayed_load=False,
         )
+        return True
 
     def _data_loader_builder(self, kwargs: Optional[Dict[str, Any]] = None):
         default_loader = self.get_train_dataloader()
         template = dict(default_loader.__dict__)
 
         # drop attributes that will be auto-initialized
         to_drop = [k for k in template if k.startswith("_") or k == "batch_sampler"]
```

## sparseml/yolov8/trainers.py

```diff
@@ -43,14 +43,15 @@
     SparseClassificationValidator,
     SparseDetectionValidator,
     SparseSegmentationValidator,
 )
 from sparsezoo import Model
 from sparsezoo.utils import validate_onnx
 from ultralytics import __version__
+from ultralytics.nn.modules import Detect, Segment
 from ultralytics.nn.tasks import SegmentationModel, attempt_load_one_weight
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
 from ultralytics.yolo.engine.model import YOLO
 from ultralytics.yolo.engine.trainer import BaseTrainer
 from ultralytics.yolo.utils import LOGGER, IterableSimpleNamespace, yaml_load
 from ultralytics.yolo.utils.checks import check_file, check_imgsz, check_yaml
@@ -709,14 +710,18 @@
                 if recipe
                 else manager
             )
 
         name = args.get("name", f"{type(self.model).__name__}.onnx")
         save_dir = args["save_dir"]
 
+        for _, m in self.model.named_modules():
+            if isinstance(m, (Detect, Segment)):
+                m.export = True
+
         exporter = ModuleExporter(self.model, save_dir)
         if save_one_shot_torch:
             if not one_shot:
                 warnings.warn(
                     "No one-shot recipe detected; "
                     "skipping one-shot model torch export..."
                 )
@@ -745,20 +750,34 @@
         except Exception:
             pass
 
         validate_onnx(complete_path)
         deployment_folder = exporter.create_deployment_folder(onnx_model_name=name)
         if args["export_samples"]:
             trainer_config = get_cfg(cfg=DEFAULT_SPARSEML_CONFIG_PATH)
+            # First check if the yaml exists locally
+            if os.path.exists(args["data"]):
+                trainer_config.data = args["data"]
+            else:
+                # If it does not exist, may be a uralytics provided yaml. Try
+                # downloading and updating path to dataset_path
+                # Does this case actually happen? I.e. is args["data"] ever not a
+                # checkpointed local yaml path?
+                try:
+                    if args["dataset_path"] is not None:
+                        args["data"] = data_from_dataset_path(
+                            args["data"], args["dataset_path"]
+                        )
+                        trainer_config.data = args["data"]
+                except ValueError:
+                    LOGGER.info(
+                        f"yaml in {args['data']} could not be found. "
+                        "Using default config"
+                    )
 
-            if args["dataset_path"] is not None:
-                args["data"] = data_from_dataset_path(
-                    args["data"], args["dataset_path"]
-                )
-            trainer_config.data = args["data"]
             trainer_config.imgsz = args["imgsz"]
             trainer = DetectionTrainer(trainer_config)
             # inconsistency in name between
             # validation and test sets
             validation_set_path = trainer.testset
             device = trainer.device
             data_loader, _ = create_dataloader(
```

## sparseml/yolov8/utils/export_samples.py

```diff
@@ -140,16 +140,15 @@
 
 def _export_torch_outputs(
     image: torch.Tensor, model: torch.nn.Module, sample_out_dir: str, file_idx: str
 ):
 
     # Run model to get torch outputs
     model_out = model(image)
-    # preds, intermediate_outputs = model_out
-    preds, _ = model_out
+    preds = model_out
 
     # Move to cpu for exporting
     preds = preds.detach().to("cpu")
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
     numpy.savez(sample_output_filename, preds)
 
@@ -160,16 +159,15 @@
     sample_out_dir: str,
     file_idx: str,
 ):
 
     # Run model to get onnxruntime outputs
     ort_inputs = {session.get_inputs()[0].name: image}
     ort_outs = session.run(None, ort_inputs)
-    # preds, interm_out1, interm_out2, interm_out3 = model_out
-    preds, *_ = ort_outs
+    preds = ort_outs
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
     numpy.savez(sample_output_filename, preds)
 
 
 def _export_inputs(image: torch.Tensor, sample_in_dir: str, file_idx: str):
```

## Comparing `sparseml_nightly-1.6.0.20230629.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230707.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230629.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230707.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230629
+Version: 1.6.0.20230707
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -33,15 +33,15 @@
 Requires-Dist: numpy (>=1.0.0)
 Requires-Dist: matplotlib (>=3.0.0)
 Requires-Dist: merge-args (>=0.1.0)
 Requires-Dist: onnx (<1.15.0,>=1.5.0)
 Requires-Dist: pandas (>=0.25.0)
 Requires-Dist: packaging (>=20.0)
 Requires-Dist: psutil (>=5.0.0)
-Requires-Dist: pydantic (>=1.5.0)
+Requires-Dist: pydantic (<2.0.0,>=1.8.2)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: tqdm (>=4.0.0)
 Requires-Dist: toposort (>=1.0)
 Requires-Dist: GPUtil (>=1.4.0)
 Requires-Dist: protobuf (>=3.12.2)
```

## Comparing `sparseml_nightly-1.6.0.20230629.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230707.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230629.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230707.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
 sparseml/pytorch/__init__.py,sha256=n1a6y27bzfG73uLbifhIx5DY9hDg1RM1pTIN1DgBpDw,2190
 sparseml/pytorch/base.py,sha256=8HUpCMuP7gg6s4nvJVHU15AksGH5yhWLfeAMW6XvW18,6155
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
 sparseml/pytorch/torch_to_onnx_exporter.py,sha256=HHgmXDopADURZcO50F5pX2wNffQGykWkwy0aTYw2H0U,10884
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
-sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
+sparseml/pytorch/datasets/registry.py,sha256=Ju8hAl3qkaplvkjZgt6WvpKmujgv0qJ690Buo1ekipg,3014
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
 sparseml/pytorch/datasets/classification/imagefolder.py,sha256=rOvwqy2Zp89VkT7zat2hQxRmgPyvCpSAhZ4mWEsL9JI,3669
 sparseml/pytorch/datasets/classification/imagenet.py,sha256=CHzsckzsSsUCLR-oxaxJ8NH7j4WBqg_Wg5ge27bPk5Q,4000
 sparseml/pytorch/datasets/classification/imagenette.py,sha256=cac2poejwyNyVUsxw4odSTmmrEkJ0AoIkDqDapAINnQ,6491
 sparseml/pytorch/datasets/classification/mnist.py,sha256=hDmxt2oCugMIuhtUPn8m4f811t-BdZx9cxjPiarZuxo,2434
 sparseml/pytorch/datasets/detection/__init__.py,sha256=RgS6mZ9-uAgaJ9GAgt40QI-kKl-gpLJf96MTrMUnd74,767
@@ -152,15 +152,15 @@
 sparseml/pytorch/image_classification/export.py,sha256=FG3TIe06X5PYlubyGmDjNKWBZHsX24wQ19gbqXMT3BQ,18265
 sparseml/pytorch/image_classification/lr_analysis.py,sha256=qweXU51KeWjW86RJknvsavKPPXMd3PGAO7bcGosjTqE,15494
 sparseml/pytorch/image_classification/pr_sensitivity.py,sha256=RA64lC4NOmFm2H11MO4HSuiw2ImtiRwvixtIw7Rol0o,14444
 sparseml/pytorch/image_classification/train.py,sha256=-My1yUclgRA5wQoV4B_jtoOMRO1nQj389WfDkebu3fs,29287
 sparseml/pytorch/image_classification/utils/__init__.py,sha256=ambjlzpSCaSZ7ZadPk2vMAB6kaZCm7f_hVqOVSWz8k8,682
 sparseml/pytorch/image_classification/utils/cli_helpers.py,sha256=qypcmjezy-fZn2Cjozv9vumZoB44_9PDe_WXnChbvLg,4278
 sparseml/pytorch/image_classification/utils/constants.py,sha256=k01fijyL2BicSWLL1EzhhdvG07WYMMXHZeFz-9fxecM,1257
-sparseml/pytorch/image_classification/utils/helpers.py,sha256=_dfAcs5d1aftAB0cNnuA0lOqD_B3KxIv5m6prTQS3G8,20676
+sparseml/pytorch/image_classification/utils/helpers.py,sha256=uAPcnGNqx7qNaXf7x-dXLgMCv-j-_A9S72JZd8wW_d0,21742
 sparseml/pytorch/image_classification/utils/trainer.py,sha256=2WOP42hSlowDG2_DyCZOu8T5yohhV38e192ZxeWXj_A,12056
 sparseml/pytorch/models/__init__.py,sha256=Lj1KLciXTQiZObA5HHgrPMHNQ1bGYswrsP776eizaUc,976
 sparseml/pytorch/models/registry.py,sha256=cJLPsK8zzhVyZPvcJ8_Kj9-Ru9lTOywv61xuE50LiC8,14753
 sparseml/pytorch/models/classification/__init__.py,sha256=opnCtf6WMl1kuQ_vRAZRLl1eFZefpG9GFc9o729HndQ,901
 sparseml/pytorch/models/classification/darknet.py,sha256=rR4XXQu7shLADU4Th0D-eodnv-Z3AmA6kj8tDgHmtxU,11658
 sparseml/pytorch/models/classification/efficientnet.py,sha256=Bs88xu2xX9P65TOZ_6rn_qO2CMa6oLsJm5xt-Y6gISI,40293
 sparseml/pytorch/models/classification/inception_v3.py,sha256=wxWU3ja6E0_ERhYniDlzcsnVWi-rvJVfgxmhsyrpuC4,16512
@@ -316,22 +316,22 @@
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
 sparseml/transformers/__init__.py,sha256=8J1vljjZiybTTdNXN9e9senxvZUmKXKHAB5-H4D_4nY,1511
-sparseml/transformers/export.py,sha256=dcRG_1JeHCdym4zfyVUZQBDeG4aycBG7viEjQQojtZQ,21290
+sparseml/transformers/export.py,sha256=A0f4AhzegFco-rHJ0ySO51MrNpzQhsrtMR_IXs-i1_0,22048
 sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
 sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
 sparseml/transformers/text_classification.py,sha256=UYCpgSGTkmeGOeePQF5Idd8uY4GHQc-ShZK5SFOlP7E,40299
 sparseml/transformers/token_classification.py,sha256=6RUe1CmXQv7dHsE35aTg-xLW1g4BGakRp6pn0un2_mE,34350
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
-sparseml/transformers/sparsification/trainer.py,sha256=lylAxTy4WMmTqthB6ie4kUg1eIevSMIe11UcAO0WU9o,43772
+sparseml/transformers/sparsification/trainer.py,sha256=d_jRopQvHB0n-3uskpTHbqbnYFCiO7GocJ4iiujUW8s,44413
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
 sparseml/transformers/utils/model.py,sha256=JRq-p0CqKlWLdbhD9e8V2YkFtSZ6xLE9B512TTR8d2M,17072
 sparseml/utils/__init__.py,sha256=-WKBN4DERhw7rTJkarilkyAM9pw4rW8qkXGRPSEJ8SM,844
 sparseml/utils/frameworks.py,sha256=S-cGkbVc6DoWfI6Hu5AkIqF0Vi1PyxKX5GfhwRfpv_E,886
@@ -356,20 +356,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=GiYoNrWxiqZMVe3Q1ThZHiA9ZQ1wVKCDmf_j7Cb1d9Q,35106
+sparseml/yolov8/trainers.py,sha256=6jr1v056lTlZy8DmPstQosAAIq6-Wj39gdHUoQABzQk,35999
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
-sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
+sparseml/yolov8/utils/export_samples.py,sha256=CF4pF4FnQndQQgidfE_CNIRhR4hPoF_fZuPW6R2LLnk,6172
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230629.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230629.dist-info/METADATA,sha256=ZMd1kbvW9kEzyVqYVeqcDa-kRzTgjE9pagT-Y0cXWe4,21775
-sparseml_nightly-1.6.0.20230629.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230629.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230629.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
-sparseml_nightly-1.6.0.20230629.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230629.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230707.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230707.dist-info/METADATA,sha256=lTlIbYrG8hPbO5uEj5jN5BvuM_eQ0nRGU7smwv8xoe8,21782
+sparseml_nightly-1.6.0.20230707.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230707.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
+sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230707.dist-info/RECORD,,
```

