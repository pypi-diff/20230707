# Comparing `tmp/dataquality-0.9.3.tar.gz` & `tmp/dataquality-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.3.tar", last modified: Wed Jun 28 15:20:32 2023, max compression
+gzip compressed data, was "dataquality-0.9.4.tar", last modified: Fri Jul  7 21:00:15 2023, max compression
```

## Comparing `dataquality-0.9.3.tar` & `dataquality-0.9.4.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.433193 dataquality-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-28 15:19:11.000000 dataquality-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-28 15:20:32.433193 dataquality-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-28 15:19:11.000000 dataquality-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.385192 dataquality-0.9.3/dataquality/
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.385192 dataquality-0.9.3/dataquality/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/clients/objectstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.389192 dataquality-0.9.3/dataquality/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/core/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.393192 dataquality-0.9.3/dataquality/dq_auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_auto/text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.393192 dataquality-0.9.3/dataquality/dq_start/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dq_start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.397192 dataquality-0.9.3/dataquality/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/integrations/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.397192 dataquality-0.9.3/dataquality/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/base_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.401193 dataquality-0.9.3/dataquality/loggers/data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/data_logger/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.401193 dataquality-0.9.3/dataquality/loggers/logger_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/logger_config/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.405192 dataquality-0.9.3/dataquality/loggers/model_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.413193 dataquality-0.9.3/dataquality/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/schemas/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.425193 dataquality-0.9.3/dataquality/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/ampli.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/auto_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/dq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/hdf5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/hf_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/od.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.429193 dataquality-0.9.3/dataquality/utils/semantic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/vaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-28 15:19:11.000000 dataquality-0.9.3/dataquality/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.385192 dataquality-0.9.3/dataquality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-28 15:20:32.000000 dataquality-0.9.3/dataquality.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-28 15:19:11.000000 dataquality-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-28 15:20:32.437193 dataquality-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:19:11.000000 dataquality-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.429193 dataquality-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_dataquality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_telemetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:20:32.433193 dataquality-0.9.3/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/ner_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-28 15:19:11.000000 dataquality-0.9.3/tests/test_utils/tc_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.110956 dataquality-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 20:58:05.000000 dataquality-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-07 21:00:15.110956 dataquality-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-07 20:58:05.000000 dataquality-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.038955 dataquality-0.9.4/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.042955 dataquality-0.9.4/dataquality/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/clients/objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.046955 dataquality-0.9.4/dataquality/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.050955 dataquality-0.9.4/dataquality/dq_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.050955 dataquality-0.9.4/dataquality/dq_start/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dq_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.054955 dataquality-0.9.4/dataquality/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.054955 dataquality-0.9.4/dataquality/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.062955 dataquality-0.9.4/dataquality/loggers/data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.070955 dataquality-0.9.4/dataquality/loggers/logger_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.074955 dataquality-0.9.4/dataquality/loggers/model_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.086955 dataquality-0.9.4/dataquality/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/schemas/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.102955 dataquality-0.9.4/dataquality/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ampli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/dq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hf_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/od.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.102955 dataquality-0.9.4/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/vaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:58:05.000000 dataquality-0.9.4/dataquality/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.038955 dataquality-0.9.4/dataquality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 21:00:15.000000 dataquality-0.9.4/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-07 20:58:05.000000 dataquality-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 21:00:15.110956 dataquality-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:58:05.000000 dataquality-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.106955 dataquality-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_dataquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_telemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:00:15.110956 dataquality-0.9.4/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/ner_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-07 20:58:05.000000 dataquality-0.9.4/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.9.3/LICENSE` & `dataquality-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/PKG-INFO` & `dataquality-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.3
+Version: 0.9.4
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.3/README.md` & `dataquality-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/__init__.py` & `dataquality-0.9.4/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
 
-__version__ = "v0.9.3"
+__version__ = "0.9.4"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.3/dataquality/analytics.py` & `dataquality-0.9.4/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/clients/api.py` & `dataquality-0.9.4/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/clients/objectstore.py` & `dataquality-0.9.4/dataquality/clients/objectstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 from functools import partial
 from tempfile import NamedTemporaryFile
 from typing import Any, Optional
 
 import requests
+from tenacity import retry, stop_after_attempt, wait_exponential_jitter
 from tqdm.auto import tqdm
 from tqdm.utils import CallbackIOWrapper
 from vaex.dataframe import DataFrame
 
 from dataquality.core._config import config
 from dataquality.core.auth import api_client
 from dataquality.utils.file import get_file_extension
@@ -122,14 +123,18 @@
         self._minio_client.fput_object(
             bucket_name=bucket_name,
             object_name=object_name,
             file_path=file_path,
             content_type=content_type,
         )
 
+    @retry(
+        stop=stop_after_attempt(4),
+        wait=wait_exponential_jitter(initial=0.1, max=10),
+    )
     def _upload_file_from_local(
         self,
         url: str,
         file_path: str,
         content_type: str = "application/octet-stream",
         progress: bool = True,
     ) -> None:
```

### Comparing `dataquality-0.9.3/dataquality/core/__init__.py` & `dataquality-0.9.4/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/core/_config.py` & `dataquality-0.9.4/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/core/auth.py` & `dataquality-0.9.4/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/core/finish.py` & `dataquality-0.9.4/dataquality/core/finish.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from dataquality.clients.api import ApiClient
 from dataquality.core._config import config
 from dataquality.core.report import build_run_report
 from dataquality.schemas import RequestType, Route
 from dataquality.schemas.job import JobName
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.dq_logger import DQ_LOG_FILE_HOME, upload_dq_log_file
-from dataquality.utils.helpers import check_noop, gpu_available, open_console_url
+from dataquality.utils.helpers import check_noop, gpu_available
 from dataquality.utils.thread_pool import ThreadPoolManager
-from dataquality.utils.version import _version_check
 
 api_client = ApiClient()
 a = Analytics(ApiClient, config)  # type: ignore
 
 
 @check_noop
 def finish(
@@ -46,16 +45,14 @@
     ThreadPoolManager.wait_for_threads()
     assert config.current_project_id, "You must have an active project to call finish"
     assert config.current_run_id, "You must have an active run to call finish"
     assert config.task_type, "You must have a task type to call finish"
     data_logger = dataquality.get_data_logger()
     data_logger.validate_labels()
 
-    _version_check()
-
     if data_logger.non_inference_logged():
         _reset_run(config.current_project_id, config.current_run_id, config.task_type)
 
     # Certain tasks require extra finish logic
     data_logger.logger_config.finish()
 
     data_logger.upload(last_epoch, create_data_embs=create_data_embs)
@@ -83,25 +80,23 @@
     )
     if data_logger.logger_config.conditions:
         print(
             "Waiting for run to process before building run report... "
             "Don't close laptop or terminate shell."
         )
         wait_for_run()
-        open_console_url(res["link"])
         build_run_report(
             data_logger.logger_config.conditions,
             data_logger.logger_config.report_emails,
             project_id=config.current_project_id,
             run_id=config.current_run_id,
             link=res["link"],
         )
     elif wait:
         wait_for_run()
-        open_console_url(res["link"])
 
     # Reset the data logger
     data_logger._cleanup()
 
     # Reset the model logger
     dataquality.get_model_logger()._cleanup()
```

### Comparing `dataquality-0.9.3/dataquality/core/init.py` & `dataquality-0.9.4/dataquality/core/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from dataquality.core.auth import login
 from dataquality.exceptions import GalileoException, GalileoWarning
 from dataquality.loggers import BaseGalileoLogger
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.dq_logger import DQ_LOG_FILE_HOME
 from dataquality.utils.helpers import check_noop
 from dataquality.utils.name import validate_name
+from dataquality.utils.version import version_check
 
 api_client = ApiClient()
 
 
 class InitManager:
     @retry(
         retry=retry_if_exception_type(GalileoException),
@@ -178,14 +179,15 @@
     :param overwrite_local: If True, the current project/run log directory will be
     cleared during this function. If logging over many sessions with checkpoints, you
     may want to set this to False. Default True
     """
     if not api_client.valid_current_user():
         login()
     _check_dq_version()
+    version_check()
     _init = InitManager()
     task_type = BaseGalileoLogger.validate_task(task_type)
     config.task_type = task_type
     if not project_name and run_name:
         # The user provided a run name and no project name. No good
         warnings.warn(
             "⚠️ You must specify a project name to initialize or create a new Galileo "
```

### Comparing `dataquality-0.9.3/dataquality/core/log.py` & `dataquality-0.9.4/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/core/report.py` & `dataquality-0.9.4/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/dq_auto/auto.py` & `dataquality-0.9.4/dataquality/dq_auto/auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     hf_model: str = "distilbert-base-uncased",
     num_train_epochs: int = 15,
     labels: Optional[List[str]] = None,
     project_name: Optional[str] = None,
     run_name: Optional[str] = None,
     wait: bool = True,
     create_data_embs: Optional[bool] = None,
+    early_stopping: bool = True,
 ) -> None:
     """Automatically gets insights on a text classification or NER dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface transformer model, and
     provide Galileo insights via a link to the Galileo Console
 
@@ -92,14 +93,15 @@
     :param create_data_embs: Whether to create data embeddings for this run. If True,
         Sentence-Transformers will be used to generate data embeddings for this dataset
         and uploaded with this run. You can access these embeddings via
         `dq.metrics.get_data_embeddings` in the `emb` column or
         `dq.metrics.get_dataframe(..., include_data_embs=True)` in the `data_emb` col
         Only available for TC currently. NER coming soon. Default True if a GPU is
         available, else default False.
+    :param early_stopping: Whether to use early stopping. Default True
 
     For text classification datasets, the only required columns are `text` and `label`
 
     For NER, the required format is the huggingface standard format of `tokens` and
     `tags` (or `ner_tags`).
     See example: https://huggingface.co/datasets/rungalileo/mit_movies
 
@@ -218,14 +220,15 @@
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             create_data_embs=create_data_embs,
             num_train_epochs=num_train_epochs,
+            early_stopping=early_stopping,
         )
     elif task_type == TaskType.text_ner:
         from dataquality.dq_auto.ner import auto as auto_ner
 
         return auto_ner(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
@@ -235,10 +238,11 @@
             inference_data=inference_data,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             num_train_epochs=num_train_epochs,
+            early_stopping=early_stopping,
         )
     else:
         raise Exception("auto is only supported for text classification and NER!")
```

### Comparing `dataquality-0.9.3/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.4/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/dq_auto/ner.py` & `dataquality-0.9.4/dataquality/dq_auto/ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
     num_train_epochs: int = 15,
     hf_model: str = "distilbert-base-uncased",
     labels: Optional[List[str]] = None,
     project_name: str = "auto_ner",
     run_name: Optional[str] = None,
     wait: bool = True,
+    early_stopping: bool = True,
 ) -> None:
     """Automatically gets insights on an NER or Token Classification dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface token classification model, and
     provide Galileo insights via a link to the Galileo Console
 
@@ -114,14 +115,15 @@
         will attempt to be extracted from the data
     :param project_name: Optional project name. If not set, a random name will
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
+    :param early_stopping: Whether to use early stopping. Default True
 
     To see auto insights on a random, pre-selected dataset, simply run
     ```python
         from dataquality.auto.ner import auto
 
         auto()
     ```
@@ -170,9 +172,11 @@
     if not run_name and isinstance(hf_data, str):
         run_name = run_name_from_hf_dataset(hf_data)
     dq.init(
         TaskType.text_ner,
         project_name=project_name,
         run_name=run_name,
     )
-    trainer, encoded_data = get_trainer(dd, hf_model, num_train_epochs, labels)
+    trainer, encoded_data = get_trainer(
+        dd, hf_model, num_train_epochs, labels, early_stopping=early_stopping
+    )
     return do_train(trainer, encoded_data, wait)
```

### Comparing `dataquality-0.9.3/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.4/dataquality/dq_auto/ner_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 
 def get_trainer(
     dd: DatasetDict,
     model_checkpoint: str,
     num_train_epochs: int,
     labels: Optional[List[str]] = None,
+    early_stopping: bool = True,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     default_cols = set(HFCol.get_fields())
     meta = [c for c in dd[Split.train].features if c not in default_cols]
     encoded_datasets = tokenize_and_log_dataset(
         dd, tokenizer, label_names=labels, meta=meta
@@ -101,19 +102,22 @@
         save_strategy=IntervalStrategy.EPOCH,
         logging_strategy=IntervalStrategy.EPOCH,
         logging_dir="./logs",
         seed=42,
         use_mps_device=mps_available(),
     )
 
+    callbacks = []
+    if early_stopping:
+        callbacks.append(EarlyStoppingCallback(early_stopping_patience=1))
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
         model_init=model_init,
         args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics,
         data_collator=DataCollatorForTokenClassification(tokenizer),
-        callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
+        callbacks=callbacks,
     )
     return trainer, encoded_datasets
```

### Comparing `dataquality-0.9.3/dataquality/dq_auto/notebook.py` & `dataquality-0.9.4/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.4/dataquality/dq_auto/tc_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 def get_trainer(
     dd: DatasetDict,
     labels: List[str],
     model_checkpoint: str,
     max_padding_length: int,
     num_train_epochs: int,
+    early_stopping: bool = True,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     encoded_datasets = dd.map(
         lambda x: preprocess_function(x, tokenizer, max_padding_length), batched=True
     )
 
@@ -89,18 +90,21 @@
         load_best_model_at_end=load_best_model,
         push_to_hub=False,
         report_to=["all"],
         seed=42,
         use_mps_device=mps_available(),
     )
 
+    callbacks = []
+    if early_stopping:
+        callbacks.append(EarlyStoppingCallback(early_stopping_patience=1))
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
         model_init=model_init,
         args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics_partial,
-        callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
+        callbacks=callbacks,
     )
     return trainer, encoded_datasets
```

### Comparing `dataquality-0.9.3/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.4/dataquality/dq_auto/text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.auto import (
     add_class_label_to_dataset,
     add_val_data_if_missing,
     run_name_from_hf_dataset,
 )
 from dataquality.utils.auto_trainer import do_train
+from dataquality.utils.setfit import _get_meta_cols
 
 a = Analytics(ApiClient, dq.config)
 a.log_import("auto_tc")
 
 
 class TCDatasetManager(BaseDatasetManager):
     DEMO_DATASETS = [
@@ -100,16 +101,15 @@
         return train_labels.names
     return sorted(set(dd[Split.train]["label"]))
 
 
 def _log_dataset_dict(dd: DatasetDict) -> None:
     for key in dd:
         ds = dd[key]
-        default_cols = ["text", "label", "id"]
-        meta = [i for i in ds.features if i not in default_cols]
+        meta = _get_meta_cols(ds.features)
         if key in Split.get_valid_keys():
             dq.log_dataset(ds, meta=meta, split=key)
         else:
             dq.log_dataset(ds, meta=meta, split=Split.inference, inference_name=key)
 
 
 def auto(
@@ -123,14 +123,15 @@
     num_train_epochs: int = 15,
     hf_model: str = "distilbert-base-uncased",
     labels: Optional[List[str]] = None,
     project_name: str = "auto_tc",
     run_name: Optional[str] = None,
     wait: bool = True,
     create_data_embs: Optional[bool] = None,
+    early_stopping: bool = True,
 ) -> Trainer:
     """Automatically gets insights on a text classification dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface transformer model, and
     provide Galileo insights via a link to the Galileo Console
 
@@ -182,14 +183,15 @@
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
     :param create_data_embs: Whether to create data embeddings for this run. Default
         False
+    :param early_stopping: Whether to use early stopping. Default True
 
     To see auto insights on a random, pre-selected dataset, simply run
     ```python
         from dataquality.auto.text_classification import auto
 
         auto()
     ```
@@ -254,10 +256,15 @@
     a.log_function("auto/tc")
     if not run_name and isinstance(hf_data, str):
         run_name = run_name_from_hf_dataset(hf_data)
     dq.init(TaskType.text_classification, project_name=project_name, run_name=run_name)
     dq.set_labels_for_run(labels)
     _log_dataset_dict(dd)
     trainer, encoded_data = get_trainer(
-        dd, labels, hf_model, max_padding_length, num_train_epochs
+        dd,
+        labels,
+        hf_model,
+        max_padding_length,
+        num_train_epochs,
+        early_stopping=early_stopping,
     )
     return do_train(trainer, encoded_data, wait, create_data_embs)
```

### Comparing `dataquality-0.9.3/dataquality/dq_start/__init__.py` & `dataquality-0.9.4/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/dqyolo.py` & `dataquality-0.9.4/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/fastai.py` & `dataquality-0.9.4/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/hf.py` & `dataquality-0.9.4/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/keras.py` & `dataquality-0.9.4/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/setfit.py` & `dataquality-0.9.4/dataquality/integrations/setfit.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.auto import _apply_column_mapping, run_name_from_hf_dataset
 from dataquality.utils.patcher import PatchManager
 from dataquality.utils.setfit import (
     SetFitModelHook,
+    _get_meta_cols,
     _prepare_config,
     _setup_patches,
     get_trainer,
     log_preds_setfit,
     validate_setfit,
 )
 
@@ -125,14 +126,15 @@
 
 def evaluate(
     model: "SetFitModel",
 ) -> Callable:
     """Watch SetFit model by replacing predict_proba function with SetFitModelHook.
     :param model: SetFit model
     :return: SetFitModelHook object"""
+
     dq_hook = SetFitModelHook(model)
     dq_store = dq_hook.store
 
     def dq_evaluate(
         dataset: Dataset,
         split: Split,
         meta: Optional[List] = None,
@@ -145,23 +147,20 @@
         :param batch: batch of data as a dictionary
         :param split: split of data (training, validation, test, inference)
         :param meta: columns that should be logged as metadata
         :param inference_name: inference name (if split is inference, must be provided)
         :param column_mapping: mapping of column names (if different from default)
         :return: output of SetFitModel.predict_proba function"""
         a.log_function("setfit/evaluate")
-
         column_mapping = column_mapping or dict(
-            text="text",
             id="id",
+            text="text",
             label="label",
         )
-
-        if column_mapping is not None:
-            dataset = _apply_column_mapping(dataset, column_mapping)
+        dataset = _apply_column_mapping(dataset, column_mapping)
         if "id" not in dataset.features:
             dataset = dataset.map(lambda x, idx: {"id": idx}, with_indices=True)
         if epoch is not None:
             dq.set_epoch(epoch)
         cur_epoch = get_data_logger().logger_config.cur_epoch
         return log_preds_setfit(
             model=model,
@@ -190,15 +189,15 @@
     labels: Optional[List[str]] = None,
     project_name: str = "auto_tc_setfit",
     run_name: Optional[str] = None,
     training_args: Optional[Dict[str, Any]] = None,
     column_mapping: Optional[Dict[str, str]] = None,
     wait: bool = True,
     create_data_embs: Optional[bool] = None,
-) -> Union["SetFitModel", "SetFitTrainer"]:
+) -> "SetFitModel":
     """Automatically processes and generates insights on a text classification dataset.
 
     Given a pandas dataframe, a file path, or a Huggingface dataset path, this
     function will load the data, train a Huggingface transformer model, and
     provide insights via a link to the Console.
 
     At least one of `hf_data`, `train_data` should be provided. If neither of
@@ -251,16 +250,16 @@
     wait : bool, optional
         Whether to wait for the processing of your run to complete. Default is True.
     create_data_embs : bool, optional
         Whether to create data embeddings for this run. Default is None.
 
     Returns
     -------
-    SetFitModel or SetFitTrainer
-        A SetFitTrainer instance trained on the provided dataset.
+    SetFitModel
+        A SetFitModel instance trained on the provided dataset.
 
     An example using `auto` with sklearn data as pandas dataframes
     ```python
         import pandas as pd
         from sklearn.datasets import fetch_20newsgroups
         from dataquality.auto.text_classification import auto
 
@@ -294,14 +293,15 @@
          test_data="test.csv",
          project_name="data_from_local",
          run_name="run_1_raw_data"
     )
     ```
     """
     manager = TCDatasetManager()
+
     dd = manager.get_dataset_dict(
         hf_data,
         hf_inference_names,
         train_data,
         val_data,
         test_data,
         inference_data,
@@ -314,79 +314,49 @@
 
     if not run_name:
         run_name = run_name_from_hf_dataset(hf_data or "setfit_auto")
     dq.init(TaskType.text_classification, project_name=project_name, run_name=run_name)
     dq.set_labels_for_run(labels)
     if isinstance(setfit_model, str):
         # Load the model and train it
-        trainer, encoded_data = get_trainer(dd, setfit_model, training_args)
-        return do_train(
-            trainer,
-            encoded_data,
-            wait,
-            create_data_embs,
-        )
-    else:
-        # Don't train, just evaluate
-        return do_model_eval(setfit_model, dd, wait, create_data_embs)
+        trainer = get_trainer(dd, setfit_model, training_args)
+        trainer.train()
+        setfit_model = trainer.model
+
+    return do_model_eval(setfit_model, dd, wait, create_data_embs)
 
 
 def do_model_eval(
     model: "SetFitModel",
     encoded_data: DatasetDict,
     wait: bool,
     create_data_embs: Optional[bool] = None,
 ) -> "SetFitModel":
     dq_evaluate = watch(
         model,
         finish=False,
     )
     for split in [Split.train, Split.test, Split.val]:
         if split in encoded_data:
+            ds = encoded_data[split]
+            meta_columns = _get_meta_cols(ds.column_names)
             dq_evaluate(
                 encoded_data[split],
                 split=split,
+                meta=meta_columns
                 # for inference set the split to inference
                 # and pass an inference_name="inference_run_1"
             )
 
     inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
     for inf_name in inf_names:
+        ds = encoded_data[inf_name]
+        meta_columns = _get_meta_cols(ds.column_names)
         dq_evaluate(
-            encoded_data[inf_name],
+            ds,
             split=Split.inference,  # type: ignore
             inference_name=inf_name,  # type: ignore
+            meta=meta_columns,
         )
 
     dq.finish(wait=wait, create_data_embs=create_data_embs)
     return model
-
-
-def do_train(
-    trainer: "SetFitTrainer",
-    encoded_data: DatasetDict,
-    wait: bool,
-    create_data_embs: Optional[bool] = None,
-) -> "SetFitTrainer":
-    watch(trainer, finish=False)
-
-    trainer.train()
-    dq_evaluate = watch(trainer, finish=False)
-    if Split.test in encoded_data:
-        # We pass in a huggingface dataset but typing wise they expect a torch dataset
-        dq_evaluate(
-            encoded_data[Split.test],
-            split=Split.test,
-            # for inference set the split to inference
-            # and pass an inference_name="inference_run_1"
-        )
-
-    inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
-    for inf_name in inf_names:
-        dq_evaluate(
-            encoded_data[inf_name],
-            split=Split.inference,  # type: ignore
-            inference_name=inf_name,  # type: ignore
-        )
-
-    dq.finish(wait=wait, create_data_embs=create_data_embs)
-    return trainer
```

### Comparing `dataquality-0.9.3/dataquality/integrations/torch.py` & `dataquality-0.9.4/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-0.9.4/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.4/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/integrations/ultralytics.py` & `dataquality-0.9.4/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/internal.py` & `dataquality-0.9.4/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/base_logger.py` & `dataquality-0.9.4/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/seq2seq.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.4/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/seq2seq.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.4/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,27 @@
         except LogBatchError as e:
             warnings.warn(
                 f"An error occurred logging this batch, it will be skipped. Error: {e}",
                 GalileoWarning,
             )
             return
         data = self._get_data_dict()
+        data = self._downcast_data_dict(data)
         self.write_model_output(data)
 
+    def _downcast_data_dict(self, data: Dict) -> Dict:
+        """Downcasts any float/int 64 types to 32 before saving batch"""
+        for key, val in data.items():
+            if isinstance(val, np.ndarray):
+                if val.dtype == np.int64:
+                    data[key] = val.astype(np.int32)
+                elif val.dtype == np.float64:
+                    data[key] = val.astype(np.float32)
+        return data
+
     def _add_threaded_log(self) -> None:
         try:
             self._log()
         except Exception as e:
             get_dq_logger().exception(
                 "Logging of model outputs failed", split=self.split, epoch=self.epoch
             )
```

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/seq2seq.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.4/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/metrics.py` & `dataquality-0.9.4/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/condition.py` & `dataquality-0.9.4/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/dataframe.py` & `dataquality-0.9.4/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/edit.py` & `dataquality-0.9.4/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/hf.py` & `dataquality-0.9.4/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/metrics.py` & `dataquality-0.9.4/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/ner.py` & `dataquality-0.9.4/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/report.py` & `dataquality-0.9.4/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/route.py` & `dataquality-0.9.4/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.4/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/seq2seq.py` & `dataquality-0.9.4/dataquality/schemas/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/split.py` & `dataquality-0.9.4/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/task_type.py` & `dataquality-0.9.4/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/schemas/torch.py` & `dataquality-0.9.4/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/ampli.py` & `dataquality-0.9.4/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/auto.py` & `dataquality-0.9.4/dataquality/utils/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,28 +207,29 @@
     ds = ds.cast_column("label", class_label)
     return ds
 
 
 def _apply_column_mapping(dataset: Dataset, column_mapping: Dict[str, str]) -> Dataset:
     """
     Applies the provided column mapping to the dataset, renaming columns accordingly.
-    Extra features not in the column mapping are prefixed with `"feat_"`.
     """
     if type(dataset) == dict:
         dataset = Dataset.from_dict(dataset)
-    dataset = dataset.rename_columns(
-        {
-            **column_mapping,
-            **{
-                col: f"feat_{col}"
-                for col in dataset.column_names
-                if col not in column_mapping
-            },
-        }
-    )
+    # Making sure the keys of the column mapping are in the dataset
+    # otherwise show a warning message and remove the key from the mapping
+    clean_column_mapping = {**column_mapping}
+    for key in list(clean_column_mapping.keys()):
+        if key not in dataset.column_names:
+            print(
+                f"Column '{key}' in the column_mapping "
+                "was not found in the dataset, so it was ignored."
+            )
+            clean_column_mapping.pop(key)
+
+    dataset = dataset.rename_columns(clean_column_mapping)
     dset_format = dataset.format
     dataset = dataset.with_format(
         type=dset_format["type"],
         columns=dataset.column_names,
         output_all_columns=dset_format["output_all_columns"],
         **dset_format["format_kwargs"],
     )
```

### Comparing `dataquality-0.9.3/dataquality/utils/auto_trainer.py` & `dataquality-0.9.4/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/cuda.py` & `dataquality-0.9.4/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/cv.py` & `dataquality-0.9.4/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/dq_logger.py` & `dataquality-0.9.4/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/dqyolo.py` & `dataquality-0.9.4/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/emb.py` & `dataquality-0.9.4/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/file.py` & `dataquality-0.9.4/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/hdf5_store.py` & `dataquality-0.9.4/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/helpers.py` & `dataquality-0.9.4/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/hf_images.py` & `dataquality-0.9.4/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.4/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/keras.py` & `dataquality-0.9.4/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/ml.py` & `dataquality-0.9.4/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/name.py` & `dataquality-0.9.4/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/od.py` & `dataquality-0.9.4/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/patcher.py` & `dataquality-0.9.4/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/profiler.py` & `dataquality-0.9.4/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.4/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.4/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.4/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.4/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.4/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/seq2seq.py` & `dataquality-0.9.4/dataquality/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/setfit.py` & `dataquality-0.9.4/dataquality/utils/setfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from dataclasses import asdict, dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from datasets import Dataset, DatasetDict
 from torch import Tensor
 
 import dataquality as dq
@@ -30,21 +30,28 @@
     def clear(self) -> None:
         """Resets the arrays of the class."""
         self.texts.clear()
         self.ids.clear()
         self.labels.clear()
 
 
+def _get_meta_cols(cols: Iterable) -> List[str]:
+    """Returns the meta columns of a dataset."""
+    default_cols = ["text", "label", "id"]
+    meta_columns = [col for col in cols if col not in default_cols]
+    return meta_columns
+
+
 def log_preds_setfit(
     model: "SetFitModel",
     dataset: Dataset,
     split: Split,
     dq_store: Dict,
     batch_size: int,
-    meta: Optional[List] = None,
+    meta: Optional[List[str]] = None,
     inference_name: Optional[str] = None,
     return_preds: bool = False,
     epoch: Optional[int] = None,
 ) -> Tensor:
     """Logs the data samples and model outputs for a SetFit model.
     :param model: The SetFit model
     :param dataset: The dataset in the form of a HuggingFace Dataset
@@ -70,14 +77,15 @@
     epoch = epoch or 0
 
     # Check if the data should be logged by checking if the split is in the
     # input_data_logged
     skip_logging = logger_config.helper_data[f"setfit_skip_input_log_{split}"]
     # Iterate over the dataset in batches and log the data samples
     # and model outputs
+    meta = _get_meta_cols(dataset.column_names)
     for i in range(0, len(dataset), batch_size):
         batch = dataset[i : i + batch_size]
         assert text_col in batch, f"column '{text_col}' must be in batch"
         assert id_col in batch, f"column '{id_col}' text must be in batch"
 
         if inference_name is None and not skip_logging:
             assert label_col in batch, f"column '{label_col}' must be in batch"
@@ -87,17 +95,22 @@
         if return_preds:
             preds.append(pred)
         # 🔭🌕 Galileo logging
         if not skip_logging:
             log_args.texts += batch[text_col]
             log_args.ids += batch[id_col]
             if meta is not None:
-                log_args.meta = {
-                    meta_col: batch[f"feat_{meta_col}"] for meta_col in meta
-                }
+                meta_colum_batch = {}
+                for meta_col in meta:
+                    if meta_col in batch:
+                        meta_colum_batch[meta_col] = batch[meta_col]
+                    else:
+                        print(f"Meta column: {meta_col} was not found in batch")
+                if meta_colum_batch:
+                    log_args.meta = meta_colum_batch
             if len(log_args.texts) >= BATCH_LOG_SIZE:
                 dq.log_data_samples(**asdict(log_args))
                 log_args.clear()
         # 🔭🌕 Galileo logging
         dq.log_model_outputs(
             ids=batch[id_col],
             probs=dq_store["output"],
@@ -128,15 +141,15 @@
 
 def _setup_patches(
     setfit: Union["SetFitModel", "SetFitTrainer"],
     labels: List[str],
     finish: bool = True,
     wait: bool = False,
     batch_size: Optional[int] = None,
-    meta: Optional[List] = None,
+    meta: Optional[List[str]] = None,
 ) -> None:
     """Sets up the patches for a SetFit model.
     :param setfit: The SetFit model or trainer
     :param labels: The labels of the model
     :param finish: Whether to finish the run
     :param wait: Whether to wait for the run to finish
     :param batch_size: The batch size
@@ -155,15 +168,15 @@
     setfitmanager.add_patch(patched_trainer)
 
 
 def validate_setfit(
     setfit: Union["SetFitModel", "SetFitTrainer"],
     labels: List[str],
     batch_size: Optional[int] = None,
-    meta: Optional[List] = None,
+    meta: Optional[List[str]] = None,
 ) -> None:
     """Validates a SetFit model.
     :param setfit: The SetFit model or trainer
     :param labels: The labels of the model
     :param wait: Whether to wait for the run to finish
     :param batch_size: The batch size
     :param meta: The meta columns
@@ -285,15 +298,15 @@
     def __init__(
         self,
         setfit_trainer: "SetFitTrainer",
         labels: List[str] = [],
         finish: bool = True,
         wait: bool = False,
         batch_size: Optional[int] = None,
-        meta: Optional[List] = None,
+        meta: Optional[List[str]] = None,
     ) -> None:
         """Patch to SetFit trainer to run dataquality after training.
         :param setfit_trainer: SetFit trainer
         :param project_name: name of project
         :param run_name: name of run
         :param labels: list of labels
         :param finish: whether to run dq.finish after evaluation
@@ -414,15 +427,15 @@
         setattr(self.model, self.function_name, self.old_fn)
 
 
 def get_trainer(
     dd: DatasetDict,
     model_checkpoint: str,
     training_args: Optional[Dict[str, Any]],
-) -> Tuple["SetFitTrainer", DatasetDict]:
+) -> "SetFitTrainer":
     from sentence_transformers.losses import CosineSimilarityLoss
     from setfit import SetFitModel, SetFitTrainer
 
     # Used to properly seed the model
     def model_init() -> Any:
         return SetFitModel.from_pretrained(model_checkpoint)
 
@@ -435,8 +448,8 @@
         setfit_args.update(training_args)
     trainer = SetFitTrainer(
         model=model_init(),
         train_dataset=dd[Split.training],
         eval_dataset=dd[Split.validation] if has_val else None,
         **setfit_args,
     )
-    return trainer, dd
+    return trainer
```

### Comparing `dataquality-0.9.3/dataquality/utils/thread_pool.py` & `dataquality-0.9.4/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/torch.py` & `dataquality-0.9.4/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/transformers.py` & `dataquality-0.9.4/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/ultralytics.py` & `dataquality-0.9.4/dataquality/utils/ultralytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 box_label(image, box, label, color)
         else:
             color = colors(int(box[-1]))
             box_label(image, box, label, color)
     # show image
     image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
     try:
-        cv2.imshow(image)  # if used in Python
+        cv2.imshow("bboxes", image)  # if used in Python
     except Exception:
         from google.colab.patches import cv2_imshow
 
         cv2_imshow(image)  # if used in Colab
 
 
 # Modified to keep logits
```

### Comparing `dataquality-0.9.3/dataquality/utils/upload.py` & `dataquality-0.9.4/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/vaex.py` & `dataquality-0.9.4/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality/utils/version.py` & `dataquality-0.9.4/dataquality/utils/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import requests
 
 from dataquality import __version__ as dq_client_version
 from dataquality.core._config import config
-from dataquality.exceptions import GalileoException
 from dataquality.schemas.route import Route
+from dataquality.utils.dq_logger import get_dq_logger
 
 
-def _version_check() -> None:
-    """_version_check.
+def version_check() -> None:
+    """version_check.
 
     Asserts that the dataquality python client and the api have
     matching major versions.
 
     https://semver.org/#summary.
 
     Returns:
         None
     """
     client_semver = _get_client_version()
     server_semver = _get_api_version()
-    try:
-        assert _major_version(client_semver) == _major_version(server_semver)
-    except AssertionError:
-        raise GalileoException(
-            "Major mismatch between client, "
+    if _major_version(client_semver) != _major_version(server_semver):
+        get_dq_logger().warning(
+            "Major version mismatched between client, "
             f"{client_semver}, and server {server_semver}."
         )
 
 
 def _major_version(v: str) -> str:
-    return str(v).split(".")[0]
+    return str(v).replace("v", "").split(".")[0]
 
 
 def _get_client_version() -> str:
     return dq_client_version
 
 
 def _get_api_version() -> str:
```

### Comparing `dataquality-0.9.3/dataquality.egg-info/PKG-INFO` & `dataquality-0.9.4/dataquality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.3
+Version: 0.9.4
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.3/dataquality.egg-info/SOURCES.txt` & `dataquality-0.9.4/dataquality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/dataquality.egg-info/requires.txt` & `dataquality-0.9.4/dataquality.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 [test]
 ultralytics
 pytest>=7.2.1
 freezegun>=1.2.2
 coverage[toml]>=7.0.5
 pytest-cov>=4.0.0
 scikit-learn>=1.0
-tensorflow>=2.9.1
+tensorflow<2.13.0,>=2.9.1
 pytest-env>=0.8.1
 pytest-xdist>=2.4.0
 types-setuptools>=67.3.0.1
 types-cachetools>=4.2.4
 torchvision>=0.13.1
 torch>=1.12.1
 torchtext>=0.13.1
```

### Comparing `dataquality-0.9.3/pyproject.toml` & `dataquality-0.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 test = [
     "ultralytics",
     "pytest>=7.2.1",
     "freezegun>=1.2.2",
     "coverage[toml]>=7.0.5",
     "pytest-cov>=4.0.0",
     "scikit-learn>=1.0",
-    "tensorflow>=2.9.1",
+    "tensorflow>=2.9.1,<2.13.0",
     "pytest-env>=0.8.1",
     "pytest-xdist>=2.4.0",
     "types-setuptools>=67.3.0.1",
     "types-cachetools>=4.2.4",
     "torchvision>=0.13.1",
     "torch>=1.12.1",
     "torchtext>=0.13.1",
```

### Comparing `dataquality-0.9.3/tests/test_dataquality.py` & `dataquality-0.9.4/tests/test_dataquality.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,30 +572,28 @@
     dataquality.core.finish._reset_run(pid, rid, TaskType.text_multi_label)
 
     assert mock_create_run.called_once_with(pid, rid, TaskType.text_multi_label)
     assert dataquality.config.current_run_id == rid
 
 
 @pytest.mark.parametrize("last_epoch", [1, 3, None, 10])
-@mock.patch.object(dataquality.core.finish, "_version_check")
 @mock.patch.object(dataquality.core.finish, "_reset_run")
 @mock.patch.object(dataquality.core.finish, "upload_dq_log_file")
 @mock.patch.object(dataquality.clients.api.ApiClient, "make_request")
 @mock.patch.object(dataquality.loggers.base_logger.BaseGalileoLogger, "_cleanup")
 @mock.patch.object(
     dataquality.loggers.data_logger.text_classification.TextClassificationDataLogger,
     "upload_in_out_frames",
 )
 def test_finish_last_epoch(
     mock_upload_frames: MagicMock,
     mock_cleanup: MagicMock,
     mock_make_request: MagicMock,
     mock_upload_log_file: MagicMock,
     mock_reset_run: MagicMock,
-    mock_version_check: MagicMock,
     set_test_config: Callable,
     cleanup_after_use: Callable,
     last_epoch: int,
 ) -> None:
     text_inputs = ["sample1", "sample2", "sample3"] * 30
     gold = ["A", "C", "B"] * 30
     ids = list(range(90))
```

### Comparing `dataquality-0.9.3/tests/test_telemetrics.py` & `dataquality-0.9.4/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/data_utils.py` & `dataquality-0.9.4/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.4/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.4/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.4/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/lightning_model.py` & `dataquality-0.9.4/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/mock_data.py` & `dataquality-0.9.4/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/mock_request.py` & `dataquality-0.9.4/tests/test_utils/mock_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,14 @@
 def mocked_healthcheck_request(request_url: str) -> MockResponse:
     if request_url.endswith("healthcheck"):
         return MockResponse({"api_version": __version__}, 200)
 
     return MockResponse({}, 200)
 
 
-def mocked_healthcheck_request_new_api_version(request_url: str) -> MockResponse:
-    if request_url.endswith("healthcheck"):
-        return MockResponse({"api_version": "100.0.0"}, 200)
-    return MockResponse({}, 200)
-
-
 def mocked_login_requests(
     request_url: str,
     json: Dict = {},
     params: Dict = {},
     headers: Dict = {},
     data: Dict = {},
     timeout: Union[int, None] = None,
```

### Comparing `dataquality-0.9.3/tests/test_utils/ner_constants.py` & `dataquality-0.9.4/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.4/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.3/tests/test_utils/tc_constants.py` & `dataquality-0.9.4/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

