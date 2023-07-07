# Comparing `tmp/optimum-1.9.0.tar.gz` & `tmp/optimum-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.9.0.tar", last modified: Fri Jun 30 01:19:24 2023, max compression
+gzip compressed data, was "optimum-1.9.1.tar", last modified: Fri Jul  7 21:08:02 2023, max compression
```

## Comparing `optimum-1.9.0.tar` & `optimum-1.9.1.tar`

### file list

```diff
@@ -1,153 +1,149 @@
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.9.0/LICENSE
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.9.0/MANIFEST.in
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12733 2023-06-30 01:19:24.367601 optimum-1.9.0/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11114 2023-05-30 06:59:27.000000 optimum-1.9.0/README.md
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.363597 optimum-1.9.0/optimum/
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/bettertransformer/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/bettertransformer/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/bettertransformer/models/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9234 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    26249 2023-06-09 09:29:41.000000 optimum-1.9.0/optimum/bettertransformer/models/attention.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8092 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/bettertransformer/models/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13124 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/decoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60021 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/models/encoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    18000 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/bettertransformer/transformation.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      952 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5872 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2475 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/env.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/export/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      716 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/export/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1340 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/export/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/commands/export/ggml.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9198 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/commands/export/onnx.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9100 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/commands/export/tflite.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      759 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1374 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3885 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/onnxruntime/optimize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4291 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/commands/onnxruntime/quantize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6871 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/optimum_cli.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/commands/register/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      621 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/commands/register/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/conftest.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/exporters/error_utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    20403 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    47953 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16370 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1051 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/constants.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38753 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    43664 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/model_configs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9286 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/model_patcher.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12499 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/onnx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    66149 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/tasks.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/exporters/tflite/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5693 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/exporters/tflite/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15712 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/exporters/tflite/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16963 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/exporters/tflite/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/exporters/tflite/model_configs.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/optimization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/optimization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/optimization/transformations.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/fx/quantization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/quantization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/quantization/functions.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/fx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15218 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/modeling_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11171 2023-05-30 06:59:28.000000 optimum-1.9.0/optimum/onnx/graph_transformations.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13025 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnx/transformations_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/onnx/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    33264 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45341 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/onnxruntime/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      901 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnxruntime/constants.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/graph.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/io_binding/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/io_binding/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/model.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31047 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/modeling_decoder.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/modeling_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    84386 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/modeling_ort.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    58294 2023-06-20 12:54:57.000000 optimum-1.9.0/optimum/onnxruntime/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15964 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/optimization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/preprocessors/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/preprocessors/quantization.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23561 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/quantization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/onnxruntime/runs/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7990 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/onnxruntime/runs/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/runs/calibrator.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      625 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/onnxruntime/runs/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    89043 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/trainer.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38387 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/trainer_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17122 2023-04-17 07:37:27.000000 optimum-1.9.0/optimum/onnxruntime/training_args.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/onnxruntime/training_args_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12010 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/onnxruntime/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/pipelines/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/pipelines/diffusers/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/pipelines/diffusers/pipeline_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13478 2023-05-31 13:23:46.000000 optimum-1.9.0/optimum/pipelines/pipelines_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/quantization_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-04-11 18:28:51.000000 optimum-1.9.0/optimum/runs_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/utils/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2084 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/constant.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/doc.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/dummy_diffusers_objects.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/file_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6422 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/import_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    25488 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/input_generators.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7836 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/logging.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/modeling_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9820 2023-06-30 00:45:49.000000 optimum-1.9.0/optimum/utils/normalized_config.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum/utils/preprocessing/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/image_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/question_answering.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2169 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/preprocessing/task_processors_manager.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4436 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/preprocessing/text_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/preprocessing/token_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/runs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-04-11 18:28:52.000000 optimum-1.9.0/optimum/utils/save_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5762 2023-04-21 12:20:55.000000 optimum-1.9.0/optimum/utils/testing_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-06-30 00:47:35.000000 optimum-1.9.0/optimum/version.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/optimum.egg-info/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12733 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4365 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/SOURCES.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/dependency_links.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/entry_points.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 13:27:45.000000 optimum-1.9.0/optimum.egg-info/not-zip-safe
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1109 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/requires.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-06-30 01:19:24.000000 optimum-1.9.0/optimum.egg-info/top_level.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.9.0/pyproject.toml
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-06-30 01:19:24.367601 optimum-1.9.0/setup.cfg
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3554 2023-06-30 00:45:49.000000 optimum-1.9.0/setup.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-06-30 01:19:24.367601 optimum-1.9.0/tests/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3382 2023-05-30 06:59:28.000000 optimum-1.9.0/tests/test_configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1936 2023-04-11 18:28:52.000000 optimum-1.9.0/tests/test_modeling_base.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.711503 optimum-1.9.1/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-07-07 21:01:23.000000 optimum-1.9.1/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-07-07 21:01:23.000000 optimum-1.9.1/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    12713 2023-07-07 21:08:02.711503 optimum-1.9.1/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)    11114 2023-07-07 21:01:23.000000 optimum-1.9.1/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/bettertransformer/
+-rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/bettertransformer/models/
+-rw-r--r--   0 ella      (1000) ella      (1000)     9234 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/models/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    26249 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/models/attention.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8092 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/models/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13124 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/models/decoder_models.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    60021 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/models/encoder_models.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18000 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/bettertransformer/transformation.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/commands/
+-rw-r--r--   0 ella      (1000) ella      (1000)      952 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/commands/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5872 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2475 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/env.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/commands/export/
+-rw-r--r--   0 ella      (1000) ella      (1000)      716 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/export/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1340 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/export/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9198 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/export/onnx.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9100 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/export/tflite.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/commands/onnxruntime/
+-rw-r--r--   0 ella      (1000) ella      (1000)      759 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/commands/onnxruntime/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1374 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/commands/onnxruntime/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3885 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/commands/onnxruntime/optimize.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4291 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/commands/onnxruntime/quantize.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6871 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/optimum_cli.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      621 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/commands/register/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17957 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/configuration_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1454 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/conftest.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/exporters/
+-rw-r--r--   0 ella      (1000) ella      (1000)      688 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      707 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      953 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/error_utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/exporters/onnx/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1918 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/onnx/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    20403 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/onnx/__main__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    47953 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/onnx/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    16370 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/onnx/config.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1051 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/onnx/constants.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38753 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/onnx/convert.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    43664 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/onnx/model_configs.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9286 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/onnx/model_patcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    12499 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/onnx/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    66149 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/exporters/tasks.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/exporters/tflite/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1209 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5693 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/__main__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15712 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1397 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/config.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    16963 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/convert.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3588 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/exporters/tflite/model_configs.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/fx/
+-rw-r--r--   0 ella      (1000) ella      (1000)      672 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/fx/optimization/
+-rw-r--r--   0 ella      (1000) ella      (1000)      866 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/optimization/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    32725 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/optimization/transformations.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.681503 optimum-1.9.1/optimum/fx/quantization/
+-rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/quantization/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13591 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/quantization/functions.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1450 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/fx/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15218 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/modeling_base.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.691503 optimum-1.9.1/optimum/onnx/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1276 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3830 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    11171 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/graph_transformations.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4316 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13025 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/transformations_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3307 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnx/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.691503 optimum-1.9.1/optimum/onnxruntime/
+-rw-r--r--   0 ella      (1000) ella      (1000)     4279 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/onnxruntime/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    33264 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    45341 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      901 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/constants.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      955 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/graph.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/onnxruntime/io_binding/
+-rw-r--r--   0 ella      (1000) ella      (1000)      675 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/io_binding/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     7767 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3915 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/model.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    31047 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/onnxruntime/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17940 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/onnxruntime/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    84386 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/modeling_ort.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    58294 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15964 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/optimization.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/onnxruntime/preprocessors/
+-rw-r--r--   0 ella      (1000) ella      (1000)      686 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/
+-rw-r--r--   0 ella      (1000) ella      (1000)      760 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3048 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1377 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1415 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1580 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2350 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/preprocessors/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    23561 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/quantization.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/onnxruntime/runs/
+-rw-r--r--   0 ella      (1000) ella      (1000)     7990 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/runs/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4070 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/runs/calibrator.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      625 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/runs/utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    89043 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38387 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17122 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1362 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/training_args_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    12010 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/onnxruntime/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/pipelines/
+-rw-r--r--   0 ella      (1000) ella      (1000)      770 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/pipelines/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.701503 optimum-1.9.1/optimum/pipelines/diffusers/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11266 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2211 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13478 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/pipelines/pipelines_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      948 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/quantization_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10268 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/runs_base.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.711503 optimum-1.9.1/optimum/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)     2084 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      845 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2001 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/doc.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      953 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/utils/dummy_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3747 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/file_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6422 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    25488 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/input_generators.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     7836 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/logging.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1295 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9740 2023-07-07 21:06:15.000000 optimum-1.9.1/optimum/utils/normalized_config.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.711503 optimum-1.9.1/optimum/utils/preprocessing/
+-rw-r--r--   0 ella      (1000) ella      (1000)      977 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10271 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4263 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/image_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3995 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/question_answering.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2169 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/task_processors_manager.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4436 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/text_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3940 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/preprocessing/token_classification.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    11609 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/runs.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2364 2023-07-07 21:05:28.000000 optimum-1.9.1/optimum/utils/save_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5762 2023-07-07 21:01:23.000000 optimum-1.9.1/optimum/utils/testing_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      639 2023-07-07 21:06:33.000000 optimum-1.9.1/optimum/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-07 21:08:02.671503 optimum-1.9.1/optimum.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    12713 2023-07-07 21:08:01.000000 optimum-1.9.1/optimum.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     4271 2023-07-07 21:08:02.000000 optimum-1.9.1/optimum.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-07-07 21:08:01.000000 optimum-1.9.1/optimum.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-07-07 21:08:02.000000 optimum-1.9.1/optimum.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-07-07 21:08:01.000000 optimum-1.9.1/optimum.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)     1109 2023-07-07 21:08:02.000000 optimum-1.9.1/optimum.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-07-07 21:08:02.000000 optimum-1.9.1/optimum.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1212 2023-07-07 21:01:23.000000 optimum-1.9.1/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      423 2023-07-07 21:08:02.711503 optimum-1.9.1/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     3554 2023-07-07 21:05:28.000000 optimum-1.9.1/setup.py
```

### Comparing `optimum-1.9.0/LICENSE` & `optimum-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/MANIFEST.in` & `optimum-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/PKG-INFO` & `optimum-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.9.0
+Version: 1.9.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -270,9 +269,7 @@
   )
 
   # Use ONNX Runtime for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/training).
-
-
```

### Comparing `optimum-1.9.0/README.md` & `optimum-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/__init__.py` & `optimum-1.9.1/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/models/__init__.py` & `optimum-1.9.1/optimum/bettertransformer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/models/attention.py` & `optimum-1.9.1/optimum/bettertransformer/models/attention.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/models/base.py` & `optimum-1.9.1/optimum/bettertransformer/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/models/decoder_models.py` & `optimum-1.9.1/optimum/bettertransformer/models/decoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.9.1/optimum/bettertransformer/models/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/bettertransformer/transformation.py` & `optimum-1.9.1/optimum/bettertransformer/transformation.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/__init__.py` & `optimum-1.9.1/optimum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/base.py` & `optimum-1.9.1/optimum/commands/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/env.py` & `optimum-1.9.1/optimum/commands/env.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/export/__init__.py` & `optimum-1.9.1/optimum/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/export/base.py` & `optimum-1.9.1/optimum/commands/export/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/export/ggml.py` & `optimum-1.9.1/optimum/exporters/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-# Copyright 2023 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines the command line for the export with ggml."""
-
-from ...exporters.ggml.convert import main_export
-
-
-class GgmlExportCommand:
-    def __init__(self, args):
-        self.args = args
-
-    def run(self):
-        main_export(
-            model_name_or_path=self.args.model,
-            output=self.args.output,
-            task=self.args.task,
-            fp16=self.args.fp16,
-        )
+from . import onnx  # noqa
+from .tasks import TasksManager  # noqa
```

### Comparing `optimum-1.9.0/optimum/commands/export/onnx.py` & `optimum-1.9.1/optimum/commands/export/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/export/tflite.py` & `optimum-1.9.1/optimum/commands/export/tflite.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/onnxruntime/__init__.py` & `optimum-1.9.1/optimum/commands/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/onnxruntime/base.py` & `optimum-1.9.1/optimum/commands/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/onnxruntime/optimize.py` & `optimum-1.9.1/optimum/commands/onnxruntime/optimize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/onnxruntime/quantize.py` & `optimum-1.9.1/optimum/commands/onnxruntime/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/optimum_cli.py` & `optimum-1.9.1/optimum/commands/optimum_cli.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/commands/register/__init__.py` & `optimum-1.9.1/optimum/commands/register/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/configuration_utils.py` & `optimum-1.9.1/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/conftest.py` & `optimum-1.9.1/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/__init__.py` & `optimum-1.9.1/optimum/fx/optimization/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # coding=utf-8
-# Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright 2022 The HuggingFace Team. All rights reserved.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-from . import onnx  # noqa
-from .tasks import TasksManager  # noqa
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+from .transformations import (  # noqa
+    ChangeTrueDivToMulByInverse,
+    FuseBatchNorm1dInLinear,
+    FuseBatchNorm2dInConv2d,
+    FuseBiasInLinear,
+    MergeLinears,
+    ReversibleTransformation,
+    Transformation,
+    compose,
+)
```

### Comparing `optimum-1.9.0/optimum/exporters/base.py` & `optimum-1.9.1/optimum/exporters/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/error_utils.py` & `optimum-1.9.1/optimum/exporters/error_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/__init__.py` & `optimum-1.9.1/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/__main__.py` & `optimum-1.9.1/optimum/exporters/onnx/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/base.py` & `optimum-1.9.1/optimum/exporters/onnx/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/config.py` & `optimum-1.9.1/optimum/exporters/onnx/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/constants.py` & `optimum-1.9.1/optimum/exporters/onnx/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/convert.py` & `optimum-1.9.1/optimum/exporters/onnx/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/model_configs.py` & `optimum-1.9.1/optimum/exporters/onnx/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/model_patcher.py` & `optimum-1.9.1/optimum/exporters/onnx/model_patcher.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/onnx/utils.py` & `optimum-1.9.1/optimum/exporters/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tasks.py` & `optimum-1.9.1/optimum/exporters/tasks.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/__init__.py` & `optimum-1.9.1/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/__main__.py` & `optimum-1.9.1/optimum/exporters/tflite/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/base.py` & `optimum-1.9.1/optimum/exporters/tflite/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/config.py` & `optimum-1.9.1/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/convert.py` & `optimum-1.9.1/optimum/exporters/tflite/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/exporters/tflite/model_configs.py` & `optimum-1.9.1/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/fx/__init__.py` & `optimum-1.9.1/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/fx/optimization/__init__.py` & `optimum-1.9.1/optimum/onnxruntime/io_binding/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-# coding=utf-8
 #  Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from .transformations import (  # noqa
-    ChangeTrueDivToMulByInverse,
-    FuseBatchNorm1dInLinear,
-    FuseBatchNorm2dInConv2d,
-    FuseBiasInLinear,
-    MergeLinears,
-    ReversibleTransformation,
-    Transformation,
-    compose,
-)
+from .io_binding_helper import IOBindingHelper, TypeHelper
```

### Comparing `optimum-1.9.0/optimum/fx/optimization/transformations.py` & `optimum-1.9.1/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/fx/quantization/__init__.py` & `optimum-1.9.1/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/fx/quantization/functions.py` & `optimum-1.9.1/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/fx/utils.py` & `optimum-1.9.1/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/modeling_base.py` & `optimum-1.9.1/optimum/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/__init__.py` & `optimum-1.9.1/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/configuration.py` & `optimum-1.9.1/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/graph_transformations.py` & `optimum-1.9.1/optimum/onnx/graph_transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/modeling_seq2seq.py` & `optimum-1.9.1/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/transformations_utils.py` & `optimum-1.9.1/optimum/onnx/transformations_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnx/utils.py` & `optimum-1.9.1/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/__init__.py` & `optimum-1.9.1/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/base.py` & `optimum-1.9.1/optimum/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/configuration.py` & `optimum-1.9.1/optimum/onnxruntime/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/constants.py` & `optimum-1.9.1/optimum/onnxruntime/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/graph.py` & `optimum-1.9.1/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from .io_binding_helper import IOBindingHelper, TypeHelper
+
+from .quantization import PreprocessorPass, QuantizationPreprocessor
```

### Comparing `optimum-1.9.0/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.9.1/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/model.py` & `optimum-1.9.1/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.9.1/optimum/onnxruntime/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.9.1/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/modeling_ort.py` & `optimum-1.9.1/optimum/onnxruntime/modeling_ort.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.9.1/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/optimization.py` & `optimum-1.9.1/optimum/onnxruntime/optimization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.9.1/optimum/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+#  Copyright 2021 The HuggingFace Team. All rights reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .quantization import PreprocessorPass, QuantizationPreprocessor
+__version__ = "1.9.1"
```

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.9.1/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/quantization.py` & `optimum-1.9.1/optimum/onnxruntime/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/runs/__init__.py` & `optimum-1.9.1/optimum/onnxruntime/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.9.1/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/runs/utils.py` & `optimum-1.9.1/optimum/onnxruntime/runs/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/trainer.py` & `optimum-1.9.1/optimum/onnxruntime/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.9.1/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/training_args.py` & `optimum-1.9.1/optimum/onnxruntime/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.9.1/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/onnxruntime/utils.py` & `optimum-1.9.1/optimum/onnxruntime/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/pipelines/__init__.py` & `optimum-1.9.1/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.9.1/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.9.1/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/pipelines/pipelines_base.py` & `optimum-1.9.1/optimum/pipelines/pipelines_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/quantization_base.py` & `optimum-1.9.1/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/runs_base.py` & `optimum-1.9.1/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/__init__.py` & `optimum-1.9.1/optimum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/constant.py` & `optimum-1.9.1/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/doc.py` & `optimum-1.9.1/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.9.1/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/file_utils.py` & `optimum-1.9.1/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/import_utils.py` & `optimum-1.9.1/optimum/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/input_generators.py` & `optimum-1.9.1/optimum/utils/input_generators.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/logging.py` & `optimum-1.9.1/optimum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/modeling_utils.py` & `optimum-1.9.1/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/normalized_config.py` & `optimum-1.9.1/optimum/utils/normalized_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     Attributes:
         config ([`PretrainedConfig`]):
             The config to normalize.
     """
 
     def __init__(self, config: Union[PretrainedConfig, Dict], allow_new: bool = False, **kwargs):
-        self.config = config if isinstance(config, PretrainedConfig) else PretrainedConfig.from_dict(config)
+        self.config = config
         for key, value in kwargs.items():
             if allow_new or hasattr(self, key.upper()):
                 setattr(self, key.upper(), value)
             else:
                 raise AttributeError(
                     f"{self.__class__} has not attribute {key}. Set allow_new=True to add a new attribute."
                 )
```

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/__init__.py` & `optimum-1.9.1/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/base.py` & `optimum-1.9.1/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/image_classification.py` & `optimum-1.9.1/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/question_answering.py` & `optimum-1.9.1/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.9.1/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/text_classification.py` & `optimum-1.9.1/optimum/utils/preprocessing/text_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/preprocessing/token_classification.py` & `optimum-1.9.1/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/runs.py` & `optimum-1.9.1/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/save_utils.py` & `optimum-1.9.1/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum/utils/testing_utils.py` & `optimum-1.9.1/optimum/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/optimum.egg-info/PKG-INFO` & `optimum-1.9.1/optimum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.9.0
+Version: 1.9.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -270,9 +269,7 @@
   )
 
   # Use ONNX Runtime for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/training).
-
-
```

### Comparing `optimum-1.9.0/optimum.egg-info/SOURCES.txt` & `optimum-1.9.1/optimum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 optimum/bettertransformer/models/encoder_models.py
 optimum/commands/__init__.py
 optimum/commands/base.py
 optimum/commands/env.py
 optimum/commands/optimum_cli.py
 optimum/commands/export/__init__.py
 optimum/commands/export/base.py
-optimum/commands/export/ggml.py
 optimum/commands/export/onnx.py
 optimum/commands/export/tflite.py
 optimum/commands/onnxruntime/__init__.py
 optimum/commands/onnxruntime/base.py
 optimum/commands/onnxruntime/optimize.py
 optimum/commands/onnxruntime/quantize.py
 optimum/commands/register/__init__.py
@@ -117,10 +116,8 @@
 optimum/utils/testing_utils.py
 optimum/utils/preprocessing/__init__.py
 optimum/utils/preprocessing/base.py
 optimum/utils/preprocessing/image_classification.py
 optimum/utils/preprocessing/question_answering.py
 optimum/utils/preprocessing/task_processors_manager.py
 optimum/utils/preprocessing/text_classification.py
-optimum/utils/preprocessing/token_classification.py
-tests/test_configuration_utils.py
-tests/test_modeling_base.py
+optimum/utils/preprocessing/token_classification.py
```

### Comparing `optimum-1.9.0/optimum.egg-info/requires.txt` & `optimum-1.9.1/optimum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/pyproject.toml` & `optimum-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.9.0/setup.py` & `optimum-1.9.1/setup.py`

 * *Files identical despite different names*

