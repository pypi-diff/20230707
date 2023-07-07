# Comparing `tmp/optimum-habana-1.6.0.tar.gz` & `tmp/optimum-habana-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-habana-1.6.0.tar", last modified: Mon Jun 26 08:33:39 2023, max compression
+gzip compressed data, was "optimum-habana-1.6.1.tar", last modified: Fri Jul  7 07:42:47 2023, max compression
```

## Comparing `optimum-habana-1.6.0.tar` & `optimum-habana-1.6.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11555 2023-06-18 22:07:26.000000 optimum-habana-1.6.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.481526 optimum-habana-1.6.0/optimum/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1040 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15117 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/pipeline_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41120 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/distributed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/distributed/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/distributed/distributed_runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6103 2023-06-22 14:31:34.000000 optimum-habana-1.6.0/optimum/habana/distributed/fast_ddp.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8387 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/deepspeed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/gaudi_configuration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/generation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/generation/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   118439 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/generation/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-06-18 17:50:35.000000 optimum-habana-1.6.0/optimum/habana/transformers/gradient_checkpointing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8063 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/modeling_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/modeling_albert.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24977 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/modeling_bloom.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      470 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/modeling_esm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15054 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/modeling_esmfold.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28275 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15756 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18811 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/modeling_gptj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/modeling_all_models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21921 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/modeling_opt.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7784 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/modeling_t5.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    92734 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17150 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29336 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/training_args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4267 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/training_args_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9955 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-06-26 08:12:18.000000 optimum-habana-1.6.0/optimum/habana/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum_habana.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2808 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 08:33:27.000000 optimum-habana-1.6.0/optimum_habana.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2967 2023-06-26 08:12:31.000000 optimum-habana-1.6.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21789 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/tests/test_diffusers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18420 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_examples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/tests/test_examples_match_transformers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2843 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_gaudi_configuration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    86178 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5804 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer_distributed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4743 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer_seq2seq.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11555 2023-07-07 07:34:39.000000 optimum-habana-1.6.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.575111 optimum-habana-1.6.1/optimum/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1040 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/diffusers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/diffusers/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15393 2023-07-07 07:34:54.000000 optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/pipeline_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    44513 2023-07-07 07:34:54.000000 optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/diffusers/schedulers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15498 2023-07-07 07:34:54.000000 optimum-habana-1.6.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/distributed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/distributed/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/distributed/distributed_runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6103 2023-07-07 07:34:39.000000 optimum-habana-1.6.1/optimum/habana/distributed/fast_ddp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8387 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/transformers/deepspeed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/transformers/gaudi_configuration.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/transformers/generation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/generation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   118439 2023-07-07 07:34:39.000000 optimum-habana-1.6.1/optimum/habana/transformers/generation/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-06-18 17:50:35.000000 optimum-habana-1.6.1/optimum/habana/transformers/gradient_checkpointing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8063 2023-07-07 07:31:27.000000 optimum-habana-1.6.1/optimum/habana/transformers/modeling_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/transformers/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.579111 optimum-habana-1.6.1/optimum/habana/transformers/models/albert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/albert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-07-06 19:01:50.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/albert/modeling_albert.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/bloom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24977 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/bloom/modeling_bloom.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/esm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/esm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      470 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/esm/modeling_esm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15054 2023-06-06 13:54:31.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/esm/modeling_esmfold.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-06 13:54:31.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28275 2023-06-06 13:54:31.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt_neox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-16 12:51:49.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt_neox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15756 2023-06-16 12:51:49.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/gptj/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-06-16 12:51:49.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gptj/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18811 2023-06-16 12:51:49.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/gptj/modeling_gptj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-07-06 19:01:50.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/modeling_all_models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/opt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-06-30 17:47:16.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/opt/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21921 2023-07-07 07:31:27.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/opt/modeling_opt.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/t5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/t5/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7784 2023-06-26 14:37:06.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/t5/modeling_t5.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/vit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/vit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum/habana/transformers/models/wav2vec2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    92734 2023-07-07 07:34:39.000000 optimum-habana-1.6.1/optimum/habana/transformers/trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17150 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/trainer_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29336 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/transformers/training_args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4267 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/optimum/habana/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9955 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/optimum/habana/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-07-07 07:36:18.000000 optimum-habana-1.6.1/optimum/habana/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/optimum_habana.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-07-07 07:42:47.000000 optimum-habana-1.6.1/optimum_habana.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2808 2023-07-07 07:42:47.000000 optimum-habana-1.6.1/optimum_habana.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-07 07:42:47.000000 optimum-habana-1.6.1/optimum_habana.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-07 07:42:39.000000 optimum-habana-1.6.1/optimum_habana.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-07-07 07:42:47.000000 optimum-habana-1.6.1/optimum_habana.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-07 07:42:47.000000 optimum-habana-1.6.1/optimum_habana.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2967 2023-07-07 07:34:54.000000 optimum-habana-1.6.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-07 07:42:47.583111 optimum-habana-1.6.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21789 2023-07-06 23:18:07.000000 optimum-habana-1.6.1/tests/test_diffusers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18420 2023-07-06 19:01:50.000000 optimum-habana-1.6.1/tests/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-06-01 21:37:59.000000 optimum-habana-1.6.1/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2843 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/tests/test_gaudi_configuration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    86178 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/tests/test_trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5804 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/tests/test_trainer_distributed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4743 2023-06-18 14:54:24.000000 optimum-habana-1.6.1/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-habana-1.6.0/LICENSE` & `optimum-habana-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/MANIFEST.in` & `optimum-habana-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/PKG-INFO` & `optimum-habana-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.6.0
+Version: 1.6.1
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-habana-1.6.0/README.md` & `optimum-habana-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/__init__.py` & `optimum-habana-1.6.1/optimum/habana/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/pipeline_utils.py` & `optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/pipeline_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,35 +184,41 @@
         from diffusers import pipelines
 
         for name, module in kwargs.items():
             # retrieve library
             if module is None:
                 register_dict = {name: (None, None)}
             else:
-                # register the original module, not the dynamo compiled one
+                # register the config from the original module, not the dynamo compiled one
                 if is_compiled_module(module):
-                    module = module._orig_mod
+                    not_compiled_module = module._orig_mod
+                else:
+                    not_compiled_module = module
 
-                library = module.__module__.split(".")[0]
+                library = not_compiled_module.__module__.split(".")[0]
                 if library == "optimum":
                     library = "optimum.habana.diffusers.schedulers"
 
                 # check if the module is a pipeline module
-                pipeline_dir = module.__module__.split(".")[-2] if len(module.__module__.split(".")) > 2 else None
-                path = module.__module__.split(".")
+                module_path_items = not_compiled_module.__module__.split(".")
+                pipeline_dir = module_path_items[-2] if len(module_path_items) > 2 else None
+
+                path = not_compiled_module.__module__.split(".")
                 is_pipeline_module = pipeline_dir in path and hasattr(pipelines, pipeline_dir)
 
                 # if library is not in GAUDI_LOADABLE_CLASSES, then it is a custom module.
                 # Or if it's a pipeline module, then the module is inside the pipeline
                 # folder so we set the library to module name.
-                if library not in GAUDI_LOADABLE_CLASSES or is_pipeline_module:
+                if is_pipeline_module:
                     library = pipeline_dir
+                elif library not in GAUDI_LOADABLE_CLASSES:
+                    library = not_compiled_module.__module__
 
                 # retrieve class_name
-                class_name = module.__class__.__name__
+                class_name = not_compiled_module.__class__.__name__
 
                 register_dict = {name: (library, class_name)}
 
             # save model index config
             self.register_to_config(**register_dict)
 
             # set models
```

### Comparing `optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-habana-1.6.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 import time
+import warnings
 from dataclasses import dataclass
 from math import ceil
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
 from diffusers.configuration_utils import FrozenDict
-from diffusers.loaders import FromCkptMixin, LoraLoaderMixin, TextualInversionLoaderMixin
+from diffusers.image_processor import VaeImageProcessor
+from diffusers.loaders import FromSingleFileMixin, LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 from diffusers.schedulers import KarrasDiffusionSchedulers
 from diffusers.utils import BaseOutput, deprecate
 from packaging import version
 from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
@@ -44,16 +46,30 @@
 @dataclass
 class GaudiStableDiffusionPipelineOutput(BaseOutput):
     images: Union[List[PIL.Image.Image], np.ndarray]
     nsfw_content_detected: Optional[List[bool]]
     throughput: float
 
 
+def rescale_noise_cfg(noise_cfg, noise_pred_text, guidance_rescale=0.0):
+    """
+    Rescale `noise_cfg` according to `guidance_rescale`. Based on findings of [Common Diffusion Noise Schedules and
+    Sample Steps are Flawed](https://arxiv.org/pdf/2305.08891.pdf). See Section 3.4
+    """
+    std_text = noise_pred_text.std(dim=list(range(1, noise_pred_text.ndim)), keepdim=True)
+    std_cfg = noise_cfg.std(dim=list(range(1, noise_cfg.ndim)), keepdim=True)
+    # rescale the results from guidance (fixes overexposure)
+    noise_pred_rescaled = noise_cfg * (std_text / std_cfg)
+    # mix with the original results from guidance by factor guidance_rescale to avoid "plain looking" images
+    noise_cfg = guidance_rescale * noise_pred_rescaled + (1 - guidance_rescale) * noise_cfg
+    return noise_cfg
+
+
 class GaudiStableDiffusionPipeline(
-    GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromCkptMixin
+    GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromSingleFileMixin
 ):
     """
     Extends the [`StableDiffusionPipeline`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion#diffusers.StableDiffusionPipeline) class:
     - Generation is performed by batches
     - Two `mark_step()` were added to add support for lazy mode
     - Added support for HPU graphs
 
@@ -182,14 +198,15 @@
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.image_processor = VaeImageProcessor(vae_scale_factor=self.vae_scale_factor)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
 
         self.to(self._device)
 
     @property
     def _execution_device(self):
         r"""
@@ -213,14 +230,15 @@
         prompt,
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
+        lora_scale: Optional[float] = None,
     ):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 prompt to be encoded
@@ -237,15 +255,22 @@
             prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
                 provided, text embeddings will be generated from `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
                 weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
                 argument.
+            lora_scale (`float`, *optional*):
+                A lora scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
         """
+        # set lora scale so that monkey patched LoRA
+        # function of text encoder can correctly access it
+        if lora_scale is not None and isinstance(self, LoraLoaderMixin):
+            self._lora_scale = lora_scale
+
         if prompt is not None and isinstance(prompt, str):
             num_prompts = 1
         elif prompt is not None and isinstance(prompt, list):
             num_prompts = len(prompt)
         else:
             num_prompts = prompt_embeds.shape[0]
 
@@ -294,15 +319,15 @@
         prompt_embeds = prompt_embeds.view(bs_embed * num_images_per_prompt, seq_len, -1)
 
         # get unconditional embeddings for classifier free guidance
         if do_classifier_free_guidance and negative_prompt_embeds is None:
             uncond_tokens: List[str]
             if negative_prompt is None:
                 uncond_tokens = [""] * num_prompts
-            elif type(prompt) is not type(negative_prompt):
+            elif prompt is not None and type(prompt) is not type(negative_prompt):
                 raise TypeError(
                     f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
                     f" {type(prompt)}."
                 )
             elif isinstance(negative_prompt, str):
                 uncond_tokens = [negative_prompt]
             elif num_prompts != len(negative_prompt):
@@ -346,26 +371,35 @@
 
             negative_prompt_embeds = negative_prompt_embeds.repeat(1, num_images_per_prompt, 1)
             negative_prompt_embeds = negative_prompt_embeds.view(num_prompts * num_images_per_prompt, seq_len, -1)
 
         return prompt_embeds, negative_prompt_embeds
 
     def run_safety_checker(self, image, device, dtype):
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(device)
+        if self.safety_checker is None:
+            has_nsfw_concept = None
+        else:
+            if torch.is_tensor(image):
+                feature_extractor_input = self.image_processor.postprocess(image, output_type="pil")
+            else:
+                feature_extractor_input = self.image_processor.numpy_to_pil(image)
+            safety_checker_input = self.feature_extractor(feature_extractor_input, return_tensors="pt").to(device)
             image, has_nsfw_concept = self.safety_checker(
                 images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
             )
-        else:
-            has_nsfw_concept = None
         return image, has_nsfw_concept
 
     def decode_latents(self, latents):
+        warnings.warn(
+            "The decode_latents method is deprecated and will be removed in a future version. Please"
+            " use VaeImageProcessor instead",
+            FutureWarning,
+        )
         latents = 1 / self.vae.config.scaling_factor * latents
-        image = self.vae.decode(latents).sample
+        image = self.vae.decode(latents, return_dict=False)[0]
         image = (image / 2 + 0.5).clamp(0, 1)
         # we always cast to float32 as this does not cause significant overhead and is compatible with bfloat16
         image = image.cpu().permute(0, 2, 3, 1).float().numpy()
         return image
 
     def prepare_extra_step_kwargs(self, generator, eta):
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
@@ -520,14 +554,15 @@
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
         callback_steps: int = 1,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        guidance_rescale: float = 0.0,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide the image generation. If not defined, one has to pass `prompt_embeds`.
@@ -582,14 +617,19 @@
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
             cross_attention_kwargs (`dict`, *optional*):
                 A kwargs dictionary that if specified is passed along to the `AttentionProcessor` as defined under
                 `self.processor` in
                 [diffusers.cross_attention](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/cross_attention.py).
+            guidance_rescale (`float`, *optional*, defaults to 0.7):
+                Guidance rescale factor proposed by [Common Diffusion Noise Schedules and Sample Steps are
+                Flawed](https://arxiv.org/pdf/2305.08891.pdf) `guidance_scale` is defined as `φ` in equation 16. of
+                [Common Diffusion Noise Schedules and Sample Steps are Flawed](https://arxiv.org/pdf/2305.08891.pdf).
+                Guidance rescale factor should fix overexposure when using zero terminal SNR.
 
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple`.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
@@ -621,22 +661,26 @@
             device = self._execution_device
             # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
             # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
             # corresponds to doing no classifier free guidance.
             do_classifier_free_guidance = guidance_scale > 1.0
 
             # 3. Encode input prompt
+            text_encoder_lora_scale = (
+                cross_attention_kwargs.get("scale", None) if cross_attention_kwargs is not None else None
+            )
             prompt_embeds, negative_prompt_embeds = self._encode_prompt(
                 prompt,
                 device,
                 num_images_per_prompt,
                 do_classifier_free_guidance,
                 negative_prompt,
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
+                lora_scale=text_encoder_lora_scale,
             )
 
             # 4. Prepare timesteps
             self.scheduler.set_timesteps(num_inference_steps, device="cpu")
             timesteps = self.scheduler.timesteps.to(device)
 
             # 5. Prepare latent variables
@@ -704,29 +748,35 @@
                     )
 
                     # perform guidance
                     if do_classifier_free_guidance:
                         noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                         noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
+                    if do_classifier_free_guidance and guidance_rescale > 0.0:
+                        # Based on 3.4. in https://arxiv.org/pdf/2305.08891.pdf
+                        noise_pred = rescale_noise_cfg(noise_pred, noise_pred_text, guidance_rescale=guidance_rescale)
+
                     # compute the previous noisy sample x_t -> x_t-1
-                    latents_batch = self.scheduler.step(noise_pred, latents_batch, **extra_step_kwargs).prev_sample
+                    latents_batch = self.scheduler.step(
+                        noise_pred, latents_batch, **extra_step_kwargs, return_dict=False
+                    )[0]
 
                     if not self.use_hpu_graphs:
                         self.htcore.mark_step()
 
                     # call the callback, if provided
                     if callback is not None and i % callback_steps == 0:
                         callback(i, timestep, latents_batch)
 
-                if output_type == "latent":
-                    image = latents_batch
-                else:
+                if not output_type == "latent":
                     # 8. Post-processing
-                    image = self.decode_latents(latents_batch)
+                    image = self.vae.decode(latents_batch / self.vae.config.scaling_factor, return_dict=False)[0]
+                else:
+                    image = latents_batch
                 outputs["images"].append(image)
 
                 self.scheduler.reset_timestep_dependent_params()
 
                 if not self.use_hpu_graphs:
                     self.htcore.mark_step()
 
@@ -742,26 +792,30 @@
 
             # Remove dummy generations if needed
             if num_dummy_samples > 0:
                 outputs["images"][-1] = outputs["images"][-1][:-num_dummy_samples]
 
             # Process generated images
             for i, image in enumerate(outputs["images"][:]):
+                if i == 0:
+                    outputs["images"].clear()
+
                 if output_type == "latent":
                     has_nsfw_concept = None
                 else:
-                    # 9. Run safety checker
                     image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
 
-                if i == 0:
-                    outputs["images"].clear()
+                if has_nsfw_concept is None:
+                    do_denormalize = [True] * image.shape[0]
+                else:
+                    do_denormalize = [not has_nsfw for has_nsfw in has_nsfw_concept]
+
+                image = self.image_processor.postprocess(image, output_type=output_type, do_denormalize=do_denormalize)
 
-                # 10. Convert to PIL
                 if output_type == "pil":
-                    image = self.numpy_to_pil(image)
                     outputs["images"] += image
                 else:
                     outputs["images"] += [*image]
 
                 if has_nsfw_concept is not None:
                     outputs["has_nsfw_concept"] += has_nsfw_concept
                 else:
@@ -777,15 +831,21 @@
             )
 
     @torch.no_grad()
     def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs, capture):
         if self.use_hpu_graphs:
             return self.capture_replay(latent_model_input, timestep, encoder_hidden_states, capture)
         else:
-            return self.unet(latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs).sample
+            return self.unet(
+                latent_model_input,
+                timestep,
+                encoder_hidden_states=encoder_hidden_states,
+                cross_attention_kwargs=cross_attention_kwargs,
+                return_dict=False,
+            )[0]
 
     @torch.no_grad()
     def capture_replay(self, latent_model_input, timestep, encoder_hidden_states, capture):
         inputs = [latent_model_input, timestep, encoder_hidden_states, False]
         h = self.ht.hpu.graphs.input_hash(inputs)
         cached = self.cache.get(h)
```

### Comparing `optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py` & `optimum-habana-1.6.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,22 @@
             Note that the thresholding method is unsuitable for latent-space diffusion models (such as
             stable-diffusion).
         dynamic_thresholding_ratio (`float`, default `0.995`):
             the ratio for the dynamic thresholding method. Default is `0.995`, the same as Imagen
             (https://arxiv.org/abs/2205.11487). Valid only when `thresholding=True`.
         sample_max_value (`float`, default `1.0`):
             the threshold value for dynamic thresholding. Valid only when `thresholding=True`.
+        timestep_spacing (`str`, default `"leading"`):
+            The way the timesteps should be scaled. Refer to Table 2. of [Common Diffusion Noise Schedules and Sample
+            Steps are Flawed](https://arxiv.org/abs/2305.08891) for more information.
+        rescale_betas_zero_snr (`bool`, default `False`):
+            whether to rescale the betas to have zero terminal SNR (proposed by https://arxiv.org/pdf/2305.08891.pdf).
+            This can enable the model to generate very bright and dark samples instead of limiting it to samples with
+            medium brightness. Loosely related to
+            [`--offset_noise`](https://github.com/huggingface/diffusers/blob/74fd735eb073eb1d774b1ab4154a0876eb82f055/examples/dreambooth/train_dreambooth.py#L506).
     """
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
@@ -79,14 +87,16 @@
         set_alpha_to_one: bool = True,
         steps_offset: int = 0,
         prediction_type: str = "epsilon",
         thresholding: bool = False,
         dynamic_thresholding_ratio: float = 0.995,
         clip_sample_range: float = 1.0,
         sample_max_value: float = 1.0,
+        timestep_spacing: str = "leading",
+        rescale_betas_zero_snr: bool = False,
     ):
         super().__init__(
             num_train_timesteps,
             beta_start,
             beta_end,
             beta_schedule,
             trained_betas,
```

### Comparing `optimum-habana-1.6.0/optimum/habana/distributed/distributed_runner.py` & `optimum-habana-1.6.1/optimum/habana/distributed/distributed_runner.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/distributed/fast_ddp.py` & `optimum-habana-1.6.1/optimum/habana/distributed/fast_ddp.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/__init__.py` & `optimum-habana-1.6.1/optimum/habana/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/deepspeed.py` & `optimum-habana-1.6.1/optimum/habana/transformers/deepspeed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/gaudi_configuration.py` & `optimum-habana-1.6.1/optimum/habana/transformers/gaudi_configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/generation/utils.py` & `optimum-habana-1.6.1/optimum/habana/transformers/generation/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/gradient_checkpointing.py` & `optimum-habana-1.6.1/optimum/habana/transformers/gradient_checkpointing.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/modeling_utils.py` & `optimum-habana-1.6.1/optimum/habana/transformers/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/__init__.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/albert/modeling_albert.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/modeling_bloom.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/bloom/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/esm/modeling_esmfold.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/esm/modeling_esmfold.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/modeling_gptj.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/gptj/modeling_gptj.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/modeling_all_models.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/modeling_all_models.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/opt/modeling_opt.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/t5/modeling_t5.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/t5/modeling_t5.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/vit/modeling_vit.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py` & `optimum-habana-1.6.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/trainer.py` & `optimum-habana-1.6.1/optimum/habana/transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/trainer_seq2seq.py` & `optimum-habana-1.6.1/optimum/habana/transformers/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/trainer_utils.py` & `optimum-habana-1.6.1/optimum/habana/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/training_args.py` & `optimum-habana-1.6.1/optimum/habana/transformers/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/transformers/training_args_seq2seq.py` & `optimum-habana-1.6.1/optimum/habana/transformers/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/utils.py` & `optimum-habana-1.6.1/optimum/habana/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/optimum/habana/version.py` & `optimum-habana-1.6.1/optimum/habana/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
```

### Comparing `optimum-habana-1.6.0/optimum_habana.egg-info/PKG-INFO` & `optimum-habana-1.6.1/optimum_habana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.6.0
+Version: 1.6.1
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-habana-1.6.0/optimum_habana.egg-info/SOURCES.txt` & `optimum-habana-1.6.1/optimum_habana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/pyproject.toml` & `optimum-habana-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/setup.py` & `optimum-habana-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 INSTALL_REQUIRES = [
     "transformers >= 4.26.0, < 4.29.0",
     "optimum",
     "torch",
     "accelerate",
-    "diffusers >= 0.12.0",
+    "diffusers >= 0.18.0",
 ]
 
 TESTS_REQUIRE = [
     "pytest",
     "psutil",
     "parameterized",
     "GitPython",
```

### Comparing `optimum-habana-1.6.0/tests/test_diffusers.py` & `optimum-habana-1.6.1/tests/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_examples.py` & `optimum-habana-1.6.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_examples_match_transformers.py` & `optimum-habana-1.6.1/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_gaudi_configuration.py` & `optimum-habana-1.6.1/tests/test_gaudi_configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_trainer.py` & `optimum-habana-1.6.1/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_trainer_distributed.py` & `optimum-habana-1.6.1/tests/test_trainer_distributed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.6.0/tests/test_trainer_seq2seq.py` & `optimum-habana-1.6.1/tests/test_trainer_seq2seq.py`

 * *Files identical despite different names*

