# Comparing `tmp/alibi-0.9.3.tar.gz` & `tmp/alibi-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibi-0.9.3.tar", last modified: Wed Jun 21 13:28:31 2023, max compression
+gzip compressed data, was "alibi-0.9.4.tar", last modified: Fri Jul  7 13:17:06 2023, max compression
```

## Comparing `alibi-0.9.3.tar` & `alibi-0.9.4.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.434628 alibi-0.9.3/
--rw-r--r--   0 janis     (1000) janis     (1000)    11354 2023-06-21 11:43:55.000000 alibi-0.9.3/LICENSE
--rw-r--r--   0 janis     (1000) janis     (1000)       58 2023-06-21 11:43:55.000000 alibi-0.9.3/MANIFEST.in
--rw-r--r--   0 janis     (1000) janis     (1000)    20926 2023-06-21 13:28:31.434628 alibi-0.9.3/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)    19975 2023-06-21 11:44:13.000000 alibi-0.9.3/README.md
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.414628 alibi-0.9.3/alibi/
--rw-r--r--   0 janis     (1000) janis     (1000)      187 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/api/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7096 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/defaults.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6960 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/api/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2793 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/api/tests/test_interfaces.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/confidence/
--rw-r--r--   0 janis     (1000) janis     (1000)      251 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18571 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/model_linearity.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/confidence/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8326 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/test_model_linearity.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2174 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/tests/test_trustscore.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8182 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/confidence/trustscore.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/data/
--rw-r--r--   0 janis     (1000) janis     (1000)   116015 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/data/cats.tar.gz
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/datasets/
--rw-r--r--   0 janis     (1000) janis     (1000)      451 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12940 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/default.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1037 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tensorflow.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi/datasets/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4559 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/datasets/tests/test_datasets.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1813 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/exceptions.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/
--rw-r--r--   0 janis     (1000) janis     (1000)     2230 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    29966 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/ale.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/anchors/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35805 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4371 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_explanation.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28076 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    49264 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12848 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_tabular_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)    24277 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27223 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/language_model_text_sampler.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16961 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/anchors/text_samplers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4211 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39331 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17733 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6141 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_tabular.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    19783 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6379 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    35184 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)    66395 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    44884 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfrl_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23850 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/cfrl_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    27167 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    56311 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    73509 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    39110 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    45107 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    80156 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/backends/
--rw-r--r--   0 janis     (1000) janis     (1000)     1321 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.421295 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4753 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/base.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4341 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8837 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/base.py
--rw-r--r--   0 janis     (1000) janis     (1000)    13302 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/grad.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2654 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/similarity/metrics.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11006 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17481 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_ale.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2582 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_base.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7874 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_image.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16247 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_tabular.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18774 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_anchor_text.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1572 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cem.py
--rw-r--r--   0 janis     (1000) janis     (1000)     6681 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cfproto.py
--rw-r--r--   0 janis     (1000) janis     (1000)    20718 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_cfrl.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4900 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_counterfactual.py
--rw-r--r--   0 janis     (1000) janis     (1000)    37074 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_integrated_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)    42674 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_partial_dependence.py
--rw-r--r--   0 janis     (1000) janis     (1000)    28620 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_pd_variance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    23539 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_permutation_importance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    65433 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_shap_wrappers.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5894 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5864 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_backends.py
--rw-r--r--   0 janis     (1000) janis     (1000)    17977 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
--rw-r--r--   0 janis     (1000) janis     (1000)     9302 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3086 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/explainers/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.424628 alibi-0.9.3/alibi/models/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/__init__.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/pytorch/
--rw-r--r--   0 janis     (1000) janis     (1000)      477 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2748 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3094 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8134 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4952 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12988 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/pytorch/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1767 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      647 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3778 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_cfrl_models.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1847 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_metrics.py
--rw-r--r--   0 janis     (1000) janis     (1000)    21220 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/pytorch/tests/test_model.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/tensorflow/
--rw-r--r--   0 janis     (1000) janis     (1000)      486 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2913 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3378 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     8692 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/models/tensorflow/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1655 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_actor_critic.py
--rw-r--r--   0 janis     (1000) janis     (1000)      643 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_autoencoder.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3708 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/models/tensorflow/tests/test_cfrl_models.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/prototypes/
--rw-r--r--   0 janis     (1000) janis     (1000)      250 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    32709 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/protoselect.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/prototypes/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)    11674 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/test_protoselect.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3195 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/prototypes/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)    16214 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/saving.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.427961 alibi-0.9.3/alibi/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      622 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/conftest.py
--rw-r--r--   0 janis     (1000) janis     (1000)     7230 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_dep_management.py
--rw-r--r--   0 janis     (1000) janis     (1000)    18797 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_saving.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1033 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/test_utils.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4809 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/tests/utils.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.431295 alibi-0.9.3/alibi/utils/
--rw-r--r--   0 janis     (1000) janis     (1000)     1276 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4968 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/approximation_methods.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2652 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3592 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/discretizer.py
--rw-r--r--   0 janis     (1000) janis     (1000)    12076 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    31311 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)      582 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/distributions.py
--rw-r--r--   0 janis     (1000) janis     (1000)      513 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/download.py
--rw-r--r--   0 janis     (1000) janis     (1000)      320 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/frameworks.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2915 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4666 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/kernel.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15019 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/lang_model.py
--rw-r--r--   0 janis     (1000) janis     (1000)     4718 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)     5365 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/missing_optional_dependency.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.434628 alibi-0.9.3/alibi/utils/tests/
--rw-r--r--   0 janis     (1000) janis     (1000)        0 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/__init__.py
--rw-r--r--   0 janis     (1000) janis     (1000)      194 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/mocked_opt_dep.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1014 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_data.py
--rw-r--r--   0 janis     (1000) janis     (1000)     3193 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_distance.py
--rw-r--r--   0 janis     (1000) janis     (1000)    15565 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_distributed.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1631 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_gradients.py
--rw-r--r--   0 janis     (1000) janis     (1000)     2855 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_import_optional.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1103 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_mapping.py
--rw-r--r--   0 janis     (1000) janis     (1000)      398 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tests/test_misc.py
--rw-r--r--   0 janis     (1000) janis     (1000)      919 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/tf.py
--rw-r--r--   0 janis     (1000) janis     (1000)    22911 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/visualization.py
--rw-r--r--   0 janis     (1000) janis     (1000)     1707 2023-06-21 11:43:55.000000 alibi-0.9.3/alibi/utils/wrappers.py
--rw-r--r--   0 janis     (1000) janis     (1000)      212 2023-06-21 13:27:29.000000 alibi-0.9.3/alibi/version.py
-drwxr-xr-x   0 janis     (1000) janis     (1000)        0 2023-06-21 13:28:31.417961 alibi-0.9.3/alibi.egg-info/
--rw-r--r--   0 janis     (1000) janis     (1000)    20926 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/PKG-INFO
--rw-r--r--   0 janis     (1000) janis     (1000)     5394 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/SOURCES.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/dependency_links.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        1 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/not-zip-safe
--rw-r--r--   0 janis     (1000) janis     (1000)      649 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/requires.txt
--rw-r--r--   0 janis     (1000) janis     (1000)        6 2023-06-21 13:28:31.000000 alibi-0.9.3/alibi.egg-info/top_level.txt
--rw-r--r--   0 janis     (1000) janis     (1000)     2121 2023-06-21 13:28:31.434628 alibi-0.9.3/setup.cfg
--rw-r--r--   0 janis     (1000) janis     (1000)     2994 2023-06-21 11:43:55.000000 alibi-0.9.3/setup.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.593403 alibi-0.9.4/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    11354 2023-07-07 12:43:00.000000 alibi-0.9.4/LICENSE
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)       58 2023-07-07 12:43:00.000000 alibi-0.9.4/MANIFEST.in
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    20876 2023-07-07 13:17:06.593403 alibi-0.9.4/PKG-INFO
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    19975 2023-07-07 12:43:00.000000 alibi-0.9.4/README.md
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      187 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/__init__.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/api/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/api/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     7096 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/api/defaults.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     6960 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/api/interfaces.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/api/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/api/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2793 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/api/tests/test_interfaces.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/confidence/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      251 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    18571 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/model_linearity.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/confidence/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     8326 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/tests/test_model_linearity.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2174 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/tests/test_trustscore.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     8182 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/confidence/trustscore.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/data/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)   116015 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/data/cats.tar.gz
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/datasets/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      451 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/datasets/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    12940 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/datasets/default.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1037 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/datasets/tensorflow.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/datasets/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/datasets/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4559 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/datasets/tests/test_datasets.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1813 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/exceptions.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi/explainers/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2230 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    29966 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/ale.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/anchors/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    35805 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4371 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_explanation.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    28076 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_image.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    49264 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_tabular.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    12848 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_tabular_distributed.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    24277 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/anchor_text.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    27223 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/language_model_text_sampler.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    16961 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/anchors/text_samplers.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/backends/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4211 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/cfrl_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    39331 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/cfrl_tabular.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/backends/pytorch/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/pytorch/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    17733 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/pytorch/cfrl_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     6141 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/pytorch/cfrl_tabular.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/backends/tensorflow/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/tensorflow/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    19783 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/tensorflow/cfrl_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     6379 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/backends/tensorflow/cfrl_tabular.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    35184 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/cem.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    66395 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/cfproto.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    44884 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/cfrl_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    23850 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/cfrl_tabular.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    27167 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/counterfactual.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    56311 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/integrated_gradients.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    73509 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/partial_dependence.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    39110 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/pd_variance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    45107 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/permutation_importance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    80156 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/shap_wrappers.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/similarity/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/__init__.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/similarity/backends/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1321 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/backends/__init__.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/similarity/backends/pytorch/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/backends/pytorch/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4753 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/backends/pytorch/base.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/similarity/backends/tensorflow/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/backends/tensorflow/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4341 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/backends/tensorflow/base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     8837 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    13302 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/grad.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2654 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/similarity/metrics.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    11006 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/conftest.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    17481 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_ale.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2582 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_anchor_base.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     7874 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_anchor_image.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    16247 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_anchor_tabular.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    18774 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_anchor_text.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1572 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_cem.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     6681 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_cfproto.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    20718 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_cfrl.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4900 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_counterfactual.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    37074 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_integrated_gradients.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    43148 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_partial_dependence.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    28620 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_pd_variance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    23539 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_permutation_importance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    65433 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_shap_wrappers.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     5894 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/conftest.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     5864 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_backends.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    17977 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     9302 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3086 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/explainers/tests/utils.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/models/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/__init__.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.585403 alibi-0.9.4/alibi/models/pytorch/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      477 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2748 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/actor_critic.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3094 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/autoencoder.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     8134 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/cfrl_models.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4952 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/metrics.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    12988 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/model.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/models/pytorch/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1767 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/test_actor_critic.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      647 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/test_autoencoder.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3778 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/test_cfrl_models.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1847 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/test_metrics.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    21220 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/pytorch/tests/test_model.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/models/tensorflow/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      486 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2913 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/actor_critic.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3378 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/autoencoder.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     8692 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/cfrl_models.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/models/tensorflow/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1655 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/tests/test_actor_critic.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      643 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/tests/test_autoencoder.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3708 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/models/tensorflow/tests/test_cfrl_models.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/prototypes/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      250 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/prototypes/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    32709 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/prototypes/protoselect.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/prototypes/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/prototypes/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    11674 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/prototypes/tests/test_protoselect.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3195 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/prototypes/tests/test_utils.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    16214 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/saving.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      622 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/conftest.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     7230 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/test_dep_management.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    18797 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/test_saving.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1033 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/test_utils.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4809 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/tests/utils.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.589403 alibi-0.9.4/alibi/utils/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1276 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4968 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/approximation_methods.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2652 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/data.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3592 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/discretizer.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    12076 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/distance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    31311 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/distributed.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      582 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/distributions.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      513 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/download.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      320 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/frameworks.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2915 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/gradients.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4666 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/kernel.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    15019 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/lang_model.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     4718 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/mapping.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     5365 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/missing_optional_dependency.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.593403 alibi-0.9.4/alibi/utils/tests/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/__init__.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      194 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/mocked_opt_dep.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1014 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_data.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     3193 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_distance.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    15565 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_distributed.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1631 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_gradients.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2855 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_import_optional.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1103 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_mapping.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      398 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tests/test_misc.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      919 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/tf.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    22911 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/visualization.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     1707 2023-07-07 12:43:00.000000 alibi-0.9.4/alibi/utils/wrappers.py
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      212 2023-07-07 12:43:13.000000 alibi-0.9.4/alibi/version.py
+drwxrwxr-x   0 ascillitoe  (1000) ascillitoe  (1000)        0 2023-07-07 13:17:06.581403 alibi-0.9.4/alibi.egg-info/
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)    20876 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/PKG-INFO
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     5394 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        1 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        1 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/not-zip-safe
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)      649 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/requires.txt
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)        6 2023-07-07 13:17:06.000000 alibi-0.9.4/alibi.egg-info/top_level.txt
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2121 2023-07-07 13:17:06.593403 alibi-0.9.4/setup.cfg
+-rw-rw-r--   0 ascillitoe  (1000) ascillitoe  (1000)     2939 2023-07-07 12:43:00.000000 alibi-0.9.4/setup.py
```

### Comparing `alibi-0.9.3/LICENSE` & `alibi-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/PKG-INFO` & `alibi-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.3
+Version: 0.9.4
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: shap
 Provides-Extra: tensorflow
 Provides-Extra: torch
 Provides-Extra: all
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.3 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.4 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-ray Provides-Extra: shap Provides-Extra: tensorflow Provides-Extra: torch
-Provides-Extra: all License-File: LICENSE
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Topic :: Scientific/Engineering Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: ray Provides-Extra: shap Provides-Extra:
+tensorflow Provides-Extra: torch Provides-Extra: all License-File: LICENSE
                                  [Alibi Logo]
  [![Build Status](https://github.com/SeldonIO/alibi-detect/workflows/CI/
 badge.svg?branch=master)][#build-status] [![Documentation Status](https://
 readthedocs.org/projects/alibi/badge/?version=latest)][#docs-package] [!
 [codecov](https://codecov.io/gh/SeldonIO/alibi/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/SeldonIO/alibi) [![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/alibi?logo=pypi&style=flat&color=blue)][#pypi-
```

### Comparing `alibi-0.9.3/README.md` & `alibi-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/api/defaults.py` & `alibi-0.9.4/alibi/api/defaults.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/api/interfaces.py` & `alibi-0.9.4/alibi/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/api/tests/test_interfaces.py` & `alibi-0.9.4/alibi/api/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/confidence/model_linearity.py` & `alibi-0.9.4/alibi/confidence/model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/confidence/tests/test_model_linearity.py` & `alibi-0.9.4/alibi/confidence/tests/test_model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/confidence/tests/test_trustscore.py` & `alibi-0.9.4/alibi/confidence/tests/test_trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/confidence/trustscore.py` & `alibi-0.9.4/alibi/confidence/trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/data/cats.tar.gz` & `alibi-0.9.4/alibi/data/cats.tar.gz`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/datasets/default.py` & `alibi-0.9.4/alibi/datasets/default.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/datasets/tensorflow.py` & `alibi-0.9.4/alibi/datasets/tensorflow.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/datasets/tests/test_datasets.py` & `alibi-0.9.4/alibi/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/exceptions.py` & `alibi-0.9.4/alibi/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/__init__.py` & `alibi-0.9.4/alibi/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/ale.py` & `alibi-0.9.4/alibi/explainers/ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_base.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_explanation.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_explanation.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_image.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_tabular.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_tabular_distributed.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_tabular_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/anchor_text.py` & `alibi-0.9.4/alibi/explainers/anchors/anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/language_model_text_sampler.py` & `alibi-0.9.4/alibi/explainers/anchors/language_model_text_sampler.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/anchors/text_samplers.py` & `alibi-0.9.4/alibi/explainers/anchors/text_samplers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/cfrl_base.py` & `alibi-0.9.4/alibi/explainers/backends/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/cfrl_tabular.py` & `alibi-0.9.4/alibi/explainers/backends/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_base.py` & `alibi-0.9.4/alibi/explainers/backends/pytorch/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/pytorch/cfrl_tabular.py` & `alibi-0.9.4/alibi/explainers/backends/pytorch/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_base.py` & `alibi-0.9.4/alibi/explainers/backends/tensorflow/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/backends/tensorflow/cfrl_tabular.py` & `alibi-0.9.4/alibi/explainers/backends/tensorflow/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/cem.py` & `alibi-0.9.4/alibi/explainers/cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/cfproto.py` & `alibi-0.9.4/alibi/explainers/cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/cfrl_base.py` & `alibi-0.9.4/alibi/explainers/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/cfrl_tabular.py` & `alibi-0.9.4/alibi/explainers/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/counterfactual.py` & `alibi-0.9.4/alibi/explainers/counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/integrated_gradients.py` & `alibi-0.9.4/alibi/explainers/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/partial_dependence.py` & `alibi-0.9.4/alibi/explainers/partial_dependence.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/pd_variance.py` & `alibi-0.9.4/alibi/explainers/pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/permutation_importance.py` & `alibi-0.9.4/alibi/explainers/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/shap_wrappers.py` & `alibi-0.9.4/alibi/explainers/shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/backends/__init__.py` & `alibi-0.9.4/alibi/explainers/similarity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/backends/pytorch/base.py` & `alibi-0.9.4/alibi/explainers/similarity/backends/pytorch/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/backends/tensorflow/base.py` & `alibi-0.9.4/alibi/explainers/similarity/backends/tensorflow/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/base.py` & `alibi-0.9.4/alibi/explainers/similarity/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/grad.py` & `alibi-0.9.4/alibi/explainers/similarity/grad.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/similarity/metrics.py` & `alibi-0.9.4/alibi/explainers/similarity/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/conftest.py` & `alibi-0.9.4/alibi/explainers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_ale.py` & `alibi-0.9.4/alibi/explainers/tests/test_ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_anchor_base.py` & `alibi-0.9.4/alibi/explainers/tests/test_anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_anchor_image.py` & `alibi-0.9.4/alibi/explainers/tests/test_anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_anchor_tabular.py` & `alibi-0.9.4/alibi/explainers/tests/test_anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_anchor_text.py` & `alibi-0.9.4/alibi/explainers/tests/test_anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_cem.py` & `alibi-0.9.4/alibi/explainers/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_cfproto.py` & `alibi-0.9.4/alibi/explainers/tests/test_cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_cfrl.py` & `alibi-0.9.4/alibi/explainers/tests/test_cfrl.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_counterfactual.py` & `alibi-0.9.4/alibi/explainers/tests/test_counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_integrated_gradients.py` & `alibi-0.9.4/alibi/explainers/tests/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_partial_dependence.py` & `alibi-0.9.4/alibi/explainers/tests/test_partial_dependence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import sys
 from copy import deepcopy
 from typing import Dict, List, Optional, Tuple, Union
+from packaging import version
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 from pytest_lazyfixture import lazy_fixture
 from sklearn.base import BaseEstimator
@@ -13,14 +14,15 @@
 from sklearn.ensemble import GradientBoostingClassifier
 from sklearn.exceptions import NotFittedError
 from sklearn.inspection import partial_dependence
 from sklearn.model_selection import train_test_split
 from sklearn.multioutput import MultiOutputClassifier
 from sklearn.pipeline import Pipeline
 from sklearn.utils import Bunch, shuffle
+import sklearn
 
 from alibi.api.defaults import DEFAULT_DATA_PD, DEFAULT_META_PD
 from alibi.api.interfaces import Explanation
 from alibi.explainers import PartialDependence, TreePartialDependence, plot_pd
 from alibi.explainers.partial_dependence import (_plot_one_pd_cat,
                                                  _plot_one_pd_num,
                                                  _plot_two_pd_cat_cat,
@@ -383,27 +385,36 @@
 @pytest.mark.parametrize('features', [
     [1], [2], [4], [5],
     [(1, 2)], [(2, 4)], [(4, 5)]
 ])
 @pytest.mark.parametrize('params', [
     {
         'percentiles': (0, 1),
-        'grid_resolution': np.inf,
         'method': 'brute',
         'kind': 'average'
     }
 ])
 def test_sklearn_categorical(rf_classifier, adult_data, features, params):
     """ Checks `alibi` pd black-box implementation against the `sklearn` implementation for categorical features."""
+
     rf, preprocessor = rf_classifier
     rf_pipeline = Pipeline(steps=[('preprocessor', preprocessor), ('predictor', rf)])
 
     # subsample data for faster computation
     X_train = adult_data['X_train'][:100]
 
+    # Behaviour depends on sklearn version, See https://github.com/SeldonIO/alibi/pull/940#issuecomment-1623783025
+    sklearn_version = version.parse(sklearn.__version__)
+    if sklearn_version >= version.parse('1.3.0'):
+        categorical_names = adult_data['metadata']['category_map']
+        categorical_names = list(categorical_names.keys())
+        params.update(categorical_features=categorical_names)
+    else:
+        params.update(grid_resolution=np.inf)
+
     # compute `sklearn` explanation
     exp_sklearn = partial_dependence(X=X_train,
                                      estimator=rf_pipeline,
                                      features=features,
                                      **params)
 
     # update intentionally grid_resolution to check that alibi behaves correctly for categorical features
@@ -428,15 +439,15 @@
 @pytest.mark.parametrize('features', [
     [1], [2], [4], [5],
     [(1, 2)], [(2, 4)], [(4, 5)]
 ])
 @pytest.mark.parametrize('params', [
     {
         'percentiles': (0, 1),
-        'grid_resolution': np.inf,
+        'grid_resolution': 30,
         'method': 'recursion',
         'kind': 'average'
     }
 ])
 def test_sklearn_recursion(predictor, binary_data, features, params):
     """ Check `alibi` pd recursion implementation against the `sklearn` implementation. """
     X_train, y_train = binary_data['X_train'], binary_data['y_train']
```

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_pd_variance.py` & `alibi-0.9.4/alibi/explainers/tests/test_pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_permutation_importance.py` & `alibi-0.9.4/alibi/explainers/tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_shap_wrappers.py` & `alibi-0.9.4/alibi/explainers/tests/test_shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/conftest.py` & `alibi-0.9.4/alibi/explainers/tests/test_simiarlity/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_backends.py` & `alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_backends.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py` & `alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py` & `alibi-0.9.4/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/explainers/tests/utils.py` & `alibi-0.9.4/alibi/explainers/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/actor_critic.py` & `alibi-0.9.4/alibi/models/pytorch/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/autoencoder.py` & `alibi-0.9.4/alibi/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/cfrl_models.py` & `alibi-0.9.4/alibi/models/pytorch/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/metrics.py` & `alibi-0.9.4/alibi/models/pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/model.py` & `alibi-0.9.4/alibi/models/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/tests/test_actor_critic.py` & `alibi-0.9.4/alibi/models/pytorch/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/tests/test_autoencoder.py` & `alibi-0.9.4/alibi/models/pytorch/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/tests/test_cfrl_models.py` & `alibi-0.9.4/alibi/models/pytorch/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/tests/test_metrics.py` & `alibi-0.9.4/alibi/models/pytorch/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/pytorch/tests/test_model.py` & `alibi-0.9.4/alibi/models/pytorch/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/actor_critic.py` & `alibi-0.9.4/alibi/models/tensorflow/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/autoencoder.py` & `alibi-0.9.4/alibi/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/cfrl_models.py` & `alibi-0.9.4/alibi/models/tensorflow/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/tests/test_actor_critic.py` & `alibi-0.9.4/alibi/models/tensorflow/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/tests/test_autoencoder.py` & `alibi-0.9.4/alibi/models/tensorflow/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/models/tensorflow/tests/test_cfrl_models.py` & `alibi-0.9.4/alibi/models/tensorflow/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/prototypes/protoselect.py` & `alibi-0.9.4/alibi/prototypes/protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/prototypes/tests/test_protoselect.py` & `alibi-0.9.4/alibi/prototypes/tests/test_protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/prototypes/tests/test_utils.py` & `alibi-0.9.4/alibi/prototypes/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/saving.py` & `alibi-0.9.4/alibi/saving.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/tests/conftest.py` & `alibi-0.9.4/alibi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/tests/test_dep_management.py` & `alibi-0.9.4/alibi/tests/test_dep_management.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/tests/test_saving.py` & `alibi-0.9.4/alibi/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/tests/test_utils.py` & `alibi-0.9.4/alibi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/tests/utils.py` & `alibi-0.9.4/alibi/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/__init__.py` & `alibi-0.9.4/alibi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/approximation_methods.py` & `alibi-0.9.4/alibi/utils/approximation_methods.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/data.py` & `alibi-0.9.4/alibi/utils/data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/discretizer.py` & `alibi-0.9.4/alibi/utils/discretizer.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/distance.py` & `alibi-0.9.4/alibi/utils/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/distributed.py` & `alibi-0.9.4/alibi/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/distributions.py` & `alibi-0.9.4/alibi/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/download.py` & `alibi-0.9.4/alibi/utils/download.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/gradients.py` & `alibi-0.9.4/alibi/utils/gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/kernel.py` & `alibi-0.9.4/alibi/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/lang_model.py` & `alibi-0.9.4/alibi/utils/lang_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/mapping.py` & `alibi-0.9.4/alibi/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/missing_optional_dependency.py` & `alibi-0.9.4/alibi/utils/missing_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_data.py` & `alibi-0.9.4/alibi/utils/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_distance.py` & `alibi-0.9.4/alibi/utils/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_distributed.py` & `alibi-0.9.4/alibi/utils/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_gradients.py` & `alibi-0.9.4/alibi/utils/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_import_optional.py` & `alibi-0.9.4/alibi/utils/tests/test_import_optional.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tests/test_mapping.py` & `alibi-0.9.4/alibi/utils/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/tf.py` & `alibi-0.9.4/alibi/utils/tf.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/visualization.py` & `alibi-0.9.4/alibi/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi/utils/wrappers.py` & `alibi-0.9.4/alibi/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi.egg-info/PKG-INFO` & `alibi-0.9.4/alibi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.3
+Version: 0.9.4
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: shap
 Provides-Extra: tensorflow
 Provides-Extra: torch
 Provides-Extra: all
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: alibi Version: 0.9.3 Summary: Algorithms for
+Metadata-Version: 2.1 Name: alibi Version: 0.9.4 Summary: Algorithms for
 monitoring and explaining machine learning models Home-page: https://
 github.com/SeldonIO/alibi Author: Seldon Technologies Ltd. Author-email:
 hello@seldon.io License: Apache 2.0 Classifier: Intended Audience :: Science/
 Research Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-ray Provides-Extra: shap Provides-Extra: tensorflow Provides-Extra: torch
-Provides-Extra: all License-File: LICENSE
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Topic :: Scientific/Engineering Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: ray Provides-Extra: shap Provides-Extra:
+tensorflow Provides-Extra: torch Provides-Extra: all License-File: LICENSE
                                  [Alibi Logo]
  [![Build Status](https://github.com/SeldonIO/alibi-detect/workflows/CI/
 badge.svg?branch=master)][#build-status] [![Documentation Status](https://
 readthedocs.org/projects/alibi/badge/?version=latest)][#docs-package] [!
 [codecov](https://codecov.io/gh/SeldonIO/alibi/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/SeldonIO/alibi) [![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/alibi?logo=pypi&style=flat&color=blue)][#pypi-
```

### Comparing `alibi-0.9.3/alibi.egg-info/SOURCES.txt` & `alibi-0.9.4/alibi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/alibi.egg-info/requires.txt` & `alibi-0.9.4/alibi.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 typing-extensions>=3.7.4.3
 dill<0.4.0,>=0.3.0
 transformers<5.0.0,>=4.7.0
 tqdm<5.0.0,>=4.28.1
 
 [all]
 ray<3.0.0,>=0.8.7
-shap<0.42.0,>=0.40.0
+shap<0.43.0,>=0.40.0
 numba!=0.54.0,<0.58.0,>=0.50.0
 tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
 torch<3.0.0,>=1.9.0
 
 [ray]
 ray<3.0.0,>=0.8.7
 
 [shap]
-shap<0.42.0,>=0.40.0
+shap<0.43.0,>=0.40.0
 numba!=0.54.0,<0.58.0,>=0.50.0
 
 [tensorflow]
 tensorflow!=2.6.0,!=2.6.1,<2.13.0,>=2.0.0
 
 [torch]
 torch<2.0.0,>=1.9.0
```

### Comparing `alibi-0.9.3/setup.cfg` & `alibi-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `alibi-0.9.3/setup.py` & `alibi-0.9.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # read version file
 exec(open('alibi/version.py').read())
 
 extras_require = {
     'ray': ['ray>=0.8.7, <3.0.0'],
     # shap is separated due to build issues, see https://github.com/slundberg/shap/pull/1802
     'shap': [
-        'shap>=0.40.0, <0.42.0',  # versioning: https://github.com/SeldonIO/alibi/issues/333
+        'shap>=0.40.0, <0.43.0',  # versioning: https://github.com/SeldonIO/alibi/issues/333
         'numba>=0.50.0, !=0.54.0, <0.58.0',  # Avoid 0.54 due to: https://github.com/SeldonIO/alibi/issues/466
     ],
 
     'tensorflow': ['tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0'],
     'torch': ['torch>=1.9.0, <2.0.0'],
     'all': [
         'ray>=0.8.7, <3.0.0',
-        'shap>=0.40.0, <0.42.0',
+        'shap>=0.40.0, <0.43.0',
         'numba>=0.50.0, !=0.54.0, <0.58.0',
         'tensorflow>=2.0.0, !=2.6.0, !=2.6.1, <2.13.0',
         'torch>=1.9.0, <3.0.0'
     ]
 }
 
 if __name__ == '__main__':
@@ -36,15 +36,15 @@
           description='Algorithms for monitoring and explaining machine learning models',
           long_description=readme(),
           long_description_content_type='text/markdown',
           url='https://github.com/SeldonIO/alibi',
           license="Apache 2.0",
           packages=find_packages(),
           include_package_data=True,
-          python_requires='>=3.7',
+          python_requires='>=3.8',
           # lower bounds based on Debian Stable versions where available
           install_requires=[
               'numpy>=1.16.2, <2.0.0',
               'pandas>=1.0.0, <3.0.0',
               'scikit-learn>=1.0.0, <2.0.0',
               'spacy[lookups]>=2.0.0, <4.0.0',
               'blis<0.8.0',  # Windows memory issues https://github.com/explosion/thinc/issues/771
@@ -62,15 +62,14 @@
           extras_require=extras_require,
           test_suite='tests',
           zip_safe=False,
           classifiers=[
               "Intended Audience :: Science/Research",
               "Operating System :: OS Independent",
               "Programming Language :: Python :: 3",
-              "Programming Language :: Python :: 3.7",
               "Programming Language :: Python :: 3.8",
               "Programming Language :: Python :: 3.9",
               "Programming Language :: Python :: 3.10",
               "Programming Language :: Python :: 3.11",
               "License :: OSI Approved :: Apache Software License",
               "Topic :: Scientific/Engineering",
           ])
```

