# Comparing `tmp/swarms-0.7.7.tar.gz` & `tmp/swarms-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.7.7.tar", last modified: Thu Jul  6 23:06:36 2023, max compression
+gzip compressed data, was "swarms-0.7.8.tar", last modified: Thu Jul  6 23:13:25 2023, max compression
```

## Comparing `swarms-0.7.7.tar` & `swarms-0.7.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 23:06:26.000000 swarms-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:06:36.772506 swarms-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-06 23:06:26.000000 swarms-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.760506 swarms-0.7.7/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-06 23:06:26.000000 swarms-0.7.7/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-06 23:06:26.000000 swarms-0.7.7/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 23:06:26.000000 swarms-0.7.7/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:06:36.772506 swarms-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-06 23:06:26.000000 swarms-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.760506 swarms-0.7.7/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.760506 swarms-0.7.7/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/boss/babyagi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/boss/boss_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/auto_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/metaprompt_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.764506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.768506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.768506 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.768506 swarms-0.7.7/swarms/agents/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.768506 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.768506 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/models/segment_anything/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/visual_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/agents/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    71905 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.772506 swarms-0.7.7/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-06 23:06:26.000000 swarms-0.7.7/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:06:36.760506 swarms-0.7.7/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:06:36.000000 swarms-0.7.7/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-06 23:06:36.000000 swarms-0.7.7/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:06:36.000000 swarms-0.7.7/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 23:06:36.000000 swarms-0.7.7/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 23:06:36.000000 swarms-0.7.7/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.886676 swarms-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 23:13:12.000000 swarms-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:13:25.886676 swarms-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-06 23:13:12.000000 swarms-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.866675 swarms-0.7.8/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-06 23:13:12.000000 swarms-0.7.8/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-06 23:13:12.000000 swarms-0.7.8/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 23:13:12.000000 swarms-0.7.8/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:13:25.886676 swarms-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-06 23:13:12.000000 swarms-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.866675 swarms-0.7.8/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.866675 swarms-0.7.8/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/boss/babyagi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/boss/boss_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/auto_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/metaprompt_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.870676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.874676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.874676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.874676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.878676 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.878676 swarms-0.7.8/swarms/agents/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.878676 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.882676 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.882676 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/models/segment_anything/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.882676 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.882676 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/visual_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/agents/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.886676 swarms-0.7.8/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.886676 swarms-0.7.8/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/tools/agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71905 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.886676 swarms-0.7.8/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-06 23:13:12.000000 swarms-0.7.8/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:13:25.866675 swarms-0.7.8/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:13:25.000000 swarms-0.7.8/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-06 23:13:25.000000 swarms-0.7.8/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:13:25.000000 swarms-0.7.8/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 23:13:25.000000 swarms-0.7.8/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 23:13:25.000000 swarms-0.7.8/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.7.7/LICENSE` & `swarms-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/PKG-INFO` & `swarms-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.7.7
+Version: 0.7.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.7.7/README.md` & `swarms-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/api/container.py` & `swarms-0.7.8/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/api/main.py` & `swarms-0.7.8/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/api/worker.py` & `swarms-0.7.8/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/setup.py` & `swarms-0.7.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.7.7',
+  version = '0.7.8',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.7.7/swarms/agents/boss/babyagi_agent.py` & `swarms-0.7.8/swarms/agents/boss/babyagi_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/boss/boss_agent.py` & `swarms-0.7.8/swarms/agents/boss/boss_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/agents.py` & `swarms-0.7.8/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/auto_worker.py` & `swarms-0.7.8/swarms/agents/workers/auto_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/metaprompt_worker.py` & `swarms-0.7.8/swarms/agents/workers/metaprompt_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/GroundingDINO/setup.py` & `swarms-0.7.8/swarms/agents/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/__init__.py` & `swarms-0.7.8/swarms/agents/workers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/models/segment_anything/setup.py` & `swarms-0.7.8/swarms/agents/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-0.7.8/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-0.7.8/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/omni_worker.py` & `swarms-0.7.8/swarms/agents/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/visual_worker.py` & `swarms-0.7.8/swarms/agents/workers/visual_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/agents/workers/worker.py` & `swarms-0.7.8/swarms/agents/workers/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/prompts/prompts.py` & `swarms-0.7.8/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/swarms.py` & `swarms-0.7.8/swarms/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/tools/agent_tools.py` & `swarms-0.7.8/swarms/tools/agent_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 from langchain.chat_models import ChatOpenAI
 from langchain.tools import tool
 
 # ---------- Constants ----------
 ROOT_DIR = "./data/"
 
 # ---------- Tools ----------
-openai_api_key = os.environ["OPENAI_API_KEY"]
-llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
+# openai_api_key = os.environ["OPENAI_API_KEY"]
+# llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
 
-worker_tools = [
-    DuckDuckGoSearchRun(),
-    WriteFileTool(root_dir=ROOT_DIR),
-    ReadFileTool(root_dir=ROOT_DIR),
-    process_csv,
+# worker_tools = [
+#     DuckDuckGoSearchRun(),
+#     WriteFileTool(root_dir=ROOT_DIR),
+#     ReadFileTool(root_dir=ROOT_DIR),
+#     process_csv,
     
-    WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
+#     WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
 
-    # Tool(name='terminal', func=Terminal.execute, description='Operates a terminal'),
-    # Tool(name='code_writer', func=CodeWriter(), description='Writes code'),
-    # Tool(name='code_editor', func=CodeEditor(), description='Edits code'),#
-]
+#     # Tool(name='terminal', func=Terminal.execute, description='Operates a terminal'),
+#     # Tool(name='code_writer', func=CodeWriter(), description='Writes code'),
+#     # Tool(name='code_editor', func=CodeEditor(), description='Edits code'),#
+# ]
 
-# ---------- Vector Store ----------
-embeddings_model = OpenAIEmbeddings()
-embedding_size = 1536
-index = faiss.IndexFlatL2(embedding_size)
-vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+# # ---------- Vector Store ----------
+# embeddings_model = OpenAIEmbeddings()
+# embedding_size = 1536
+# index = faiss.IndexFlatL2(embedding_size)
+# vectorstore = FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
```

### Comparing `swarms-0.7.7/swarms/tools/main.py` & `swarms-0.7.8/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms/utils/utils.py` & `swarms-0.7.8/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms.egg-info/PKG-INFO` & `swarms-0.7.8/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.7.7
+Version: 0.7.8
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.7.7/swarms.egg-info/SOURCES.txt` & `swarms-0.7.8/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.7.7/swarms.egg-info/requires.txt` & `swarms-0.7.8/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

