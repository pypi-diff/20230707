# Comparing `tmp/triton_model_navigator-0.6.0-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,147 +1,147 @@
-Zip file size: 254299 bytes, number of entries: 145
--rw-r--r--  2.0 unx      881 b- defN 23-Jun-28 12:15 model_navigator/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 23-Jun-28 12:15 model_navigator/__version__.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jun-28 12:15 model_navigator/exceptions.py
--rw-rw-rw-  2.0 unx     1716 b- defN 23-Jun-28 12:15 model_navigator/api/__init__.py
--rw-rw-rw-  2.0 unx    24220 b- defN 23-Jun-30 11:34 model_navigator/api/config.py
--rw-rw-rw-  2.0 unx     6263 b- defN 23-Jun-30 11:34 model_navigator/api/jax.py
--rw-rw-rw-  2.0 unx     5268 b- defN 23-Jun-30 11:34 model_navigator/api/onnx.py
--rw-rw-rw-  2.0 unx    16279 b- defN 23-Jun-30 11:34 model_navigator/api/package.py
--rw-rw-rw-  2.0 unx     4795 b- defN 23-Jun-28 12:15 model_navigator/api/python.py
--rw-rw-rw-  2.0 unx     7751 b- defN 23-Jun-28 12:15 model_navigator/api/pytriton.py
--rw-rw-rw-  2.0 unx     6350 b- defN 23-Jun-30 11:34 model_navigator/api/tensorflow.py
--rw-rw-rw-  2.0 unx     6158 b- defN 23-Jun-30 11:34 model_navigator/api/torch.py
--rw-rw-rw-  2.0 unx     1553 b- defN 23-Jun-28 12:15 model_navigator/api/triton.py
--rw-rw-rw-  2.0 unx     1811 b- defN 23-Jun-28 12:15 model_navigator/api/utilities.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/__init__.py
--rw-rw-rw-  2.0 unx     5542 b- defN 23-Jun-28 12:15 model_navigator/commands/base.py
--rw-rw-rw-  2.0 unx     9486 b- defN 23-Jun-28 12:15 model_navigator/commands/execution_context.py
--rw-rw-rw-  2.0 unx    12793 b- defN 23-Jun-28 12:15 model_navigator/commands/infer_metadata.py
--rw-rw-rw-  2.0 unx     3325 b- defN 23-Jun-28 12:15 model_navigator/commands/load.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/__init__.py
--rw-rw-rw-  2.0 unx     9868 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/base.py
--rw-rw-rw-  2.0 unx     7633 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/tf.py
--rw-rw-rw-  2.0 unx    10029 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/torch.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/__init__.py
--rw-rw-rw-  2.0 unx     3418 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-rw-rw-  2.0 unx     3105 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/ts2onnx.py
--rw-rw-rw-  2.0 unx     4992 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-rw-rw-  2.0 unx      680 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/__init__.py
--rw-rw-rw-  2.0 unx     1727 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-rw-rw-  2.0 unx    10733 b- defN 23-Jun-30 11:34 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-rw-rw-  2.0 unx     2235 b- defN 23-Jun-28 12:15 model_navigator/commands/convert/onnx/trt_load_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/copy/__init__.py
--rw-rw-rw-  2.0 unx     1798 b- defN 23-Jun-28 12:15 model_navigator/commands/copy/onnx.py
--rw-rw-rw-  2.0 unx      678 b- defN 23-Jun-28 12:15 model_navigator/commands/correctness/__init__.py
--rw-rw-rw-  2.0 unx     5674 b- defN 23-Jun-28 12:15 model_navigator/commands/correctness/correctness.py
--rw-rw-rw-  2.0 unx     4733 b- defN 23-Jun-28 15:05 model_navigator/commands/correctness/correctness_script.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/data_dump/__init__.py
--rw-rw-rw-  2.0 unx    10740 b- defN 23-Jun-28 12:15 model_navigator/commands/data_dump/samples.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/export/__init__.py
--rw-rw-rw-  2.0 unx     3611 b- defN 23-Jun-28 12:15 model_navigator/commands/export/jax.py
--rw-rw-rw-  2.0 unx     5598 b- defN 23-Jun-28 12:15 model_navigator/commands/export/tf.py
--rw-rw-rw-  2.0 unx     9156 b- defN 23-Jun-28 12:15 model_navigator/commands/export/torch.py
--rw-rw-rw-  2.0 unx     1056 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/__init__.py
--rw-rw-rw-  2.0 unx     3945 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-rw-rw-  2.0 unx     3171 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-rw-rw-  2.0 unx     3122 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-rw-rw-  2.0 unx     3077 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/torch2onnx.py
--rw-rw-rw-  2.0 unx     2728 b- defN 23-Jun-28 12:15 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-rw-rw-  2.0 unx      715 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/__init__.py
--rw-rw-rw-  2.0 unx     7156 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-rw-rw-  2.0 unx     3075 b- defN 23-Jun-28 12:15 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-rw-rw-  2.0 unx      784 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/__init__.py
--rw-rw-rw-  2.0 unx     5260 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/performance.py
--rw-rw-rw-  2.0 unx     6964 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/profile.py
--rw-rw-rw-  2.0 unx     3104 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/profile_script.py
--rw-rw-rw-  2.0 unx     7269 b- defN 23-Jun-28 15:05 model_navigator/commands/performance/profiler.py
--rw-rw-rw-  2.0 unx     5476 b- defN 23-Jun-28 12:15 model_navigator/commands/performance/results.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/commands/verification/__init__.py
--rw-rw-rw-  2.0 unx     4657 b- defN 23-Jun-28 12:15 model_navigator/commands/verification/verify.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/configuration/__init__.py
--rw-rw-rw-  2.0 unx     2002 b- defN 23-Jun-28 12:15 model_navigator/configuration/common_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/configuration/model/__init__.py
--rw-rw-rw-  2.0 unx    15653 b- defN 23-Jun-30 11:34 model_navigator/configuration/model/model_config.py
--rw-rw-rw-  2.0 unx    13677 b- defN 23-Jun-30 11:34 model_navigator/configuration/model/model_config_builder.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/core/__init__.py
--rw-rw-rw-  2.0 unx     1389 b- defN 23-Jun-30 11:34 model_navigator/core/constants.py
--rw-rw-rw-  2.0 unx     5299 b- defN 23-Jun-28 12:15 model_navigator/core/logger.py
--rw-rw-rw-  2.0 unx     9941 b- defN 23-Jun-28 12:15 model_navigator/core/tensor.py
--rw-rw-rw-  2.0 unx     2147 b- defN 23-Jun-28 12:15 model_navigator/core/workspace.py
--rw-rw-rw-  2.0 unx     2817 b- defN 23-Jun-28 12:15 model_navigator/frameworks/__init__.py
--rw-rw-rw-  2.0 unx      669 b- defN 23-Jun-28 12:15 model_navigator/frameworks/jax/__init__.py
--rw-rw-rw-  2.0 unx     1554 b- defN 23-Jun-28 12:15 model_navigator/frameworks/jax/model.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/onnx/__init__.py
--rw-rw-rw-  2.0 unx     1085 b- defN 23-Jun-28 12:15 model_navigator/frameworks/onnx/utils.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/tensorrt/__init__.py
--rw-rw-rw-  2.0 unx    27191 b- defN 23-Jun-28 12:15 model_navigator/frameworks/tensorrt/cuda.py
--rw-rw-rw-  2.0 unx    10627 b- defN 23-Jun-30 11:34 model_navigator/frameworks/tensorrt/utils.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/frameworks/torch/__init__.py
--rw-rw-rw-  2.0 unx     1513 b- defN 23-Jun-28 12:15 model_navigator/frameworks/torch/utils.py
--rw-rw-rw-  2.0 unx      622 b- defN 23-Jun-28 12:15 model_navigator/package/__init__.py
--rw-rw-rw-  2.0 unx    12176 b- defN 23-Jun-28 13:04 model_navigator/package/builder.py
--rw-rw-rw-  2.0 unx     4651 b- defN 23-Jun-28 12:15 model_navigator/package/loader.py
--rw-rw-rw-  2.0 unx    11755 b- defN 23-Jun-28 15:05 model_navigator/package/package.py
--rw-rw-rw-  2.0 unx     2819 b- defN 23-Jun-28 12:15 model_navigator/package/profiling_results.py
--rw-rw-rw-  2.0 unx    21135 b- defN 23-Jun-30 11:34 model_navigator/package/status.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/pipelines/__init__.py
--rw-rw-rw-  2.0 unx     5232 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline.py
--rw-rw-rw-  2.0 unx    14762 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline_context.py
--rw-rw-rw-  2.0 unx     3832 b- defN 23-Jun-28 12:15 model_navigator/pipelines/pipeline_manager.py
--rw-rw-rw-  2.0 unx     9693 b- defN 23-Jun-30 11:34 model_navigator/pipelines/validation.py
--rw-rw-rw-  2.0 unx     1883 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/__init__.py
--rw-rw-rw-  2.0 unx     2106 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/correctness.py
--rw-rw-rw-  2.0 unx     5682 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-rw-rw-  2.0 unx     1660 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/jax.py
--rw-rw-rw-  2.0 unx     2509 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/onnx.py
--rw-rw-rw-  2.0 unx     2516 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/performance.py
--rw-rw-rw-  2.0 unx     2239 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/preprocessing.py
--rw-rw-rw-  2.0 unx     2504 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/profiling.py
--rw-rw-rw-  2.0 unx     2921 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/tensorflow.py
--rw-rw-rw-  2.0 unx     3326 b- defN 23-Jun-30 11:34 model_navigator/pipelines/builders/torch.py
--rw-rw-rw-  2.0 unx     2112 b- defN 23-Jun-28 12:15 model_navigator/pipelines/builders/verify.py
--rw-rw-rw-  2.0 unx      622 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/__init__.py
--rw-rw-rw-  2.0 unx     2747 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/optimize.py
--rw-rw-rw-  2.0 unx     4881 b- defN 23-Jun-28 12:15 model_navigator/pipelines/wrappers/profile.py
--rw-rw-rw-  2.0 unx     1584 b- defN 23-Jun-28 12:15 model_navigator/runners/__init__.py
--rw-rw-rw-  2.0 unx    13796 b- defN 23-Jun-28 12:15 model_navigator/runners/base.py
--rw-rw-rw-  2.0 unx     2620 b- defN 23-Jun-28 12:15 model_navigator/runners/jax.py
--rw-rw-rw-  2.0 unx     9999 b- defN 23-Jun-28 12:15 model_navigator/runners/onnx.py
--rw-rw-rw-  2.0 unx     2267 b- defN 23-Jun-28 12:15 model_navigator/runners/python.py
--rw-rw-rw-  2.0 unx     2290 b- defN 23-Jun-28 12:15 model_navigator/runners/registry.py
--rw-rw-rw-  2.0 unx     7976 b- defN 23-Jun-28 12:15 model_navigator/runners/tensorflow.py
--rw-rw-rw-  2.0 unx    26748 b- defN 23-Jun-28 14:25 model_navigator/runners/tensorrt.py
--rw-rw-rw-  2.0 unx    10041 b- defN 23-Jun-29 08:01 model_navigator/runners/torch.py
--rw-rw-rw-  2.0 unx     3559 b- defN 23-Jun-28 12:15 model_navigator/runners/utils.py
--rw-rw-rw-  2.0 unx      937 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/__init__.py
--rw-rw-rw-  2.0 unx    11714 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/analyzer.py
--rw-rw-rw-  2.0 unx     2304 b- defN 23-Jun-28 12:15 model_navigator/runtime_analyzer/strategy.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/triton/__init__.py
--rw-rw-rw-  2.0 unx     3180 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config.py
--rw-rw-rw-  2.0 unx     5218 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config_builder.py
--rw-rw-rw-  2.0 unx    23090 b- defN 23-Jun-28 12:15 model_navigator/triton/model_config_generator.py
--rw-rw-rw-  2.0 unx    15243 b- defN 23-Jun-30 11:34 model_navigator/triton/model_repository.py
--rw-rw-rw-  2.0 unx     2081 b- defN 23-Jun-28 12:15 model_navigator/triton/utils.py
--rw-rw-rw-  2.0 unx      944 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/__init__.py
--rw-rw-rw-  2.0 unx     2872 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/base_model_config.py
--rw-rw-rw-  2.0 unx    22326 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/common.py
--rw-rw-rw-  2.0 unx     2229 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/internal.py
--rw-rw-rw-  2.0 unx     2685 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-rw-rw-  2.0 unx     1785 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/python_model_config.py
--rw-rw-rw-  2.0 unx     2239 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-rw-rw-  2.0 unx     3162 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-rw-rw-  2.0 unx     3040 b- defN 23-Jun-28 12:15 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-rw-rw-  2.0 unx      627 b- defN 23-Jun-28 12:15 model_navigator/utils/__init__.py
--rw-rw-rw-  2.0 unx    14528 b- defN 23-Jun-30 12:44 model_navigator/utils/common.py
--rw-rw-rw-  2.0 unx     8132 b- defN 23-Jun-28 12:15 model_navigator/utils/dataloader.py
--rw-rw-rw-  2.0 unx     3902 b- defN 23-Jun-28 12:15 model_navigator/utils/devices.py
--rw-rw-rw-  2.0 unx     1308 b- defN 23-Jun-28 12:15 model_navigator/utils/enums.py
--rw-rw-rw-  2.0 unx     6163 b- defN 23-Jun-28 12:15 model_navigator/utils/environment.py
--rw-rw-rw-  2.0 unx     4096 b- defN 23-Jun-28 12:15 model_navigator/utils/format_helpers.py
--rw-rw-rw-  2.0 unx     2330 b- defN 23-Jun-28 12:15 model_navigator/utils/module.py
--rw-rw-rw-  2.0 unx    10140 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    10798 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    14493 b- defN 23-Jun-30 15:48 triton_model_navigator-0.6.0.dist-info/RECORD
-145 files, 768630 bytes uncompressed, 230679 bytes compressed:  70.0%
+Zip file size: 254320 bytes, number of entries: 145
+-rw-r--r--  2.0 unx      881 b- defN 23-Jul-07 09:14 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      649 b- defN 23-Jul-07 10:38 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     3915 b- defN 23-Jul-07 09:14 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-Jul-07 09:14 model_navigator/api/__init__.py
+-rw-rw-rw-  2.0 unx    24220 b- defN 23-Jul-07 10:38 model_navigator/api/config.py
+-rw-rw-rw-  2.0 unx     6263 b- defN 23-Jul-07 10:38 model_navigator/api/jax.py
+-rw-rw-rw-  2.0 unx     5268 b- defN 23-Jul-07 10:38 model_navigator/api/onnx.py
+-rw-rw-rw-  2.0 unx    16279 b- defN 23-Jul-07 10:38 model_navigator/api/package.py
+-rw-r--r--  2.0 unx     4795 b- defN 23-Jul-07 09:14 model_navigator/api/python.py
+-rw-rw-rw-  2.0 unx     7751 b- defN 23-Jul-07 10:38 model_navigator/api/pytriton.py
+-rw-rw-rw-  2.0 unx     6350 b- defN 23-Jul-07 10:38 model_navigator/api/tensorflow.py
+-rw-rw-rw-  2.0 unx     6158 b- defN 23-Jul-07 10:38 model_navigator/api/torch.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-Jul-07 09:14 model_navigator/api/triton.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-Jul-07 09:14 model_navigator/api/utilities.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/__init__.py
+-rw-rw-rw-  2.0 unx     5542 b- defN 23-Jul-07 10:38 model_navigator/commands/base.py
+-rw-r--r--  2.0 unx     9486 b- defN 23-Jul-07 09:14 model_navigator/commands/execution_context.py
+-rw-r--r--  2.0 unx    12793 b- defN 23-Jul-07 09:14 model_navigator/commands/infer_metadata.py
+-rw-r--r--  2.0 unx     3325 b- defN 23-Jul-07 09:14 model_navigator/commands/load.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/__init__.py
+-rw-rw-rw-  2.0 unx     9868 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/base.py
+-rw-rw-rw-  2.0 unx     7633 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/tf.py
+-rw-rw-rw-  2.0 unx    10029 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/torch.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/__init__.py
+-rw-r--r--  2.0 unx     3418 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-r--r--  2.0 unx     4992 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-r--r--  2.0 unx      680 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/__init__.py
+-rw-r--r--  2.0 unx     1727 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-rw-rw-  2.0 unx    10733 b- defN 23-Jul-07 10:38 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-r--r--  2.0 unx     2235 b- defN 23-Jul-07 09:14 model_navigator/commands/convert/onnx/trt_load_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/copy/__init__.py
+-rw-r--r--  2.0 unx     1798 b- defN 23-Jul-07 09:14 model_navigator/commands/copy/onnx.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Jul-07 09:14 model_navigator/commands/correctness/__init__.py
+-rw-rw-rw-  2.0 unx     5674 b- defN 23-Jul-07 10:38 model_navigator/commands/correctness/correctness.py
+-rw-r--r--  2.0 unx     4733 b- defN 23-Jul-07 09:14 model_navigator/commands/correctness/correctness_script.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/data_dump/__init__.py
+-rw-r--r--  2.0 unx    10740 b- defN 23-Jul-07 09:14 model_navigator/commands/data_dump/samples.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/export/__init__.py
+-rw-r--r--  2.0 unx     3611 b- defN 23-Jul-07 09:14 model_navigator/commands/export/jax.py
+-rw-r--r--  2.0 unx     5598 b- defN 23-Jul-07 09:14 model_navigator/commands/export/tf.py
+-rw-r--r--  2.0 unx     9156 b- defN 23-Jul-07 09:14 model_navigator/commands/export/torch.py
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/__init__.py
+-rw-r--r--  2.0 unx     3945 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Jul-07 09:14 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-r--r--  2.0 unx     7156 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-r--r--  2.0 unx     3075 b- defN 23-Jul-07 09:14 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/__init__.py
+-rw-r--r--  2.0 unx     5260 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/performance.py
+-rw-r--r--  2.0 unx     6964 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profile.py
+-rw-r--r--  2.0 unx     3104 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profile_script.py
+-rw-r--r--  2.0 unx     7269 b- defN 23-Jul-07 09:14 model_navigator/commands/performance/profiler.py
+-rw-rw-rw-  2.0 unx     5476 b- defN 23-Jul-07 10:38 model_navigator/commands/performance/results.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/commands/verification/__init__.py
+-rw-r--r--  2.0 unx     4657 b- defN 23-Jul-07 09:14 model_navigator/commands/verification/verify.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/configuration/__init__.py
+-rw-rw-rw-  2.0 unx     2002 b- defN 23-Jul-07 10:38 model_navigator/configuration/common_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/configuration/model/__init__.py
+-rw-rw-rw-  2.0 unx    15653 b- defN 23-Jul-07 10:38 model_navigator/configuration/model/model_config.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-Jul-07 10:38 model_navigator/configuration/model/model_config_builder.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/core/__init__.py
+-rw-rw-rw-  2.0 unx     1389 b- defN 23-Jul-07 10:38 model_navigator/core/constants.py
+-rw-r--r--  2.0 unx     5299 b- defN 23-Jul-07 09:14 model_navigator/core/logger.py
+-rw-r--r--  2.0 unx     9941 b- defN 23-Jul-07 09:14 model_navigator/core/tensor.py
+-rw-r--r--  2.0 unx     2147 b- defN 23-Jul-07 09:14 model_navigator/core/workspace.py
+-rw-r--r--  2.0 unx     2817 b- defN 23-Jul-07 09:14 model_navigator/frameworks/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jul-07 09:14 model_navigator/frameworks/jax/__init__.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-07 09:14 model_navigator/frameworks/jax/model.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/onnx/__init__.py
+-rw-r--r--  2.0 unx     1085 b- defN 23-Jul-07 09:14 model_navigator/frameworks/onnx/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/tensorrt/__init__.py
+-rw-r--r--  2.0 unx    27191 b- defN 23-Jul-07 09:14 model_navigator/frameworks/tensorrt/cuda.py
+-rw-rw-rw-  2.0 unx    10627 b- defN 23-Jul-07 10:38 model_navigator/frameworks/tensorrt/utils.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/frameworks/torch/__init__.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jul-07 09:14 model_navigator/frameworks/torch/utils.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-07 09:14 model_navigator/package/__init__.py
+-rw-r--r--  2.0 unx    12176 b- defN 23-Jul-07 09:14 model_navigator/package/builder.py
+-rw-r--r--  2.0 unx     4651 b- defN 23-Jul-07 09:14 model_navigator/package/loader.py
+-rw-rw-rw-  2.0 unx    11860 b- defN 23-Jul-07 10:38 model_navigator/package/package.py
+-rw-rw-rw-  2.0 unx     2819 b- defN 23-Jul-07 10:38 model_navigator/package/profiling_results.py
+-rw-rw-rw-  2.0 unx    21135 b- defN 23-Jul-07 10:38 model_navigator/package/status.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5232 b- defN 23-Jul-07 09:14 model_navigator/pipelines/pipeline.py
+-rw-rw-rw-  2.0 unx    14762 b- defN 23-Jul-07 10:38 model_navigator/pipelines/pipeline_context.py
+-rw-r--r--  2.0 unx     3832 b- defN 23-Jul-07 09:14 model_navigator/pipelines/pipeline_manager.py
+-rw-rw-rw-  2.0 unx     9693 b- defN 23-Jul-07 10:38 model_navigator/pipelines/validation.py
+-rw-rw-rw-  2.0 unx     1883 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/__init__.py
+-rw-r--r--  2.0 unx     2106 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/correctness.py
+-rw-rw-rw-  2.0 unx     5682 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/jax.py
+-rw-rw-rw-  2.0 unx     2509 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/onnx.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/performance.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/preprocessing.py
+-rw-r--r--  2.0 unx     2504 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/profiling.py
+-rw-rw-rw-  2.0 unx     2921 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/tensorflow.py
+-rw-rw-rw-  2.0 unx     3326 b- defN 23-Jul-07 10:38 model_navigator/pipelines/builders/torch.py
+-rw-r--r--  2.0 unx     2112 b- defN 23-Jul-07 09:14 model_navigator/pipelines/builders/verify.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/__init__.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/optimize.py
+-rw-r--r--  2.0 unx     4881 b- defN 23-Jul-07 09:14 model_navigator/pipelines/wrappers/profile.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jul-07 09:14 model_navigator/runners/__init__.py
+-rw-r--r--  2.0 unx    13796 b- defN 23-Jul-07 09:14 model_navigator/runners/base.py
+-rw-r--r--  2.0 unx     2620 b- defN 23-Jul-07 09:14 model_navigator/runners/jax.py
+-rw-r--r--  2.0 unx     9999 b- defN 23-Jul-07 09:14 model_navigator/runners/onnx.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-Jul-07 09:14 model_navigator/runners/python.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-Jul-07 09:14 model_navigator/runners/registry.py
+-rw-r--r--  2.0 unx     7976 b- defN 23-Jul-07 09:14 model_navigator/runners/tensorflow.py
+-rw-r--r--  2.0 unx    26748 b- defN 23-Jul-07 09:14 model_navigator/runners/tensorrt.py
+-rw-r--r--  2.0 unx    10041 b- defN 23-Jul-07 09:14 model_navigator/runners/torch.py
+-rw-r--r--  2.0 unx     3559 b- defN 23-Jul-07 09:14 model_navigator/runners/utils.py
+-rw-r--r--  2.0 unx      937 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/__init__.py
+-rw-r--r--  2.0 unx    11714 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/analyzer.py
+-rw-r--r--  2.0 unx     2304 b- defN 23-Jul-07 09:14 model_navigator/runtime_analyzer/strategy.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/triton/__init__.py
+-rw-rw-rw-  2.0 unx     3180 b- defN 23-Jul-07 10:38 model_navigator/triton/model_config.py
+-rw-r--r--  2.0 unx     5218 b- defN 23-Jul-07 09:14 model_navigator/triton/model_config_builder.py
+-rw-r--r--  2.0 unx    23090 b- defN 23-Jul-07 09:14 model_navigator/triton/model_config_generator.py
+-rw-r--r--  2.0 unx    15243 b- defN 23-Jul-07 09:14 model_navigator/triton/model_repository.py
+-rw-r--r--  2.0 unx     2081 b- defN 23-Jul-07 09:14 model_navigator/triton/utils.py
+-rw-r--r--  2.0 unx      944 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/__init__.py
+-rw-rw-rw-  2.0 unx     2872 b- defN 23-Jul-07 10:38 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-r--r--  2.0 unx    22326 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/common.py
+-rw-r--r--  2.0 unx     2229 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/internal.py
+-rw-r--r--  2.0 unx     2685 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-r--r--  2.0 unx     3162 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Jul-07 09:14 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-07 09:14 model_navigator/utils/__init__.py
+-rw-rw-rw-  2.0 unx    14509 b- defN 23-Jul-07 10:38 model_navigator/utils/common.py
+-rw-r--r--  2.0 unx     8132 b- defN 23-Jul-07 09:14 model_navigator/utils/dataloader.py
+-rw-r--r--  2.0 unx     3902 b- defN 23-Jul-07 09:14 model_navigator/utils/devices.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jul-07 09:14 model_navigator/utils/enums.py
+-rw-r--r--  2.0 unx     6163 b- defN 23-Jul-07 09:14 model_navigator/utils/environment.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jul-07 09:14 model_navigator/utils/format_helpers.py
+-rw-r--r--  2.0 unx     2330 b- defN 23-Jul-07 09:14 model_navigator/utils/module.py
+-rw-r--r--  2.0 unx    10140 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10798 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    14493 b- defN 23-Jul-07 12:40 triton_model_navigator-0.6.1.dist-info/RECORD
+145 files, 768716 bytes uncompressed, 230700 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -414,23 +414,23 @@
 
 Filename: model_navigator/utils/format_helpers.py
 Comment: 
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
-Filename: triton_model_navigator-0.6.0.dist-info/LICENSE
+Filename: triton_model_navigator-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.6.0.dist-info/METADATA
+Filename: triton_model_navigator-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.6.0.dist-info/WHEEL
+Filename: triton_model_navigator-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.6.0.dist-info/top_level.txt
+Filename: triton_model_navigator-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.6.0.dist-info/RECORD
+Filename: triton_model_navigator-0.6.1.dist-info/RECORD
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
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

## model_navigator/package/package.py

```diff
@@ -10,21 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Package module - structure to snapshot optimization result."""
 import copy
 import pathlib
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import yaml
 
 from model_navigator.api.config import (
     CUSTOM_CONFIGS_MAPPING,
     SERIALIZED_FORMATS,
+    CustomConfigForFormat,
     DeviceKind,
     Format,
     OptimizationProfile,
     TensorType,
 )
 from model_navigator.commands.base import CommandStatus
 from model_navigator.commands.correctness.correctness import Correctness
@@ -296,23 +297,25 @@
         if path.exists():
             path.unlink()
 
     @property
     def _target_formats(self):
         return tuple(Format(target_format) for target_format in self.status.config["target_formats"])
 
-    def _get_custom_configs(self, custom_configs: Dict[str, Dict]) -> Dict:
+    def _get_custom_configs(self, custom_configs: Dict[str, Union[Dict, CustomConfigForFormat]]) -> Dict:
         """Build custom configs from config data.
 
         Args:
             custom_configs: Dictionary with custom configs data
 
         Returns:
             List with mapped objects
         """
         custom_configs_mapped = {}
-        for class_name, fields in custom_configs.items():
-            custom_config_class = CUSTOM_CONFIGS_MAPPING[class_name]
-            obj = custom_config_class.from_dict(fields)  # pytype: disable=not-instantiable
+        for class_name, obj in custom_configs.items():
+            if isinstance(obj, dict):
+                custom_config_class = CUSTOM_CONFIGS_MAPPING[class_name]
+                obj = custom_config_class.from_dict(obj)  # pytype: disable=not-instantiable
+
             custom_configs_mapped[class_name] = obj
 
         return custom_configs_mapped
```

## model_navigator/utils/common.py

```diff
@@ -79,16 +79,14 @@
                 Defaults to None.
             parse (bool, optional): If True recursively parse field values to jsonable representation.
                 Defaults to False.
 
         Returns:
             Dict: Data serialized to a dictionary.
         """
-        data = {}
-
         if filter_fields:
             filtered_data = DataObject.filter_data(
                 data=self.__dict__,
                 filter_fields=filter_fields,
             )
         else:
             filtered_data = self.__dict__
```

## Comparing `triton_model_navigator-0.6.0.dist-info/LICENSE` & `triton_model_navigator-0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.6.0.dist-info/METADATA` & `triton_model_navigator-0.6.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.6.0
+Version: 0.6.1
 Summary: Triton Model Navigator provides tools supporting to create Deep Learning production ready inference models
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.6.0.dist-info/RECORD` & `triton_model_navigator-0.6.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 model_navigator/__init__.py,sha256=YQ8MA8xQgnLgxeQ_oK_E7W8Tpxavwj0SKvbiq4r-JJE,881
-model_navigator/__version__.py,sha256=W3QIw5mWecu8uoAzvIDja1C1lD37ya3_K2g7NUKuHJM,649
+model_navigator/__version__.py,sha256=ECVKemedbrrIEIqnW9Awybdq6tFv_UIZ-6WA1YCq-v8,649
 model_navigator/exceptions.py,sha256=AnYKlbe6WHk4_3lEhksgONKjtcNK7_g0-qs8mIHARuA,3915
 model_navigator/api/__init__.py,sha256=Jt9Du5gr7UP0ljMEur81SAqLg99DokO0vyw1qaonOqY,1716
 model_navigator/api/config.py,sha256=buMLeLqvirV4efpIAxgDBFo0gSoHGNttOns4dHkU_V4,24220
 model_navigator/api/jax.py,sha256=QwOjMl89TPZpj4lOOMLrGOnNrWMoVMCFhgTgk1mmCLA,6263
 model_navigator/api/onnx.py,sha256=CwX50QTt6seCbCDAOvgPLbOQjw29sL-bVWvMViFlU18,5268
 model_navigator/api/package.py,sha256=BqPo9VD_alP4aMbvvQCdqGEZZ3YrQ1PNMcDH-B-uBC8,16279
 model_navigator/api/python.py,sha256=n3Pdc_2TK9Q1yYui4R2rLh8ImC3ezhHnh-n0K1Hcom0,4795
@@ -76,15 +76,15 @@
 model_navigator/frameworks/tensorrt/cuda.py,sha256=T2mHYLdgBTqf2eIgryECZmp_EiTTLIVZEuK_Q3Gl7JA,27191
 model_navigator/frameworks/tensorrt/utils.py,sha256=ZzerG6EUlJx4hivcknnyN92b7SSaZdQuXRmgg_Nby4Y,10627
 model_navigator/frameworks/torch/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/frameworks/torch/utils.py,sha256=dv3m37LjHV286b4THAOefyDX9jBi2J3iJWRMET6M2H4,1513
 model_navigator/package/__init__.py,sha256=ygs5wE6IuzQ0w4g8nWq8jrkkoYoWtdPY0zxJmKiW80M,622
 model_navigator/package/builder.py,sha256=H_G2_9UVcQWCvL7nwzaRML-gG3Ppc50-azmEUqFweuw,12176
 model_navigator/package/loader.py,sha256=gv61Ks9vDJ0nHWK4Tug_RIycBLkWkBsUYKOOndiJHL0,4651
-model_navigator/package/package.py,sha256=pYEN7wxN4QYZmsWgi-cM1XEiz0Al8hWoiopH52oa6Dw,11755
+model_navigator/package/package.py,sha256=Q3RW3h-n3TU8BX43jpObycSW-jCGJZju-sf3cHJBa3k,11860
 model_navigator/package/profiling_results.py,sha256=SPT3JXXwzIJK355ccegFtIXdXI6jqqqIUciwulkH0bw,2819
 model_navigator/package/status.py,sha256=WqKhUhkjWj0LZEINO35PE1Aizqy-lxtuEN55NgqvnIo,21135
 model_navigator/pipelines/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
 model_navigator/pipelines/pipeline.py,sha256=81YfJxylmZUt1_AYinwnq8h9lqy5tl5UDPOa_fikXps,5232
 model_navigator/pipelines/pipeline_context.py,sha256=_ZDSiSFXyFiPJI8GERvIq5J2qTJYYFZhP5c_y-gKTIs,14762
 model_navigator/pipelines/pipeline_manager.py,sha256=Moy6zVv9ya6Bl2vrAICMonpsPvxcwLK841ZXqQ0nuwg,3832
 model_navigator/pipelines/validation.py,sha256=8W57a57B5IfnEQKLoMu16V8SWfH73p-3oRoc0FT-92o,9693
@@ -127,19 +127,19 @@
 model_navigator/triton/specialized_configs/internal.py,sha256=R42XlgUEOC5B-WotI_dAQs8sQyHJOnVyTvVk3CaZ6kM,2229
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=oN76Ux7JI4eqlarlEVSSiIbbajAqdrF3bW0n6WQBPPw,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=NGijgogtoJnbBLL1hQqhw-n4rBo_OgFsCdn9ezw24VI,1785
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=GxJnFB4UpnUwB75t09d5XZ2iqeMZM1SmTbGe2aqmph8,2239
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=C_qMi-5TAWTSL_wBDIoJju3gHRHX10RBbHvBE9of780,3162
 model_navigator/triton/specialized_configs/tensorrt_model_config.py,sha256=ikNi_i_cPjL2Mhea1uJHXe3KElvpHkiPH_zXK895pQU,3040
 model_navigator/utils/__init__.py,sha256=gn5THrzWdJIS7lRXqx3nug16lH-O5AoZFLTCD2AWMpw,627
-model_navigator/utils/common.py,sha256=7VBJ-f0V9aqvdGLjxsAwZEP_VuoNwASxfNh5W3bq7Mk,14528
+model_navigator/utils/common.py,sha256=zDD3FCSPJsig7GK2EcqzKX-q2umzO34xg4a8tL7iuxw,14509
 model_navigator/utils/dataloader.py,sha256=r549fsb5tq7ZQpnKFw4Zk9Mgc8WKzwP4wZHlpWXNj1g,8132
 model_navigator/utils/devices.py,sha256=pGjRBByJqFjG6dyJ0H2E6GJA7hIgF6rgeINLNdS27kU,3902
 model_navigator/utils/enums.py,sha256=T-G5VV5CqimxpctOqPaCvVoAwx-pp10Eeo0rKlWoVGU,1308
 model_navigator/utils/environment.py,sha256=MnpdF5eCx2DJpHtaq8fUSky0hdT03qTJrGnJDhCnFhM,6163
 model_navigator/utils/format_helpers.py,sha256=3UGJhNTFZiMorbMQrciDzJgfFW2nvLMroNmeqC8FlGs,4096
 model_navigator/utils/module.py,sha256=BX9Da3b-tOHvOFb4Ffts0Qc1i9hbgwreGbScqq_DINY,2330
-triton_model_navigator-0.6.0.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.6.0.dist-info/METADATA,sha256=MrRwS7J2lUYKGmEnXnqZ1qJgIZx8MXRllABfi8XDiTM,10798
-triton_model_navigator-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-triton_model_navigator-0.6.0.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.6.0.dist-info/RECORD,,
+triton_model_navigator-0.6.1.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.6.1.dist-info/METADATA,sha256=67GVztavILQkw37c074Z6seXgk-NoebcEg0vA8e9y10,10798
+triton_model_navigator-0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+triton_model_navigator-0.6.1.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.6.1.dist-info/RECORD,,
```

