# Comparing `tmp/molgraph-0.4.2.tar.gz` & `tmp/molgraph-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.4.2.tar", last modified: Fri Jul  7 13:23:00 2023, max compression
+gzip compressed data, was "molgraph-0.5.0.tar", last modified: Fri Jul  7 16:19:32 2023, max compression
```

## Comparing `molgraph-0.4.2.tar` & `molgraph-0.5.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.4.2/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2023-07-07 13:23:00.044896 molgraph-0.4.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5896 2023-07-07 13:22:31.000000 molgraph-0.4.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-07 13:22:31.000000 molgraph-0.4.2/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.4.2/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6644 2023-07-04 20:05:31.000000 molgraph-0.4.2/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.4.2/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.4.2/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.4.2/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.4.2/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.4.2/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.4.2/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.4.2/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.4.2/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.4.2/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.4.2/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.4.2/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12879 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11687 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9875 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11815 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10798 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17095 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.4.2/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10194 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10144 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11216 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10507 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.4.2/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9933 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10823 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1585 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25884 2023-07-07 12:49:35.000000 molgraph-0.4.2/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.4.2/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16270 2023-07-07 12:49:35.000000 molgraph-0.4.2/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14446 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.4.2/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10724 2023-07-07 13:13:35.000000 molgraph-0.4.2/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.4.2/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3407 2023-07-05 11:38:46.000000 molgraph-0.4.2/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2013 2023-07-05 11:38:48.000000 molgraph-0.4.2/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2023-07-05 11:38:49.000000 molgraph-0.4.2/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.4.2/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10911 2023-07-05 11:38:52.000000 molgraph-0.4.2/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-07-05 11:38:54.000000 molgraph-0.4.2/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9713 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-07-05 11:38:58.000000 molgraph-0.4.2/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11737 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6665 2023-07-05 11:39:05.000000 molgraph-0.4.2/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20385 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.4.2/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6398 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4579 2023-07-07 12:49:35.000000 molgraph-0.4.2/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3285 2023-07-05 11:39:31.000000 molgraph-0.4.2/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6239 2023-07-05 11:39:33.000000 molgraph-0.4.2/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5347 2023-07-07 12:49:35.000000 molgraph-0.4.2/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.040896 molgraph-0.4.2/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.4.2/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2425 2023-06-14 11:03:03.000000 molgraph-0.4.2/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5371 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.4.2/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2023-07-05 14:45:34.000000 molgraph-0.4.2/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      518 2023-07-05 14:38:06.000000 molgraph-0.4.2/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-07 12:52:08.000000 molgraph-0.4.2/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7774 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6952 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6857 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.4.2/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23572 2023-07-07 12:52:08.000000 molgraph-0.4.2/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.4.2/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.044896 molgraph-0.4.2/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.4.2/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.4.2/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1849 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    51923 2023-07-07 12:40:08.000000 molgraph-0.4.2/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 13:23:00.036896 molgraph-0.4.2/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6616 2023-07-07 13:22:59.000000 molgraph-0.4.2/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-07 13:23:00.000000 molgraph-0.4.2/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-07 13:22:59.000000 molgraph-0.4.2/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       87 2023-07-07 13:22:59.000000 molgraph-0.4.2/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-07 13:22:59.000000 molgraph-0.4.2/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-07 13:23:00.044896 molgraph-0.4.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1448 2023-07-07 13:22:31.000000 molgraph-0.4.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-07 16:19:32.809165 molgraph-0.5.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5888 2023-07-07 16:19:15.000000 molgraph-0.5.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-07 16:19:15.000000 molgraph-0.5.0/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.0/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6644 2023-07-04 20:05:31.000000 molgraph-0.5.0/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.0/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.0/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.0/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.0/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.0/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.0/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.0/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12879 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11687 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9875 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11815 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10798 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17095 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.0/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10194 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10144 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11216 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10507 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.0/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9933 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10823 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1585 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25884 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.0/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16270 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14446 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.0/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10724 2023-07-07 13:13:35.000000 molgraph-0.5.0/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.0/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3407 2023-07-05 11:38:46.000000 molgraph-0.5.0/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2013 2023-07-05 11:38:48.000000 molgraph-0.5.0/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2023-07-05 11:38:49.000000 molgraph-0.5.0/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.0/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10911 2023-07-05 11:38:52.000000 molgraph-0.5.0/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-07-05 11:38:54.000000 molgraph-0.5.0/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9713 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-07-05 11:38:58.000000 molgraph-0.5.0/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11737 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6665 2023-07-05 11:39:05.000000 molgraph-0.5.0/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20385 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.0/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6398 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4579 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3285 2023-07-05 11:39:31.000000 molgraph-0.5.0/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6239 2023-07-05 11:39:33.000000 molgraph-0.5.0/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5347 2023-07-07 12:49:35.000000 molgraph-0.5.0/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.0/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2425 2023-06-14 11:03:03.000000 molgraph-0.5.0/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5371 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.0/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2023-07-05 14:45:34.000000 molgraph-0.5.0/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      518 2023-07-05 14:38:06.000000 molgraph-0.5.0/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.805165 molgraph-0.5.0/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-07 12:52:08.000000 molgraph-0.5.0/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7774 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6952 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6857 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.0/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23572 2023-07-07 12:52:08.000000 molgraph-0.5.0/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.0/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.809165 molgraph-0.5.0/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.0/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.0/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1849 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    51923 2023-07-07 12:40:08.000000 molgraph-0.5.0/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-07 16:19:32.801165 molgraph-0.5.0/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6608 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       87 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-07 16:19:32.000000 molgraph-0.5.0/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-07 16:19:32.809165 molgraph-0.5.0/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1448 2023-07-07 13:22:31.000000 molgraph-0.5.0/setup.py
```

### Comparing `molgraph-0.4.2/LICENSE` & `molgraph-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/PKG-INFO` & `molgraph-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -72,15 +72,15 @@
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 **Important notes**
-- Since version **0.4.2**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -142,15 +142,15 @@
 gnn_model.fit(x_train, y_train, epochs=50)
 scores = gnn_model.evaluate(x_test, y_test)
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
-maps = gam_model.predict(x_train)
+maps = gam_model(x_train)
 ```
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
 - **TensorFlow** (version >= 2.7.0 recommended)
 - **RDKit** (version >= 2022.3.3 recommended)
 - **NumPy** (version >= 1.21.2 recommended)
```

### Comparing `molgraph-0.4.2/README.md` & `molgraph-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 **Important notes**
-- Since version **0.4.2**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -124,15 +124,15 @@
 gnn_model.fit(x_train, y_train, epochs=50)
 scores = gnn_model.evaluate(x_test, y_test)
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
-maps = gam_model.predict(x_train)
+maps = gam_model(x_train)
 ```
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
 - **TensorFlow** (version >= 2.7.0 recommended)
 - **RDKit** (version >= 2022.3.3 recommended)
 - **NumPy** (version >= 1.21.2 recommended)
```

### Comparing `molgraph-0.4.2/molgraph/_filter_warnings.py` & `molgraph-0.5.0/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/applications/graph_transformer.py` & `molgraph-0.5.0/molgraph/applications/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/__init__.py` & `molgraph-0.5.0/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.0/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.0/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.0/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.0/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.0/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.0/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/encoders.py` & `molgraph-0.5.0/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/features.py` & `molgraph-0.5.0/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.0/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/ops.py` & `molgraph-0.5.0/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/chemistry/vis.py` & `molgraph-0.5.0/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/__init__.py` & `molgraph-0.5.0/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.0/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.0/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.0/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.0/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.0/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.0/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.0/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.0/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/gnn_layer.py` & `molgraph-0.5.0/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/gnn_ops.py` & `molgraph-0.5.0/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.0/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.0/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.0/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.0/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.0/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.0/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.0/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.0/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.0/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.0/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.0/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.0/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/losses/link_losses.py` & `molgraph-0.5.0/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/losses/masked_losses.py` & `molgraph-0.5.0/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.0/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.0/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/__init__.py` & `molgraph-0.5.0/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/dgin.py` & `molgraph-0.5.0/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/dmpnn.py` & `molgraph-0.5.0/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.0/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.0/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/mpnn.py` & `molgraph-0.5.0/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.0/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.0/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.0/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.0/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.0/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.0/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -72,15 +72,15 @@
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
 **Important notes**
-- Since version **0.4.2**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -142,15 +142,15 @@
 gnn_model.fit(x_train, y_train, epochs=50)
 scores = gnn_model.evaluate(x_test, y_test)
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
-maps = gam_model.predict(x_train)
+maps = gam_model(x_train)
 ```
 
 ## Requirements/dependencies
 - **Python** (version >= 3.6 recommended)
 - **TensorFlow** (version >= 2.7.0 recommended)
 - **RDKit** (version >= 2022.3.3 recommended)
 - **NumPy** (version >= 1.21.2 recommended)
```

### Comparing `molgraph-0.4.2/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.0/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.4.2/setup.py` & `molgraph-0.5.0/setup.py`

 * *Files identical despite different names*

