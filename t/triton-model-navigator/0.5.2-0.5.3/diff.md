# Comparing `tmp/triton_model_navigator-0.5.2-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,131 +1,131 @@
-Zip file size: 212950 bytes, number of entries: 129
--rw-r--r--  2.0 unx      881 b- defN 23-Apr-12 10:00 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Apr-12 10:00 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-Apr-12 10:00 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     9474 b- defN 23-Apr-12 10:00 model_navigator/execution_context.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Apr-12 10:00 model_navigator/logger.py
--rw-rw-rw-  2.0 unx     1520 b- defN 23-Apr-12 10:00 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    21958 b- defN 23-Apr-12 10:00 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6362 b- defN 23-Apr-12 10:00 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5372 b- defN 23-Apr-12 10:00 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    11854 b- defN 23-Apr-12 10:00 model_navigator/api/package.py
--rw-rw-rw-  2.0 unx     4861 b- defN 23-Apr-12 10:00 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7800 b- defN 23-Apr-12 10:00 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6462 b- defN 23-Apr-12 10:00 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6257 b- defN 23-Apr-12 10:00 model_navigator/api/torch.py
--rw-rw-rw-  2.0 unx     1553 b- defN 23-Apr-12 10:00 model_navigator/api/triton.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     4938 b- defN 23-Apr-12 10:00 model_navigator/commands/base.py
--rw-rw-rw-  2.0 unx    10071 b- defN 23-Apr-12 10:00 model_navigator/commands/infer_metadata.py
--rw-rw-rw-  2.0 unx     3289 b- defN 23-Apr-12 10:00 model_navigator/commands/load.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     7039 b- defN 23-Apr-12 12:21 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7838 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx    10151 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/torch.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/__init__.py
--rw-rw-rw-  2.0 unx     3418 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-rw-rw-  2.0 unx     3105 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/ts2onnx.py
--rw-rw-rw-  2.0 unx     4992 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-rw-rw-  2.0 unx      680 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/__init__.py
--rw-rw-rw-  2.0 unx     1728 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10453 b- defN 23-Apr-12 12:21 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-rw-rw-  2.0 unx     2236 b- defN 23-Apr-12 10:00 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/copy/__init__.py
--rw-rw-rw-  2.0 unx     1729 b- defN 23-Apr-12 10:00 model_navigator/commands/copy/onnx.py
--rw-rw-rw-  2.0 unx      678 b- defN 23-Apr-12 10:00 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5595 b- defN 23-Apr-12 10:00 model_navigator/commands/correctness/correctness.py
--rw-rw-rw-  2.0 unx     4631 b- defN 23-Apr-12 12:21 model_navigator/commands/correctness/correctness_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/data_dump/__init__.py
--rw-rw-rw-  2.0 unx    11168 b- defN 23-Apr-12 10:00 model_navigator/commands/data_dump/samples.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/export/__init__.py
--rw-rw-rw-  2.0 unx     3527 b- defN 23-Apr-12 10:00 model_navigator/commands/export/jax.py
--rw-rw-rw-  2.0 unx     5486 b- defN 23-Apr-12 10:00 model_navigator/commands/export/tf.py
--rw-rw-rw-  2.0 unx     8895 b- defN 23-Apr-12 10:00 model_navigator/commands/export/torch.py
--rw-rw-rw-  2.0 unx     1061 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/__init__.py
--rw-rw-rw-  2.0 unx     3945 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-rw-rw-  2.0 unx     3172 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-rw-rw-  2.0 unx     3123 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-rw-rw-  2.0 unx     3077 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/torch2onnx.py
--rw-rw-rw-  2.0 unx     2603 b- defN 23-Apr-12 10:00 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-rw-rw-  2.0 unx      715 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/__init__.py
--rw-rw-rw-  2.0 unx     6397 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-rw-rw-  2.0 unx     2985 b- defN 23-Apr-12 10:00 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-rw-rw-  2.0 unx      688 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/__init__.py
--rw-rw-rw-  2.0 unx    15771 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/performance.py
--rw-rw-rw-  2.0 unx     3038 b- defN 23-Apr-12 10:00 model_navigator/commands/performance/performance_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/commands/verification/__init__.py
--rw-rw-rw-  2.0 unx     5447 b- defN 23-Apr-12 10:00 model_navigator/commands/verification/verify.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2478 b- defN 23-Apr-12 10:00 model_navigator/configuration/common_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    14775 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/model_config.py
--rw-rw-rw-  2.0 unx    13482 b- defN 23-Apr-12 10:00 model_navigator/configuration/model/model_config_builder.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1213 b- defN 23-Apr-12 10:00 model_navigator/core/constants.py
--rw-rw-rw-  2.0 unx    20118 b- defN 23-Apr-12 10:00 model_navigator/core/package.py
--rw-rw-rw-  2.0 unx    20332 b- defN 23-Apr-12 10:00 model_navigator/core/status.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/pipelines/__init__.py
--rw-rw-rw-  2.0 unx     5451 b- defN 23-Apr-12 10:00 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx     7334 b- defN 23-Apr-12 10:00 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9810 b- defN 23-Apr-12 10:00 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1884 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/__init__.py
--rw-rw-rw-  2.0 unx     2036 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     4749 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-rw-rw-  2.0 unx     1647 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2395 b- defN 23-Apr-12 12:21 model_navigator/pipelines/builders/onnx.py
--rw-rw-rw-  2.0 unx     2365 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/preprocessing.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2869 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3261 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/torch.py
--rw-rw-rw-  2.0 unx     2042 b- defN 23-Apr-12 10:00 model_navigator/pipelines/builders/verify.py
--rw-rw-rw-  2.0 unx     1513 b- defN 23-Apr-12 12:21 model_navigator/runners/__init__.py
--rw-rw-rw-  2.0 unx    10683 b- defN 23-Apr-12 12:21 model_navigator/runners/base.py
--rw-rw-rw-  2.0 unx     2620 b- defN 23-Apr-12 10:00 model_navigator/runners/jax.py
--rw-rw-rw-  2.0 unx     4513 b- defN 23-Apr-12 12:21 model_navigator/runners/onnx.py
--rw-rw-rw-  2.0 unx     2267 b- defN 23-Apr-12 10:00 model_navigator/runners/python.py
--rw-rw-rw-  2.0 unx     2285 b- defN 23-Apr-12 10:00 model_navigator/runners/registry.py
--rw-rw-rw-  2.0 unx     7980 b- defN 23-Apr-12 10:00 model_navigator/runners/tensorflow.py
--rw-rw-rw-  2.0 unx     2468 b- defN 23-Apr-12 12:21 model_navigator/runners/tensorrt.py
--rw-rw-rw-  2.0 unx     7631 b- defN 23-Apr-12 10:00 model_navigator/runners/torch.py
--rw-rw-rw-  2.0 unx     1153 b- defN 23-Apr-12 10:00 model_navigator/runners/utils.py
--rw-rw-rw-  2.0 unx      937 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/__init__.py
--rw-rw-rw-  2.0 unx    11706 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/analyzer.py
--rw-rw-rw-  2.0 unx     2304 b- defN 23-Apr-12 10:00 model_navigator/runtime_analyzer/strategy.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/triton/__init__.py
--rw-rw-rw-  2.0 unx     3182 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config.py
--rw-rw-rw-  2.0 unx     5218 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config_builder.py
--rw-rw-rw-  2.0 unx    23090 b- defN 23-Apr-12 10:00 model_navigator/triton/model_config_generator.py
--rw-rw-rw-  2.0 unx    15198 b- defN 23-Apr-12 10:00 model_navigator/triton/model_repository.py
--rw-rw-rw-  2.0 unx     2082 b- defN 23-Apr-12 10:00 model_navigator/triton/utils.py
--rw-rw-rw-  2.0 unx      944 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/__init__.py
--rw-rw-rw-  2.0 unx     2874 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/base_model_config.py
--rw-rw-rw-  2.0 unx    22326 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/common.py
--rw-rw-rw-  2.0 unx     2231 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/internal.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-rw-rw-  2.0 unx     1785 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/python_model_config.py
--rw-rw-rw-  2.0 unx     2239 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-rw-rw-  2.0 unx     3162 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-rw-rw-  2.0 unx     3040 b- defN 23-Apr-12 10:00 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Apr-12 10:00 model_navigator/utils/__init__.py
--rw-rw-rw-  2.0 unx     7436 b- defN 23-Apr-12 12:21 model_navigator/utils/common.py
--rw-rw-rw-  2.0 unx     8001 b- defN 23-Apr-12 10:00 model_navigator/utils/dataloader.py
--rw-rw-rw-  2.0 unx     3902 b- defN 23-Apr-12 10:00 model_navigator/utils/devices.py
--rw-rw-rw-  2.0 unx     1308 b- defN 23-Apr-12 10:00 model_navigator/utils/enums.py
--rw-rw-rw-  2.0 unx     6163 b- defN 23-Apr-12 10:00 model_navigator/utils/environment.py
--rw-rw-rw-  2.0 unx     3533 b- defN 23-Apr-12 10:00 model_navigator/utils/format_helpers.py
--rw-rw-rw-  2.0 unx     2497 b- defN 23-Apr-12 12:21 model_navigator/utils/framework.py
--rw-rw-rw-  2.0 unx     1554 b- defN 23-Apr-12 10:00 model_navigator/utils/jax.py
--rw-rw-rw-  2.0 unx     2325 b- defN 23-Apr-12 10:00 model_navigator/utils/module.py
--rw-rw-rw-  2.0 unx     1085 b- defN 23-Apr-12 10:00 model_navigator/utils/onnx.py
--rw-rw-rw-  2.0 unx     3239 b- defN 23-Apr-12 10:00 model_navigator/utils/package.py
--rw-rw-rw-  2.0 unx     1331 b- defN 23-Apr-12 10:00 model_navigator/utils/pipelines.py
--rw-rw-rw-  2.0 unx     3171 b- defN 23-Apr-12 10:00 model_navigator/utils/runners.py
--rw-rw-rw-  2.0 unx     8054 b- defN 23-Apr-12 10:00 model_navigator/utils/tensor.py
--rw-rw-rw-  2.0 unx     2848 b- defN 23-Apr-12 12:21 model_navigator/utils/tensorrt.py
--rw-rw-rw-  2.0 unx     1508 b- defN 23-Apr-12 10:00 model_navigator/utils/torch.py
--rw-rw-rw-  2.0 unx    10140 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13041 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    12813 b- defN 23-Apr-12 12:24 triton_model_navigator-0.5.2.dist-info/RECORD
-129 files, 627383 bytes uncompressed, 192082 bytes compressed:  69.4%
+Zip file size: 212993 bytes, number of entries: 129
+-rw-r--r--  2.0 unx      881 b- defN 23-Apr-18 16:22 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Apr-19 12:21 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3668 b- defN 23-Apr-18 16:22 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     9474 b- defN 23-Apr-18 16:22 model_navigator/execution_context.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Apr-18 16:22 model_navigator/logger.py
+-rw-r--r--  2.0 unx     1520 b- defN 23-Apr-18 16:22 model_navigator/api/__init__.py
+-rw-r--r--  2.0 unx    21958 b- defN 23-Apr-18 16:22 model_navigator/api/config.py
+-rw-r--r--  2.0 unx     6360 b- defN 23-Apr-18 16:22 model_navigator/api/jax.py
+-rw-r--r--  2.0 unx     5372 b- defN 23-Apr-18 16:22 model_navigator/api/onnx.py
+-rw-r--r--  2.0 unx    11854 b- defN 23-Apr-18 16:22 model_navigator/api/package.py
+-rw-r--r--  2.0 unx     4861 b- defN 23-Apr-18 16:22 model_navigator/api/python.py
+-rw-r--r--  2.0 unx     7800 b- defN 23-Apr-18 16:22 model_navigator/api/pytriton.py
+-rw-r--r--  2.0 unx     6460 b- defN 23-Apr-18 16:22 model_navigator/api/tensorflow.py
+-rw-r--r--  2.0 unx     6257 b- defN 23-Apr-18 16:22 model_navigator/api/torch.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-Apr-18 16:22 model_navigator/api/triton.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/__init__.py
+-rw-r--r--  2.0 unx     4938 b- defN 23-Apr-18 16:22 model_navigator/commands/base.py
+-rw-r--r--  2.0 unx    10071 b- defN 23-Apr-18 16:22 model_navigator/commands/infer_metadata.py
+-rw-r--r--  2.0 unx     3289 b- defN 23-Apr-18 16:22 model_navigator/commands/load.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/__init__.py
+-rw-r--r--  2.0 unx     7039 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/base.py
+-rw-r--r--  2.0 unx     7838 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/tf.py
+-rw-r--r--  2.0 unx    10151 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/torch.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/converters/__init__.py
+-rw-r--r--  2.0 unx     3418 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-r--r--  2.0 unx     4992 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-r--r--  2.0 unx      680 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/onnx/__init__.py
+-rw-r--r--  2.0 unx     1728 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10453 b- defN 23-Apr-19 12:21 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-r--r--  2.0 unx     2236 b- defN 23-Apr-18 16:22 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/copy/__init__.py
+-rw-r--r--  2.0 unx     1729 b- defN 23-Apr-18 16:22 model_navigator/commands/copy/onnx.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Apr-18 16:22 model_navigator/commands/correctness/__init__.py
+-rw-r--r--  2.0 unx     5595 b- defN 23-Apr-18 16:22 model_navigator/commands/correctness/correctness.py
+-rw-rw-rw-  2.0 unx     4631 b- defN 23-Apr-19 12:21 model_navigator/commands/correctness/correctness_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/data_dump/__init__.py
+-rw-r--r--  2.0 unx    11168 b- defN 23-Apr-18 16:22 model_navigator/commands/data_dump/samples.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/export/__init__.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-Apr-18 16:22 model_navigator/commands/export/jax.py
+-rw-r--r--  2.0 unx     5486 b- defN 23-Apr-18 16:22 model_navigator/commands/export/tf.py
+-rw-r--r--  2.0 unx     8895 b- defN 23-Apr-18 16:22 model_navigator/commands/export/torch.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/__init__.py
+-rw-r--r--  2.0 unx     3945 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-r--r--  2.0 unx     3172 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-r--r--  2.0 unx     3123 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-r--r--  2.0 unx     2603 b- defN 23-Apr-18 16:22 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Apr-18 16:22 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-r--r--  2.0 unx     6397 b- defN 23-Apr-18 16:22 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-r--r--  2.0 unx     2985 b- defN 23-Apr-18 16:22 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-r--r--  2.0 unx      688 b- defN 23-Apr-18 16:22 model_navigator/commands/performance/__init__.py
+-rw-r--r--  2.0 unx    15771 b- defN 23-Apr-18 16:22 model_navigator/commands/performance/performance.py
+-rw-r--r--  2.0 unx     3038 b- defN 23-Apr-18 16:22 model_navigator/commands/performance/performance_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/commands/verification/__init__.py
+-rw-r--r--  2.0 unx     5447 b- defN 23-Apr-18 16:22 model_navigator/commands/verification/verify.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/configuration/__init__.py
+-rw-r--r--  2.0 unx     2478 b- defN 23-Apr-18 16:22 model_navigator/configuration/common_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/configuration/model/__init__.py
+-rw-r--r--  2.0 unx    14775 b- defN 23-Apr-18 16:22 model_navigator/configuration/model/model_config.py
+-rw-r--r--  2.0 unx    13482 b- defN 23-Apr-18 16:22 model_navigator/configuration/model/model_config_builder.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/core/__init__.py
+-rw-r--r--  2.0 unx     1213 b- defN 23-Apr-18 16:22 model_navigator/core/constants.py
+-rw-r--r--  2.0 unx    20116 b- defN 23-Apr-18 16:22 model_navigator/core/package.py
+-rw-r--r--  2.0 unx    20332 b- defN 23-Apr-18 16:22 model_navigator/core/status.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5451 b- defN 23-Apr-18 16:22 model_navigator/pipelines/pipeline.py
+-rw-r--r--  2.0 unx     7334 b- defN 23-Apr-18 16:22 model_navigator/pipelines/pipeline_manager.py
+-rw-r--r--  2.0 unx     9810 b- defN 23-Apr-18 16:22 model_navigator/pipelines/validation.py
+-rw-r--r--  2.0 unx     1884 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/__init__.py
+-rw-r--r--  2.0 unx     2036 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/correctness.py
+-rw-r--r--  2.0 unx     4749 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-r--r--  2.0 unx     1647 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2395 b- defN 23-Apr-19 12:21 model_navigator/pipelines/builders/onnx.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/preprocessing.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/profiling.py
+-rw-r--r--  2.0 unx     2869 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/tensorflow.py
+-rw-r--r--  2.0 unx     3261 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/torch.py
+-rw-r--r--  2.0 unx     2042 b- defN 23-Apr-18 16:22 model_navigator/pipelines/builders/verify.py
+-rw-rw-rw-  2.0 unx     1513 b- defN 23-Apr-19 12:21 model_navigator/runners/__init__.py
+-rw-rw-rw-  2.0 unx    10683 b- defN 23-Apr-19 12:21 model_navigator/runners/base.py
+-rw-r--r--  2.0 unx     2620 b- defN 23-Apr-18 16:22 model_navigator/runners/jax.py
+-rw-rw-rw-  2.0 unx     4597 b- defN 23-Apr-19 12:21 model_navigator/runners/onnx.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-Apr-18 16:22 model_navigator/runners/python.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Apr-18 16:22 model_navigator/runners/registry.py
+-rw-r--r--  2.0 unx     7976 b- defN 23-Apr-18 16:22 model_navigator/runners/tensorflow.py
+-rw-rw-rw-  2.0 unx     2552 b- defN 23-Apr-19 12:21 model_navigator/runners/tensorrt.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-Apr-18 16:22 model_navigator/runners/torch.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Apr-18 16:22 model_navigator/runners/utils.py
+-rw-r--r--  2.0 unx      937 b- defN 23-Apr-18 16:22 model_navigator/runtime_analyzer/__init__.py
+-rw-r--r--  2.0 unx    11706 b- defN 23-Apr-18 16:22 model_navigator/runtime_analyzer/analyzer.py
+-rw-r--r--  2.0 unx     2304 b- defN 23-Apr-18 16:22 model_navigator/runtime_analyzer/strategy.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/triton/__init__.py
+-rw-r--r--  2.0 unx     3180 b- defN 23-Apr-18 16:22 model_navigator/triton/model_config.py
+-rw-r--r--  2.0 unx     5218 b- defN 23-Apr-18 16:22 model_navigator/triton/model_config_builder.py
+-rw-r--r--  2.0 unx    23090 b- defN 23-Apr-18 16:22 model_navigator/triton/model_config_generator.py
+-rw-r--r--  2.0 unx    15198 b- defN 23-Apr-18 16:22 model_navigator/triton/model_repository.py
+-rw-r--r--  2.0 unx     2082 b- defN 23-Apr-18 16:22 model_navigator/triton/utils.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/__init__.py
+-rw-r--r--  2.0 unx     2872 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-r--r--  2.0 unx    22326 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/common.py
+-rw-r--r--  2.0 unx     2229 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/internal.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-r--r--  2.0 unx     3162 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Apr-18 16:22 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 16:22 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx     7436 b- defN 23-Apr-19 12:21 model_navigator/utils/common.py
+-rw-r--r--  2.0 unx     8001 b- defN 23-Apr-18 16:22 model_navigator/utils/dataloader.py
+-rw-r--r--  2.0 unx     3902 b- defN 23-Apr-18 16:22 model_navigator/utils/devices.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Apr-18 16:22 model_navigator/utils/enums.py
+-rw-r--r--  2.0 unx     6163 b- defN 23-Apr-18 16:22 model_navigator/utils/environment.py
+-rw-r--r--  2.0 unx     3533 b- defN 23-Apr-18 16:22 model_navigator/utils/format_helpers.py
+-rw-rw-rw-  2.0 unx     2497 b- defN 23-Apr-19 12:21 model_navigator/utils/framework.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Apr-18 16:22 model_navigator/utils/jax.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Apr-18 16:22 model_navigator/utils/module.py
+-rw-r--r--  2.0 unx     1085 b- defN 23-Apr-18 16:22 model_navigator/utils/onnx.py
+-rw-r--r--  2.0 unx     3239 b- defN 23-Apr-18 16:22 model_navigator/utils/package.py
+-rw-r--r--  2.0 unx     1331 b- defN 23-Apr-18 16:22 model_navigator/utils/pipelines.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Apr-18 16:22 model_navigator/utils/runners.py
+-rw-r--r--  2.0 unx     8052 b- defN 23-Apr-18 16:22 model_navigator/utils/tensor.py
+-rw-rw-rw-  2.0 unx     2848 b- defN 23-Apr-19 12:21 model_navigator/utils/tensorrt.py
+-rw-r--r--  2.0 unx     1508 b- defN 23-Apr-18 16:22 model_navigator/utils/torch.py
+-rw-r--r--  2.0 unx    10140 b- defN 23-Apr-19 12:24 triton_model_navigator-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13041 b- defN 23-Apr-19 12:24 triton_model_navigator-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 12:24 triton_model_navigator-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-19 12:24 triton_model_navigator-0.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12813 b- defN 23-Apr-19 12:24 triton_model_navigator-0.5.3.dist-info/RECORD
+129 files, 627533 bytes uncompressed, 192125 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -366,23 +366,23 @@
 
 Filename: model_navigator/utils/tensorrt.py
 Comment: 
 
 Filename: model_navigator/utils/torch.py
 Comment: 
 
-Filename: triton_model_navigator-0.5.2.dist-info/LICENSE
+Filename: triton_model_navigator-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.5.2.dist-info/METADATA
+Filename: triton_model_navigator-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.5.2.dist-info/WHEEL
+Filename: triton_model_navigator-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.5.2.dist-info/top_level.txt
+Filename: triton_model_navigator-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.5.2.dist-info/RECORD
+Filename: triton_model_navigator-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # noqa: D100
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

## model_navigator/api/jax.py

```diff
@@ -84,15 +84,15 @@
         verify_func: Function for additional model verifcation
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if target_device == DeviceKind.CPU and any(
-        [device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()]
+        device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()
     ):
         raise ModelNavigatorConfigurationError(
             "\n"
             "    'target_device == nav.DeviceKind.CPU' is not supported for TensorFlow2 "
             "(exported from JAX) when GPU is available.\n"
             "    To optimize model for CPU, disable GPU with: "
             "'tf.config.set_visible_devices([], 'GPU')' directly after importing TensorFlow.\n"
```

## model_navigator/api/tensorflow.py

```diff
@@ -85,15 +85,15 @@
         verify_func: Function for additional model verifcation
         custom_configs: Sequence of CustomConfigs used to control produced artifacts
 
     Returns:
         Package descriptor representing created package.
     """
     if target_device == DeviceKind.CPU and any(
-        [device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()]
+        device.device_type == "GPU" for device in tensorflow.config.get_visible_devices()
     ):
         raise ModelNavigatorConfigurationError(
             "\n"
             "    'target_device == nav.DeviceKind.CPU' is not supported for TensorFlow2 when GPU is available.\n"
             "    To optimize model for CPU, disable GPU with: "
             "'tf.config.set_visible_devices([], 'GPU')' directly after importing TensorFlow.\n"
         )
```

## model_navigator/core/package.py

```diff
@@ -166,15 +166,15 @@
 
         Returns:
             Package.
         """
 
         def _filter_out_generated_files(paths: List[str]):
             generated_files_extensions = [".log", ".sh", ".py"]
-            return [p for p in paths if not any([p.endswith(suffix) for suffix in generated_files_extensions])]
+            return [p for p in paths if not any(p.endswith(suffix) for suffix in generated_files_extensions)]
 
         def _extract_pkg_version(status_dict):
             return version.parse(status_dict.get("model_navigator_version", "0.3.0"))
 
         path = Path(path)
         if workspace is None:
             workspace = get_default_workspace()
```

## model_navigator/runners/onnx.py

```diff
@@ -63,15 +63,16 @@
             active_providers = self._runner.sess.get_providers()
             if self._provider not in active_providers:
                 raise RuntimeError(f"Unable to initialize defined provider: {self._provider}.")
 
     def infer_impl(self, feed_dict):
         input_metadata = self.get_onnx_input_metadata()
         feed_dict = {name: tensor for name, tensor in feed_dict.items() if name in input_metadata}
-        return self._runner.infer_impl(feed_dict)
+        out_dict = self._runner.infer_impl(feed_dict)
+        return {k: v for k, v in out_dict.items() if k in self.output_metadata}
 
     def deactivate_impl(self):
         self._runner.deactivate_impl()
 
 
 class OnnxrtCPURunner(_BaseOnnxrtRunner):
     """ONNX runner for CPU runtime provider."""
```

## model_navigator/runners/tensorflow.py

```diff
@@ -93,15 +93,15 @@
 
 
 class TensorFlowSavedModelCPURunner(_BaseTFRunner):
     """Runs inference for TensorFlow SavedModels."""
 
     def activate_impl(self):
         """Runner activation implementation."""
-        if any([device.device_type == "GPU" for device in tf.config.get_visible_devices()]):
+        if any(device.device_type == "GPU" for device in tf.config.get_visible_devices()):
             tf.config.set_visible_devices([], "GPU")
         self._loaded_model = tf.keras.models.load_model(str(self._model))
 
     def deactivate_impl(self):
         """Runner deactivation implementation."""
 
     def _infer_impl(self, feed_dict: Dict):
@@ -187,15 +187,15 @@
 
 
 class TensorFlowCPURunner(_BaseTFRunner):
     """Runs inference for TensorFlow models in source."""
 
     def activate_impl(self):
         """Runner activation implementation."""
-        if any([device.device_type == "GPU" for device in tf.config.get_visible_devices()]):
+        if any(device.device_type == "GPU" for device in tf.config.get_visible_devices()):
             tf.config.set_visible_devices([], "GPU")
         self._loaded_model = self.model
 
     def deactivate_impl(self):
         """Runner deactivation implementation."""
         super().deactivate_impl()
         # TODO: this does not allow other processes to use the memory, but allows TF to use it
```

## model_navigator/runners/tensorrt.py

```diff
@@ -55,15 +55,16 @@
         """Activate implementation."""
         self._runner.activate_impl()
 
     def infer_impl(self, feed_dict):
         """Inference implementation."""
         input_metadata = self._runner.get_input_metadata()
         feed_dict = {name: tensorrt.cast_tensor(tensor) for name, tensor in feed_dict.items() if name in input_metadata}
-        return self._runner.infer_impl(feed_dict)
+        out_dict = self._runner.infer_impl(feed_dict)
+        return {k: v for k, v in out_dict.items() if k in self.output_metadata}
 
     def deactivate_impl(self):
         """Deactivate implementation."""
         self._runner.deactivate_impl()
 
 
 def register_tensorrt_runners():
```

## model_navigator/triton/model_config.py

```diff
@@ -57,15 +57,15 @@
         """Validate the configuration for early error handling."""
         if not self.backend and not self.platform:
             raise ModelNavigatorWrongParameterError("Backend or platform has to be defined. None was provided.")
 
         if self.batching and self.max_batch_size <= 0:
             raise ModelNavigatorWrongParameterError("The `max_batch_size` must be greater or equal to 1.")
 
-        if self.backend != Backend.TensorRT and any([group.profile for group in self.instance_groups]):
+        if self.backend != Backend.TensorRT and any(group.profile for group in self.instance_groups):
             raise ModelNavigatorWrongParameterError(
                 "Invalid `profile` option. The value can be set only for `backend=Backend.TensorRT`"
             )
 
         if type(self.batcher) not in [DynamicBatcher, SequenceBatcher]:
             raise ModelNavigatorWrongParameterError("Unsupported batcher type provided.")
```

## model_navigator/triton/specialized_configs/base_model_config.py

```diff
@@ -49,15 +49,15 @@
         """Validate the configuration for early error handling."""
         if self.batching and self.max_batch_size <= 0:
             raise ModelNavigatorWrongParameterError("The `max_batch_size` must be greater or equal to 1.")
 
         if type(self.batcher) not in [DynamicBatcher, SequenceBatcher]:
             raise ModelNavigatorWrongParameterError("Unsupported batcher type provided.")
 
-        if self.backend != Backend.TensorRT and any([group.profile for group in self.instance_groups]):
+        if self.backend != Backend.TensorRT and any(group.profile for group in self.instance_groups):
             raise ModelNavigatorWrongParameterError(
                 "Invalid `profile` option. The value can be set only for `backend=Backend.TensorRT`"
             )
 
     @property
     @abc.abstractmethod
     def backend(self) -> Backend:
```

## model_navigator/triton/specialized_configs/internal.py

```diff
@@ -43,15 +43,15 @@
 
 
 def is_shape_correct(name: str, value: Optional[Tuple], optional: bool = False):
     """Validate if of parameter is correct."""
     if not value and not optional:
         raise ModelNavigatorWrongParameterError(f"Empty {name} is not supported.")
 
-    if not all([is_dim_correct(dim) for dim in value]):
+    if not all(is_dim_correct(dim) for dim in value):
         raise ModelNavigatorWrongParameterError(
             f"{name} items should be integers equal to -1 or positive numbers. Got {value}."
         )
 
 
 def cast_dtype(dtype: Union[np.dtype, Type[np.dtype]]):
     """Cast provided argument to np.dtype."""
```

## model_navigator/utils/tensor.py

```diff
@@ -57,15 +57,15 @@
             # int equal to -1 or positive number
             return isinstance(dim, int) and (dim == -1 or dim > 0)
 
         _expect_type("name", self.name, str)
         _expect_type("shape", self.shape, tuple)
         _expect_type("dtype", self.dtype, np.dtype, optional=True)
         _expect_type("optional", self.optional, bool, optional=True)
-        if not all([_is_dim_correct(dim) for dim in self.shape]):
+        if not all(_is_dim_correct(dim) for dim in self.shape):
             raise TypeError(f"Shape items should be integers equal to -1 or positive numbers. Got {self.shape}")
 
     def astype(self, dtype: Union[np.dtype, Type[np.dtype]]) -> "TensorSpec":
         """Change the TensorSpec dtype."""
         tensor = TensorSpec(name=self.name, shape=self.shape, dtype=np.dtype(dtype), optional=self.optional)
         return tensor
```

## Comparing `triton_model_navigator-0.5.2.dist-info/LICENSE` & `triton_model_navigator-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.5.2.dist-info/METADATA` & `triton_model_navigator-0.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.5.2
+Version: 0.5.3
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.5.2.dist-info/RECORD` & `triton_model_navigator-0.5.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=wdjyiPqcy9thC_Z8iQnQrvUMqi5_PP5GlvWcZrQyGY4,649
+model_navigator/__version__.py,sha256=dCv8qM6xmW58YODRaplH6qxkkxCmzt831dksVt1EWPE,649
 model_navigator/exceptions.py,sha256=6wR9REQeNkmHOklMPQ46SrGC61EJVH4jz0n2BC4e7ek,3668
 model_navigator/execution_context.py,sha256=eYV2YJU4V8X-v-dWTI6Oi5zJl3RdtK41XWtPxPRxNvU,9474
 model_navigator/logger.py,sha256=-qSYoA16yl2NdJOyqazlUUY73jTyWqaMCB6xt0KuNpc,3793
 model_navigator/api/__init__.py,sha256=gnYVwaepcIMj_380kVpdKxdEU0HpyWHDedNoBbZJpAA,1520
 model_navigator/api/config.py,sha256=u2VRwZh1v3s6y_rnEWGi1FLPc1oTv7cXy-axs4ch0Jo,21958
-model_navigator/api/jax.py,sha256=6sZHQuG1wQXl5R0xWn1cCInLhbde4M5CfTWWEP2iBeg,6362
+model_navigator/api/jax.py,sha256=ReQjD0e8kTwkQNJZnqd732DFa5OxK5GU0hzFFK3oLE0,6360
 model_navigator/api/onnx.py,sha256=acon_yfZNeQUw20uZOfdIek3KH0rLiXVxReoxwUFAiM,5372
 model_navigator/api/package.py,sha256=_ksTa01pgUidpozNSA4AGXmkqIyrrIzhZiLm2YmrXGw,11854
 model_navigator/api/python.py,sha256=ocDQMGTQ5lEDIb36n2jponEBof6etYPpv6xfB5dq_zM,4861
 model_navigator/api/pytriton.py,sha256=OvkztWzqDo53PshxbFEGyuu1CBOTd1jUBlgfUalWcSE,7800
-model_navigator/api/tensorflow.py,sha256=FH6Ve2zfsmY7XvRsb-BU5JxOca5O2v1HaGXjIBtycPs,6462
+model_navigator/api/tensorflow.py,sha256=0FIN2-QvgtT90JeyhNmVk9FuOZ8NzQPwiiNaVa06K5k,6460
 model_navigator/api/torch.py,sha256=nQo2Oa_elF5Ia65fhbohiPYOQTqFSr2VX0-RDb1m9Gs,6257
 model_navigator/api/triton.py,sha256=hdrU_WJn5DFzhJ5slcdJqzRcC7n69vhmP0RKa1B3QYQ,1553
 model_navigator/commands/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/commands/base.py,sha256=O75ENxJH4GtjYHru56h5XSLrR_iqnsbaQE7YHbtOnLk,4938
 model_navigator/commands/infer_metadata.py,sha256=KqWupE_d4wPv6o90uIuT1y3Pze0yxR9S1oesqfk1yjE,10071
 model_navigator/commands/load.py,sha256=7v1YqLbG0VZOf981XW-2Y6ad828d4Ynq2HNmj7_a8ys,3289
 model_navigator/commands/convert/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
@@ -57,15 +57,15 @@
 model_navigator/configuration/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/configuration/common_config.py,sha256=6DWPjzYWN5K6T3WMYZbSiySZIINJpXK-2hQ2Hh4kmPA,2478
 model_navigator/configuration/model/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/configuration/model/model_config.py,sha256=_CS3i4OGmHmWyGAywrgV6T6y0I_9Cd-2NhWT_7U8CN8,14775
 model_navigator/configuration/model/model_config_builder.py,sha256=HBMlQYpoVHHHdPZpVpnnuf4IqdFywrehDQCR37EDTtw,13482
 model_navigator/core/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/core/constants.py,sha256=ZexQn5QcgGiw1mLBTxgVcgDURGqxCqqBgPIhV7qPrKI,1213
-model_navigator/core/package.py,sha256=dKbkYc0DlIGgVueuz4wZztCuu5cQc3nMcUsYedihia4,20118
+model_navigator/core/package.py,sha256=aHXS6kmmYZ_wPqEPEuu6VbzNoNCIwylDvxcyVeq-VGk,20116
 model_navigator/core/status.py,sha256=yX5FeszIQikqL_K5KJnOONWioTutZf5crI7VYR5ePig,20332
 model_navigator/pipelines/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/pipelines/pipeline.py,sha256=vdf2Hp1TRa_biNFo-Af9fVjKBTs9ddOE-lfHKQSdixo,5451
 model_navigator/pipelines/pipeline_manager.py,sha256=YQL2Om9ncR_cpxZJL2hkdwSkEH28311zhLwHbNIoDu0,7334
 model_navigator/pipelines/validation.py,sha256=VI5aXRdamesaGpk0W7QVTzlO3Fvg15s6WROyv4tI6xE,9810
 model_navigator/pipelines/builders/__init__.py,sha256=ACocrstiz-vJgSJDzZAfGS_PlJeUZlgj2gNXebnTd4c,1884
 model_navigator/pipelines/builders/correctness.py,sha256=LIm_qCMu33l1tbKw2FcJ_8rAlumg7hHZxsXwuRylJCM,2036
@@ -76,34 +76,34 @@
 model_navigator/pipelines/builders/profiling.py,sha256=sa3q3AvdQOVLJiCxEG50RYuS12LZcLJx2iGEU9XloNk,2685
 model_navigator/pipelines/builders/tensorflow.py,sha256=vFt59zR0XiRr2BF2sbSpnRgaSG6VyywexiAx_0qnrb8,2869
 model_navigator/pipelines/builders/torch.py,sha256=Cd-dNkKqhwSDzu898s0hzqE1jyipTRaLx0efRFTaZWk,3261
 model_navigator/pipelines/builders/verify.py,sha256=GIK2mGl1h45TSdqXYOzFyCkBovTaYSsEzcJ9DssrGTU,2042
 model_navigator/runners/__init__.py,sha256=psra620ntIJRnqn4t6X2K9OnrCh8_vaoLumt6yZCx4U,1513
 model_navigator/runners/base.py,sha256=txmgzDNilaagi5DxehYQo3EuyG6sHWqft9jSLJC4YXE,10683
 model_navigator/runners/jax.py,sha256=4zDe8dhv08-alz2aKJUmbkr_XgqAzkWOgjPPMtRKDjo,2620
-model_navigator/runners/onnx.py,sha256=rEJnMUZPt6jN_6xteh0zEJTmkgjfWFJ1ma8uGllsWDE,4513
+model_navigator/runners/onnx.py,sha256=gtp2nZwq1lAo2crV0sdYviH6jlJkCaoKEvY24h0NxPE,4597
 model_navigator/runners/python.py,sha256=8B9ttZbMZ5Iau0TttHQJvb59HoyzHg6u-2XIcqBB7Qg,2267
 model_navigator/runners/registry.py,sha256=FmCtd7gAP5thuPzKnRZpgU_jmPhPBO_O3GenbmyCCJE,2285
-model_navigator/runners/tensorflow.py,sha256=7QbbHnIJZoy_VbRvy5FOPVA0NJm9ltaFEfMRjf-O0WU,7980
-model_navigator/runners/tensorrt.py,sha256=YB_ltgBOsoOFe3EFTH3PtbW0EypxKJQRy-3MVWyZ4cE,2468
+model_navigator/runners/tensorflow.py,sha256=ghITBvu0A6w7tMvlyYCNM9JSCXalY_6jXDLssG_xWYw,7976
+model_navigator/runners/tensorrt.py,sha256=qatbsfX_ehTJzA9SJewOk7nN9jgqCGlSao_vlGIjwAs,2552
 model_navigator/runners/torch.py,sha256=9GvyaZaeCTK2j5qkmoenM0ZSDdNbsL9fo61ch4XtMGI,7631
 model_navigator/runners/utils.py,sha256=FNNg4sPIE4DKFBspTwp3RU3Moe1rqcFQwKQZS8vzqkg,1153
 model_navigator/runtime_analyzer/__init__.py,sha256=BrhKs-NzpT0ilLmYe38kUtOS7AJ-KfzyV-Hc7ANJWEE,937
 model_navigator/runtime_analyzer/analyzer.py,sha256=Y5vBtEEKPv7Ce1Mg3GV6sxe61zDj_fz7RZD8Ge6NM8s,11706
 model_navigator/runtime_analyzer/strategy.py,sha256=L6dqnf1OS0s5mrBvxTTFgNPghKbuEFC2X_2tMm3_Hs4,2304
 model_navigator/triton/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/triton/model_config.py,sha256=XeYfhPjYc9U6owzz9SWGFZx6_lAjltrCbGmJshcJfT8,3182
+model_navigator/triton/model_config.py,sha256=Efcx0_48bmkmBwJgqm6Ejsuwh0ZPnYmyR1o6bz4Y5to,3180
 model_navigator/triton/model_config_builder.py,sha256=4uh5xArtOMnyzIKO2Duliz9SRltrP5El2xPqzE1At_0,5218
 model_navigator/triton/model_config_generator.py,sha256=i45y9ezQJ9xcQmNcGHW_5r0TZ7-Ikxvmzb9pgfBlZaY,23090
 model_navigator/triton/model_repository.py,sha256=Eh_yTQc4GG7bZyJIbmwsWaFgY4iSPNqz20yOb3Wm0r4,15198
 model_navigator/triton/utils.py,sha256=hlzxBk1qoDfLNe84-f3wzvTLMey7rjLel482l1haAQY,2082
 model_navigator/triton/specialized_configs/__init__.py,sha256=lcQy-49A74vMSidK-avYy6xdX4p3OG3ygzSw6y9-OQw,944
-model_navigator/triton/specialized_configs/base_model_config.py,sha256=DSz9Og5B4Hku8BurijB71STyuauS_zbz5ZoWLNXvfPc,2874
+model_navigator/triton/specialized_configs/base_model_config.py,sha256=UOeuce-xT9lC3Zv3H3BbdSem7cTNyn7boKybxChzRgs,2872
 model_navigator/triton/specialized_configs/common.py,sha256=l6FPhZTU1WQHDVXG8HxEXx2c8s87EWgYUvtQrxqUH1k,22326
-model_navigator/triton/specialized_configs/internal.py,sha256=UM7klO7-IMn_g0bghENX-bEyliSEt0GpfnJ-NXYAlTI,2231
+model_navigator/triton/specialized_configs/internal.py,sha256=R42XlgUEOC5B-WotI_dAQs8sQyHJOnVyTvVk3CaZ6kM,2229
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=oN76Ux7JI4eqlarlEVSSiIbbajAqdrF3bW0n6WQBPPw,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=NGijgogtoJnbBLL1hQqhw-n4rBo_OgFsCdn9ezw24VI,1785
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=GxJnFB4UpnUwB75t09d5XZ2iqeMZM1SmTbGe2aqmph8,2239
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=C_qMi-5TAWTSL_wBDIoJju3gHRHX10RBbHvBE9of780,3162
 model_navigator/triton/specialized_configs/tensorrt_model_config.py,sha256=ikNi_i_cPjL2Mhea1uJHXe3KElvpHkiPH_zXK895pQU,3040
 model_navigator/utils/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/utils/common.py,sha256=ZQfPl4e8B42qKFXSF4sW_yGXCBUCyBwBZP803jBepWQ,7436
@@ -115,15 +115,15 @@
 model_navigator/utils/framework.py,sha256=0QwlBigjgxVBgjFgDuU5J1vvgZrFNSOCjL_K0WCIx-c,2497
 model_navigator/utils/jax.py,sha256=WROviV0IDfQKkfneaX88wZm7f3WhrB4DwB3-bl4_Qio,1554
 model_navigator/utils/module.py,sha256=fkokQmxhWgShqrhsXDPa-g-jBA0XaUQvuVuM74WPOIM,2325
 model_navigator/utils/onnx.py,sha256=L3IDVu0r-_BHSdf4htXwsmMVPoInk9Qset6SA66LusI,1085
 model_navigator/utils/package.py,sha256=exDhwNvvNXGQlZXSjRuVOzX6z4N9eI28Nb2VxbqfxnU,3239
 model_navigator/utils/pipelines.py,sha256=70riAoXSEezI3KDv_6el-SiuWyB6pW44EgN_rwYswwY,1331
 model_navigator/utils/runners.py,sha256=euFHUjrB3_sSvHI0ClEAx1pDa5RbvQAlPrRY1LwG4bc,3171
-model_navigator/utils/tensor.py,sha256=C2T3JIj-XYLjAwPD1kR4lOrGeNVhcFQSYdfxM7U1kPE,8054
+model_navigator/utils/tensor.py,sha256=21C_4LlFnakdc2Ix1QVRcvL917QoFcsi5f-xgN94O3k,8052
 model_navigator/utils/tensorrt.py,sha256=qx5Ed47xLZC2CYSQk6kUUf3-nBvsV92GJA8t5_jUWbQ,2848
 model_navigator/utils/torch.py,sha256=czQ3umUl1UtYydDApapftpEOBZsWCAdVyPD5wF9Gjq8,1508
-triton_model_navigator-0.5.2.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.5.2.dist-info/METADATA,sha256=hMMAyRabXVGgp9zPr0g4mQ5CNeRSPmVy_UebAPuKUck,13041
-triton_model_navigator-0.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.5.2.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.5.2.dist-info/RECORD,,
+triton_model_navigator-0.5.3.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.5.3.dist-info/METADATA,sha256=A_0NeVUhdmhe0nmtXZl-U-CO3qVvyqF0hEQyWDiHU-s,13041
+triton_model_navigator-0.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.5.3.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.5.3.dist-info/RECORD,,
```

