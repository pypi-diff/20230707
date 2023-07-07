# Comparing `tmp/alibi-detect-0.9.1.tar.gz` & `tmp/alibi-detect-0.9.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibi-detect-0.9.1.tar", last modified: Fri Apr  1 13:37:41 2022, max compression
+gzip compressed data, was "alibi-detect-0.9.1.dev0.tar", last modified: Fri Apr  1 12:43:09 2022, max compression
```

## Comparing `alibi-detect-0.9.1.tar` & `alibi-detect-0.9.1.dev0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.755849 alibi-detect-0.9.1/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    30049 2022-04-01 13:37:41.755849 alibi-detect-0.9.1/PKG-INFO
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    26029 2022-04-01 12:38:22.000000 alibi-detect-0.9.1/README.md
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.723849 alibi-detect-0.9.1/alibi_detect/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      135 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/__init__.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.727849 alibi-detect-0.9.1/alibi_detect/ad/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      151 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/ad/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    13233 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/ad/adversarialae.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7811 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/ad/model_distillation.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2900 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/base.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.731849 alibi-detect-0.9.1/alibi_detect/cd/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1007 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3611 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/_domain_clf.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    47560 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/base.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    13939 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/base_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6343 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/chisquare.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10376 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/classifier.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6691 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/context_aware.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3766 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/cvm.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    13155 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/cvm_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4988 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/fet.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    14198 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/fet_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3632 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/ks.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7399 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/learned_kernel.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5548 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/lsdd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6146 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/lsdd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5503 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/mmd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5884 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/mmd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    12522 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/model_uncertainty.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3470 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/preprocess.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.735849 alibi-detect-0.9.1/alibi_detect/cd/pytorch/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      113 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9307 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/classifier.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    12485 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/context_aware.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    11085 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/learned_kernel.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8125 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/lsdd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10117 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/lsdd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6066 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/mmd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9495 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/mmd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2399 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/preprocess.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10386 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/spot_the_diff.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      444 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/pytorch/utils.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.739849 alibi-detect-0.9.1/alibi_detect/cd/sklearn/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/sklearn/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    11391 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/sklearn/classifier.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8593 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/spot_the_diff.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7317 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tabular.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.743849 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      129 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8367 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/classifier.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    12895 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/context_aware.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9962 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/learned_kernel.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6882 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/lsdd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9224 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/lsdd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5120 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/mmd.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8959 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/mmd_online.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4509 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/preprocess.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10088 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/spot_the_diff.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      272 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/tensorflow/utils.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4302 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/cd/utils.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    18427 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/datasets.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.743849 alibi-detect-0.9.1/alibi_detect/models/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/__init__.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.743849 alibi-detect-0.9.1/alibi_detect/models/pytorch/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      130 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/pytorch/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2138 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/pytorch/embedding.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1982 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/pytorch/trainer.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.743849 alibi-detect-0.9.1/alibi_detect/models/tensorflow/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      338 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    14713 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/autoencoder.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3720 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/embedding.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3268 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/gmm.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7346 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/losses.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    47591 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/pixelcnn.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    15500 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/resnet.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4184 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/models/tensorflow/trainer.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.747849 alibi-detect-0.9.1/alibi_detect/od/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      577 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9232 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/ae.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     7665 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/aegmm.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4948 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/isolationforest.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    13732 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/llr.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    14246 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/mahalanobis.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8526 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/prophet.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    13431 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/seq2seq.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    15746 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/sr.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    11280 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/vae.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9580 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/od/vaegmm.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.751849 alibi-detect-0.9.1/alibi_detect/utils/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      230 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/_types.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1920 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/data.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2735 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/discretizer.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    10260 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/distance.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    16649 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/fetching.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      312 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/frameworks.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4692 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/mapping.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      317 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/metrics.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1556 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/misc.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    31912 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/perturbation.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      593 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/prediction.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.751849 alibi-detect-0.9.1/alibi_detect/utils/pytorch/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      560 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      547 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/data.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     8813 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/distance.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     5628 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/kernels.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1556 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/misc.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     4639 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/pytorch/prediction.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1126 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/sampling.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    60731 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/saving.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2312 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/statstest.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.755849 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      660 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/__init__.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     1105 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/data.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     9211 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/distance.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     6398 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/kernels.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2661 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/misc.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3426 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/tensorflow/prediction.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    11826 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/alibi_detect/utils/visualize.py
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      212 2022-04-01 13:36:12.000000 alibi-detect-0.9.1/alibi_detect/version.py
-drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 13:37:41.727849 alibi-detect-0.9.1/alibi_detect.egg-info/
--rw-rw-r--   0 oliver    (1000) oliver    (1000)    30049 2022-04-01 13:37:41.000000 alibi-detect-0.9.1/alibi_detect.egg-info/PKG-INFO
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     3735 2022-04-01 13:37:41.000000 alibi-detect-0.9.1/alibi_detect.egg-info/SOURCES.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2022-04-01 13:37:41.000000 alibi-detect-0.9.1/alibi_detect.egg-info/dependency_links.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2022-04-01 12:43:09.000000 alibi-detect-0.9.1/alibi_detect.egg-info/not-zip-safe
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      483 2022-04-01 13:37:41.000000 alibi-detect-0.9.1/alibi_detect.egg-info/requires.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)       13 2022-04-01 13:37:41.000000 alibi-detect-0.9.1/alibi_detect.egg-info/top_level.txt
--rw-rw-r--   0 oliver    (1000) oliver    (1000)      937 2022-04-01 13:37:41.755849 alibi-detect-0.9.1/setup.cfg
--rw-rw-r--   0 oliver    (1000) oliver    (1000)     2171 2022-04-01 12:28:52.000000 alibi-detect-0.9.1/setup.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.893611 alibi-detect-0.9.1.dev0/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    30054 2022-04-01 12:43:09.893611 alibi-detect-0.9.1.dev0/PKG-INFO
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    26029 2022-04-01 12:38:22.000000 alibi-detect-0.9.1.dev0/README.md
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.845611 alibi-detect-0.9.1.dev0/alibi_detect/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      135 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/__init__.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.849611 alibi-detect-0.9.1.dev0/alibi_detect/ad/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      151 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/ad/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    13233 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/ad/adversarialae.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7811 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/ad/model_distillation.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2900 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/base.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.861611 alibi-detect-0.9.1.dev0/alibi_detect/cd/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1007 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3611 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/_domain_clf.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    47560 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/base.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    13939 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/base_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6343 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/chisquare.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10376 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/classifier.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6691 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/context_aware.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3766 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/cvm.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    13155 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/cvm_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4988 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/fet.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    14198 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/fet_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3632 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/ks.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7399 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/learned_kernel.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5548 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/lsdd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6146 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/lsdd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5503 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/mmd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5884 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/mmd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    12522 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/model_uncertainty.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3470 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/preprocess.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.865611 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      113 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9307 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/classifier.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    12485 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/context_aware.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    11085 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/learned_kernel.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8125 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/lsdd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10117 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/lsdd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6066 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/mmd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9495 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/mmd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2399 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/preprocess.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10386 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/spot_the_diff.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      444 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/utils.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.865611 alibi-detect-0.9.1.dev0/alibi_detect/cd/sklearn/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/sklearn/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    11391 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/sklearn/classifier.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8593 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/spot_the_diff.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7317 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tabular.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.869611 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      129 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8367 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/classifier.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    12895 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/context_aware.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9962 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/learned_kernel.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6882 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/lsdd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9224 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/lsdd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5120 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/mmd.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8959 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/mmd_online.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4509 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/preprocess.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10088 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/spot_the_diff.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      272 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/utils.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4302 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/cd/utils.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    18427 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/datasets.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.869611 alibi-detect-0.9.1.dev0/alibi_detect/models/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/__init__.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.869611 alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      130 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2138 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/embedding.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1982 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/trainer.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.873611 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      338 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    14713 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/autoencoder.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3720 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/embedding.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3268 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/gmm.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7346 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/losses.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    47591 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/pixelcnn.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    15500 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/resnet.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4184 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/trainer.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.877611 alibi-detect-0.9.1.dev0/alibi_detect/od/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      577 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9232 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/ae.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     7665 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/aegmm.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4948 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/isolationforest.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    13732 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/llr.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    14246 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/mahalanobis.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8526 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/prophet.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    13431 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/seq2seq.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    15746 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/sr.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    11280 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/vae.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9580 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/od/vaegmm.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.881611 alibi-detect-0.9.1.dev0/alibi_detect/utils/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      230 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/_types.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1920 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/data.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2735 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/discretizer.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    10260 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/distance.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    16649 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/fetching.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      312 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/frameworks.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4692 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/mapping.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      317 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/metrics.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1556 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/misc.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    31912 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/perturbation.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      593 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/prediction.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.885611 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      560 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      547 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/data.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     8813 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/distance.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     5628 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/kernels.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1556 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/misc.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     4639 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/prediction.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1126 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/sampling.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    60731 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/saving.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2312 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/statstest.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.893611 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      660 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/__init__.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     1105 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/data.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     9211 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/distance.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     6398 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/kernels.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2661 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/misc.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3426 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/prediction.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    11826 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/utils/visualize.py
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      215 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/alibi_detect/version.py
+drwxrwxr-x   0 oliver    (1000) oliver    (1000)        0 2022-04-01 12:43:09.849611 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)    30054 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/PKG-INFO
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     3735 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/SOURCES.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/dependency_links.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)        1 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/not-zip-safe
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      483 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/requires.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)       13 2022-04-01 12:43:09.000000 alibi-detect-0.9.1.dev0/alibi_detect.egg-info/top_level.txt
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)      937 2022-04-01 12:43:09.893611 alibi-detect-0.9.1.dev0/setup.cfg
+-rw-rw-r--   0 oliver    (1000) oliver    (1000)     2171 2022-04-01 12:28:52.000000 alibi-detect-0.9.1.dev0/setup.py
```

### Comparing `alibi-detect-0.9.1/PKG-INFO` & `alibi-detect-0.9.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi-detect
-Version: 0.9.1
+Version: 0.9.1.dev0
 Summary: Algorithms for outlier detection, concept drift and metrics.
 Home-page: https://github.com/SeldonIO/alibi-detect
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: <p align="center">
           <img src="https://raw.githubusercontent.com/SeldonIO/alibi-detect/master/doc/source/_static/Alibi_Detect_Logo_rgb.png" alt="Alibi Detect Logo" width="50%">
```

### Comparing `alibi-detect-0.9.1/README.md` & `alibi-detect-0.9.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/ad/adversarialae.py` & `alibi-detect-0.9.1.dev0/alibi_detect/ad/adversarialae.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/ad/model_distillation.py` & `alibi-detect-0.9.1.dev0/alibi_detect/ad/model_distillation.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/base.py` & `alibi-detect-0.9.1.dev0/alibi_detect/base.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/__init__.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/_domain_clf.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/_domain_clf.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/base.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/base.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/base_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/base_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/chisquare.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/chisquare.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/classifier.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/classifier.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/context_aware.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/context_aware.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/cvm.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/cvm.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/cvm_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/cvm_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/fet.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/fet.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/fet_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/fet_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/ks.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/ks.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/learned_kernel.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/learned_kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/lsdd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/lsdd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/lsdd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/lsdd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/mmd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/mmd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/mmd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/mmd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/model_uncertainty.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/preprocess.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/preprocess.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/classifier.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/classifier.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/context_aware.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/context_aware.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/learned_kernel.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/learned_kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/lsdd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/lsdd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/lsdd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/lsdd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/mmd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/mmd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/mmd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/mmd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/preprocess.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/preprocess.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/pytorch/spot_the_diff.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/pytorch/spot_the_diff.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/sklearn/classifier.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/sklearn/classifier.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/spot_the_diff.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/spot_the_diff.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tabular.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/classifier.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/classifier.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/context_aware.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/context_aware.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/learned_kernel.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/learned_kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/lsdd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/lsdd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/lsdd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/lsdd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/mmd.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/mmd.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/mmd_online.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/mmd_online.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/preprocess.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/preprocess.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/tensorflow/spot_the_diff.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/tensorflow/spot_the_diff.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/cd/utils.py` & `alibi-detect-0.9.1.dev0/alibi_detect/cd/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/datasets.py` & `alibi-detect-0.9.1.dev0/alibi_detect/datasets.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/pytorch/embedding.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/embedding.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/pytorch/trainer.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/autoencoder.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/embedding.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/embedding.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/gmm.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/gmm.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/losses.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/losses.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/pixelcnn.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/pixelcnn.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/resnet.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/resnet.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/models/tensorflow/trainer.py` & `alibi-detect-0.9.1.dev0/alibi_detect/models/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/__init__.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/ae.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/ae.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/aegmm.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/aegmm.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/isolationforest.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/isolationforest.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/llr.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/llr.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/mahalanobis.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/mahalanobis.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/prophet.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/prophet.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/seq2seq.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/seq2seq.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/sr.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/sr.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/vae.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/vae.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/od/vaegmm.py` & `alibi-detect-0.9.1.dev0/alibi_detect/od/vaegmm.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/data.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/data.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/discretizer.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/discretizer.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/distance.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/fetching.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/fetching.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/mapping.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/misc.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/misc.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/perturbation.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/perturbation.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/prediction.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/__init__.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/data.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/data.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/distance.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/kernels.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/kernels.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/misc.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/misc.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/pytorch/prediction.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/pytorch/prediction.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/sampling.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/saving.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/saving.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/statstest.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/statstest.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/__init__.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/data.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/data.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/distance.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/kernels.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/kernels.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/misc.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/misc.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/tensorflow/prediction.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/tensorflow/prediction.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect/utils/visualize.py` & `alibi-detect-0.9.1.dev0/alibi_detect/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/alibi_detect.egg-info/PKG-INFO` & `alibi-detect-0.9.1.dev0/alibi_detect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi-detect
-Version: 0.9.1
+Version: 0.9.1.dev0
 Summary: Algorithms for outlier detection, concept drift and metrics.
 Home-page: https://github.com/SeldonIO/alibi-detect
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: <p align="center">
           <img src="https://raw.githubusercontent.com/SeldonIO/alibi-detect/master/doc/source/_static/Alibi_Detect_Logo_rgb.png" alt="Alibi Detect Logo" width="50%">
```

### Comparing `alibi-detect-0.9.1/alibi_detect.egg-info/SOURCES.txt` & `alibi-detect-0.9.1.dev0/alibi_detect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/setup.cfg` & `alibi-detect-0.9.1.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `alibi-detect-0.9.1/setup.py` & `alibi-detect-0.9.1.dev0/setup.py`

 * *Files identical despite different names*

