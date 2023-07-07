# Comparing `tmp/agilerl-0.1.6.tar.gz` & `tmp/agilerl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agilerl-0.1.6.tar", max compression
+gzip compressed data, was "agilerl-0.1.7.tar", max compression
```

## Comparing `agilerl-0.1.6.tar` & `agilerl-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.6/agilerl/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.6/agilerl/algorithms/__init__.py
--rw-r--r--   0        0        0    20456 2023-05-05 09:35:55.662695 agilerl-0.1.6/agilerl/algorithms/bc_lm.py
--rw-r--r--   0        0        0    12694 2023-05-23 16:32:48.664828 agilerl-0.1.6/agilerl/algorithms/cqn.py
--rw-r--r--   0        0        0    17154 2023-05-17 09:02:17.797477 agilerl-0.1.6/agilerl/algorithms/ddpg.py
--rw-r--r--   0        0        0    12392 2023-05-17 09:16:01.664740 agilerl-0.1.6/agilerl/algorithms/dqn.py
--rw-r--r--   0        0        0    72764 2023-05-05 09:35:55.678696 agilerl-0.1.6/agilerl/algorithms/ilql.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.6/agilerl/components/__init__.py
--rw-r--r--   0        0        0     3874 2023-05-19 14:45:03.354134 agilerl-0.1.6/agilerl/components/replay_buffer.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.678696 agilerl-0.1.6/agilerl/data/__init__.py
--rw-r--r--   0        0        0     1688 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/language_environment.py
--rw-r--r--   0        0        0     8013 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/rl_data.py
--rw-r--r--   0        0        0     1303 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/tokenizer.py
--rw-r--r--   0        0        0     1175 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/torch_datasets.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.6/agilerl/hpo/__init__.py
--rw-r--r--   0        0        0    20187 2023-05-19 14:21:08.490783 agilerl-0.1.6/agilerl/hpo/mutation.py
--rw-r--r--   0        0        0     2153 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/hpo/tournament.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.6/agilerl/networks/__init__.py
--rw-r--r--   0        0        0    37557 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_bert.py
--rw-r--r--   0        0        0    25101 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_cnn.py
--rw-r--r--   0        0        0    37684 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_gpt.py
--rw-r--r--   0        0        0    14781 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/networks/evolvable_mlp.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.6/agilerl/training/__init__.py
--rw-r--r--   0        0        0     7408 2023-05-22 13:31:33.225917 agilerl-0.1.6/agilerl/training/train.py
--rw-r--r--   0        0        0     8771 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/training/train_bc_lm.py
--rw-r--r--   0        0        0     9326 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/training/train_ilql.py
--rw-r--r--   0        0        0     6662 2023-05-22 10:14:40.179051 agilerl-0.1.6/agilerl/training/train_offline.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/utils/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/utils/cache.py
--rw-r--r--   0        0        0     3952 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/ilql_utils.py
--rw-r--r--   0        0        0    10349 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/load_objects.py
--rw-r--r--   0        0        0     2444 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/log_utils.py
--rw-r--r--   0        0        0      120 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/mp_cache.py
--rw-r--r--   0        0        0     2205 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/sampling_utils.py
--rw-r--r--   0        0        0     3307 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/utils/serve_queue.py
--rw-r--r--   0        0        0     1496 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/utils/torch_utils.py
--rw-r--r--   0        0        0     4092 2023-05-22 14:05:48.103293 agilerl-0.1.6/agilerl/utils/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/wordle/__init__.py
--rw-r--r--   0        0        0     7021 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/wordle/policy.py
--rw-r--r--   0        0        0     5900 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_dataset.py
--rw-r--r--   0        0        0     1119 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_env.py
--rw-r--r--   0        0        0     9110 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_evaluators.py
--rw-r--r--   0        0        0    11117 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_game.py
--rw-r--r--   0        0        0     2510 2023-05-05 09:35:55.736340 agilerl-0.1.6/agilerl/wordle/wordle_tokenizer.py
--rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.6/LICENSE
--rw-r--r--   0        0        0      728 2023-05-24 08:41:30.075862 agilerl-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    32090 2023-05-23 16:32:45.722183 agilerl-0.1.6/README.md
--rw-r--r--   0        0        0    32755 1970-01-01 00:00:00.000000 agilerl-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.7/agilerl/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.7/agilerl/algorithms/__init__.py
+-rw-r--r--   0        0        0    22560 2023-07-07 11:17:43.248466 agilerl-0.1.7/agilerl/algorithms/bc_lm.py
+-rw-r--r--   0        0        0    15623 2023-07-07 11:17:43.249466 agilerl-0.1.7/agilerl/algorithms/cqn.py
+-rw-r--r--   0        0        0    21969 2023-07-07 11:17:43.250660 agilerl-0.1.7/agilerl/algorithms/ddpg.py
+-rw-r--r--   0        0        0    15306 2023-07-07 11:17:43.251693 agilerl-0.1.7/agilerl/algorithms/dqn.py
+-rw-r--r--   0        0        0    73846 2023-07-07 11:17:43.252868 agilerl-0.1.7/agilerl/algorithms/ilql.py
+-rw-r--r--   0        0        0    28355 2023-07-07 11:17:43.252868 agilerl-0.1.7/agilerl/algorithms/td3.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.7/agilerl/components/__init__.py
+-rw-r--r--   0        0        0     4078 2023-07-07 11:17:43.253977 agilerl-0.1.7/agilerl/components/replay_buffer.py
+-rw-r--r--   0        0        0      649 2023-07-07 11:17:43.255092 agilerl-0.1.7/agilerl/components/replay_data.py
+-rw-r--r--   0        0        0      705 2023-07-07 11:17:43.255092 agilerl-0.1.7/agilerl/components/sampler.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.678696 agilerl-0.1.7/agilerl/data/__init__.py
+-rw-r--r--   0        0        0     1688 2023-05-05 09:35:55.686685 agilerl-0.1.7/agilerl/data/language_environment.py
+-rw-r--r--   0        0        0     8013 2023-05-05 09:35:55.686685 agilerl-0.1.7/agilerl/data/rl_data.py
+-rw-r--r--   0        0        0     1303 2023-05-05 09:35:55.686685 agilerl-0.1.7/agilerl/data/tokenizer.py
+-rw-r--r--   0        0        0     1175 2023-05-05 09:35:55.686685 agilerl-0.1.7/agilerl/data/torch_datasets.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.7/agilerl/hpo/__init__.py
+-rw-r--r--   0        0        0    22991 2023-07-07 11:17:43.256090 agilerl-0.1.7/agilerl/hpo/mutation.py
+-rw-r--r--   0        0        0     2193 2023-07-07 11:17:43.257087 agilerl-0.1.7/agilerl/hpo/tournament.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.7/agilerl/networks/__init__.py
+-rw-r--r--   0        0        0    37610 2023-07-07 11:17:43.258084 agilerl-0.1.7/agilerl/networks/evolvable_bert.py
+-rw-r--r--   0        0        0    26079 2023-07-07 11:17:43.259081 agilerl-0.1.7/agilerl/networks/evolvable_cnn.py
+-rw-r--r--   0        0        0    37944 2023-07-07 11:17:43.261076 agilerl-0.1.7/agilerl/networks/evolvable_gpt.py
+-rw-r--r--   0        0        0    15244 2023-07-07 11:17:43.261076 agilerl-0.1.7/agilerl/networks/evolvable_mlp.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.7/agilerl/training/__init__.py
+-rw-r--r--   0        0        0    11953 2023-07-07 11:17:43.262073 agilerl-0.1.7/agilerl/training/train.py
+-rw-r--r--   0        0        0     8811 2023-07-07 11:17:43.263071 agilerl-0.1.7/agilerl/training/train_bc_lm.py
+-rw-r--r--   0        0        0     9366 2023-07-07 11:17:43.264068 agilerl-0.1.7/agilerl/training/train_ilql.py
+-rw-r--r--   0        0        0    11697 2023-07-07 11:17:43.265065 agilerl-0.1.7/agilerl/training/train_offline.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.703476 agilerl-0.1.7/agilerl/utils/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-05 09:35:55.703476 agilerl-0.1.7/agilerl/utils/cache.py
+-rw-r--r--   0        0        0     4094 2023-07-07 11:17:43.266063 agilerl-0.1.7/agilerl/utils/ilql_utils.py
+-rw-r--r--   0        0        0    10398 2023-07-07 11:17:43.267059 agilerl-0.1.7/agilerl/utils/load_objects.py
+-rw-r--r--   0        0        0     2444 2023-05-05 09:35:55.711952 agilerl-0.1.7/agilerl/utils/log_utils.py
+-rw-r--r--   0        0        0      120 2023-05-05 09:35:55.711952 agilerl-0.1.7/agilerl/utils/mp_cache.py
+-rw-r--r--   0        0        0     2241 2023-07-07 11:17:43.268057 agilerl-0.1.7/agilerl/utils/sampling_utils.py
+-rw-r--r--   0        0        0     3433 2023-07-07 11:17:43.268057 agilerl-0.1.7/agilerl/utils/serve_queue.py
+-rw-r--r--   0        0        0     1516 2023-07-07 11:17:43.269055 agilerl-0.1.7/agilerl/utils/torch_utils.py
+-rw-r--r--   0        0        0     5853 2023-07-07 11:17:43.270052 agilerl-0.1.7/agilerl/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.719952 agilerl-0.1.7/agilerl/wordle/__init__.py
+-rw-r--r--   0        0        0     7021 2023-05-05 09:35:55.719952 agilerl-0.1.7/agilerl/wordle/policy.py
+-rw-r--r--   0        0        0     6016 2023-07-07 11:17:43.270052 agilerl-0.1.7/agilerl/wordle/wordle_dataset.py
+-rw-r--r--   0        0        0     1119 2023-05-05 09:35:55.728286 agilerl-0.1.7/agilerl/wordle/wordle_env.py
+-rw-r--r--   0        0        0    10054 2023-07-07 11:17:43.271049 agilerl-0.1.7/agilerl/wordle/wordle_evaluators.py
+-rw-r--r--   0        0        0    11187 2023-07-07 11:17:43.272046 agilerl-0.1.7/agilerl/wordle/wordle_game.py
+-rw-r--r--   0        0        0     2752 2023-07-07 11:17:43.272046 agilerl-0.1.7/agilerl/wordle/wordle_tokenizer.py
+-rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.7/LICENSE
+-rw-r--r--   0        0        0      728 2023-07-07 11:18:32.150837 agilerl-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    44135 2023-07-07 11:17:43.247171 agilerl-0.1.7/README.md
+-rw-r--r--   0        0        0    44563 1970-01-01 00:00:00.000000 agilerl-0.1.7/PKG-INFO
```

### Comparing `agilerl-0.1.6/agilerl/algorithms/bc_lm.py` & `agilerl-0.1.7/agilerl/algorithms/bc_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from typing import Any, Callable, Optional, Tuple, Union
 import numpy as np
 from agilerl.networks.evolvable_gpt import EvolvableGPT
 from agilerl.data.rl_data import DataPoint, RL_Dataset
 from agilerl.data.language_environment import Language_Observation, interact_environment
-from agilerl.utils.sampling_utils import process_logits, pad_sequence, map_all_kvs, update_kvs, always_terminate
+from agilerl.utils.sampling_utils import process_logits, pad_sequence, map_all_kvs, \
+    update_kvs, always_terminate
 
 class BC_LM(nn.Module):
     def __init__(self, 
                  dataset: RL_Dataset, 
                  net_config,
                  device: Union[torch.device, str] = "cuda", 
                  transition_weight: float=0.0, 
@@ -54,38 +55,46 @@
         set_pos_ids = prefix_attn_mask is not None
         if prefix_attn_mask is not None and attn_mask is not None:
             input_attn_mask = torch.cat((prefix_attn_mask, attn_mask), dim=1)
         else:
             input_attn_mask = None
         position_ids = torch.cumsum(input_attn_mask, dim=1)-1 if set_pos_ids else None
         if remove_prefix_position_embs:
-            prefix_embs -= self.model.transformer.wpe(position_ids[:, :prefix_embs.shape[1]])
-        input_embeddings = torch.cat((prefix_embs, self.model.transformer.wte(tokens)), dim=1)
+            prefix_embs -= self.model.transformer.wpe(
+                position_ids[:, :prefix_embs.shape[1]])
+        input_embeddings = torch.cat((prefix_embs, self.model.transformer.wte(tokens)), 
+                                     dim=1)
         
-        model_outputs, _, model_past_key_values, _ = self.model(tok_emb=input_embeddings, 
+        model_outputs, _, model_past_key_values, _ = self.model(
+                                   tok_emb=input_embeddings, 
                                    attn_mask=input_attn_mask, 
                                    pos=position_ids, 
                                    **kwargs)
         return model_outputs, model_past_key_values
     
     def get_weights(self, 
                     tokens: torch.Tensor, 
                     action_idxs: torch.Tensor):
         weights = torch.full(tokens.shape, self.transition_weight).to(self.device)
         if action_idxs.shape[1] == 0:
             n = torch.zeros((tokens.shape[0],)).long().to(self.device)
         else:
             n = torch.argmax(action_idxs, dim=1)+1
         for i in range(tokens.shape[0]):
-            weights[i] = torch.scatter(weights[i], dim=0, index=action_idxs[i, :n[i]], src=torch.full((n[i].item(),), 1.0).to(self.device))
+            weights[i] = torch.scatter(weights[i], 
+                                       dim=0, 
+                                       index=action_idxs[i, :n[i]], 
+                                       src=torch.full((n[i].item(),), 
+                                                      1.0).to(self.device))
         return weights
     
     def awac_loss(self, tokens, attn_mask, logits, w):
         w = w.detach()
-        losses = F.cross_entropy(logits[:, :-1, :].reshape(-1, logits.shape[-1]), tokens[:, 1:].reshape(-1), reduction='none')
+        losses = F.cross_entropy(logits[:, :-1, :].reshape(-1, logits.shape[-1]), 
+                                 tokens[:, 1:].reshape(-1), reduction='none')
         losses = losses.reshape(tokens.shape[0], tokens.shape[1]-1)
         return (losses * w[:, :-1] * attn_mask[:, 1:]).sum() / attn_mask[:, 1:].sum()
 
     def get_loss(self, items):
         prepared_inputs = self.prepare_inputs(items)
         tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
         a_idx = prepared_inputs['action_idxs']
@@ -165,60 +174,83 @@
             max_length = self.bc_lm.model.block_size
         max_length = min(max_length, self.bc_lm.model.block_size)
         device = self.bc_lm.device
         bsize = tokens.shape[0]
         n = bsize * num_generations
         if max_generation_len is None:
             max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        input_strs = [tokenizer.decode(
+            tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
+            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        logits, past_key_values = self.bc_lm(tokens=tokens, attn_mask=attn_mask, prefix_embs=prefix_embs, 
+        logits, past_key_values = self.bc_lm(tokens=tokens, 
+                                   attn_mask=attn_mask, 
+                                   prefix_embs=prefix_embs, 
                                    prefix_attn_mask=prefix_attn_mask, 
                                    remove_prefix_position_embs=remove_prefix_position_embs,
                                    is_causal=False)
         dialogue_kvs = past_key_values
         dialogue_lens = attn_mask.sum(dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), max_length, tokenizer.pad_token_id, device, 1)
+        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), 
+                              max_length, tokenizer.pad_token_id, device, 1)
         dialogue_lens = torch.repeat_interleave(dialogue_lens, num_generations, dim=0)
-        dialogue_kvs = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), max_length, 0.0, device, 2), dialogue_kvs)
+        dialogue_kvs = map_all_kvs(lambda x: pad_sequence(
+            torch.repeat_interleave(x, num_generations, dim=0), 
+            max_length, 0.0, device, 2), dialogue_kvs)
         log_probs = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         termination_mask = torch.full((dialogue_lens.shape[0],), 1).to(device)
         t = torch.min(dialogue_lens).int()
         while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
             curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], dialogue_kvs)
-            logits, past_key_values = self.bc_lm(curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False)
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], 
+                                            dialogue_kvs)
+            logits, past_key_values = self.bc_lm(curr_token, None, 
+                                                 past_key_values=curr_dialogue_kvs, 
+                                                 is_causal=False)
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, 
+                                                               float('-inf'), 1e7)
+            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), 
+                   tokens[:, t]] = logits[torch.arange(0, n).to(device), 
+                                          torch.full((n,), 0).to(device), 
+                                          tokens[:, t]].masked_fill_(t < dialogue_lens, 
+                                                                     1e7)
             logits = process_logits(logits, temp=temp, top_k=top_k, top_p=top_p)
             cat_dist = torch.distributions.categorical.Categorical(logits=logits[:, 0])
             new_tokens = cat_dist.sample()
             log_probs += cat_dist.log_prob(new_tokens)
             tokens[:, t] = new_tokens
-            dialogue_kvs = update_kvs(dialogue_kvs, past_key_values, torch.arange(0, n).to(device), (t+prefix_t)-1)
+            dialogue_kvs = update_kvs(dialogue_kvs, past_key_values, 
+                                      torch.arange(0, n).to(device), (t+prefix_t)-1)
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(), 
-                                                                                             clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= (1 - int(termination_condition(
+                        tokenizer.decode(tokens[idx, :].tolist(), 
+                                         clean_up_tokenization_spaces=False))))
             t += 1
             termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
     
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        output_strs = [tokenizer.decode(
+            tokens[i, :].tolist(),
+            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(num_generations):
-                processed_str = output_strs[i*num_generations+x][len(input_strs[i]):].strip()
+                processed_str = output_strs[i*num_generations+x][len(
+                    input_strs[i]):].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
-        return list(zip(input_strs, processed_outputs)), log_probs.reshape(-1, num_generations)
+        return list(zip(input_strs, processed_outputs)), log_probs.reshape(-1, 
+                                                                           num_generations)
     
     def beam_raw(self, 
                  tokens: torch.Tensor, attn_mask: torch.Tensor, 
                  termination_condition: Callable[[np.ndarray], bool], 
                  beam_width=1, max_generation_len=None, 
                  prefix_embs: Optional[torch.Tensor]=None, 
                  prefix_attn_mask: Optional[torch.Tensor]=None, 
@@ -229,61 +261,95 @@
             max_length = self.bc_lm.model.block_size
         max_length = min(max_length, self.bc_lm.model.block_size)
         device = self.bc_lm.device
         bsize, vocab_size = tokens.shape[0], tokenizer.num_tokens()
         n = bsize * beam_width
         if max_generation_len is None:
             max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        input_strs = [tokenizer.decode(
+            tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
+            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        logits, past_key_values = self.bc_lm(tokens, attn_mask, prefix_embs=prefix_embs, 
+        logits, past_key_values = self.bc_lm(tokens, attn_mask, 
+                                             prefix_embs=prefix_embs, 
                                    prefix_attn_mask=prefix_attn_mask, 
                                    remove_prefix_position_embs=remove_prefix_position_embs,
                                    is_causal=False)
         dialogue_kvs = past_key_values
         original_dialogue_lens = attn_mask.sum(dim=1)
-        batch_indicator = torch.stack(beam_width*[torch.arange(0, bsize).to(device)], dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), max_length, tokenizer.pad_token_id, device, 1)
-        dialogue_lens = torch.repeat_interleave(original_dialogue_lens, beam_width, dim=0)
-        dialogue_kvs = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), max_length, 0.0, device, 2), dialogue_kvs)
+        batch_indicator = torch.stack(beam_width*[torch.arange(0, bsize).to(device)], 
+                                      dim=1)
+        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), 
+                              max_length, tokenizer.pad_token_id, device, 1)
+        dialogue_lens = torch.repeat_interleave(original_dialogue_lens, beam_width, 
+                                                dim=0)
+        dialogue_kvs = map_all_kvs(
+            lambda x: pad_sequence(
+            torch.repeat_interleave(x, beam_width, dim=0), max_length, 
+            0.0, device, 2), dialogue_kvs)
         curr_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         termination_mask = torch.full((n,), 1).to(device)
         t = torch.min(dialogue_lens).int()
         while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
             curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], dialogue_kvs)
-            logits, past_key_values = self.bc_lm(curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False)
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
-            scores = (torch.log(F.softmax(logits, dim=-1)).reshape(1, bsize, beam_width, -1).permute(3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(1, bsize, -1)  # (time, batch, k*vocab)
-            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_((t == original_dialogue_lens).unsqueeze(1).repeat(1, scores.shape[2]-vocab_size), float('-inf'))
-            curr_scores, top_k = torch.topk(scores[0, :, :], k=beam_width, dim=1)  # (batch, k), (batch, k)
-            tokens = tokens[(batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :]
+            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], 
+                                            dialogue_kvs)
+            logits, past_key_values = self.bc_lm(
+                curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False)
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, 
+                                                               float('-inf'), 1e7)
+            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), 
+                   tokens[:, t]] = logits[torch.arange(0, n).to(device), 
+                                          torch.full((n,), 0).to(
+                device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            scores = (torch.log(F.softmax(logits, dim=-1)).reshape(
+                1, bsize, beam_width, -1).permute(
+                3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(
+                1, bsize, -1)  # (time, batch, k*vocab)
+            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_(
+                (t == original_dialogue_lens).unsqueeze(1).repeat(
+                1, scores.shape[2]-vocab_size), float('-inf'))
+            curr_scores, top_k = torch.topk(
+                scores[0, :, :], k=beam_width, dim=1)  # (batch, k), (batch, k)
+            tokens = tokens[(
+                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :]
             tokens[:, t] = top_k.reshape(-1) % vocab_size  # (batch*k,)
-            fixed_dialogue_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :, :, :], past_key_values)
-            dialogue_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :, :, :], dialogue_kvs)
-            dialogue_kvs = update_kvs(dialogue_kvs, fixed_dialogue_kvs, torch.arange(0, n).to(device), (t+prefix_t)-1)
-            dialogue_lens = dialogue_lens[(batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
-            termination_mask = termination_mask[(batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
+            fixed_dialogue_kvs = map_all_kvs(
+                lambda x: x[(
+                batch_indicator * beam_width + (top_k // vocab_size)).reshape(
+                -1), :, :, :], past_key_values)
+            dialogue_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + (
+                top_k // vocab_size)).reshape(-1), :, :, :], dialogue_kvs)
+            dialogue_kvs = update_kvs(
+                dialogue_kvs, fixed_dialogue_kvs, torch.arange(0, n).to(
+                device), (t+prefix_t)-1)
+            dialogue_lens = dialogue_lens[(
+                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
+            termination_mask = termination_mask[(
+                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(),
-                                                                                             clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= (1 - int(termination_condition(
+                        tokenizer.decode(tokens[idx, :].tolist(), 
+                                         clean_up_tokenization_spaces=False))))
             t += 1
             termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False) for i in range(n)]
+        output_strs = [tokenizer.decode(tokens[i, :].tolist(),
+                                 clean_up_tokenization_spaces=False) for i in range(n)]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(beam_width):
                 processed_str = output_strs[i*beam_width+x][len(input_strs[i]):].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         return list(zip(input_strs, processed_outputs)), curr_scores
     
     def generate(self, items, 
                  termination_condition: Callable[[np.ndarray], bool], **kwargs):
         prepared_inputs = self.bc_lm.prepare_inputs(items)
@@ -296,17 +362,21 @@
             raise NotImplementedError
         generations, probs = method(tokens, attn_mask, 
                                     termination_condition, 
                                     **kwargs)
         return generations, probs
     
     def act(self, obs: Language_Observation) -> str:
-        item = DataPoint.from_obs(obs, self.bc_lm.dataset.tokenizer, self.bc_lm.dataset.token_reward)
-        generations, probs = self.generate([item], always_terminate, **self.generation_kwargs)
-        sorted_outputs = list(zip(*sorted(zip(generations[0][1], probs[0]), key=lambda x: -x[1])))[0]
+        item = DataPoint.from_obs(obs, 
+                                  self.bc_lm.dataset.tokenizer, 
+                                  self.bc_lm.dataset.token_reward)
+        generations, probs = self.generate([item], always_terminate, 
+                                           **self.generation_kwargs)
+        sorted_outputs = list(zip(*sorted(zip(
+            generations[0][1], probs[0]), key=lambda x: -x[1])))[0]
         return sorted_outputs[0]
     
     def train(self):
         self.bc_lm.train()
     
     def eval(self):
         self.bc_lm.eval()
@@ -324,26 +394,29 @@
         tokens = model.prepare_inputs(items)['tokens']
         n = tokens.shape[0]
         total_token_reward = 0
         total_env_reward = 0
         for i in range(n):
             result, sequence = interact_environment(self.env, policy, None)
             env_reward = sum(map(lambda x: x[2], sequence))
-            token_reward = sum(DataPoint.get_token_reward(result, model.dataset.tokenizer, model.dataset.token_reward))
+            token_reward = sum(DataPoint.get_token_reward(result, 
+                                                          model.dataset.tokenizer, 
+                                                          model.dataset.token_reward))
             total_env_reward += env_reward
             total_token_reward += token_reward
             if self.verbose:
                 print(result)
                 print('='*25)
                 print('token reward:', token_reward)
                 print('env reward:', env_reward)
                 print('avg token reward:', total_token_reward / (i + 1))
                 print('avg env reward:', total_env_reward / (i + 1))
                 print('='*25)
-        return {'token_reward': (total_token_reward / n, n), 'env_reward': (total_env_reward / n, n)}
+        return {'token_reward':(total_token_reward/n,n),
+                'env_reward':(total_env_reward/n,n)}
 
 def to(item: Any, device: torch.device):
     return map_pytree(lambda x: torch.tensor(x).to(device), item)
 
 def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any],
                item: Any):
     if isinstance(item, dict):
```

### Comparing `agilerl-0.1.6/agilerl/algorithms/cqn.py` & `agilerl-0.1.7/agilerl/algorithms/dqn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import random
 import copy
+import dill
 import numpy as np
 import torch
 import torch.nn as nn
-from torch.nn.utils import clip_grad_norm_
 import torch.optim as optim
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 from agilerl.networks.evolvable_cnn import EvolvableCNN
 
 
-class CQN():
-    """The CQN algorithm class. CQN paper: https://arxiv.org/abs/2006.04779
+class DQN():
+    """The DQN algorithm class. DQN paper: https://arxiv.org/abs/1312.5602
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding, used with discrete observation spaces
     :type one_hot: bool
-    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
+    :param index: Index to keep track of object instance during tournament selection 
+    and mutation, defaults to 0
     :type index: int, optional
     :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
     :type net_config: dict, optional
-    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
+    :param batch_size: Size of batched sample from replay buffer for learning, defaults 
+    to 64
     :type batch_size: int, optional
     :param lr: Learning rate for optimizer, defaults to 1e-4
     :type lr: float, optional
     :param learn_step: Learning frequency, defaults to 5
     :type learn_step: int, optional
     :param gamma: Discount factor, defaults to 0.99
     :type gamma: float, optional
@@ -34,157 +36,174 @@
     :type tau: float, optional
     :param mutation: Most recent mutation to agent, defaults to None
     :type mutation: str, optional
     :param double: Use double Q-learning, defaults to False
     :type double: bool, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    :param wrap: Wrap models for distributed training upon creation, defaults to True
+    :type wrap: bool, optional
     """
 
-    def __init__(
-        self,
-        state_dim,
-        action_dim,
-        one_hot,
-        index=0,
-        net_config={
-            'arch': 'mlp',
-            'h_size': [64, 64]
-            },
-        batch_size=64,
-        lr=1e-4,
-        learn_step=5,
-        gamma=0.99,
-        tau=1e-3,
-        mutation=None,
-        double=False,
-        device='cpu'):
-        
-        self.algo = 'CQN'
+    def __init__(self, state_dim, action_dim, one_hot, index=0, 
+                 net_config={'arch': 'mlp', 'h_size':[64,64]}, batch_size=64, lr=1e-4, 
+                 learn_step=5, gamma=0.99, tau=1e-3, mutation=None, double=False, 
+                 device='cpu', accelerator=None, wrap=True):
+        self.algo = 'DQN'
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
         self.learn_step = learn_step
         self.gamma = gamma
         self.tau = tau
         self.mut = mutation
         self.device = device
+        self.accelerator = accelerator
 
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         self.double = double
 
         # model
         if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
             self.actor = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
         elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
             self.actor = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                normalize=self.net_config['normalize'],
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                normalize=self.net_config['normalize'],
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
-        self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
+
+        if self.accelerator is not None:
+            self.optimizer = self.optimizer_type
+            if wrap:
+                self.wrap_models()          
+        else:
+            self.actor = self.actor.to(self.device)
+            self.actor_target = self.actor_target.to(self.device)
+            self.optimizer = self.optimizer_type
+
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. Epsilon is the 
-        probability of taking a random action, used for exploration.
+        """Returns the next action to take in the environment. 
+        Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: State observation, or multiple observations in a batch
         :type state: float or List[float]
-        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
+        :param epsilon: Probablilty of taking a random action for exploration, defaults 
+        to 0
         :type epsilon: float, optional
         """
-        state = torch.from_numpy(state).float().to(self.device)
+        state = torch.from_numpy(state).float()
+        if self.accelerator is None:
+            state = state.to(self.device)
 
         if self.one_hot:
             state = nn.functional.one_hot(
                 state.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if len(state.size()) < 2:
             state = state.unsqueeze(0)
 
         # epsilon-greedy
         if random.random() < epsilon:
-            action = np.random.randint(0, self.action_dim, size=state.size()[0])[0]
+            action = np.random.randint(0, self.action_dim, size=state.size()[0])
         else:
             self.actor.eval()
             with torch.no_grad():
                 action_values = self.actor(state)
             self.actor.train()
-            action = np.argmax(action_values.cpu().data.numpy(), axis=1)[0]
+
+            action = np.argmax(action_values.cpu().data.numpy(), axis=1)
+
         return action
+    
+    def _squeeze_exp(self, experiences):
+        """Remove first dim created by dataloader.
+        
+        :param experiences: List of batched states, actions, rewards, next_states, 
+        dones in that order.
+        :type state: List[torch.Tensor[float]]
+        """
+        st, ac, re, ne, do = experiences
+        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
 
     def learn(self, experiences):
         """Updates agent network parameters to learn from experiences.
 
-        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
+        :param experiences: List of batched states, actions, rewards, next_states, 
+        dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         states, actions, rewards, next_states, dones = experiences
 
         if self.one_hot:
             states = nn.functional.one_hot(
                 states.long(), num_classes=self.state_dim[0]).float().squeeze()
             next_states = nn.functional.one_hot(
                 next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if self.double: # Double Q-learning
             q_idx = self.actor_target(next_states).argmax(dim=1).unsqueeze(1)
-            q_target_next = self.actor(next_states).gather(dim=1, index=q_idx).detach()
+            q_target = self.actor(next_states).gather(dim=1, index=q_idx).detach()
         else:
-            q_target_next = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
+            q_target = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
 
         # target, if terminal then y_j = rewards
-        q_target = rewards + self.gamma * q_target_next * (1 - dones)
-        q_a_s = self.actor(states)
-        q_eval = q_a_s.gather(1, actions.long())
+        y_j = rewards + self.gamma * q_target * (1 - dones)
+        q_eval = self.actor(states).gather(1, actions.long())
 
         # loss backprop
-        cql1_loss = torch.logsumexp(q_a_s, dim=1).mean() - q_a_s.mean()
-        loss = self.criterion(q_eval, q_target)
-        q1_loss = cql1_loss + 0.5 * loss
+        loss = self.criterion(q_eval, y_j)
         self.optimizer.zero_grad()
-        q1_loss.backward()
-        clip_grad_norm_(self.actor.parameters(), 1)
+        if self.accelerator is not None:
+            self.accelerator.backward(loss)
+        else:
+            loss.backward()
         self.optimizer.step()
 
         # soft update target network
         self.softUpdate()
 
     def softUpdate(self):
         """Soft updates target network.
@@ -195,43 +214,44 @@
                 self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
-        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
+        :param swap_channels: Swap image channels dimension from last to first 
+        [H, W, C] -> [C, H, W], defaults to False
         :type swap_channels: bool, optional
         :param max_steps: Maximum number of testing steps, defaults to 500
         :type max_steps: int, optional
-        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean over these tests. Defaults to 3
+        :param loop: Number of testing loops/epsiodes to complete. The returned score 
+        is the mean over these tests. Defaults to 3
         :type loop: int, optional
         """
         with torch.no_grad():
             rewards = []
             for i in range(loop):
                 state = env.reset()[0]
                 score = 0
                 for idx_step in range(max_steps):
                     if swap_channels:
                         state = np.moveaxis(state, [3], [1])
                     action = self.getAction(state, epsilon=0)
                     state, reward, done, _, _ = env.step(action)
                     score += reward
-                    if done:
-                        break
                 rewards.append(score)
         mean_fit = np.mean(rewards)
         self.fitness.append(mean_fit)
         return mean_fit
 
-    def clone(self, index=None):
+    def clone(self, index=None, wrap=True):
         """Returns cloned agent identical to self.
 
-        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
+        :param index: Index to keep track of agent for tournament selection and 
+        mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
         clone = type(self)(state_dim=self.state_dim,
                            action_dim=self.action_dim,
@@ -241,25 +261,51 @@
                            batch_size=self.batch_size,
                            lr=self.lr,
                            learn_step=self.learn_step,
                            gamma=self.gamma,
                            tau=self.tau,
                            mutation=self.mut,
                            device=self.device,
-                           )
+                           accelerator=self.accelerator,
+                           wrap=wrap)
 
-        clone.actor = self.actor.clone().to(self.device)
-        clone.actor_target = self.actor_target.clone().to(self.device)
-        clone.optimizer = optim.Adam(clone.actor.parameters(), lr=clone.lr)
+        actor = self.actor.clone()
+        actor_target = self.actor_target.clone()
+        optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
+        clone.optimizer_type = optimizer
+        if self.accelerator is not None:
+            if wrap:
+                clone.actor, clone.actor_target, clone.optimizer = self.accelerator.prepare(
+                                                                                        actor, 
+                                                                                        actor_target,
+                                                                                        optimizer)
+            else:
+                clone.actor, clone.actor_target, clone.optimizer = actor, actor_target, optimizer
+        else:
+            clone.actor = actor.to(self.device)
+            clone.actor_target = actor_target.to(self.device)
+            clone.optimizer = optimizer
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
 
+    def wrap_models(self):
+        if self.accelerator is not None:
+            self.actor, self.actor_target, self.optimizer = self.accelerator.prepare(self.actor, 
+                                                                            self.actor_target, 
+                                                                            self.optimizer)
+    
+    def unwrap_models(self):
+        if self.accelerator is not None:
+            self.actor = self.accelerator.unwrap_model(self.actor)
+            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
+            self.optimizer = self.accelerator.unwrap_model(self.optimizer)
+
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
         torch.save({
@@ -275,38 +321,36 @@
             'gamma': self.gamma,
             'tau': self.tau,
             'mutation': self.mut,
             'index': self.index,
             'scores': self.scores,
             'fitness': self.fitness,
             'steps': self.steps,
-        }, path)
+        }, path, pickle_module=dill)
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
-        checkpoint = torch.load(path)
+        checkpoint = torch.load(path, pickle_module=dill)
         self.net_config = checkpoint['net_config']
         if self.net_config['arch'] == 'mlp':
             self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(
-                **checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
         elif self.net_config['arch'] == 'cnn':
             self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(
-                **checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
+        self.lr = checkpoint['lr']
+        self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
         self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(
-            checkpoint['actor_target_state_dict'])
+        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
         self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
         self.batch_size = checkpoint['batch_size']
-        self.lr = checkpoint['lr']
         self.learn_step = checkpoint['learn_step']
         self.gamma = checkpoint['gamma']
         self.tau = checkpoint['tau']
         self.mut = checkpoint['mutation']
         self.index = checkpoint['index']
         self.scores = checkpoint['scores']
         self.fitness = checkpoint['fitness']
```

### Comparing `agilerl-0.1.6/agilerl/algorithms/ddpg.py` & `agilerl-0.1.7/agilerl/algorithms/ddpg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import copy
+import dill
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 from agilerl.networks.evolvable_cnn import EvolvableCNN
 
@@ -13,168 +14,182 @@
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding, used with discrete observation spaces
     :type one_hot: bool
-    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
+    :param index: Index to keep track of object instance during tournament selection 
+    and mutation, defaults to 0
     :type index: int, optional
     :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
     :type net_config: dict, optional
-    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
+    :param batch_size: Size of batched sample from replay buffer for learning, 
+    defaults to 64
     :type batch_size: int, optional
     :param lr: Learning rate for optimizer, defaults to 1e-4
     :type lr: float, optional
     :param learn_step: Learning frequency, defaults to 5
     :type learn_step: int, optional
     :param gamma: Discount factor, defaults to 0.99
     :type gamma: float, optional
     :param tau: For soft update of target network parameters, defaults to 1e-3
     :type tau: float, optional
     :param mutation: Most recent mutation to agent, defaults to None
     :type mutation: str, optional
-    :param policy_freq: Frequency of target network updates compared to policy network, defaults to 2
+    :param policy_freq: Frequency of target network updates compared to policy network, 
+    defaults to 2
     :type policy_freq: int, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    :param wrap: Wrap models for distributed training upon creation, defaults to True
+    :type wrap: bool, optional
     """
 
-    def __init__(
-        self,
-        state_dim,
-        action_dim,
-        one_hot,
-        index=0,
-        net_config={
-            'arch': 'mlp',
-            'h_size': [
-            64,
-            64]},
-            batch_size=64,
-            lr=1e-4,
-            learn_step=5,
-            gamma=0.99,
-            tau=1e-3,
-            mutation=None,
-            policy_freq=2,
-            device='cpu'):
+    def __init__(self, state_dim, action_dim, one_hot, index=0, 
+                 net_config={'arch': 'mlp', 'h_size': [64,64]}, batch_size=64, lr=1e-4, 
+                 learn_step=5, gamma=0.99, tau=1e-3, mutation=None, policy_freq=2, 
+                 device='cpu', accelerator=None, wrap=True):
         self.algo = 'DDPG'
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
         self.learn_step = learn_step
         self.gamma = gamma
         self.tau = tau
         self.mut = mutation
         self.policy_freq = policy_freq
         self.device = device
+        self.accelerator = accelerator
 
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         # model
         if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
             self.actor = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
                 hidden_size=self.net_config['h_size'],
                 output_activation='tanh',
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
                 hidden_size=self.net_config['h_size'],
                 output_activation='tanh',
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
             self.critic = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.critic_target = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
                 hidden_size=self.net_config['h_size'],
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.critic_target.load_state_dict(self.critic.state_dict())
 
         elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
             self.actor = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
+                normalize=self.net_config['normalize'],
                 mlp_activation='tanh',
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
+                normalize=self.net_config['normalize'],
                 mlp_activation='tanh',
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
             self.critic = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
+                normalize=self.net_config['normalize'],
                 mlp_activation='tanh',
                 critic=True,
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.critic_target = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
                 channel_size=self.net_config['c_size'],
                 kernal_size=self.net_config['k_size'],
                 stride_size=self.net_config['s_size'],
                 hidden_size=self.net_config['h_size'],
+                normalize=self.net_config['normalize'],
                 mlp_activation='tanh',
                 critic=True,
-                device=self.device).to(
-                self.device)
+                device=self.device,
+                accelerator=self.accelerator)
             self.critic_target.load_state_dict(self.critic.state_dict())
 
-        self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.critic_optimizer = optim.Adam(
-            self.critic.parameters(), lr=self.lr)
+        self.actor_optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.critic_optimizer_type = optim.Adam(self.critic.parameters(), lr=self.lr)
+
+        if self.accelerator is not None:
+            self.actor_optimizer = self.actor_optimizer_type
+            self.critic_optimizer = self.critic_optimizer_type
+            if wrap:
+                self.wrap_models()          
+        else:
+            self.actor = self.actor.to(self.device)
+            self.actor_target = self.actor_target.to(self.device)
+            self.critic = self.critic.to(self.device)
+            self.critic_target = self.critic_target.to(self.device)
+            self.actor_optimizer = self.actor_optimizer_type
+            self.critic_optimizer = self.critic_optimizer_type
+
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. Epsilon is the probability of taking a random action, used for exploration.
+        """Returns the next action to take in the environment. 
+        Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: Environment observation, or multiple observations in a batch
         :type state: float or List[float]
-        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
+        :param epsilon: Probablilty of taking a random action for exploration, defaults 
+        to 0
         :type epsilon: float, optional
         """
-        state = torch.from_numpy(state).float().to(self.device)
+        state = torch.from_numpy(state).float()
+        if self.accelerator is None:
+            state = state.to(self.device)
 
         if self.one_hot:
             state = nn.functional.one_hot(
                 state.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if len(state.size()) < 2:
             state = state.unsqueeze(0)       
@@ -188,23 +203,35 @@
             with torch.no_grad():
                 action_values = self.actor(state)
             self.actor.train()
 
             action = action_values.cpu().data.numpy()
 
         return action
+    
+    def _squeeze_exp(self, experiences):
+        """Remove first dim created by dataloader.
+        
+        :param experiences: List of batched states, actions, rewards, next_states, 
+        dones in that order.
+        :type state: List[torch.Tensor[float]]
+        """
+        st, ac, re, ne, do = experiences
+        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
 
     def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
         """Updates agent network parameters to learn from experiences.
 
-        :param experience: List of batched states, actions, rewards, next_states, dones in that order.
+        :param experience: List of batched states, actions, rewards, next_states, 
+        dones in that order.
         :type experience: List[torch.Tensor[float]]
         :param noise_clip: Maximum noise limit to apply to actions, defaults to 0.5
         :type noise_clip: float, optional
-        :param policy_noise: Standard deviation of noise applied to policy, defaults to 0.2
+        :param policy_noise: Standard deviation of noise applied to policy, defaults 
+        to 0.2
         :type policy_noise: float, optional
         """
         states, actions, rewards, next_states, dones = experiences
 
         if self.one_hot:
             states = nn.functional.one_hot(
                 states.long(), num_classes=self.state_dim[0]).float().squeeze()
@@ -214,46 +241,52 @@
         if self.net_config['arch'] == 'mlp':
             input_combined = torch.cat([states, actions], 1)
             q_value = self.critic(input_combined)
         elif self.net_config['arch'] == 'cnn':
             q_value = self.critic(states, actions)
 
         next_actions = self.actor_target(next_states)
-        noise = actions.data.normal_(0, policy_noise).to(self.device)
+        noise = actions.data.normal_(0, policy_noise)
         noise = noise.clamp(-noise_clip, noise_clip)
         next_actions = (next_actions + noise)
 
         if self.net_config['arch'] == 'mlp':
             next_input_combined = torch.cat([next_states, next_actions], 1)
             q_value_next_state = self.critic_target(next_input_combined)
         elif self.net_config['arch'] == 'cnn':
-            q_value_next_state = self.critic(next_states, next_actions)
+            q_value_next_state = self.critic_target(next_states, next_actions)
 
-        y_j = rewards + (self.gamma * q_value_next_state).detach()
+        y_j = rewards + ((1-dones)*self.gamma * q_value_next_state).detach()
 
         critic_loss = self.criterion(q_value, y_j)
 
         # critic loss backprop
         self.critic_optimizer.zero_grad()
-        critic_loss.backward()
+        if self.accelerator is not None:
+            self.accelerator.backward(critic_loss)
+        else:
+            critic_loss.backward()
         self.critic_optimizer.step()
 
         # update actor and targets every policy_freq episodes
         if len(self.scores) % self.policy_freq == 0:
             if self.net_config['arch'] == 'mlp':
                 input_combined = torch.cat(
                     [states, self.actor.forward(states)], 1)
                 actor_loss = -self.critic(input_combined).mean()
             elif self.net_config['arch'] == 'cnn':
                 actor_loss = - \
                     self.critic(states, self.actor.forward(states)).mean()
 
             # actor loss backprop
             self.actor_optimizer.zero_grad()
-            actor_loss.backward()
+            if self.accelerator is not None:
+                self.accelerator.backward(actor_loss)
+            else:
+                actor_loss.backward()
             self.actor_optimizer.step()
 
             self.softUpdate(self.actor, self.actor_target)
             self.softUpdate(self.critic, self.critic_target)
 
     def softUpdate(self, net, target):
         """Soft updates target network.
@@ -263,41 +296,44 @@
                 self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
-        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
+        :param swap_channels: Swap image channels dimension from last to first 
+        [H, W, C] -> [C, H, W], defaults to False
         :type swap_channels: bool, optional
         :param max_steps: Maximum number of testing steps, defaults to 500
         :type max_steps: int, optional
-        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean over these tests. Defaults to 3
+        :param loop: Number of testing loops/epsiodes to complete. The returned score 
+        is the mean over these tests. Defaults to 3
         :type loop: int, optional
         """
         with torch.no_grad():
             rewards = []
             for i in range(loop):
                 state = env.reset()[0]
                 score = 0
                 for idx_step in range(max_steps):
                     if swap_channels:
                         state = np.moveaxis(state, [3], [1])
                     action = self.getAction(state, epsilon=0)
-                    state, reward, done, _, _ = env.step(action)
+                    state, reward, done, trunc, info = env.step(action)
                     score += reward
                 rewards.append(score)
         mean_fit = np.mean(rewards)
         self.fitness.append(mean_fit)
         return mean_fit
 
-    def clone(self, index=None):
+    def clone(self, index=None, wrap=True):
         """Returns cloned agent identical to self.
 
-        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
+        :param index: Index to keep track of agent for tournament selection and 
+        mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
         clone = type(self)(state_dim=self.state_dim,
                            action_dim=self.action_dim,
@@ -308,32 +344,74 @@
                            lr=self.lr,
                            learn_step=self.learn_step,
                            gamma=self.gamma,
                            tau=self.tau,
                            mutation=self.mut,
                            policy_freq=self.policy_freq,
                            device=self.device,
-                           )
-
-        clone.actor = self.actor.clone().to(self.device)
-        clone.actor_target = self.actor_target.clone().to(self.device)
-        clone.critic = self.critic.clone().to(self.device)
-        clone.critic_target = self.critic_target.clone().to(self.device)
-
-        clone.actor_optimizer = optim.Adam(
-            clone.actor.parameters(), lr=clone.lr)
-        clone.critic_optimizer = optim.Adam(
-            clone.critic.parameters(), lr=clone.lr)
+                           accelerator=self.accelerator,
+                           wrap=wrap)
+        
+        if self.accelerator is not None:
+            self.unwrap_models()
+        actor = self.actor.clone()
+        actor_target = self.actor_target.clone()
+        critic = self.critic.clone()
+        critic_target = self.critic_target.clone()
+        actor_optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
+        critic_optimizer = optim.Adam(critic.parameters(), lr=clone.lr)
+        clone.actor_optimizer_type = actor_optimizer
+        clone.critic_optimizer_type = critic_optimizer
+
+        if self.accelerator is not None:
+            if wrap:
+                clone.actor, clone.actor_target, clone.critic, clone.critic_target, \
+                clone.actor_optimizer, clone.critic_optimizer = self.accelerator.prepare(actor,
+                                                                                actor_target,
+                                                                                critic,
+                                                                                critic_target,
+                                                                                actor_optimizer,
+                                                                                critic_optimizer)
+            else:
+                clone.actor, clone.actor_target, clone.critic, clone.critic_target, \
+                clone.actor_optimizer, clone.critic_optimizer = actor, actor_target, critic, \
+                critic_target, actor_optimizer, critic_optimizer
+        else:
+            clone.actor = actor.to(self.device)
+            clone.actor_target = actor_target.to(self.device)
+            clone.critic = critic.to(self.device)
+            clone.critic_target = critic_target.to(self.device)
+            clone.actor_optimizer = actor_optimizer
+            clone.critic_optimizer = critic_optimizer
 
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
 
+    def wrap_models(self):
+        if self.accelerator is not None:
+            self.actor, self.actor_target, self.critic, self.critic_target, \
+            self.actor_optimizer, self.critic_optimizer = self.accelerator.prepare(self.actor,
+                                                                            self.actor_target,
+                                                                            self.critic,
+                                                                            self.critic_target,
+                                                                            self.actor_optimizer_type,
+                                                                            self.critic_optimizer_type)
+    
+    def unwrap_models(self):
+        if self.accelerator is not None:
+            self.actor = self.accelerator.unwrap_model(self.actor)
+            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
+            self.critic = self.accelerator.unwrap_model(self.critic)
+            self.critic_target = self.accelerator.unwrap_model(self.critic_target)
+            self.actor_optimizer = self.accelerator.unwrap_model(self.actor_optimizer)
+            self.critic_optimizer = self.accelerator.unwrap_model(self.critic_optimizer)
+
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
         torch.save({
@@ -354,50 +432,44 @@
             'gamma': self.gamma,
             'tau': self.tau,
             'mutation': self.mut,
             'index': self.index,
             'scores': self.scores,
             'fitness': self.fitness,
             'steps': self.steps,
-        }, path)
+        }, path, pickle_module=dill)
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
-        checkpoint = torch.load(path)
+        checkpoint = torch.load(path, pickle_module=dill)
         self.net_config = checkpoint['net_config']
         if self.net_config['arch'] == 'mlp':
             self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(
-                **checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
             self.critic = EvolvableMLP(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableMLP(
-                **checkpoint['critic_target_init_dict'])
+            self.critic_target = EvolvableMLP(**checkpoint['critic_target_init_dict'])
         elif self.net_config['arch'] == 'cnn':
             self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(
-                **checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
             self.critic = EvolvableCNN(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableCNN(
-                **checkpoint['critic_target_init_dict'])
+            self.critic_target = EvolvableCNN(**checkpoint['critic_target_init_dict'])
+        self.lr = checkpoint['lr']
+        self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.critic_optimizer = optim.Adam(self.critic.parameters(), lr=self.lr)
         self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(
-            checkpoint['actor_target_state_dict'])
+        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
         self.critic.load_state_dict(checkpoint['critic_state_dict'])
-        self.critic_target.load_state_dict(
-            checkpoint['critic_target_state_dict'])
-        self.actor_optimizer.load_state_dict(
-            checkpoint['actor_optimizer_state_dict'])
-        self.critic_optimizer.load_state_dict(
-            checkpoint['critic_optimizer_state_dict'])
+        self.critic_target.load_state_dict(checkpoint['critic_target_state_dict'])
+        self.actor_optimizer.load_state_dict(checkpoint['actor_optimizer_state_dict'])
+        self.critic_optimizer.load_state_dict(checkpoint['critic_optimizer_state_dict'])
         self.batch_size = checkpoint['batch_size']
-        self.lr = checkpoint['lr']
         self.learn_step = checkpoint['learn_step']
         self.gamma = checkpoint['gamma']
         self.tau = checkpoint['tau']
         self.mut = checkpoint['mutation']
         self.index = checkpoint['index']
         self.scores = checkpoint['scores']
         self.fitness = checkpoint['fitness']
```

### Comparing `agilerl-0.1.6/agilerl/algorithms/ilql.py` & `agilerl-0.1.7/agilerl/algorithms/ilql.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,19 +475,18 @@
 
     def get_dm_loss(self, qs, data_qs, terminals, margin):
         n = (1 - terminals[:, :-1]).sum()
         if self.double_q:
             q1, q2 = qs
             data_q1, data_q2 = data_qs
             return (((torch.max(q1 - data_q1.unsqueeze(-1) + margin,
-                                torch.tensor(0.0).to(self.device)) ** 2).sum(dim=-1) * (1 - terminals[:,
-                                                                                                      :-1])) + ((torch.max(q2 - data_q2.unsqueeze(-1) + margin,
-                                                                                                                           torch.tensor(0.0).to(self.device)) ** 2).sum(dim=-1) * (1 - terminals[:,
-                                                                                                                                                                                                 :-1]))).sum() / max(n.item(),
-                                                                                                                                                                                                                     1.0)
+                                torch.tensor(0.0).to(self.device)) ** 2).sum(
+                dim=-1) * (1 - terminals[:,:-1])) + ((torch.max(q2 - data_q2.unsqueeze(-1) + margin, 
+                                                                torch.tensor(0.0).to(self.device)) ** 2).sum(
+                dim=-1) * (1 - terminals[:,:-1]))).sum() / max(n.item(), 1.0)
         return ((torch.max(qs - data_qs.unsqueeze(-1) + margin, torch.tensor(0.0).to(self.device))
                 ** 2).sum(dim=-1) * (1 - terminals[:, :-1])).sum() / max(n.item(), 1.0)
 
     def prepare_inputs(self, items):
         if isinstance(items, dict):
             return items
         return to(self.dataset.collate(items, self.device), self.device)
@@ -514,17 +513,19 @@
         full_qs = qs
         if self.double_q:
             q1, q2 = qs
             q1 = torch.gather(
                 q1, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
             q2 = torch.gather(
                 q2, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
-            # tok_seq = [self.dataset.tokenizer.id_to_token(token) for token in select_tokens[0].detach().cpu().tolist()][:(1-terminals[0, :-1]).sum()]
+            # tok_seq = [self.dataset.tokenizer.id_to_token(
+            #   token) for token in select_tokens[0].detach().cpu().tolist()][:(1-terminals[0, :-1]).sum()]
             # max_q_seq = torch.max(q1, q2)[0, :(1-terminals[0, :-1]).sum()].detach().cpu().tolist()
-            # print(self.dataset.tokenizer.decode(tokens[0, :][:attn_mask[0, :].sum().long()].tolist(), clean_up_tokenization_spaces=False))
+            # print(self.dataset.tokenizer.decode(tokens[0, :][:attn_mask[0, :].sum().long()].tolist(), 
+            #   clean_up_tokenization_spaces=False))
             # print(list(zip(tok_seq, max_q_seq)))
             # print(rs)
             qs = (q1, q2,)
         else:
             qs = torch.gather(
                 qs, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
         dm_term = self.get_dm_loss(full_qs, qs, terminals, self.dm_margin)
@@ -627,15 +628,17 @@
                          (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), 1)
         act_weights = torch.gather(weights, dim=1, index=a_idx)
         logs['act_weight_avg'] = (
             ((act_weights * (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), n)
         logs['transformer'] = transformer_logs
 
         def postproc_f(x):
-            return x.update({'loss': awac_weight * x['token_loss'] + q_loss_weight * x['q_loss'] + v_loss_weight * x['v_loss'] + cql_loss_weight * x['cql_loss'] + dm_loss_weight * x['dm_loss']})
+            return x.update({'loss': awac_weight * x['token_loss'] + q_loss_weight * x[
+                'q_loss'] + v_loss_weight * x['v_loss'] + cql_loss_weight * x[
+                    'cql_loss'] + dm_loss_weight * x['dm_loss']})
         def hist_f(x):
             return x.update({'advantage_hist': wandb.Histogram(advantages)})
         
         return loss, logs, [postproc_f, hist_f]
 
     def score(self,
               tokens: torch.Tensor,
@@ -979,40 +982,47 @@
             max_length = self.iql_model.model.block_size
         max_length = min(max_length, self.iql_model.model.block_size)
         device = self.iql_model.device
         bsize = tokens.shape[0]
         n = bsize * num_generations
         if max_generation_len is None:
             max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
+                                       clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
         model_outputs = self.iql_model(tokens, 
                                        state_idxs, action_idxs, attn_mask,
                                        prefix_embs=prefix_embs, 
                                        prefix_attn_mask=prefix_attn_mask, 
                                        remove_prefix_position_embs=remove_prefix_position_embs,
                                        is_causal=False)['model_outputs']
         kvs = {'qv': model_outputs['qv_model_outputs']['past_key_values']}
         if self.iql_model.actor_target is not None:
             kvs['target'] = model_outputs['target_model_outputs']['past_key_values']
         if self.iql_model.actor is not None:
             kvs['policy'] = model_outputs['policy_model_outputs']['past_key_values']
         dialogue_lens = attn_mask.sum(dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), max_length, tokenizer.pad_token_id, device, 1)
+        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), max_length, 
+                              tokenizer.pad_token_id, device, 1)
         dialogue_lens = torch.repeat_interleave(dialogue_lens, num_generations, dim=0)
-        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), max_length, 0.0, device, 2), kvs['qv'])
+        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
+                                                       max_length, 0.0, device, 2), kvs['qv'])
         if 'target' in kvs:
-            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), max_length, 0.0, device, 2), kvs['target'])
+            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
+                                                               max_length, 0.0, device, 2), kvs['target'])
         if 'policy' in kvs:
-            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), max_length, 0.0, device, 2), kvs['policy'])
+            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
+                                                               max_length, 0.0, device, 2), kvs['policy'])
         log_probs = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
-        kls = torch.full((dialogue_lens.shape[0],), math.log(num_generations)-((num_generations-1)/num_generations)).to(device)
+        kls = torch.full((dialogue_lens.shape[0],), math.log(
+            num_generations)-((num_generations-1)/num_generations)).to(device)
         advantages = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         termination_mask = torch.full((dialogue_lens.shape[0],), 1).to(device)
-        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device)
+        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), \
+            torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device)
         t = torch.min(dialogue_lens).int()
         base_logits = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
             curr_token = tokens[:, t-1].unsqueeze(1)
             curr_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['qv'])
             curr_target_kvs, curr_policy_kvs = curr_kvs, curr_kvs
             if 'target' in kvs:
@@ -1023,64 +1033,79 @@
                                          qv_kwargs={'past_key_values': curr_kvs}, 
                                          policy_kwargs={'past_key_values': curr_policy_kvs}, 
                                          target_kwargs={'past_key_values': curr_target_kvs},
                                          is_causal=False)
             model_outputs, logits = iql_outputs['model_outputs'], iql_outputs['logits']
             
             logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
+                device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full(
+                (n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
             edited_logits = process_logits(logits.clone(), temp=temp, top_k=top_k, top_p=top_p)
 
             vs, qs = iql_outputs['target_vs'], iql_outputs['target_qs']
             if exp_adv:
                 adv_logits = adv_weight * (qs - vs.unsqueeze(2))
             else:
                 adv_sign = ((qs - vs.unsqueeze(2)) > 0.0).float()
                 adv_logits = adv_weight * adv_sign + (1 - adv_weight) * (1 - adv_sign)
                 adv_logits = torch.log(adv_logits)
             if adv_clip is not None:
                 adv_logits = torch.clip(adv_logits, max=adv_clip)
             adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
+                device), tokens[:, t]] = adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
+                device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
 
-            full_logits = (edited_logits if include_logits else 0.0) + (adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
+            full_logits = (edited_logits if include_logits else 0.0) + (
+                adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
 
             cat_dist = torch.distributions.categorical.Categorical(logits=full_logits[:, 0])
             original_cat_dist = torch.distributions.categorical.Categorical(logits=logits[:, 0])
 
             new_tokens = cat_dist.sample()
             log_probs += cat_dist.log_prob(new_tokens)
             kls += (cat_dist.log_prob(new_tokens) - original_cat_dist.log_prob(new_tokens))
             qs_chosen = torch.gather(qs.squeeze(1), dim=1, index=new_tokens.unsqueeze(1)).squeeze(1)
             advantages += (qs_chosen - vs.squeeze(1))
             tokens[:, t] = new_tokens
-            kvs['qv'] = update_kvs(kvs['qv'], model_outputs['qv_model_outputs']['past_key_values'], torch.arange(0, n).to(device), (t+prefix_t)-1)
+            kvs['qv'] = update_kvs(kvs['qv'], 
+                                   model_outputs['qv_model_outputs']['past_key_values'], 
+                                   torch.arange(0, n).to(device), (t+prefix_t)-1)
             if 'target' in kvs:
-                kvs['target'] = update_kvs(kvs['target'], model_outputs['target_model_outputs']['past_key_values'], torch.arange(0, n).to(device), (t+prefix_t)-1)
+                kvs['target'] = update_kvs(kvs['target'], 
+                                           model_outputs['target_model_outputs']['past_key_values'], 
+                                           torch.arange(0, n).to(device), (t+prefix_t)-1)
             if 'policy' in kvs:
-                kvs['policy'] = update_kvs(kvs['policy'], model_outputs['policy_model_outputs']['past_key_values'], torch.arange(0, n).to(device), (t+prefix_t)-1)
+                kvs['policy'] = update_kvs(kvs['policy'], 
+                                           model_outputs['policy_model_outputs']['past_key_values'], 
+                                           torch.arange(0, n).to(device), (t+prefix_t)-1)
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
                     termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(), 
                                                                                              clean_up_tokenization_spaces=False))))
             t += 1
             termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
 
-        scores = ((advantages * rerank_advantage_weight) + (log_probs * rerank_log_prob_weight)).reshape(-1, num_generations)
+        scores = ((advantages * rerank_advantage_weight) + (
+            log_probs * rerank_log_prob_weight)).reshape(-1, num_generations)
         order = torch.argsort(-scores, dim=1)
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        output_strs = [tokenizer.decode(tokens[i, :].tolist(), 
+                                        clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(num_generations):
                 processed_str = output_strs[i*num_generations+order[i, x]][len(input_strs[i]):].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(
+                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         scores = torch.gather(scores, dim=1, index=order)
         log_probs = torch.gather(log_probs.reshape(-1, num_generations), dim=1, index=order)
         kls = torch.gather(kls.reshape(-1, num_generations), dim=1, index=order)
         return list(zip(input_strs, processed_outputs)), log_probs.reshape(-1, num_generations), kls
     
@@ -1102,39 +1127,45 @@
             max_length = self.iql_model.model.block_size
         max_length = min(max_length, self.iql_model.model.block_size)
         device = self.iql_model.device
         bsize, vocab_size = tokens.shape[0], tokenizer.num_tokens()
         n = bsize * beam_width
         if max_generation_len is None:
             max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
+                                       clean_up_tokenization_spaces=False) for i in range(len(tokens))]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
         model_outputs = self.iql_model(tokens, state_idxs, action_idxs, attn_mask,
                                        prefix_embs=prefix_embs, prefix_attn_mask=prefix_attn_mask,
                                        remove_prefix_position_embs=remove_prefix_position_embs,
                                        is_causal=False)['model_outputs']
         kvs = {'qv': model_outputs['qv_model_outputs']['past_key_values']}
         if self.iql_model.actor_target is not None:
             kvs['target'] = model_outputs['target_model_outputs']['past_key_values']
         if self.iql_model.actor is not None:
             kvs['policy'] = model_outputs['policy_model_outputs']['past_key_values']
         original_dialogue_lens = attn_mask.sum(dim=1)
         batch_indicator = torch.stack(beam_width*[torch.arange(0, bsize).to(device)], dim=1)
 
-        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), max_length, tokenizer.pad_token_id, device, 1)
+        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), max_length, 
+                              tokenizer.pad_token_id, device, 1)
         dialogue_lens = torch.repeat_interleave(original_dialogue_lens, beam_width, dim=0)
-        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), max_length, 0.0, device, 2), kvs['qv'])
+        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
+                                                       max_length, 0.0, device, 2), kvs['qv'])
         if 'target' in kvs:
-            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), max_length, 0.0, device, 2), kvs['target'])
+            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
+                                                               max_length, 0.0, device, 2), kvs['target'])
         if 'policy' in kvs:
-            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), max_length, 0.0, device, 2), kvs['policy'])
+            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
+                                                               max_length, 0.0, device, 2), kvs['policy'])
         curr_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         logit_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         termination_mask = torch.full((n,), 1).to(device)
-        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device)
+        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), torch.zeros(
+            (dialogue_lens.shape[0], 1,)).long().to(device)
         t = torch.min(dialogue_lens).int()
         base_logits = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
             curr_token = tokens[:, t-1].unsqueeze(1)
             curr_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['qv'])
             curr_target_kvs, curr_policy_kvs = curr_kvs, curr_kvs
             if 'target' in kvs:
@@ -1148,49 +1179,67 @@
                                          qv_kwargs={'past_key_values': curr_kvs}, 
                                          policy_kwargs={'past_key_values': curr_policy_kvs}, 
                                          target_kwargs={'past_key_values': curr_target_kvs}, 
                                          is_causal=False)
             model_outputs, logits = iql_outputs['model_outputs'], iql_outputs['logits']
             
             logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(
+                0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
             edited_logits = process_logits(logits.clone(), temp=temp, top_k=top_k, top_p=top_p)
             
             vs, qs = iql_outputs['target_vs'], iql_outputs['target_qs']
             if exp_adv:
                 adv_logits = adv_weight * (qs - vs.unsqueeze(2))
             else:
                 adv_sign = ((qs - vs.unsqueeze(2)) > 0.0).float()
                 adv_logits = adv_weight * adv_sign + (1 - adv_weight) * (1 - adv_sign)
                 adv_logits = torch.log(adv_logits)
             if adv_clip is not None:
                 adv_logits = torch.clip(adv_logits, max=adv_clip)
             adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
+            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = adv_logits[
+                torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(
+                t < dialogue_lens, 1e7)
 
-            full_logits = (edited_logits if include_logits else 0.0) + (adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
+            full_logits = (edited_logits if include_logits else 0.0) + (
+                adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
             
-            scores = (torch.log(F.softmax(full_logits, dim=-1)).reshape(1, bsize, beam_width, -1).permute(3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(1, bsize, -1)  # (time, batch, k*vocab)
-            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_((t == original_dialogue_lens).unsqueeze(1).repeat(1, scores.shape[2]-vocab_size), float('-inf'))
+            scores = (torch.log(F.softmax(full_logits, dim=-1)).reshape(1, bsize, beam_width, -1).permute(
+                3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(1, bsize, -1)  # (time, batch, k*vocab)
+            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_((t == original_dialogue_lens).unsqueeze(
+                1).repeat(1, scores.shape[2]-vocab_size), float('-inf'))
             curr_scores, top_k_ = torch.topk(scores[0, :, :], k=beam_width, dim=1)  # (batch, k), (batch, k)
             tokens = tokens[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1), :]
             logits = logits[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1), :, :]
-            logit_scores += torch.gather(torch.log(F.softmax(logits, dim=-1)).squeeze(1), dim=1, index=(top_k_.reshape(-1) % vocab_size).unsqueeze(1)).squeeze(1).reshape(-1, beam_width)
+            logit_scores += torch.gather(torch.log(F.softmax(logits, dim=-1)).squeeze(1), dim=1, index=(top_k_.reshape(
+                -1) % vocab_size).unsqueeze(1)).squeeze(1).reshape(-1, beam_width)
             tokens[:, t] = top_k_.reshape(-1) % vocab_size  # (batch*k,)
-            fixed_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], model_outputs['qv_model_outputs']['past_key_values'])
-            kvs['qv'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['qv'])
+            fixed_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
+                model_outputs['qv_model_outputs']['past_key_values'])
+            kvs['qv'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['qv'])
             kvs['qv'] = update_kvs(kvs['qv'], fixed_kvs, torch.arange(0, n).to(device), (t+prefix_t)-1)
             if 'target' in kvs:
-                fixed_target_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], model_outputs['target_model_outputs']['past_key_values'])
-                kvs['target'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['target'])
-                kvs['target'] = update_kvs(kvs['target'], fixed_target_kvs, torch.arange(0, n).to(device), (t+prefix_t)-1)
+                fixed_target_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
+                    model_outputs['target_model_outputs']['past_key_values'])
+                kvs['target'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['target'])
+                kvs['target'] = update_kvs(kvs['target'], fixed_target_kvs, torch.arange(0, n).to(device), 
+                                           (t+prefix_t)-1)
             if 'policy' in kvs:
-                fixed_policy_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], model_outputs['policy_model_outputs']['past_key_values'])
-                kvs['policy'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['policy'])
-                kvs['policy'] = update_kvs(kvs['policy'], fixed_policy_kvs, torch.arange(0, n).to(device), (t+prefix_t)-1)
+                fixed_policy_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
+                    model_outputs['policy_model_outputs']['past_key_values'])
+                kvs['policy'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
+                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['policy'])
+                kvs['policy'] = update_kvs(kvs['policy'], fixed_policy_kvs, torch.arange(0, n).to(device), 
+                                           (t+prefix_t)-1)
             termination_mask = termination_mask[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1)]
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
                     termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(),
                                                                                              clean_up_tokenization_spaces=False))))
             t += 1
             termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
@@ -1198,17 +1247,19 @@
         output_strs = [tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False) for i in range(n)]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(beam_width):
                 processed_str = output_strs[i*beam_width+x][len(input_strs[i]):].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(
+                        tokenizer.pad_token_id))].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(
+                        tokenizer.eoa_token_id))].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         return list(zip(input_strs, processed_outputs)), curr_scores, -logit_scores
 
     def generate(self, items, 
                  termination_condition: Callable[[np.ndarray], bool], **kwargs):
         prepared_inputs = self.iql_model.prepare_inputs(items)
@@ -1268,15 +1319,17 @@
                 print('env reward:', env_reward)
                 print('avg token reward:', total_token_reward / (i + 1))
                 print('avg env reward:', total_env_reward / (i + 1))
                 print('='*25)
         kl_total = sum(policy.kls_all)
         entropy_total = -sum(policy.logprobs_all)
         self.all_entropy.extend(policy.logprobs_all)
-        return {'token_reward': (total_token_reward / tokens.shape[0], tokens.shape[0]), 'env_reward': (total_env_reward / tokens.shape[0], tokens.shape[0]), 'kl': (kl_total / len(policy.kls_all), len(policy.kls_all)), 
+        return {'token_reward': (total_token_reward / tokens.shape[0], tokens.shape[0]), 'env_reward': (
+            total_env_reward / tokens.shape[0], tokens.shape[0]), 'kl': (kl_total / len(policy.kls_all), len(
+            policy.kls_all)), 
                 'entropy': (entropy_total / len(policy.logprobs_all), len(policy.logprobs_all))}
     
     def dump(self):
         return {'results': self.all_results, 'entropies': self.all_entropy}
 
 
 class TopAdvantageNGrams():
@@ -1303,21 +1356,23 @@
                     if x-self.n_gram >= 0 and a_idx[0, x-self.n_gram].item() > a_idx[0, start_idx].item():
                         start_idx = x-self.n_gram
                     if x-start_idx < self.n_gram:
                         continue
                 elif select_tokens[x].item() != self.data.tokenizer.eoa_token_id:
                     continue
                 total_advantage = advantages[start_idx:x].sum().item()
-                utterance = self.data.tokenizer.decode(tokens[0, (a_idx[0, start_idx].item()+1):(a_idx[0, x].item()+1)].detach().cpu().tolist())
+                utterance = self.data.tokenizer.decode(tokens[0, (
+                    a_idx[0, start_idx].item()+1):(a_idx[0, x].item()+1)].detach().cpu().tolist())
                 top_actions[utterance] += total_advantage
                 total_actions[utterance] += 1
                 if select_tokens[x].item() == self.data.tokenizer.eoa_token_id:
                     curr_idx = x+1
             if i % self.print_every == 0:
-                ranked_actions = sorted({k: top_actions[k] / total_actions[k] for k in total_actions.keys()}.items(), key=lambda x: x[1])
+                ranked_actions = sorted(
+                    {k: top_actions[k] / total_actions[k] for k in total_actions.keys()}.items(), key=lambda x: x[1])
                 print(ranked_actions[-self.print_k:])
                 print(ranked_actions[:self.print_k])
 
 def interact_environment(env, policy, obs):
     obs_sequence = []
     if obs is None:
         obs = env.reset()
```

### Comparing `agilerl-0.1.6/agilerl/components/replay_buffer.py` & `agilerl-0.1.7/agilerl/components/replay_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import torch
 import numpy as np
 from collections import deque, namedtuple
 import random
 
 
 class ReplayBuffer():
-    """The Experience Replay Buffer class. Used to store experiences and allow off-policy learning.
+    """The Experience Replay Buffer class. Used to store experiences and allow 
+    off-policy learning.
 
     :param n_actions: Action dimension
     :type n_actions: int
     :param memory_size: Maximum length of replay buffer
     :type memory_size: int
-    :param field_names: Field names for experience named tuple, e.g. ['state', 'action', 'reward']
+    :param field_names: Field names for experience named tuple, 
+    e.g. ['state', 'action', 'reward']
     :type field_names: List[str]
-    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
+    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to None
     :type device: str, optional
     """
 
-    def __init__(self, action_dim, memory_size, field_names, device='cpu'):
+    def __init__(self, action_dim, memory_size, field_names, device=None):
         self.n_actions = action_dim
         self.memory = deque(maxlen=memory_size)
         self.experience = namedtuple("Experience", field_names=field_names)
         self.counter = 0    # update cycle counter
         self.device = device
 
     def __len__(self):
@@ -36,23 +38,28 @@
 
         :param batch_size: Number of samples to return
         :type batch_size: int
         """
         experiences = random.sample(self.memory, k=batch_size)
 
         states = torch.from_numpy(np.stack(
-            [e.state for e in experiences if e is not None], axis=0)).to(self.device)
+            [e.state for e in experiences if e is not None], axis=0))
         actions = torch.from_numpy(
-            np.vstack([e.action for e in experiences if e is not None])).to(self.device)
+            np.vstack([e.action for e in experiences if e is not None]))
         rewards = torch.from_numpy(np.vstack(
-            [e.reward for e in experiences if e is not None])).float().to(self.device)
+            [e.reward for e in experiences if e is not None])).float()
         next_states = torch.from_numpy(np.stack(
-            [e.next_state for e in experiences if e is not None], axis=0)).float().to(self.device)
+            [e.next_state for e in experiences if e is not None], axis=0)).float()
         dones = torch.from_numpy(np.vstack([e.done for e in experiences if e is not None]).astype(
-            np.uint8)).float().to(self.device)
+            np.uint8)).float()
+        
+        if self.device is not None:
+            states, actions, rewards, next_states, dones = states.to(self.device), \
+                actions.to(self.device), rewards.to(self.device), \
+                    next_states.to(self.device), dones.to(self.device)
 
         return (states, actions, rewards, next_states, dones)
 
     def save2memory(self, state, action, reward, next_state, done):
         """Saves experience to memory.
 
         :param state: Environment observation
```

### Comparing `agilerl-0.1.6/agilerl/data/language_environment.py` & `agilerl-0.1.7/agilerl/data/language_environment.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/data/rl_data.py` & `agilerl-0.1.7/agilerl/data/rl_data.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/data/tokenizer.py` & `agilerl-0.1.7/agilerl/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/data/torch_datasets.py` & `agilerl-0.1.7/agilerl/data/torch_datasets.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/hpo/mutation.py` & `agilerl-0.1.7/agilerl/hpo/mutation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 import fastrand
 
 
 class Mutations():
     """The Mutations class for evolutionary hyperparameter optimization.
 
-    :param algo: RL algorithm used. Use str e.g. 'DQN' if using AgileRL implementation of algorithm, or provide a dict with names of agent networks
+    :param algo: RL algorithm used. Use str e.g. 'DQN' if using AgileRL implementation of algorithm, or provide a dict 
+    with names of agent networks
     :type algo: str or dict
     :param no_mutation: Relative probability of no mutation
     :type no_mutation: float
     :param architecture: Relative probability of architecture mutation
     :type architecture: float
     :param new_layer_prob: Relative probability of new layer mutation (type of architecture mutation)
     :type new_layer_prob: float
@@ -25,56 +26,46 @@
     :type mutation_sd: float
     :param arch: Network architecture type. 'mlp' or 'cnn', defaults to 'mlp'
     :type arch: str, optional
     :param rand_seed: Random seed for repeatability, defaults to None
     :type rand_seed: int, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
-    def __init__(
-            self,
-            algo,
-            no_mutation,
-            architecture,
-            new_layer_prob,
-            parameters,
-            activation,
-            rl_hp,
-            rl_hp_selection,
-            mutation_sd,
-            arch='mlp',
-            rand_seed=None,
-            device='cpu'):
+    def __init__(self, algo, no_mutation, architecture, new_layer_prob, parameters, 
+                 activation, rl_hp, rl_hp_selection, mutation_sd, arch='mlp', 
+                 rand_seed=None, device='cpu', accelerator=None):
         # Random seed for repeatability
         self.rng = np.random.RandomState(rand_seed)
 
         self.arch = arch    # Network architecture type
 
         # Relative probabilities of mutation
         self.no_mut = no_mutation               # No mutation
         self.architecture_mut = architecture    # Architecture mutation
         # New layer mutation (type of architecture mutation)
         self.new_layer_prob = new_layer_prob
         self.parameters_mut = parameters        # Network parameters mutation
         self.activation_mut = activation        # Activation layer mutation
         self.rl_hp_mut = rl_hp                  # Learning HP mutation
-
         self.rl_hp_selection = rl_hp_selection  # Learning HPs to choose from
         self.mutation_sd = mutation_sd          # Mutation strength
+        self.device = device
+        self.accelerator = accelerator
 
         # Set algorithm dictionary with agent network names for mutation
         # Use custom agent dict, or pre-configured agent from API
         if isinstance(algo, dict):
             self.algo = algo
         else:
             self.algo = self.get_algo_nets(algo)
 
-        self.device = device
-
     def no_mutation(self, individual):
         """Returns individual from population without mutation.
 
         :param individual: Individual agent from population
         :type individual: object
         """
         individual.mut = 'None'  # No mutation
@@ -126,31 +117,64 @@
 
             offspring_actor = getattr(individual, self.algo['actor']['eval'])
 
             # Reinitialise target network with frozen weights due to potential
             # mutation in architecture of value network
             ind_target = type(offspring_actor)(**offspring_actor.init_dict)
             ind_target.load_state_dict(offspring_actor.state_dict())
-            setattr(individual, self.algo['actor']
-                    ['target'], ind_target.to(self.device))
+            if self.accelerator is not None:
+                setattr(individual, self.algo['actor']['target'], ind_target)
+            else:
+                setattr(individual, self.algo['actor']['target'], 
+                        ind_target.to(self.device))
 
             # If algorithm has critics, reinitialize their respective target networks
             # too
             for critic in self.algo['critics']:
                 offspring_critic = getattr(individual, critic['eval'])
                 ind_target = type(offspring_critic)(
                     **offspring_critic.init_dict)
                 ind_target.load_state_dict(offspring_critic.state_dict())
-                setattr(individual, critic['target'],
-                        ind_target.to(self.device))
+                if self.accelerator is not None:
+                    setattr(individual, critic['target'], ind_target)
+                else:
+                    setattr(individual, critic['target'],
+                            ind_target.to(self.device))
 
             mutated_population.append(individual)
 
         return mutated_population
 
+    def reinit_opt(self, individual):
+        # Reinitialise optimizer
+        actor_opt = getattr(individual, self.algo['actor']['optimizer'])
+        net_params = getattr(
+            individual, self.algo['actor']['eval']).parameters()
+        if self.accelerator is not None:
+            setattr(individual, 
+                    self.algo['actor']['optimizer'].replace('_type', ''), 
+                    type(actor_opt)(net_params, lr=individual.lr))
+        else:
+            setattr(individual, 
+                    self.algo['actor']['optimizer'].replace('_type', ''), 
+                    type(actor_opt)(net_params, lr=individual.lr))
+
+        # If algorithm has critics, reinitialise their optimizers too
+        for critic in self.algo['critics']:
+            critic_opt = getattr(individual, critic['optimizer'])
+            net_params = getattr(individual, critic['eval']).parameters()
+            if self.accelerator is not None:
+                setattr(individual, 
+                        critic['optimizer'].replace('_type', ''), 
+                        type(critic_opt)(net_params, lr=individual.lr))
+            else:
+                setattr(individual, 
+                        critic['optimizer'].replace('_type', ''), 
+                        type(critic_opt)(net_params, lr=individual.lr))
+
     def rl_hyperparam_mutation(self, individual):
         """Returns individual from population with RL hyperparameter mutation.
 
         :param individual: Individual agent from population
         :type individual: object
         """
         # Learning hyperparameter mutation
@@ -172,26 +196,15 @@
         elif mutate_param == 'lr':
             if random_num > 0.5:
                 individual.lr = min(0.005, max(0.00001, individual.lr * 1.2))
             else:
                 individual.lr = min(0.005, max(0.00001, individual.lr * 0.8))
 
             # Reinitialise optimizer if new learning rate
-            actor_opt = getattr(individual, self.algo['actor']['optimizer'])
-            net_params = getattr(
-                individual, self.algo['actor']['eval']).parameters()
-            setattr(individual, self.algo['actor']['optimizer'], type(
-                actor_opt)(net_params, lr=individual.lr))
-
-            # If algorithm has critics, reinitialise their optimizers too
-            for critic in self.algo['critics']:
-                critic_opt = getattr(individual, critic['optimizer'])
-                net_params = getattr(individual, critic['eval']).parameters()
-                setattr(individual, critic['optimizer'], type(
-                    critic_opt)(net_params, lr=individual.lr))
+            self.reinit_opt(individual)
             individual.mut = 'lr'
 
         elif mutate_param == 'learn_step':
             if random_num > 0.5:
                 individual.learn_step = min(
                     1, max(0, int(individual.learn_step * 1.5)))
             else:
@@ -205,28 +218,39 @@
 
         :param individual: Individual agent from population
         :type individual: object
         """
         if individual.algo == 'DDPG':   # Needs to stay tanh for DDPG continuous actions
             individual.mut = 'None'
             return individual
+        
+        if individual.algo == 'TD3':   # Needs to stay tanh for TD3 continuous actions
+            individual.mut = 'None'
+            return individual
 
         # Mutate network activation layer
         offspring_actor = getattr(individual, self.algo['actor']['eval'])
         offspring_actor = self._permutate_activation(
             offspring_actor)   # Mutate activation function
-        setattr(individual, self.algo['actor']
-                ['eval'], offspring_actor.to(self.device))
+        if self.accelerator is not None:
+            setattr(individual, self.algo['actor']
+                    ['eval'], offspring_actor)
+        else:
+            setattr(individual, self.algo['actor']
+                    ['eval'], offspring_actor.to(self.device))
 
         # If algorithm has critics, mutate their activations too
         for critic in self.algo['critics']:
             offspring_critic = getattr(individual, critic['eval'])
             offspring_critic = self._permutate_activation(offspring_critic)
-            setattr(individual, critic['eval'],
-                    offspring_critic.to(self.device))
+            if self.accelerator is not None:
+                setattr(individual, critic['eval'], offspring_critic)
+            else:
+                setattr(individual, critic['eval'],
+                        offspring_critic.to(self.device))
 
         individual.mut = 'act'
         return individual
 
     def _permutate_activation(self, network):
         # Function to change network activation layer
         possible_activations = ['relu', 'elu', 'gelu']
@@ -245,28 +269,34 @@
             net_dict['cnn_activation'] = new_activation
         else:   # mlp, gpt or bert
             net_dict['activation'] = new_activation
         new_network = type(network)(**net_dict)
         new_network.load_state_dict(network.state_dict())
         network = new_network
 
-        return network.to(self.device)
+        if self.accelerator is None:
+            network = network.to(self.device)
+
+        return network
 
     def parameter_mutation(self, individual):
         """Returns individual from population with network parameters mutation.
 
         :param individual: Individual agent from population
         :type individual: object
         """
         # Mutate network parameters
         offspring_actor = getattr(individual, self.algo['actor']['eval'])
         offspring_actor = self.classic_parameter_mutation(
             offspring_actor)  # Network parameter mutation function
-        setattr(individual, self.algo['actor']
-                ['eval'], offspring_actor.to(self.device))
+        if self.accelerator is not None:
+            setattr(individual, self.algo['actor']['eval'], offspring_actor)
+        else:
+            setattr(individual, self.algo['actor']
+                    ['eval'], offspring_actor.to(self.device))
         individual.mut = 'param'
         return individual
 
     def regularize_weight(self, weight, mag):
         if weight > mag:
             weight = mag
         if weight < -mag:
@@ -318,15 +348,19 @@
                 else:  # mutauion even normal
                     W[ind_dim1, ind_dim2] += self.rng.normal(
                         0, np.abs(mut_strength * W[ind_dim1, ind_dim2].item()))
 
                 # Regularization hard limit
                 W[ind_dim1, ind_dim2] = self.regularize_weight(
                     W[ind_dim1, ind_dim2].item(), 1000000)
-        return network.to(self.device)
+        
+        if self.accelerator is None:
+            network = network.to(self.device)
+
+        return network
 
     def architecture_mutate(self, individual):
         """Returns individual from population with network architecture mutation.
 
         :param individual: Individual agent from population
         :type individual: object
         """
@@ -410,20 +444,27 @@
                     for offspring_critic in offspring_critics:
                         offspring_critic.add_node(**node_dict)
                 else:
                     node_dict = offspring_actor.remove_node()
                     for offspring_critic in offspring_critics:
                         offspring_critic.remove_node(**node_dict)
 
-        setattr(individual, self.algo['actor']
-                ['eval'], offspring_actor.to(self.device))
+        if self.accelerator is not None:
+            setattr(individual, self.algo['actor']['eval'], offspring_actor)
+        else:
+            setattr(individual, self.algo['actor']
+                    ['eval'], offspring_actor.to(self.device))
         for offspring_critic, critic in zip(offspring_critics, self.algo['critics']):
-            setattr(individual, critic['eval'],
-                    offspring_critic.to(self.device))
+            if self.accelerator is not None:
+                setattr(individual, critic['eval'], offspring_critic)
+            else:
+                setattr(individual, critic['eval'],
+                        offspring_critic.to(self.device))
 
+        self.reinit_opt(individual) # Reinitialise optimizer
         individual.mut = 'arch'
         return individual
 
     def get_algo_nets(self, algo):
         """Returns dictionary with agent network names.
 
         :param algo: RL algorithm
@@ -431,43 +472,60 @@
         """
         # Function to return dictionary with names of agent networks to allow mutation
         if algo == 'DQN':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
-                    'optimizer': 'optimizer'
+                    'optimizer': 'optimizer_type'
                 },
                 'critics': []
             }
         elif algo == 'DDPG':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
-                    'optimizer': 'actor_optimizer'
+                    'optimizer': 'actor_optimizer_type'
                 },
                 'critics': [{
                     'eval': 'critic',
                     'target': 'critic_target',
-                    'optimizer': 'critic_optimizer'
+                    'optimizer': 'critic_optimizer_type'
                 }]
             }
         elif algo == 'CQN':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
-                    'optimizer': 'optimizer'
+                    'optimizer': 'optimizer_type'
                 },
                 'critics': []
             }
         elif algo == 'ILQL':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
                     'optimizer': 'optimizer'
                 },
                 'critics': []
             }
+        elif algo == 'TD3':
+            nets = {
+                'actor': {
+                    'eval': 'actor',
+                    'target': 'actor_target',
+                    'optimizer': 'actor_optimizer'
+                },
+                'critics': [{
+                    'eval': 'critic_1',
+                    'target': 'critic_target_1',
+                    'optimizer': 'critic_1_optimizer'
+                },{
+                    'eval': 'critic_2',
+                    'target': 'critic_target_2',
+                    'optimizer': 'critic_2_optimizer'
+                }]
+            }
         return nets
```

### Comparing `agilerl-0.1.6/agilerl/hpo/tournament.py` & `agilerl-0.1.7/agilerl/hpo/tournament.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,24 +36,25 @@
         """
         last_fitness = [np.mean(indi.fitness[-self.evo_step:])
                         for indi in population]
         rank = np.argsort(last_fitness).argsort()
 
         max_id = max([ind.index for ind in population])
 
-        elite = copy.deepcopy([population[np.argsort(rank)[-1]]][0])
+        model = population[np.argsort(rank)[-1]]
+        elite = copy.deepcopy(model)
 
         new_population = []
         if self.elitism:  # keep top agent in population
-            new_population.append(elite.clone())
+            new_population.append(elite.clone(wrap=False))
             selection_size = self.population_size - 1
         else:
             selection_size = self.population_size
 
         # select parents of next gen using tournament selection
         for idx in range(selection_size):
             max_id += 1
             actor_parent = population[self._tournament(rank)]
-            new_individual = actor_parent.clone(max_id)
+            new_individual = actor_parent.clone(max_id, wrap=False)
             new_population.append(new_individual)
 
         return elite, new_population
```

### Comparing `agilerl-0.1.6/agilerl/networks/evolvable_bert.py` & `agilerl-0.1.7/agilerl/networks/evolvable_bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     :type n_head: int, optional
     :param dropout: Dropout value, defaults to 0.1
     :type dropout: float, optional
     :param activation: Activation function of encoder/decoder intermediate layer, defaults to 'relu'
     :type activation: str, optional
     :param layer_norm_eps: Epsilon value in layer normalization components, defaults to 1e-5
     :type layer_norm_eps: float, optional
-    :param batch_first: Input and output tensor order. If True, (batch, seq, feature). If False, (seq, batch, feature). Defaults to False
+    :param batch_first: Input and output tensor order. If True, (batch, seq, feature). If False, (seq, batch, feature). 
+    Defaults to False
     :type batch_first: bool, optional
     :param norm_first: Perform LayerNorm before other attention and feedforward operations, defaults to False
     :type norm_first: bool, optional
     :param max_encoder_layers: Maximum number of encoder layers, defaults to 12
     :type max_encoder_layers: int, optional
     :param max_decoder_layers: Maximum number of decoder layers, defaults to 12
     :type max_decoder_layers: int, optional
@@ -173,15 +174,16 @@
                 self.d_model, eps=self.layer_norm_eps, device=self.device)
 
         self._reset_parameters()
 
         return nn.ModuleDict(encoder_dict), nn.ModuleDict(decoder_dict)
 
     def generate_square_subsequent_mask(self, sz):
-        """Returns a square mask for the sequence that prevents the model from looking into the future words when making predictions.
+        """Returns a square mask for the sequence that prevents the model from looking into the future words when 
+        making predictions.
         The masked positions are filled with float('-inf'). Unmasked positions are filled with float(0.0).
 
         :param sz: Size of mask to generate
         :type sz: int
         """
         mask = (torch.triu(torch.ones((sz, sz), device=self.device))
                 == 1).transpose(0, 1)
@@ -243,15 +245,16 @@
         :type memory_mask: torch.Tensor, optional
         :param src_key_padding_mask: Tensor mask for src keys per batch, defaults to None
         :type src_key_padding_mask: torch.Tensor, optional
         :param tgt_key_padding_mask: Tensor mask for tgt keys per batch, defaults to None
         :type tgt_key_padding_mask: torch.Tensor, optional
         :param memory_key_padding_mask: Tensor mask for memory keys per batch, defaults to None
         :type memory_key_padding_mask: torch.Tensor, optional
-        :param is_causal: Applies a causal mask as mask and ignores attn_mask for computing scaled dot product attention, defaults to False
+        :param is_causal: Applies a causal mask as mask and ignores attn_mask for computing scaled dot product 
+        attention, defaults to False
         :type is_causal: bool, optional
         """
         encoder_output, encoder_hidden_states = self.encode(
             src, src_mask, src_key_padding_mask, is_causal)
         memory = encoder_output
         decoder_output, decoder_hidden_states = self.decode(
             tgt, memory, tgt_mask, memory_mask, tgt_key_padding_mask, memory_key_padding_mask)
@@ -266,15 +269,16 @@
 
         :param src: Encoder input sequence
         :type src: torch.Tensor
         :param src_mask: Additive mask for the src sequence, defaults to None
         :type src_mask: torch.Tensor, optional
         :param src_key_padding_mask: Tensor mask for src keys per batch, defaults to None
         :type src_key_padding_mask: torch.Tensor, optional
-        :param is_causal: Applies a causal mask as mask and ignores attn_mask for computing scaled dot product attention, defaults to False
+        :param is_causal: Applies a causal mask as mask and ignores attn_mask for computing scaled dot product 
+        attention, defaults to False
         :type is_causal: bool, optional
         """
         if self.end2end:
             src = self.positional_encoding(self.src_tok_emb(src))
 
         # Encoder forward pass preparation
         src_key_padding_mask = _canonical_mask(
@@ -285,15 +289,16 @@
             target_type=src.dtype
         )
         encoder_output = src
         first_layer = self.encoder[self.encoder_keys[0]]
         str_first_layer = "self.net[0]"
         src_key_padding_mask_for_layers = src_key_padding_mask
         encoder_output, convert_to_nested, src_key_padding_mask_for_layers = self.check_encoder_sparsity_fast_path(
-            src, encoder_output, first_layer, str_first_layer, src_mask, src_key_padding_mask, src_key_padding_mask_for_layers)
+            src, encoder_output, first_layer, str_first_layer, 
+            src_mask, src_key_padding_mask, src_key_padding_mask_for_layers)
 
         # Prevent type refinement
         make_causal = (is_causal is True)
 
         if is_causal is None:
             if src_mask is not None:
                 sz = src_mask.size(0)
@@ -445,15 +450,15 @@
                 first_layer.linear2.bias,
             )
 
             if not (src.is_cuda or 'cpu' in str(src.device)):
                 why_not_sparsity_fast_path = "src is neither CUDA nor CPU"
             elif torch.is_grad_enabled() and any(x.requires_grad for x in tensor_args):
                 why_not_sparsity_fast_path = (
-                    "grad is enabled and at least one of query or the input/output projection weights or biases requires_grad")
+                    "grad is enabled and at least one of query or the i/o projection weights or biases requires_grad")
 
             if (not why_not_sparsity_fast_path) and (src_key_padding_mask is not None):
                 convert_to_nested = True
                 output = torch._nested_tensor_from_mask(
                     output, src_key_padding_mask.logical_not(), mask_check=False)
                 src_key_padding_mask_for_layers = None
 
@@ -769,15 +774,16 @@
                 torch.zeros_like(mask, dtype=target_type)
                 .masked_fill_(mask, float("-inf"))
             )
     return mask
 
 
 class PositionalEncoder(nn.Module):
-    """The Positional Encoder class. Adds positional encoding to the token embedding to introduce a notion of word order.
+    """The Positional Encoder class. 
+    Adds positional encoding to the token embedding to introduce a notion of word order.
 
     :param emb_size: Number of expected features
     :type emb_size: int
     :param dropout: Dropout value, defaults to 0.1
     :type dropout: float, optional
     :param maxlen: Maximum length of sequence, defaults to 5000
     :type maxlen: int, optional
@@ -802,15 +808,16 @@
         :param x: Input to positional encoder, shape [seq_len, batch_size, embedding_dim]
         :type x: torch.Tensor
         """
         return self.dropout(x + self.pos_embedding[:x.size(0), :])
 
 
 class PositionalEncoding(nn.Module):
-    """The positional embedding class. Converts tensor of input indices into corresponding tensor of position embeddings."""
+    """The positional embedding class. 
+    Converts tensor of input indices into corresponding tensor of position embeddings."""
 
     def __init__(self, max_positions: int, emb_size):
         super(PositionalEncoding, self).__init__()
         self.embedding = nn.Embedding(max_positions, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
```

### Comparing `agilerl-0.1.6/agilerl/networks/evolvable_cnn.py` & `agilerl-0.1.7/agilerl/networks/evolvable_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,20 @@
     :type layer_norm: bool, optional
     :param stored_values: Stored network weights, defaults to None
     :type stored_values: numpy.array(), optional
     :param rainbow: Using Rainbow DQN, defaults to False
     :type rainbow: bool, optional
     :param critic: CNN is a critic network, defaults to False
     :type critic: bool, optional
+    :param normalize: Normalize CNN inputs, defaults to True
+    :type normalize: bool, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
     def __init__(
             self,
             input_shape: List[int],
             channel_size: List[int],
             kernal_size: List[int],
@@ -137,15 +141,17 @@
             num_atoms=51,
             mlp_activation='relu',
             cnn_activation='relu',
             layer_norm=False,
             stored_values=None,
             rainbow=False,
             critic=False,
-            device='cpu'):
+            normalize=True,
+            device='cpu',
+            accelerator=None):
 
         super(EvolvableCNN, self).__init__()
 
         self.input_shape = input_shape
         self.channel_size = channel_size
         self.kernal_size = kernal_size
         self.stride_size = stride_size
@@ -153,22 +159,23 @@
         self.num_actions = num_actions
         self.num_atoms = num_atoms
         self.mlp_activation = mlp_activation
         self.cnn_activation = cnn_activation
         self.layer_norm = layer_norm
         self.rainbow = rainbow
         self.critic = critic
+        self.normalize = normalize
         self.device = device
+        self.accelerator = accelerator
 
         self.net = self.create_nets()
         self.feature_net, self.value_net, self.advantage_net = self.create_nets()
-
+        
         if stored_values is not None:
-            self.inject_parameters(
-                pvec=stored_values, without_layer_norm=False)
+            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
 
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
         :type activation_names: str
         """
@@ -260,32 +267,38 @@
                 name="value")
             advantage_net = self.create_mlp(
                 input_size,
                 output_size=self.num_atoms *
                 self.num_actions,
                 hidden_size=self.hidden_size,
                 name="advantage")
-            advantage_net.to(self.device)
+            if self.accelerator is not None:
+                feature_net, value_net, advantage_net \
+                    = self.accelerator.prepare(feature_net, value_net, advantage_net)
+            else:
+                self.feature_net, self.value_net, self.advantage_net \
+                    = feature_net.to(self.device), value_net.to(self.device), \
+                        advantage_net.to(self.device)
         else:
             if self.critic:
                 value_net = self.create_mlp(
                     input_size,
                     output_size=1,
                     hidden_size=self.hidden_size,
                     name="value")
             else:
                 value_net = self.create_mlp(
                     input_size,
                     output_size=self.num_actions,
                     hidden_size=self.hidden_size,
                     name="value")
             advantage_net = None
-
-        feature_net.to(self.device)
-        value_net.to(self.device)
+            if self.accelerator is None:
+                self.feature_net, self.value_net, = feature_net.to(self.device), \
+                    value_net.to(self.device)
 
         return feature_net, value_net, advantage_net
 
     def reset_noise(self):
         """Resets noise of value and advantage networks.
         """
         for layer in self.value_net:
@@ -304,15 +317,17 @@
         :param xc: Actions to be evaluated by critic, defaults to None
         :type xc: torch.Tensor() or np.array, optional
         """
         if not isinstance(x, torch.Tensor):
             x = torch.FloatTensor(x)
 
         batch_size = x.size(0)
-        x = x / 255.
+        
+        if self.normalize:
+            x = x / 255.
 
         x = self.feature_net(x)
         x = x.reshape(batch_size, -1)
 
         if self.critic:
             x = torch.cat([x, xc], dim=1)
 
@@ -351,15 +366,16 @@
         count = 0
         for name, param in self.named_parameters():
             if not without_layer_norm or 'layer_norm' not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
-        """Returns current pytorch gradient in same order as genome's flattened parameter vector.
+        """Returns current pytorch gradient in same order as genome's flattened 
+        parameter vector.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
@@ -383,15 +399,16 @@
             if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
-        """Injects a flat vector of neural network parameters into the model's current neural network weights.
+        """Injects a flat vector of neural network parameters into the model's current 
+        neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
@@ -433,15 +450,16 @@
             "hidden_size": self.hidden_size,
             "num_actions": self.num_actions,
             "num_atoms": self.num_atoms,
             "mlp_activation": self.mlp_activation,
             "cnn_activation": self.cnn_activation,
             "layer_norm": self.layer_norm,
             "critic": self.critic,
-            "device": self.device}
+            "device": self.device,
+            "accelerator": self.accelerator}
         return initdict
 
     def add_mlp_layer(self):
         """Adds a hidden layer to Multi-layer Perceptron.
         """
         if len(self.hidden_size) < 3:  # HARD LIMIT
             self.hidden_size += [self.hidden_size[-1]]
@@ -500,27 +518,28 @@
             self.add_cnn_layer()
 
     def add_cnn_channel(self, hidden_layer=None, numb_new_channels=None):
         """Adds channel to hidden layer of Convolutional Neural Network.
 
         :param hidden_layer: Depth of hidden layer to add channel to, defaults to None
         :type hidden_layer: int, optional
-        :param numb_new_channels: Number of channels to add to hidden layer, defaults to None
+        :param numb_new_channels: Number of channels to add to hidden layer, defaults 
+        to None
         :type numb_new_channels: int, optional
         """
         if hidden_layer is None:
             hidden_layer = np.random.randint(0, len(self.channel_size), 1)[0]
         else:
             hidden_layer = min(hidden_layer, len(self.channel_size) - 1)
         if numb_new_channels is None:
-            numb_new_nodes = np.random.choice([8, 16, 32], 1)[0]
+            numb_new_channels = np.random.choice([8, 16, 32], 1)[0]
 
-        if self.channel_size[hidden_layer] + numb_new_nodes <= 256:  # HARD LIMIT
+        if self.channel_size[hidden_layer] + numb_new_channels <= 256:  # HARD LIMIT
 
-            self.channel_size[hidden_layer] += numb_new_nodes
+            self.channel_size[hidden_layer] += numb_new_channels
 
             self.recreate_nets()
 
         return {"hidden_layer": hidden_layer, "numb_new_channels": numb_new_channels}
 
     def recreate_nets(self):
         """Recreates neural networks.
```

### Comparing `agilerl-0.1.6/agilerl/networks/evolvable_gpt.py` & `agilerl-0.1.7/agilerl/networks/evolvable_gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     :type max_layers: int, optional
     :param bias: Use bias in Linears and LayerNorms, defaults to True
     :type bias: bool, optional
     :param stored_values: Stored network weights, defaults to None
     :type stored_values: numpy.array(), optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
     def __init__(
             self,
             n_layer: int = 12,
             vocab_size: int = 50257,
             n_embd: int = 768,
@@ -54,31 +56,32 @@
             dropout: float = 0.0,
             activation: str = 'gelu',
             layer_norm_eps: float = 1e-5,
             min_layers: int = 8,
             max_layers: int = 16,
             bias: bool = True,
             stored_values = None,
-            device='cpu'):
+            device='cpu',
+            accelerator=None):
         super(EvolvableGPT, self).__init__()
 
         self.n_layer = n_layer
         self.vocab_size = vocab_size
         self.n_embd = n_embd
         self.n_head = n_head
         self.dim_feedfwd = dim_feedfwd
         self.block_size = block_size
         self.dropout = dropout
         self.activation = activation
         self.layer_norm_eps = layer_norm_eps
         self.min_layers = min_layers
         self.max_layers = max_layers
         self.bias = bias
-
         self.device = device
+        self.accelerator = accelerator
 
         self.transformer = self.create_net()
         self.transformer_keys = list(self.transformer.keys())
 
         self.lm_head = nn.Linear(self.n_embd, self.vocab_size, bias=False)
 
         self.transformer.wte.weight = self.lm_head.weight
@@ -152,15 +155,16 @@
                                              self.block_size,
                                              self.dim_feedfwd,
                                              self.activation,
                                              self.layer_norm_eps) for _ in range(self.n_layer)])
         net_dict['ln_f'] = LayerNorm(self.n_embd, bias=self.bias)
         return nn.ModuleDict(net_dict)
 
-    def forward(self, idx=None, tok_emb=None, targets=None, attn_mask=None, past_key_values=None, pos=None, is_causal=True):
+    def forward(self, idx=None, tok_emb=None, targets=None, attn_mask=None, past_key_values=None, pos=None, 
+                is_causal=True):
         """Forward pass through evolvable GPT model.
         
         :param idxs: Input ids
         :type idxs: torch.Tensor
         :param targets: Target ids
         :type targets: torch.Tensor
         """
@@ -346,15 +350,16 @@
 
         # validate that we considered every parameter
         param_dict = {pn: p for pn, p in self.named_parameters()}
         inter_params = decay & no_decay
         union_params = decay | no_decay
         assert len(
             inter_params) == 0, "parameters %s made it into both decay/no_decay sets!" % (str(inter_params), )
-        assert len(param_dict.keys() - union_params) == 0, "parameters %s were not separated into either decay/no_decay set!" \
+        assert len(
+            param_dict.keys() - union_params) == 0, "parameters %s were not separated into either decay/no_decay set!" \
             % (str(param_dict.keys() - union_params), )
 
         # create the pytorch optimizer object
         optim_groups = [
             {"params": [param_dict[pn] for pn in sorted(
                 list(decay))], "weight_decay": weight_decay},
             {"params": [param_dict[pn]
@@ -805,15 +810,16 @@
     """
     def forward(self, x):
         return 0.5 * x * (1.0 + torch.tanh(math.sqrt(2.0 / math.pi)
                       * (x + 0.044715 * torch.pow(x, 3.0))))
 
 
 class PositionalEncoding(nn.Module):
-    """The positional embedding class. Converts tensor of input indices into corresponding tensor of position embeddings."""
+    """The positional embedding class. 
+    Converts tensor of input indices into corresponding tensor of position embeddings."""
 
     def __init__(self, max_positions: int, emb_size):
         super(PositionalEncoding, self).__init__()
         self.embedding = nn.Embedding(max_positions, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
```

### Comparing `agilerl-0.1.6/agilerl/networks/evolvable_mlp.py` & `agilerl-0.1.7/agilerl/networks/evolvable_mlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,37 +24,41 @@
     :type layer_norm: bool, optional
     :param output_vanish: Vanish output by multiplying by 0.1, defaults to True
     :type output_vanish: bool, optional
     :param stored_values: Stored network weights, defaults to None
     :type stored_values: numpy.array(), optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
     def __init__(
             self,
             num_inputs: int,
             num_outputs: int,
             hidden_size: List[int],
             activation='relu',
             output_activation=None,
             layer_norm=False,
             output_vanish=True,
             stored_values=None,
-            device='cpu'):
+            device='cpu',
+            accelerator=None):
         super(EvolvableMLP, self).__init__()
 
         self.num_inputs = num_inputs
         self.num_outputs = num_outputs
         self.activation = activation
         self.output_activation = output_activation
         self.layer_norm = layer_norm
         self.output_vanish = output_vanish
         self.hidden_size = hidden_size
         self.device = device
+        self.accelerator = accelerator
 
         self.net = self.create_net()
 
         if stored_values is not None:
             self.inject_parameters(
                 pvec=stored_values, without_layer_norm=False)
 
@@ -105,28 +109,33 @@
             output_layer.weight.data.mul_(0.1)
             output_layer.bias.data.mul_(0.1)
 
         net_dict["linear_layer_output"] = output_layer
         if self.output_activation is not None:
             net_dict["activation_output"] = self.get_activation(
                 self.output_activation)
+            
+        net = nn.Sequential(net_dict)
+            
+        if self.accelerator is None:
+            net = net.to(self.device)
 
-        return nn.Sequential(net_dict)
+        return net
 
     def forward(self, x):
         """Returns output of neural network.
 
         :param x: Neural network input
         :type x: torch.Tensor() or np.array
         """
         if not isinstance(x, torch.Tensor):
-            x = torch.FloatTensor(np.array(x)).to(self.device)
-
-        for value in self.net:
-            x = value(x)
+            x = torch.FloatTensor(np.array(x))
+            if self.accelerator is None:
+                x = x.to(self.device)
+        x = self.net(x)
         return x
 
     def get_model_dict(self):
         """Returns dictionary with model information and weights.
         """
         model_dict = self.init_dict
         model_dict.update(
@@ -142,15 +151,16 @@
         count = 0
         for name, param in self.named_parameters():
             if not without_layer_norm or 'layer_norm' not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
-        """Returns current pytorch gradient in same order as genome's flattened parameter vector.
+        """Returns current pytorch gradient in same order as genome's flattened 
+        parameter vector.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
@@ -174,15 +184,16 @@
             if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
-        """Injects a flat vector of neural network parameters into the model's current neural network weights.
+        """Injects a flat vector of neural network parameters into the model's current 
+        neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
@@ -204,15 +215,16 @@
         init_dict = {
             "num_inputs": self.num_inputs,
             "num_outputs": self.num_outputs,
             "hidden_size": self.hidden_size,
             "activation": self.activation,
             "output_activation": self.output_activation,
             "layer_norm": self.layer_norm,
-            "device": self.device}
+            "device": self.device,
+            "accelerator":self.accelerator}
         return init_dict
 
     @property
     def short_dict(self):
         """Returns shortened version of model information in dictionary.
         """
         short_dict = {
@@ -273,17 +285,19 @@
             self.net = new_net
 
         return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
 
     def remove_node(self, hidden_layer=None, numb_new_nodes=None):
         """Removes nodes from hidden layer of neural network.
 
-        :param hidden_layer: Depth of hidden layer to remove nodes from, defaults to None
+        :param hidden_layer: Depth of hidden layer to remove nodes from, defaults to 
+        None
         :type hidden_layer: int, optional
-        :param numb_new_nodes: Number of nodes to remove from hidden layer, defaults to None
+        :param numb_new_nodes: Number of nodes to remove from hidden layer, defaults to 
+        None
         :type numb_new_nodes: int, optional
         """
         if hidden_layer is None:
             hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
         else:
             hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
         if numb_new_nodes is None:
```

### Comparing `agilerl-0.1.6/agilerl/training/train_bc_lm.py` & `agilerl-0.1.7/agilerl/training/train_bc_lm.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     if cfg['evaluator'] is not None:
         evaluator = load_item(cfg['evaluator'], system_cfg['device'])
 
     model = load_item(cfg['model'], system_cfg['device'])
     model.train()
 
     if hasattr(model, 'param_groups'):
-        params = [{'params': frozenset().union(*list(map(lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
+        params = [{'params': frozenset().union(*list(map(
+            lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
     else:
         params = model.parameters()
     optim = torch.optim.AdamW(params, lr=train_cfg['lr'], weight_decay=train_cfg['weight_decay'])
     if train_cfg['optim_state_path'] is not None and os.path.exists(train_cfg['optim_state_path']):
         print(f'loading optimizer state from: {train_cfg["optim_state_path"]}')
         optim.load_state_dict(torch.load(train_cfg['optim_state_path'], map_location=system_cfg['device']))
         print('loaded.')
@@ -139,15 +140,16 @@
                 model.train()
             if train_cfg['save_every'] is not None and (step + 1) % train_cfg['save_every'] == 0:
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
                     print('saving checkpoint...')
                     if not os.path.exists(train_cfg['save_checkpoint_dir']):
                         os.makedirs(train_cfg['save_checkpoint_dir'])
-                    if (train_cfg['max_checkpoints'] is not None) and (len(saved_checkpoints) >= train_cfg['max_checkpoints']):
+                    if (train_cfg['max_checkpoints'] is not None) and (len(
+                        saved_checkpoints) >= train_cfg['max_checkpoints']):
                         os.system('rm -rf %s' % (saved_checkpoints.popleft()))
                     torch.save(accelerator.unwrap_model(model).state_dict(),
                                 os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
                     saved_checkpoints.append(os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
                     print('saved.')
                 accelerator.wait_for_everyone()
             step += 1
```

### Comparing `agilerl-0.1.6/agilerl/training/train_ilql.py` & `agilerl-0.1.7/agilerl/training/train_ilql.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
     if cfg['evaluator'] is not None:
         evaluator = load_item(cfg['evaluator'], system_cfg['device'])
 
     model = load_item(cfg['model'], system_cfg['device'])
     model.train()
 
     if hasattr(model, 'param_groups'):
-        params = [{'params': frozenset().union(*list(map(lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
+        params = [{'params': frozenset().union(*list(
+            map(lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
         model.optimizer = torch.optim.AdamW(
             params, lr=model.lr, weight_decay=model.weight_decay)
     optim = model.optimizer
 
     if train_cfg['optim_state_path'] is not None and os.path.exists(train_cfg['optim_state_path']):
         print(f'loading optimizer state from: {train_cfg["optim_state_path"]}')
         optim.load_state_dict(torch.load(train_cfg['optim_state_path'], map_location=system_cfg['device']))
@@ -151,15 +152,16 @@
                 model.train()
             if train_cfg['save_every'] is not None and (step + 1) % train_cfg['save_every'] == 0:
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
                     print('saving checkpoint...')
                     if not os.path.exists(train_cfg['save_checkpoint_dir']):
                         os.makedirs(train_cfg['save_checkpoint_dir'])
-                    if (train_cfg['max_checkpoints'] is not None) and (len(saved_checkpoints) >= train_cfg['max_checkpoints']):
+                    if (train_cfg['max_checkpoints'] is not None) and (len(
+                        saved_checkpoints) >= train_cfg['max_checkpoints']):
                         os.system('rm -rf %s' % (saved_checkpoints.popleft()))
                     torch.save(accelerator.unwrap_model(model).state_dict(),
                                 os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
                     saved_checkpoints.append(os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
                     print('saved.')
                 accelerator.wait_for_everyone()
             step += 1
```

### Comparing `agilerl-0.1.6/agilerl/utils/cache.py` & `agilerl-0.1.7/agilerl/utils/cache.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/utils/ilql_utils.py` & `agilerl-0.1.7/agilerl/utils/ilql_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,20 @@
     with open(pkl_path, 'wb') as f:
         pkl.dump(d, f)
 
 def convert_old_ad_model(model_path, dataset, multiple_transformers=False):
     w = torch.load(model_path, map_location='cpu')
     embs = w['model.transformer.wte.weight']
     if embs.shape[0] < dataset.tokenizer.num_tokens():
-        w['model.transformer.wte.weight'] = torch.cat((embs, torch.zeros(dataset.tokenizer.num_tokens()-embs.shape[0], embs.shape[1])), dim=0)
+        w['model.transformer.wte.weight'] = torch.cat((embs, torch.zeros(dataset.tokenizer.num_tokens()-embs.shape[0], 
+                                                                         embs.shape[1])), dim=0)
     head = w['model.lm_head.weight']
     if head.shape[0] < dataset.tokenizer.num_tokens():
-        w['model.lm_head.weight'] = torch.cat((head, torch.zeros(dataset.tokenizer.num_tokens()-head.shape[0], head.shape[1])), dim=0)
+        w['model.lm_head.weight'] = torch.cat((head, torch.zeros(dataset.tokenizer.num_tokens()-head.shape[0], 
+                                                                 head.shape[1])), dim=0)
     if multiple_transformers:
         for k, v in list(w.items()):
             if k.startswith('model.'):
                 w['lm_policy.'+k[len('model.'):]] = v.clone()
                 w['lm_target.'+k[len('model.'):]] = v.clone()
     torch.save(w, model_path)
```

### Comparing `agilerl-0.1.6/agilerl/utils/load_objects.py` & `agilerl-0.1.7/agilerl/utils/load_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import torch
 from agilerl.algorithms.bc_lm import BC_LM, BC_Evaluator, BC_Policy
 from agilerl.algorithms.ilql import ILQL, ILQL_Policy, ILQL_Evaluator, TopAdvantageNGrams
 from agilerl.networks.evolvable_gpt import EvolvableGPT
 from agilerl.utils.ilql_utils import convert_path
 from agilerl.data.rl_data import ConstantTokenReward, SepcifiedTokenReward
-from agilerl.wordle.policy import MixturePolicy, MonteCarloPolicy, OptimalPolicy, RandomMixturePolicy, RepeatPolicy, StartWordPolicy, UserPolicy, WrongPolicy
+from agilerl.wordle.policy import MixturePolicy, MonteCarloPolicy, OptimalPolicy, RandomMixturePolicy, RepeatPolicy, \
+    StartWordPolicy, UserPolicy, WrongPolicy
 from agilerl.wordle.wordle_dataset import WordleHumanDataset, WordleIterableDataset, WordleListDataset
 from agilerl.wordle.wordle_env import WordleEnvironment
 from agilerl.wordle.wordle_game import Vocabulary
 from agilerl.wordle.wordle_evaluators import Action_Ranking_Evaluator, Action_Ranking_Evaluator_Adversarial
 
 registry = {}
 cache = {}
@@ -206,15 +207,16 @@
 @register('wordle_human_dataset')
 def load_human_dataset(config, device, verbose=True):
     token_reward = load_item(config['token_reward'], device, verbose=verbose)
     game_indexes = None
     if config['index_file'] is not None:
         with open(convert_path(config['index_file']), 'r') as f:
             game_indexes = json.load(f)
-    return WordleHumanDataset.from_file(convert_path(config['file_path']), config['use_true_word'], config['max_len'], token_reward, 
+    return WordleHumanDataset.from_file(convert_path(config['file_path']), config['use_true_word'], 
+                                        config['max_len'], token_reward, 
                                         game_indexes, config['top_p'])
 
 @register('action_ranking_evaluator')
 def load_action_ranking_evaluator(config, device, verbose=True):
     branching_data = load_item(config['branching_data'], device, verbose=verbose)
     return Action_Ranking_Evaluator(branching_data)
```

### Comparing `agilerl-0.1.6/agilerl/utils/log_utils.py` & `agilerl-0.1.7/agilerl/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/utils/sampling_utils.py` & `agilerl-0.1.7/agilerl/utils/sampling_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import torch
 import torch.nn.functional as F
 import numpy as np
 
 def select_batch_idxs(x, idxs):
-    return torch.gather(x, dim=0, index=idxs.repeat(*x.shape[1:], 1).permute(len(x.shape) - 1, *list(range(len(x.shape) - 1))))
+    return torch.gather(x, dim=0, 
+                        index=idxs.repeat(*x.shape[1:], 1).permute(len(x.shape) - 1, *list(range(len(x.shape) - 1))))
 
 def map_all_kvs(f, kvs):
     return tuple([tuple(map(f, items)) for items in kvs])
 
 def map_decoder_kvs(f, kvs):
     return tuple([(tuple(map(f, items[:2])) + tuple(items[2:])) for items in kvs])
 
 def pad_sequence(seq, to_len, val, device, dim):
-    return torch.cat((seq, torch.full((*seq.shape[:dim], to_len - seq.shape[dim], *seq.shape[dim + 1:]), val).to(device)), dim=dim)
+    return torch.cat((seq, torch.full(
+        (*seq.shape[:dim], to_len - seq.shape[dim], *seq.shape[dim + 1:]), val).to(device)), dim=dim)
 
 def update_kvs(kvs, updated_kvs, lens_chosen, idx):
     for i, layer in enumerate(kvs):
         for x, item in enumerate(layer):
             item[lens_chosen, :, idx, :] = updated_kvs[i][x][:, :, idx, :]
     return kvs
```

### Comparing `agilerl-0.1.6/agilerl/utils/serve_queue.py` & `agilerl-0.1.7/agilerl/utils/serve_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,33 +14,40 @@
     init_message = '__init_message__'
 
 def serve_class(ModelCls):
     cache_cls = pkl.dumps(ModelCls)
     class WrappedModel:
         def __init__(self, *args, **kwargs):
             self.r = redis.Redis(host=Config.redis_host, port=Config.redis_port, db=Config.redis_db)
-            self.Q = initalize_server(self, super().__getattribute__('r'), cache_cls, args, kwargs)
+            self.Q = initalize_server(self, super().__getattribute__(
+                'r'), cache_cls, args, kwargs)
         
         def __getattribute__(self, name):
-            return partial(build_method(name, super().__getattribute__('r'), super().__getattribute__('Q')), self)
+            return partial(build_method(name, super().__getattribute__(
+                'r'), super().__getattribute__('Q')), self)
     
         def __call__(self, *args, **kwargs):
-            return build_method('__call__',  super().__getattribute__('r'), super().__getattribute__('Q'))(self, *args, **kwargs)
+            return build_method('__call__',  super().__getattribute__(
+                'r'), super().__getattribute__('Q'))(self, *args, **kwargs)
         
         def __getitem__(self, key):
-            return build_method('__getitem__',  super().__getattribute__('r'), super().__getattribute__('Q'))(self, key)
+            return build_method('__getitem__',  super().__getattribute__(
+                'r'), super().__getattribute__('Q'))(self, key)
         
         def __setitem__(self, key, value):
-            return build_method('__setitem__',  super().__getattribute__('r'), super().__getattribute__('Q'))(self, key, value)
+            return build_method('__setitem__',  super().__getattribute__(
+                'r'), super().__getattribute__('Q'))(self, key, value)
         
         def __contains__(self, key):
-            return build_method('__contains__',  super().__getattribute__('r'), super().__getattribute__('Q'))(self, key)
+            return build_method('__contains__',  super().__getattribute__(
+                'r'), super().__getattribute__('Q'))(self, key)
         
         def __len__(self):
-            return build_method('__len__',  super().__getattribute__('r'), super().__getattribute__('Q'))(self)
+            return build_method('__len__',  super().__getattribute__(
+                'r'), super().__getattribute__('Q'))(self)
     return WrappedModel
 
 def build_method(method, r, Q):
     def call_method(self, *args, **kwargs):
         request_id = int(r.incr('request_id_counter'))
         Q.put((request_id, method, args, kwargs,))
         while not r.exists(f'result_{request_id}'):
```

### Comparing `agilerl-0.1.6/agilerl/utils/torch_utils.py` & `agilerl-0.1.7/agilerl/utils/torch_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,12 +28,14 @@
     for param in model.parameters():
         norm += (param.norm() ** 2).item()
     return math.sqrt(norm)
 
 def get_transformer_logs(attentions: List[torch.Tensor], model: nn.Module, attn_mask: torch.Tensor):
     logs = {}
     n = attn_mask.sum()
-    model_attention_entropy = -sum(map(lambda x: ((x * torch.log(x+1e-7)).sum(dim=-1) * attn_mask.unsqueeze(1)).sum().item(), attentions)) / (len(attentions) * n)
+    model_attention_entropy = -sum(map(
+        lambda x: ((x * torch.log(x+1e-7)).sum(
+        dim=-1) * attn_mask.unsqueeze(1)).sum().item(), attentions)) / (len(attentions) * n)
     model_parameter_norm = parameter_norm(model)
     logs['attention_entropy'] = (model_attention_entropy, n * len(attentions))
     logs['parameter_norm'] = (model_parameter_norm, 1)
     return logs
```

### Comparing `agilerl-0.1.6/agilerl/utils/utils.py` & `agilerl-0.1.7/agilerl/utils/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import gymnasium as gym
 import numpy as np
 import matplotlib.pyplot as plt
 from agilerl.algorithms.cqn import CQN
 from agilerl.algorithms.dqn import DQN
 from agilerl.algorithms.ddpg import DDPG
-
+from agilerl.algorithms.td3 import TD3
 
 def makeVectEnvs(env_name, num_envs=1):
     """Returns async-vectorized gym environments.
 
     :param env_name: Gym environment name
     :type env_name: str
     :param num_envs: Number of vectorized environments, defaults to 1
     :type num_envs: int, optional
     """
     return gym.vector.AsyncVectorEnv(
         [lambda: gym.make(env_name) for i in range(num_envs)])
 
 
 def initialPopulation(algo, state_dim, action_dim, one_hot,
-                      net_config, INIT_HP, population_size=1, device='cpu'):
+                      net_config, INIT_HP, population_size=1, device='cpu', 
+                      accelerator=None):
     """Returns population of identical agents.
 
     :param algo: RL algorithm
     :type algo: str
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
@@ -32,14 +33,16 @@
     :type one_hot: bool
     :param INIT_HP: Initial hyperparameters
     :type INIT_HP: dict
     :param population_size: Number of agents in population, defaults to 1
     :type population_size: int, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
     population = []
 
     if algo == 'DQN':
         for idx in range(population_size):
             agent = DQN(
                 state_dim=state_dim,
@@ -49,15 +52,16 @@
                 net_config=net_config,
                 batch_size=INIT_HP['BATCH_SIZE'],
                 lr=INIT_HP['LR'],
                 learn_step=INIT_HP['LEARN_STEP'],
                 gamma=INIT_HP['GAMMA'],
                 tau=INIT_HP['TAU'],
                 double=INIT_HP['DOUBLE'],
-                device=device
+                device=device,
+                accelerator=accelerator
             )
             population.append(agent)
 
     elif algo == 'DDPG':
         for idx in range(population_size):
             agent = DDPG(
                 state_dim=state_dim,
@@ -67,15 +71,16 @@
                 net_config=net_config,
                 batch_size=INIT_HP['BATCH_SIZE'],
                 lr=INIT_HP['LR'],
                 learn_step=INIT_HP['LEARN_STEP'],
                 gamma=INIT_HP['GAMMA'],
                 tau=INIT_HP['TAU'],
                 policy_freq=INIT_HP['POLICY_FREQ'],
-                device=device
+                device=device,
+                accelerator=accelerator
             )
             population.append(agent)
 
     elif algo == 'CQN':
         for idx in range(population_size):
             agent = CQN(
                 state_dim=state_dim,
@@ -85,14 +90,54 @@
                 net_config=net_config,
                 batch_size=INIT_HP['BATCH_SIZE'],
                 lr=INIT_HP['LR'],
                 learn_step=INIT_HP['LEARN_STEP'],
                 gamma=INIT_HP['GAMMA'],
                 tau=INIT_HP['TAU'],
                 double=INIT_HP['DOUBLE'],
+                device=device,
+                accelerator=accelerator
+            )
+            population.append(agent)
+
+    elif algo == 'TD3':
+        for idx in range(population_size):
+            agent = TD3(
+                state_dim=state_dim,
+                action_dim=action_dim,
+                one_hot=one_hot,
+                max_action=INIT_HP['MAX_ACTION'],
+                index=idx,
+                net_config=net_config,
+                batch_size=INIT_HP['BATCH_SIZE'],
+                lr=INIT_HP['LR'],
+                learn_step=INIT_HP['LEARN_STEP'],
+                gamma=INIT_HP['GAMMA'],
+                tau=INIT_HP['TAU'],
+                policy_freq=INIT_HP['POLICY_FREQ'],
+                device=device,
+                accelerator=accelerator
+            )
+            population.append(agent)
+
+    elif algo == 'TD3':
+        for idx in range(population_size):
+            agent = TD3(
+                state_dim=state_dim,
+                action_dim=action_dim,
+                one_hot=one_hot,
+                max_action=INIT_HP['MAX_ACTION'],
+                index=idx,
+                net_config=net_config,
+                batch_size=INIT_HP['BATCH_SIZE'],
+                lr=INIT_HP['LR'],
+                learn_step=INIT_HP['LEARN_STEP'],
+                gamma=INIT_HP['GAMMA'],
+                tau=INIT_HP['TAU'],
+                policy_freq=INIT_HP['POLICY_FREQ'],
                 device=device
             )
             population.append(agent)
 
     return population
```

### Comparing `agilerl-0.1.6/agilerl/wordle/policy.py` & `agilerl-0.1.7/agilerl/wordle/policy.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/wordle/wordle_dataset.py` & `agilerl-0.1.7/agilerl/wordle/wordle_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,31 +31,34 @@
     def from_file(cls, file_path: str, max_len: Optional[int], vocab: Optional[Vocabulary], token_reward: TokenReward):
         with open(file_path, 'rb') as f:
             d = pkl.load(f)
         if vocab is None:
             vocab = Vocabulary.from_file(convert_path(d['vocab_path']))
             if d['vocab_cache_path'] is not None:
                 vocab.cache.load(convert_path(d['vocab_cache_path']))
-        wordle_items = [WordleObservation(WordleGame(item['state'], vocab.update_vocab(item['state']), item['actions'])) for item in tqdm(d['state_actions'])]
-        meta = [{**item['meta'], 'self': wordle_items[i]} if 'meta' in item else {'self': wordle_items[i]} for i, item in enumerate(d['state_actions'])]
+        wordle_items = [WordleObservation(WordleGame(item['state'], vocab.update_vocab(
+            item['state']), item['actions'])) for item in tqdm(d['state_actions'])]
+        meta = [{**item['meta'], 'self': wordle_items[i]} if 'meta' in item else {
+            'self': wordle_items[i]} for i, item in enumerate(d['state_actions'])]
         return WordleListDataset(list(zip(wordle_items, meta)), max_len, token_reward)
     
 class WordleIterableDataset(Iterable_RL_Dataset):
     def __init__(self, 
                  policy: Policy, 
                  vocab: Vocabulary, 
                  max_len: Optional[int], 
                  token_reward: TokenReward) -> None:
         tokenizer = WordleTokenizer()
         super().__init__(tokenizer, token_reward, max_len)
         self.policy = policy
         self.env = WordleEnvironment(vocab)
 
     def sample_item(self):
-        return DataPoint.from_obs(interact_environment(self.env, self.policy, None)[0], self.tokenizer, self.token_reward, None)
+        return DataPoint.from_obs(interact_environment(self.env, self.policy, None)[0], self.tokenizer, 
+                                  self.token_reward, None)
 
 class WordleHumanDataset(Iterable_RL_Dataset):
     def __init__(self, 
                  games: List[Tuple[str, List[str]]], 
                  transitions: Dict[str, Dict[str, List[str]]], 
                  use_true_word: bool, 
                  max_len: Optional[int], 
@@ -76,28 +79,30 @@
 
     def sample_item(self):
         true_word, game = random.choice(self.games)
         if self.use_true_word:
             while True:
                 actions = []
                 for transition in game:
-                    if transition not in self.transitions[true_word] or len(self.transitions[true_word][transition]) == 0:
+                    if transition not in self.transitions[true_word] or len(
+                        self.transitions[true_word][transition]) == 0:
                         break
                     actions.append(random.choice(self.transitions[true_word][transition]))
                 if len(actions) == len(game):
                     break
                 else:
                     true_word, game = random.choice(self.games)
         else:
             word_choices = list(self.transitions.keys())
             while True:
                 true_word = random.choice(word_choices)
                 actions = []
                 for transition in game:
-                    if transition not in self.transitions[true_word] or len(self.transitions[true_word][transition]) == 0:
+                    if transition not in self.transitions[true_word] or len(
+                        self.transitions[true_word][transition]) == 0:
                         break
                     actions.append(random.choice(self.transitions[true_word][transition]))
                 if len(actions) == len(game):
                     break
                 else:
                     true_word, game = random.choice(self.games)
         state = WordleState.initial_state()
```

### Comparing `agilerl-0.1.6/agilerl/wordle/wordle_env.py` & `agilerl-0.1.7/agilerl/wordle/wordle_env.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/agilerl/wordle/wordle_evaluators.py` & `agilerl-0.1.7/agilerl/wordle/wordle_evaluators.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,23 +36,29 @@
         total_correct_target = [0 for _ in range(N_CHARS+1)]
         total = 0
         for _ in range(tokens.shape[0]):
             s, a = random.choice(self.states)
             obs = WordleObservation(WordleGame(s, self.vocab.update_vocab(s), list(a)))
             expert_state, _, _ = obs.game.next(random.choice(self.expert_actions[self.hashable_state((s, a,))]))
             non_expert_state, _, _ = obs.game.next(random.choice(self.non_expert_actions[self.hashable_state((s, a,))]))
-            expert_datapoint = DataPoint.from_obs(WordleObservation(expert_state), self.branching_data.token_reward, self.branching_data.tokenizer)
-            non_expert_datapoint = DataPoint.from_obs(WordleObservation(non_expert_state), self.branching_data.token_reward, self.branching_data.tokenizer)
+            expert_datapoint = DataPoint.from_obs(WordleObservation(expert_state), self.branching_data.token_reward, 
+                                                  self.branching_data.tokenizer)
+            non_expert_datapoint = DataPoint.from_obs(WordleObservation(non_expert_state), 
+                                                      self.branching_data.token_reward, self.branching_data.tokenizer)
             iql_outputs = model.get_qvs([expert_datapoint, non_expert_datapoint])
             qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
             for i in range(N_CHARS+1):
-                total_correct[i] += int(qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (1 - terminals[1, :-1]).sum()-1-i])
-                total_correct_target[i] += int(target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                total_correct[i] += int(qs[0, 
+                                           (1 - terminals[0, :-1]).sum()-1-i] > qs[1, 
+                                                                                   (1 - terminals[1, :-1]).sum()-1-i])
+                total_correct_target[i] += int(
+                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
             total += 1
-        return {**{('q_rank_acc_-%d' % (i+1)): (total_correct[i] / total, total) for i in range(N_CHARS+1)}, **{('q_target_rank_acc_-%d' % (i+1)): (total_correct_target[i] / total, total) for i in range(N_CHARS+1)}}
+        return {**{('q_rank_acc_-%d' % (i+1)): (total_correct[i] / total, total) for i in range(N_CHARS+1)}, **{
+            ('q_target_rank_acc_-%d' % (i+1)): (total_correct_target[i] / total, total) for i in range(N_CHARS+1)}}
 
 class Action_Ranking_Evaluator_Adversarial():
     def __init__(self, adversarial_data: WordleListDataset) -> None:
         self.adversarial_data = adversarial_data
         self.expert_actions = defaultdict(list)
         self.adversarial_actions = defaultdict(list)
         self.suboptimal_actions = defaultdict(list)
@@ -89,35 +95,51 @@
         for _ in range(tokens.shape[0]):
             initial_s, initial_a = random.choice(self.initial_states)
             initial_obs = WordleObservation(WordleGame(initial_s, self.vocab.update_vocab(initial_s), list(initial_a)))
             initial_expert_a = random.choice(self.expert_actions[self.hashable_state((initial_s, initial_a,))])
             initial_suboptimal_a = random.choice(self.suboptimal_actions[self.hashable_state((initial_s, initial_a,))])
             initial_expert_state, _, _ = initial_obs.game.next(initial_expert_a)
             initial_suboptimal_state, _, _ = initial_obs.game.next(initial_suboptimal_a)
-            initial_expert_datapoint = DataPoint.from_obs(WordleObservation(initial_expert_state), self.adversarial_data.tokenizer, self.adversarial_data.token_reward)
-            initial_suboptimal_datapoint = DataPoint.from_obs(WordleObservation(initial_suboptimal_state), self.adversarial_data.tokenizer, self.adversarial_data.token_reward)
+            initial_expert_datapoint = DataPoint.from_obs(WordleObservation(initial_expert_state), 
+                                                          self.adversarial_data.tokenizer, 
+                                                          self.adversarial_data.token_reward)
+            initial_suboptimal_datapoint = DataPoint.from_obs(WordleObservation(initial_suboptimal_state), 
+                                                              self.adversarial_data.tokenizer, 
+                                                              self.adversarial_data.token_reward)
             iql_outputs = model.get_qvs([initial_expert_datapoint, initial_suboptimal_datapoint])
             qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
             for i in range(N_CHARS+1):
-                initial_total_correct[i] += int(qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (1 - terminals[1, :-1]).sum()-1-i])
-                initial_total_correct_target[i] += int(target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                initial_total_correct[i] += int(qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (
+                    1 - terminals[1, :-1]).sum()-1-i])
+                initial_total_correct_target[i] += int(
+                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
             
             branch_s, branch_a = random.choice(self.branch_states)
             branch_obs = WordleObservation(WordleGame(branch_s, self.vocab.update_vocab(branch_s), list(branch_a)))
             branch_expert_a = random.choice(self.expert_actions[self.hashable_state((branch_s, branch_a,))])
             branch_adversarial_a = random.choice(self.adversarial_actions[self.hashable_state((branch_s, branch_a,))])
             branch_expert_state, _, _ = branch_obs.game.next(branch_expert_a)
             branch_adversarial_state, _, _ = branch_obs.game.next(branch_adversarial_a)
-            branch_expert_datapoint = DataPoint.from_obs(WordleObservation(branch_expert_state), self.adversarial_data.tokenizer, self.adversarial_data.token_reward)
-            branch_adversarial_datapoint = DataPoint.from_obs(WordleObservation(branch_adversarial_state), self.adversarial_data.tokenizer, self.adversarial_data.token_reward)
+            branch_expert_datapoint = DataPoint.from_obs(WordleObservation(branch_expert_state), 
+                                                         self.adversarial_data.tokenizer, 
+                                                         self.adversarial_data.token_reward)
+            branch_adversarial_datapoint = DataPoint.from_obs(WordleObservation(branch_adversarial_state), 
+                                                              self.adversarial_data.tokenizer, 
+                                                              self.adversarial_data.token_reward)
             iql_outputs = model.get_qvs([branch_expert_datapoint, branch_adversarial_datapoint])
             qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
             for i in range(N_CHARS+1):
-                branch_total_correct[i] += int(qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (1 - terminals[1, :-1]).sum()-1-i])
-                branch_total_correct_target[i] += int(target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                branch_total_correct[i] += int(
+                    qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                branch_total_correct_target[i] += int(
+                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
             total += 1
         return {
-                **{('initial_q_rank_acc_-%d' % (i+1)): (initial_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('initial_q_target_rank_acc_-%d' % (i+1)): (initial_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('branch_q_rank_acc_-%d' % (i+1)): (branch_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('branch_q_target_rank_acc_-%d' % (i+1)): (branch_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
+                **{('initial_q_rank_acc_-%d' % (i+1)): (
+                    initial_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
+                **{('initial_q_target_rank_acc_-%d' % (i+1)): (
+                    initial_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
+                **{('branch_q_rank_acc_-%d' % (i+1)): (
+                    branch_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
+                **{('branch_q_target_rank_acc_-%d' % (i+1)): (
+                    branch_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
                }
```

### Comparing `agilerl-0.1.6/agilerl/wordle/wordle_game.py` & `agilerl-0.1.7/agilerl/wordle/wordle_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,26 +182,29 @@
         if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
             new_mdp = WordleGame(self.state, self.vocab, action_history=self.action_history+[action])
             return new_mdp, new_mdp.reward(), new_mdp.is_terminal()
         if self.is_terminal():
             return None
         word = self.vocab.get_random_word_filtered()
         new_state = self.state.transition_state(action, word)
-        new_mdp = WordleGame(new_state, self.vocab.update_vocab(new_state), action_history=self.action_history+[action])
+        new_mdp = WordleGame(new_state, self.vocab.update_vocab(new_state), 
+        action_history=self.action_history+[action])
         return new_mdp, new_mdp.reward(), new_mdp.is_terminal()
     
     def all_next(self, action: str):
         if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
             return [(WordleGame(self.state, self.vocab, action_history=self.action_history+[action]), 1,)]
         if self.is_terminal():
             return []
         new_states = defaultdict(list)
         for word in self.vocab.filtered_vocab:
             new_states[self.state.transition_state(action, word)].append(word)
-        return [(WordleGame(new_state, self.vocab.update_vocab(new_state), action_history=self.action_history+[words[0]]), len(words)) for new_state, words in new_states.items()]
+        return [(WordleGame(new_state, self.vocab.update_vocab(new_state), 
+                            action_history=self.action_history+[words[0]]), 
+                            len(words)) for new_state, words in new_states.items()]
     
     def __str__(self):
         all_action_strs = []
         for action in self.action_history:
             if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
                 all_action_strs.append(action)
                 continue
```

### Comparing `agilerl-0.1.6/agilerl/wordle/wordle_tokenizer.py` & `agilerl-0.1.7/agilerl/wordle/wordle_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 import re
 from agilerl.data.tokenizer import Tokenizer
 
 class WordleTokenizer(Tokenizer):
     def __init__(self):
-        self.special_vocab = ['<g>', '<b>', '<y>', '<|pad|>', '</a>', '</s>', '<s>', '<a>', '</eod>']
+        self.special_vocab = ['<g>', '<b>', '<y>', '<|pad|>', '</a>', '</s>', '<s>', 
+                              '<a>', '</eod>']
         self.vocab = list('abcdefghijklmnopqrstuvwxyz') + self.special_vocab
         self.t2i = {w: i for i, w in enumerate(self.vocab)}
         super().__init__(self.token_to_id('<|pad|>'), 
                          self.token_to_id('</s>'), 
                          self.token_to_id('</a>'), 
                          self.token_to_id('<s>'), 
                          self.token_to_id('<a>'), 
                          self.token_to_id('</eod>'))
     
     def encode(self, str_, **kwargs):
         if isinstance(str_, str):
             special_idxs = []
             for special_char in self.special_vocab:
-                special_idxs += list(map(lambda x: (x.start(), x.end(), self.token_to_id(special_char)), re.finditer(re.escape(special_char), str_)))
+                special_idxs += list(map(lambda x: (x.start(), x.end(), 
+                                                    self.token_to_id(special_char)), 
+                                                    re.finditer(re.escape(special_char), 
+                                                                str_)))
             special_idxs.sort(key=lambda x: x[0])
             tokens = []
             curr = 0
             for s, e, tok in special_idxs:
                 tokens.extend([self.token_to_id(c) for c in str_[curr:s]])
                 tokens.append(tok)
                 curr = e
             tokens.extend([self.token_to_id(c) for c in str_[curr:]])
             return tokens, [int(t != self.pad_token_id) for t in tokens]
         elif isinstance(str_, list):
             tokens, pads = zip(*[self.encode(item) for item in str_])
             max_len = max(map(len, tokens))
-            return [list(item)+([self.pad_token_id]*(max_len-len(item))) for item in tokens], [list(item)+([0]*(max_len-len(item))) for item in pads]
+            return [list(item)+([self.pad_token_id]*(max_len-len(
+                item))) for item in tokens], [list(item)+([0]*(max_len-len(
+                item))) for item in pads]
         else:
             raise ValueError('str_ must be a string or a list of strings')
     
     def decode(self, tokens, **kwargs):
         if len(tokens) == 0:
             return ''
         if not isinstance(tokens[0], list):
```

### Comparing `agilerl-0.1.6/LICENSE` & `agilerl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.6/pyproject.toml` & `agilerl-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agilerl"
-version = "0.1.6"
+version = "0.1.7"
 description = "AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps."
 authors = ["Nick Ustaran-Anderegg <dev@agilerl.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agilerl-0.1.6/README.md` & `agilerl-0.1.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 <div align="center">
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Documentation Status](https://readthedocs.org/projects/agilerl/badge/?version=latest)](https://agilerl.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/badge/agilerl)](https://pypi.python.org/pypi/agilerl/)
 [![Discord](https://dcbadge.vercel.app/api/server/eB8HyTA2ux?style=flat)](https://discord.gg/eB8HyTA2ux)
 
+**_NEW: AgileRL now supports distributed training with HuggingFace Accelerate!<br>
+Train even faster by taking full advantage of your entire compute stack._**
+
 </div>
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
   
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
@@ -29,14 +32,15 @@
   * [Get Started](#get-started)
   * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
   * [Train an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-online)
     + [Custom Online Training Loop](#custom-online-training-loop)
   * [Train an agent on data (Offline)](#train-an-agent-on-data-offline)
     + [Custom Offline Training Loop](#custom-offline-training-loop)
   * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
+  * [Distributed training](#distributed-training)
 
 ## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
 In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
@@ -55,22 +59,27 @@
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
 If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
 
 Demo:
 ```bash
-python demo.py
+python demo_online.py
+```
+or to demo distributed training:
+```bash
+accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
 ```
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
   * CQL
   * ILQL
+  * TD3
 
 ## Train an agent on a Gym environment (Online)
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
@@ -119,46 +128,45 @@
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16)
 try:
     state_dim = env.single_observation_space.n          # Discrete observation space
     one_hot = True                                      # Requires one-hot encoding
-except:
+except Exception:
     state_dim = env.single_observation_space.shape      # Continuous observation space
     one_hot = False                                     # Does not require one-hot encoding
 try:
     action_dim = env.single_action_space.n             # Discrete action space
-except:
+except Exception:
     action_dim = env.single_action_space.shape[0]      # Continuous action space
 
 if INIT_HP['CHANNELS_LAST']:
     state_dim = (state_dim[2], state_dim[0], state_dim[1])
 
 agent_pop = initialPopulation(algo=INIT_HP['ALGO'],                 # Algorithm
                               state_dim=state_dim,                  # State dimension
                               action_dim=action_dim,                # Action dimension
                               one_hot=one_hot,                      # One-hot encoding
                               net_config=NET_CONFIG,                # Network configuration
                               INIT_HP=INIT_HP,                      # Initial hyperparameters
                               population_size=INIT_HP['POP_SIZE'],  # Population size
-                              device=torch.device("cuda"))
+                              device=device)
 ```
 Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
 ```python
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
-import torch
 
 field_names = ["state", "action", "reward", "next_state", "done"]
 memory = ReplayBuffer(action_dim=action_dim,                # Number of agent actions
                       memory_size=INIT_HP['MEMORY_SIZE'],   # Max replay buffer size
                       field_names=field_names,              # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament selection size
                                  elitism=INIT_HP['ELITISM'],            # Elitism in tournament selection
                                  population_size=INIT_HP['POP_SIZE'],   # Population size
                                  evo_step=INIT_HP['EVO_EPOCHS'])        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo=INIT_HP['ALGO'],                                 # Algorithm
@@ -168,34 +176,33 @@
                       parameters=MUTATION_PARAMS['PARAMS_MUT'],             # Network parameters mutation
                       activation=MUTATION_PARAMS['ACT_MUT'],                # Activation layer mutation
                       rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
                       rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
                       mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
                       arch=NET_CONFIG['arch'],                              # Network architecture
                       rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 ```
 The easiest training loop implementation is to use our <code>training.train.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
 ```python
 from agilerl.training.train import train
 
-trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
-                                   env_name=INIT_HP['ENV_NAME'],        # Environment name
-                                   algo=INIT_HP['ALGO'],                # Algorithm
-                                   pop=agent_pop,                       # Population of agents
-                                   memory=memory,                       # Replay buffer
-                                   swap_channels=False,                 # Swap image channel from last to first
-                                   n_episodes=INIT_HP['EPISODES'],      # Max number of training episodes
-                                   evo_epochs=INIT_HP['EVO_EPOCHS'],    # Evolution frequency
-                                   evo_loop=1,                          # Number of evaluation episodes per agent
-                                   target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
-                                   tournament=tournament,               # Tournament selection object
-                                   mutation=mutations,                  # Mutations object
-                                   wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
-                                   device=torch.device("cuda"))
+trained_pop, pop_fitnesses = train(env=env,                                 # Gym-style environment
+                                   env_name=INIT_HP['ENV_NAME'],            # Environment name
+                                   algo=INIT_HP['ALGO'],                    # Algorithm
+                                   pop=agent_pop,                           # Population of agents
+                                   memory=memory,                           # Replay buffer
+                                   swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                   n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                   evo_epochs=INIT_HP['EVO_EPOCHS'],        # Evolution frequency
+                                   evo_loop=1,                              # Number of evaluation episodes per agent
+                                   target=INIT_HP['TARGET_SCORE'],          # Target score for early stopping
+                                   tournament=tournament,                   # Tournament selection object
+                                   mutation=mutations,                      # Mutations object
+                                   wb=INIT_HP['WANDB'])                     # Weights and Biases tracking
 ```
 
 ### Custom Online Training Loop
 Alternatively, use a custom training loop. Combining all of the above:
 
 ```python
 from agilerl.utils.utils import makeVectEnvs, initialPopulation
@@ -217,28 +224,46 @@
             'LR': 1e-3,             # Learning rate
             'GAMMA': 0.99,          # Discount factor
             'LEARN_STEP': 1,        # Learning frequency
             'TAU': 1e-3,            # For soft update of target network parameters
             'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
           }
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+env = makeVectEnvs('LunarLander-v2', num_envs=16)   # Create environment
+
+try:
+    state_dim = env.single_observation_space.n       # Discrete observation space
+    one_hot = True                            # Requires one-hot encoding
+except Exception:
+    state_dim = env.single_observation_space.shape   # Continuous observation space
+    one_hot = False                           # Does not require one-hot encoding
+try:
+    action_dim = env.single_action_space.n           # Discrete action space
+except Exception:
+    action_dim = env.single_action_space.shape[0]    # Continuous action space
+
+if INIT_HP['CHANNELS_LAST']:
+    state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
 pop = initialPopulation(algo='DQN',             # Algorithm
-                        state_dim=(8,),         # State dimension
-                        action_dim=4,           # Action dimension
-                        one_hot=False,          # One-hot encoding
+                        state_dim=state_dim,    # State dimension
+                        action_dim=action_dim,  # Action dimension
+                        one_hot=one_hot,        # One-hot encoding
                         net_config=NET_CONFIG,  # Network configuration
                         INIT_HP=INIT_HP,        # Initial hyperparameters
                         population_size=6,      # Population size
-                        device=torch.device("cuda"))
+                        device=device)
 
 field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=4,             # Number of agent actions
+memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                       memory_size=10000,        # Max replay buffer size
                       field_names=field_names,  # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=2, # Tournament selection size
                                  elitism=True,      # Elitism in tournament selection
                                  population_size=6, # Population size
                                  evo_step=1)        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo='DQN',                           # Algorithm
@@ -248,41 +273,46 @@
                       parameters=0.2,                       # Network parameters mutation
                       activation=0,                         # Activation layer mutation
                       rl_hp=0.2,                            # Learning HP mutation
                       rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
                       mutation_sd=0.1,                      # Mutation strength
                       arch=NET_CONFIG['arch'],              # Network architecture
                       rand_seed=1,                          # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 
 max_episodes = 1000 # Max training episodes
 max_steps = 500     # Max steps per episode
 
 # Exploration params
 eps_start = 1.0     # Max exploration
 eps_end = 0.1       # Min exploration
 eps_decay = 0.995   # Decay per episode
 epsilon = eps_start
 
 evo_epochs = 5      # Evolution frequency
 evo_loop = 1        # Number of evaluation episodes
 
-env = makeVectEnvs('LunarLander-v2', num_envs=16)   # Create environment
-
 # TRAINING LOOP
 for idx_epi in range(max_episodes):
     for agent in pop:   # Loop through population
         state = env.reset()[0]  # Reset environment at start of episode
         score = 0
         for idx_step in range(max_steps):
+            if INIT_HP['CHANNELS_LAST']:
+                state = np.moveaxis(state, [3], [1])
             action = agent.getAction(state, epsilon)    # Get next action from agent
             next_state, reward, done, _, _ = env.step(action)   # Act in environment
             
             # Save experience to replay buffer
-            memory.save2memoryVectEnvs(state, action, reward, next_state, done)
+            if INIT_HP['CHANNELS_LAST']:
+                memory.save2memoryVectEnvs(
+                    state, action, reward, np.moveaxis(next_state, [3], [1]), done)
+            else:
+                memory.save2memoryVectEnvs(
+                    state, action, reward, next_state, done)
 
             # Learn according to learning frequency
             if memory.counter % agent.learn_step == 0 and len(memory) >= agent.batch_size:
                 experiences = memory.sample(agent.batch_size) # Sample replay buffer
                 agent.learn(experiences)    # Learn according to agent's RL algorithm
             
             state = next_state
@@ -290,15 +320,15 @@
 
     epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
         
         # Evaluate population
-        fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
+        fitnesses = [agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
         # Tournament selection and population mutation
         elite, pop = tournament.select(pop)
@@ -349,59 +379,59 @@
 NET_CONFIG = {
     'arch': 'mlp',      # Network architecture
     'h_size': [32, 32], # Actor hidden size
 }
 ```
 First, use <code>utils.utils.initialPopulation</code> to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
 ```python
-from agilerl.utils.utils import initialPopulation
+from agilerl.utils.utils import makeVectsEnvs, initialPopulation
 import torch
 import h5py
 import gymnasium as gym
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-env = gym.make(INIT_HP['ENV_NAME'])
+env = makeVectEnvs(INIT_HP['ENV_NAME'], num_envs=1)
 try:
-    state_dim = env.observation_space.n       # Discrete observation space
-    one_hot = True                            # Requires one-hot encoding
+    state_dim = env.single_observation_space.n          # Discrete observation space
+    one_hot = True                                      # Requires one-hot encoding
 except Exception:
-    state_dim = env.observation_space.shape   # Continuous observation space
-    one_hot = False                           # Does not require one-hot encoding
+    state_dim = env.single_observation_space.shape      # Continuous observation space
+    one_hot = False                                     # Does not require one-hot encoding
 try:
-    action_dim = env.action_space.n           # Discrete action space
+    action_dim = env.single_action_space.n             # Discrete action space
 except Exception:
-    action_dim = env.action_space.shape[0]    # Continuous action space
+    action_dim = env.single_action_space.shape[0]      # Continuous action space
 
 if INIT_HP['CHANNELS_LAST']:
     state_dim = (state_dim[2], state_dim[0], state_dim[1])
 
 dataset = h5py.File(INIT_HP['DATASET'], 'r')
 
 agent_pop = initialPopulation(algo=INIT_HP['ALGO'],                 # Algorithm
                               state_dim=state_dim,                  # State dimension
                               action_dim=action_dim,                # Action dimension
                               one_hot=one_hot,                      # One-hot encoding
                               net_config=NET_CONFIG,                # Network configuration
                               INIT_HP=INIT_HP,                      # Initial hyperparameters
                               population_size=INIT_HP['POP_SIZE'],  # Population size
-                              device=torch.device("cuda"))
+                              device=device)
 ```
 Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
 ```python
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
 import torch
 
 field_names = ["state", "action", "reward", "next_state", "done"]
 memory = ReplayBuffer(action_dim=action_dim,                # Number of agent actions
                       memory_size=INIT_HP['MEMORY_SIZE'],   # Max replay buffer size
                       field_names=field_names,              # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament selection size
                                  elitism=INIT_HP['ELITISM'],            # Elitism in tournament selection
                                  population_size=INIT_HP['POP_SIZE'],   # Population size
                                  evo_step=INIT_HP['EVO_EPOCHS'])        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo=INIT_HP['ALGO'],                                 # Algorithm
@@ -411,49 +441,48 @@
                       parameters=MUTATION_PARAMS['PARAMS_MUT'],             # Network parameters mutation
                       activation=MUTATION_PARAMS['ACT_MUT'],                # Activation layer mutation
                       rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
                       rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
                       mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
                       arch=NET_CONFIG['arch'],                              # Network architecture
                       rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 ```
 The easiest training loop implementation is to use our <code>training.train_offline.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
 ```python
 from agilerl.training.train_offline import train
 
-trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
-                                   env_name=INIT_HP['ENV_NAME'],        # Environment name
-                                   dataset=dataset,                     # Offline dataset
-                                   algo=INIT_HP['ALGO'],                # Algorithm
-                                   pop=agent_pop,                       # Population of agents
-                                   memory=memory,                       # Replay buffer
-                                   swap_channels=False,                 # Swap image channel from last to first
-                                   n_episodes=INIT_HP['EPISODES'],      # Max number of training episodes
-                                   evo_epochs=INIT_HP['EVO_EPOCHS'],    # Evolution frequency
-                                   evo_loop=1,                          # Number of evaluation episodes per agent
-                                   target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
-                                   tournament=tournament,               # Tournament selection object
-                                   mutation=mutations,                  # Mutations object
-                                   wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
-                                   device=torch.device("cuda"))
+trained_pop, pop_fitnesses = train(env=env,                                 # Gym-style environment
+                                   env_name=INIT_HP['ENV_NAME'],            # Environment name
+                                   dataset=dataset,                         # Offline dataset
+                                   algo=INIT_HP['ALGO'],                    # Algorithm
+                                   pop=agent_pop,                           # Population of agents
+                                   memory=memory,                           # Replay buffer
+                                   swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                   n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                   evo_epochs=INIT_HP['EVO_EPOCHS'],        # Evolution frequency
+                                   evo_loop=1,                              # Number of evaluation episodes per agent
+                                   target=INIT_HP['TARGET_SCORE'],          # Target score for early stopping
+                                   tournament=tournament,                   # Tournament selection object
+                                   mutation=mutations,                      # Mutations object
+                                   wb=INIT_HP['WANDB'])                     # Weights and Biases tracking
 ```
 
 ### Custom Offline Training Loop
 Alternatively, use a custom training loop. Combining all of the above:
 
 ```python
-from agilerl.utils.utils import initialPopulation
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
-import gymnasium as gym
 import h5py
 import numpy as np
 import torch
+from tqdm import trange
 
 NET_CONFIG = {
                 'arch': 'mlp',       # Network architecture
                 'h_size': [32, 32],  # Actor hidden size
              }
 
 INIT_HP = {
@@ -462,28 +491,47 @@
             'LR': 1e-3,             # Learning rate
             'GAMMA': 0.99,          # Discount factor
             'LEARN_STEP': 1,        # Learning frequency
             'TAU': 1e-3,            # For soft update of target network parameters
             'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
           }
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+env = gym.make('CartPole-v1')   # Create environment
+dataset = h5py.File('data/cartpole/cartpole_random_v1.1.0.h5', 'r')  # Load dataset
+
+try:
+    state_dim = env.single_observation_space.n          # Discrete observation space
+    one_hot = True                                      # Requires one-hot encoding
+except Exception:
+    state_dim = env.single_observation_space.shape      # Continuous observation space
+    one_hot = False                                     # Does not require one-hot encoding
+try:
+    action_dim = env.single_action_space.n             # Discrete action space
+except Exception:
+    action_dim = env.single_action_space.shape[0]      # Continuous action space
+
+if INIT_HP['CHANNELS_LAST']:
+    state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
 pop = initialPopulation(algo='CQN',             # Algorithm
-                        state_dim=(4,),         # State dimension
-                        action_dim=2,           # Action dimension
-                        one_hot=False,          # One-hot encoding
+                        state_dim=state_dim,    # State dimension
+                        action_dim=action_dim,  # Action dimension
+                        one_hot=one_hot,        # One-hot encoding
                         net_config=NET_CONFIG,  # Network configuration
                         INIT_HP=INIT_HP,        # Initial hyperparameters
                         population_size=6,      # Population size
-                        device=torch.device("cuda"))
+                        device=device)
 
 field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=2,             # Number of agent actions
+memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                       memory_size=10000,        # Max replay buffer size
                       field_names=field_names,  # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=2, # Tournament selection size
                                  elitism=True,      # Elitism in tournament selection
                                  population_size=6, # Population size
                                  evo_step=1)        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo='CQN',                           # Algorithm
@@ -493,41 +541,39 @@
                       parameters=0.2,                       # Network parameters mutation
                       activation=0,                         # Activation layer mutation
                       rl_hp=0.2,                            # Learning HP mutation
                       rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
                       mutation_sd=0.1,                      # Mutation strength
                       arch=NET_CONFIG['arch'],              # Network architecture
                       rand_seed=1,                          # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 
 max_episodes = 1000 # Max training episodes
 max_steps = 500     # Max steps per episode
 
 evo_epochs = 5      # Evolution frequency
 evo_loop = 1        # Number of evaluation episodes
 
-env = gym.make('CartPole-v1')   # Create environment
-
-dataset = h5py.File('data/cartpole/cartpole_random_v1.1.0.h5', 'r')  # Load dataset
-
 # Save transitions to replay buffer
 dataset_length = dataset['rewards'].shape[0]
-for i in range(dataset_length-1):
+for i in trange(dataset_length-1):
     state = dataset['observations'][i]
     next_state = dataset['observations'][i+1]
-    if swap_channels:
+    if INIT_HP['CHANNELS_LAST']:
         state = np.moveaxis(state, [3], [1])
         next_state = np.moveaxis(next_state, [3], [1])
     action = dataset['actions'][i]
     reward = dataset['rewards'][i]
     done = bool(dataset['terminals'][i])
+    # Save experience to replay buffer
     memory.save2memory(state, action, reward, next_state, done)
 
+
 # TRAINING LOOP
-for idx_epi in range(max_episodes):
+for idx_epi in trange(max_episodes):
     for agent in pop:   # Loop through population
         for idx_step in range(max_steps):
             experiences = memory.sample(agent.batch_size)   # Sample replay buffer
             # Learn according to agent's RL algorithm
             agent.learn(experiences)
 
     # Now evolve population if necessary
@@ -560,8 +606,199 @@
 If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
 
 Similarly, to then run ILQL and perform RLHF on the BC model:
 ```bash
 python run_ilql.py
 ```
 
+## Distributed training
+AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace 
+<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction. 
+This should make implementations simple, but also highly customisable, by continuing to expose the PyTorch training loop beneath it all.
+
+To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example 
+config file has been provided at <code>configs/accelerate/accelerate.yaml</code>.
+
+Putting this all together, launching a distributed training script can be done as follows:
+```bash
+accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
+```
+
+There are some key considerations to bear in mind when implementing a distributed training run:
+  * If you only want to execute something once, rather than repeating it for each process, e.g printing a statement, logging to W&B, then use <code>if accelerator.is_main_process:</code>.
+  * Training happens in parallel on each device, meaning that steps in a RL environment happen on each device too. In order to count the number of global training steps taken, you must multiply the number of steps you have taken on a singular device by the number of devices (assuming they are equal). If you want to use distributed training to train more quickly, and normally you would train for 100,000 steps on one device, you can now train for just 25,000 steps if using four devices.
+
+Example distributed training loop:
+
+```python
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
+from agilerl.components.replay_buffer import ReplayBuffer
+from agilerl.components.replay_data import ReplayDataset
+from agilerl.components.sampler import Sampler
+from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations
+from accelerate import Accelerator
+import numpy as np
+import os
+from torch.utils.data import DataLoader
+from tqdm import trange
+
+if __name__ == '__main__':
+
+    accelerator = Accelerator()
+
+    NET_CONFIG = {
+        'arch': 'mlp',       # Network architecture
+        'h_size': [32, 32],  # Actor hidden size
+    }
+
+    INIT_HP = {
+        'POPULATION_SIZE': 4,   # Population size
+        'DOUBLE': True,         # Use double Q-learning in DQN or CQN
+        'BATCH_SIZE': 128,      # Batch size
+        'LR': 1e-3,             # Learning rate
+        'GAMMA': 0.99,          # Discount factor
+        'LEARN_STEP': 1,        # Learning frequency
+        'TAU': 1e-3,            # For soft update of target network parameters
+        'POLICY_FREQ': 2,       # DDPG target network update frequency vs policy network
+        # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        'CHANNELS_LAST': False
+    }
+
+    env = makeVectEnvs('LunarLander-v2', num_envs=8)   # Create environment
+    try:
+        state_dim = env.single_observation_space.n          # Discrete observation space
+        one_hot = True                                      # Requires one-hot encoding
+    except Exception:
+        state_dim = env.single_observation_space.shape      # Continuous observation space
+        one_hot = False                                     # Does not require one-hot encoding
+    try:
+        action_dim = env.single_action_space.n             # Discrete action space
+    except Exception:
+        action_dim = env.single_action_space.shape[0]      # Continuous action space
+
+    if INIT_HP['CHANNELS_LAST']:
+        state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
+    pop = initialPopulation(algo='DQN',                 # Algorithm
+                            state_dim=state_dim,        # State dimension
+                            action_dim=action_dim,      # Action dimension
+                            one_hot=one_hot,            # One-hot encoding
+                            net_config=NET_CONFIG,      # Network configuration
+                            INIT_HP=INIT_HP,            # Initial hyperparameters
+                            population_size=INIT_HP['POPULATION_SIZE'], # Population size
+                            accelerator=accelerator)    # Accelerator
+
+    field_names = ["state", "action", "reward", "next_state", "done"]
+    memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
+                        memory_size=10000,        # Max replay buffer size
+                        field_names=field_names)  # Field names to store in memory
+    replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE'])
+    replay_dataloader = DataLoader(replay_dataset, batch_size=None)
+    replay_dataloader = accelerator.prepare(replay_dataloader)
+    sampler = Sampler(distributed=True, 
+                    dataset=replay_dataset, 
+                    dataloader=replay_dataloader)
+
+    tournament = TournamentSelection(tournament_size=2,  # Tournament selection size
+                                    elitism=True,      # Elitism in tournament selection
+                                    population_size=INIT_HP['POPULATION_SIZE'],  # Population size
+                                    evo_step=1)        # Evaluate using last N fitness scores
+
+    mutations = Mutations(algo='DQN',                           # Algorithm
+                        no_mutation=0.4,                      # No mutation
+                        architecture=0.2,                     # Architecture mutation
+                        new_layer_prob=0.2,                   # New layer mutation
+                        parameters=0.2,                       # Network parameters mutation
+                        activation=0,                         # Activation layer mutation
+                        rl_hp=0.2,                            # Learning HP mutation
+                        rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
+                        mutation_sd=0.1,                      # Mutation strength
+                        arch=NET_CONFIG['arch'],              # Network architecture
+                        rand_seed=1,                          # Random seed
+                        accelerator=accelerator)              # Accelerator)
+
+    max_episodes = 1000 # Max training episodes
+    max_steps = 500     # Max steps per episode
+
+    # Exploration params
+    eps_start = 1.0     # Max exploration
+    eps_end = 0.1       # Min exploration
+    eps_decay = 0.995   # Decay per episode
+    epsilon = eps_start
+
+    evo_epochs = 5      # Evolution frequency
+    evo_loop = 1        # Number of evaluation episodes
+
+    accel_temp_models_path = 'models/{}'.format('LunarLander-v2')
+    if accelerator.is_main_process:
+        if not os.path.exists(accel_temp_models_path):
+            os.makedirs(accel_temp_models_path)
+
+    print(f'\nDistributed training on {accelerator.device}...')
+
+    # TRAINING LOOP
+    for idx_epi in trange(max_episodes):
+        accelerator.wait_for_everyone()
+        for agent in pop:   # Loop through population
+            state = env.reset()[0]  # Reset environment at start of episode
+            score = 0
+            for idx_step in range(max_steps):
+                # Get next action from agent
+                action = agent.getAction(state, epsilon)
+                next_state, reward, done, _, _ = env.step(
+                    action)   # Act in environment
+
+                # Save experience to replay buffer
+                memory.save2memoryVectEnvs(
+                    state, action, reward, next_state, done)
+
+                # Learn according to learning frequency
+                if memory.counter % agent.learn_step == 0 and len(
+                        memory) >= agent.batch_size:
+                    # Sample dataloader
+                    experiences = sampler.sample(agent.batch_size)
+                    # Learn according to agent's RL algorithm
+                    agent.learn(experiences)
+
+                state = next_state
+                score += reward
+
+        # Update epsilon for exploration
+        epsilon = max(eps_end, epsilon * eps_decay)
+
+        # Now evolve population if necessary
+        if (idx_epi + 1) % evo_epochs == 0:
+
+            # Evaluate population
+            fitnesses = [
+                agent.test(
+                    env,
+                    swap_channels=False,
+                    max_steps=max_steps,
+                    loop=evo_loop) for agent in pop]
+
+            if accelerator.is_main_process:
+                print(f'Episode {idx_epi+1}/{max_episodes}')
+                print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
+                print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
+
+            # Tournament selection and population mutation
+            accelerator.wait_for_everyone()
+            for model in pop:
+                model.unwrap_models()
+            accelerator.wait_for_everyone()
+            if accelerator.is_main_process:
+                elite, pop = tournament.select(pop)
+                pop = mutations.mutation(pop)
+                for pop_i, model in enumerate(pop):
+                    model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+            accelerator.wait_for_everyone()
+            if not accelerator.is_main_process:
+                for pop_i, model in enumerate(pop):
+                    model.loadCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+            accelerator.wait_for_everyone()
+            for model in pop:
+                model.wrap_models()
+```
+
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -7,15 +7,17 @@
                     Join the Discord_Server to collaborate.
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
      opensource.org/licenses/Apache-2.0) [![Documentation Status](https://
        readthedocs.org/projects/agilerl/badge/?version=latest)](https://
     agilerl.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://
   static.pepy.tech/badge/agilerl)](https://pypi.python.org/pypi/agilerl/) [!
 [Discord](https://dcbadge.vercel.app/api/server/eB8HyTA2ux?style=flat)](https:/
-                            /discord.gg/eB8HyTA2ux)
+/discord.gg/eB8HyTA2ux) **_NEW: AgileRL now supports distributed training with
+                            HuggingFace Accelerate!
+  Train even faster by taking full advantage of your entire compute stack._**
 This is a Deep Reinforcement Learning library focused on improving development
 by introducing RLOps - MLOps for reinforcement learning. This library is
 initially focused on reducing the time taken for training models and
 hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for
 reinforcement learning.
 Evolutionary HPO has been shown to drastically reduce overall training times by
 automatically converging on optimal hyperparameters, without requiring numerous
@@ -30,282 +32,303 @@
                              optimization process.
 ## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
 * [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
 an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-
 online) + [Custom Online Training Loop](#custom-online-training-loop) * [Train
 an agent on data (Offline)](#train-an-agent-on-data-offline) + [Custom Offline
 Training Loop](#custom-offline-training-loop) * [Train an agent on a language
-environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) ##
-Benchmarks Reinforcement learning algorithms and libraries are usually
-benchmarked once the optimal hyperparameters for training are known, but it
-often takes hundreds or thousands of experiments to discover these. This is
-unrealistic and does not reflect the true, total time taken for training. What
-if we could remove the need to conduct all these prior experiments? In the
-charts below, a single AgileRL run, which automatically tunes hyperparameters,
-is benchmarked against Optuna's multiple training runs traditionally required
-for hyperparameter optimization, demonstrating the real time savings possible.
-Global steps is the sum of every step taken by any agent in the environment,
-including across an entire population.
+environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) *
+[Distributed training](#distributed-training) ## Benchmarks Reinforcement
+learning algorithms and libraries are usually benchmarked once the optimal
+hyperparameters for training are known, but it often takes hundreds or
+thousands of experiments to discover these. This is unrealistic and does not
+reflect the true, total time taken for training. What if we could remove the
+need to conduct all these prior experiments? In the charts below, a single
+AgileRL run, which automatically tunes hyperparameters, is benchmarked against
+Optuna's multiple training runs traditionally required for hyperparameter
+optimization, demonstrating the real time savings possible. Global steps is the
+sum of every step taken by any agent in the environment, including across an
+entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
-data.zip here. Demo: ```bash python demo.py ``` ## Algorithms implemented (more
-coming soon!) * DQN * DDPG * CQL * ILQL ## Train an agent on a Gym environment
-(Online) Before starting training, there are some meta-hyperparameters and
-settings that must be set. These are defined in INIT_HP, for general
-parameters, and MUTATION_PARAMS, which define the evolutionary probabilities,
-and NET_CONFIG, which defines the network architecture. For example: ```python
-INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN',
-# Algorithm 'DOUBLE': True, # Use double Q-learning 'CHANNELS_LAST': False, #
-Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
-'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate 'EPISODES': 2000, #
-Max no. episodes 'TARGET_SCORE': 200., # Early training stop at avg score of
-last 100 episodes 'GAMMA': 0.99, # Discount factor 'MEMORY_SIZE': 10000, # Max
-memory buffer size 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For
-soft update of target parameters 'TOURN_SIZE': 2, # Tournament size 'ELITISM':
-True, # Elitism in tournament selection 'POP_SIZE': 6, # Population size
-'EVO_EPOCHS': 20, # Evolution frequency 'POLICY_FREQ': 2, # Policy network
-update frequency 'WANDB': True # Log with Weights and Biases } ``` ```python
-MUTATION_PARAMS = { # Relative probabilities 'NO_MUT': 0.4, # No mutation
-'ARCH_MUT': 0.2, # Architecture mutation 'NEW_LAYER': 0.2, # New layer mutation
-'PARAMS_MUT': 0.2, # Network parameters mutation 'ACT_MUT': 0, # Activation
-layer mutation 'RL_HP_MUT': 0.2, # Learning HP mutation 'RL_HP_SELECTION':
-['lr', 'batch_size'], # Learning HPs to choose from 'MUT_SD': 0.1, # Mutation
-strength 'RAND_SEED': 1, # Random seed } ``` ```python NET_CONFIG = { 'arch':
-'mlp', # Network architecture 'h_size': [32, 32], # Actor hidden size } ```
-First, use utils.utils.initialPopulation to create a list of agents - our
-population that will evolve and mutate to the optimal hyperparameters.
-```python from agilerl.utils.utils import makeVectEnvs, initialPopulation
-import torch device = torch.device("cuda" if torch.cuda.is_available() else
-"cpu") env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16) try:
-state_dim = env.single_observation_space.n # Discrete observation space one_hot
-= True # Requires one-hot encoding except: state_dim =
-env.single_observation_space.shape # Continuous observation space one_hot =
-False # Does not require one-hot encoding try: action_dim =
-env.single_action_space.n # Discrete action space except: action_dim =
-env.single_action_space.shape[0] # Continuous action space if INIT_HP
-['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
-agent_pop = initialPopulation(algo=INIT_HP['ALGO'], # Algorithm
+data.zip here. Demo: ```bash python demo_online.py ``` or to demo distributed
+training: ```bash accelerate_launch --config_file configs/accelerate/
+accelerate.yaml demo_online_distributed.py ``` ## Algorithms implemented (more
+coming soon!) * DQN * DDPG * CQL * ILQL * TD3 ## Train an agent on a Gym
+environment (Online) Before starting training, there are some meta-
+hyperparameters and settings that must be set. These are defined in INIT_HP,
+for general parameters, and MUTATION_PARAMS, which define the evolutionary
+probabilities, and NET_CONFIG, which defines the network architecture. For
+example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment
+name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double Q-learning
+'CHANNELS_LAST': False, # Swap image channels dimension from last to first [H,
+W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate
+'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training
+stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount factor
+'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning
+frequency 'TAU': 1e-3, # For soft update of target parameters 'TOURN_SIZE': 2,
+# Tournament size 'ELITISM': True, # Elitism in tournament selection
+'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution frequency
+'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True # Log with
+Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative probabilities
+'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture mutation
+'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network parameters
+mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2, # Learning
+HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs to choose
+from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed } ```
+```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32,
+32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
+create a list of agents - our population that will evolve and mutate to the
+optimal hyperparameters. ```python from agilerl.utils.utils import
+makeVectEnvs, initialPopulation import torch device = torch.device("cuda" if
+torch.cuda.is_available() else "cpu") env = makeVectEnvs(env_name=INIT_HP
+['ENV_NAME'], num_envs=16) try: state_dim = env.single_observation_space.n #
+Discrete observation space one_hot = True # Requires one-hot encoding except
+Exception: state_dim = env.single_observation_space.shape # Continuous
+observation space one_hot = False # Does not require one-hot encoding try:
+action_dim = env.single_action_space.n # Discrete action space except
+Exception: action_dim = env.single_action_space.shape[0] # Continuous action
+space if INIT_HP['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0],
+state_dim[1]) agent_pop = initialPopulation(algo=INIT_HP['ALGO'], # Algorithm
 state_dim=state_dim, # State dimension action_dim=action_dim, # Action
 dimension one_hot=one_hot, # One-hot encoding net_config=NET_CONFIG, # Network
 configuration INIT_HP=INIT_HP, # Initial hyperparameters
-population_size=INIT_HP['POP_SIZE'], # Population size device=torch.device
-("cuda")) ``` Next, create the tournament, mutations and experience replay
-buffer objects that allow agents to share memory and efficiently perform
-evolutionary HPO. ```python from agilerl.components.replay_buffer import
-ReplayBuffer from agilerl.hpo.tournament import TournamentSelection from
-agilerl.hpo.mutation import Mutations import torch field_names = ["state",
-"action", "reward", "next_state", "done"] memory = ReplayBuffer
-(action_dim=action_dim, # Number of agent actions memory_size=INIT_HP
-['MEMORY_SIZE'], # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament
-selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament selection
-population_size=INIT_HP['POP_SIZE'], # Population size evo_step=INIT_HP
-['EVO_EPOCHS']) # Evaluate using last N fitness scores mutations = Mutations
-(algo=INIT_HP['ALGO'], # Algorithm no_mutation=MUTATION_PARAMS['NO_MUT'], # No
-mutation architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
+population_size=INIT_HP['POP_SIZE'], # Population size device=device) ``` Next,
+create the tournament, mutations and experience replay buffer objects that
+allow agents to share memory and efficiently perform evolutionary HPO.
+```python from agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
+import Mutations field_names = ["state", "action", "reward", "next_state",
+"done"] memory = ReplayBuffer(action_dim=action_dim, # Number of agent actions
+memory_size=INIT_HP['MEMORY_SIZE'], # Max replay buffer size
+field_names=field_names, # Field names to store in memory device=device)
+tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], #
+Tournament selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament
+selection population_size=INIT_HP['POP_SIZE'], # Population size
+evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness scores
+mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
+no_mutation=MUTATION_PARAMS['NO_MUT'], # No mutation
+architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
 new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], # New layer mutation
 parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
 activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
 rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
 rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
 from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
 ['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
-Random seed device=torch.device("cuda")) ``` The easiest training loop
-implementation is to use our training.train.train() function. It requires the
-agent have functions getAction() and learn(). ```python from
-agilerl.training.train import train trained_pop, pop_fitnesses = train(env=env,
-# Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment name
-algo=INIT_HP['ALGO'], # Algorithm pop=agent_pop, # Population of agents
-memory=memory, # Replay buffer swap_channels=False, # Swap image channel from
-last to first n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
+Random seed device=device) ``` The easiest training loop implementation is to
+use our training.train.train() function. It requires the agent have functions
+getAction() and learn(). ```python from agilerl.training.train import train
+trained_pop, pop_fitnesses = train(env=env, # Gym-style environment
+env_name=INIT_HP['ENV_NAME'], # Environment name algo=INIT_HP['ALGO'], #
+Algorithm pop=agent_pop, # Population of agents memory=memory, # Replay buffer
+swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image channel from last to first
+n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
 evo_epochs=INIT_HP['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of
 evaluation episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score
 for early stopping tournament=tournament, # Tournament selection object
-mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
-Biases tracking device=torch.device("cuda")) ``` ### Custom Online Training
-Loop Alternatively, use a custom training loop. Combining all of the above:
-```python from agilerl.utils.utils import makeVectEnvs, initialPopulation from
-agilerl.components.replay_buffer import ReplayBuffer from
-agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
-import Mutations import gymnasium as gym import numpy as np import torch
-NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32], #
-Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
-'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
-Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
-update of target network parameters 'CHANNELS_LAST': False # Swap image
-channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
-initialPopulation(algo='DQN', # Algorithm state_dim=(8,), # State dimension
-action_dim=4, # Action dimension one_hot=False, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=6, # Population size device=torch.device
-("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=4, # Number of agent actions
+mutation=mutations, # Mutations object wb=INIT_HP['WANDB']) # Weights and
+Biases tracking ``` ### Custom Online Training Loop Alternatively, use a custom
+training loop. Combining all of the above: ```python from agilerl.utils.utils
+import makeVectEnvs, initialPopulation from agilerl.components.replay_buffer
+import ReplayBuffer from agilerl.hpo.tournament import TournamentSelection from
+agilerl.hpo.mutation import Mutations import gymnasium as gym import numpy as
+np import torch NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-
+learning 'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA':
+0.99, # Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, #
+For soft update of target network parameters 'CHANNELS_LAST': False # Swap
+image channels dimension from last to first [H, W, C] -> [C, H, W] } device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env = makeVectEnvs
+('LunarLander-v2', num_envs=16) # Create environment try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='DQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=6, # Population size device=device)
+field_names = ["state", "action", "reward", "next_state", "done"] memory =
+ReplayBuffer(action_dim=action_dim, # Number of agent actions
 memory_size=10000, # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=2, # Tournament selection size
-elitism=True, # Elitism in tournament selection population_size=6, # Population
-size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
-(algo='DQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
-Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
-# Network parameters mutation activation=0, # Activation layer mutation
-rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
-Learning HPs to choose from mutation_sd=0.1, # Mutation strength
-arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random seed
-device=torch.device("cuda")) max_episodes = 1000 # Max training episodes
-max_steps = 500 # Max steps per episode # Exploration params eps_start = 1.0 #
-Max exploration eps_end = 0.1 # Min exploration eps_decay = 0.995 # Decay per
-episode epsilon = eps_start evo_epochs = 5 # Evolution frequency evo_loop = 1 #
-Number of evaluation episodes env = makeVectEnvs('LunarLander-v2', num_envs=16)
-# Create environment # TRAINING LOOP for idx_epi in range(max_episodes): for
-agent in pop: # Loop through population state = env.reset()[0] # Reset
-environment at start of episode score = 0 for idx_step in range(max_steps):
-action = agent.getAction(state, epsilon) # Get next action from agent
-next_state, reward, done, _, _ = env.step(action) # Act in environment # Save
-experience to replay buffer memory.save2memoryVectEnvs(state, action, reward,
-next_state, done) # Learn according to learning frequency if memory.counter %
-agent.learn_step == 0 and len(memory) >= agent.batch_size: experiences =
-memory.sample(agent.batch_size) # Sample replay buffer agent.learn(experiences)
-# Learn according to agent's RL algorithm state = next_state score += reward
-epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration #
-Now evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
-population fitnesses = [agent.test(env, swap_channels=False,
-max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
-{idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
-fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
-for agent in pop]}') # Tournament selection and population mutation elite, pop
-= tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
-data (Offline) Like with online RL, above, there are some meta-hyperparameters
-and settings that must be set before starting training. These are defined in
-INIT_HP, for general parameters, and MUTATION_PARAMS, which define the
-evolutionary probabilities, and NET_CONFIG, which defines the network
-architecture. For example: ```python INIT_HP = { 'ENV_NAME': 'CartPole-v1', #
-Gym environment name 'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', #
-Offline RL dataset 'ALGO': 'CQN', # Algorithm 'DOUBLE': True, # Use double Q-
-learning # Swap image channels dimension from last to first [H, W, C] -> [C, H,
-W] 'CHANNELS_LAST': False, 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
-Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
-Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
-factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
-Learning frequency 'TAU': 1e-3, # For soft update of target parameters
-'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
-selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
-frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
-Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
-probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
-mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
-parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
-# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
-to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
-} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
-[32, 32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
-create a list of agents - our population that will evolve and mutate to the
-optimal hyperparameters. ```python from agilerl.utils.utils import
-initialPopulation import torch import h5py import gymnasium as gym device =
-torch.device("cuda" if torch.cuda.is_available() else "cpu") env = gym.make
-(INIT_HP['ENV_NAME']) try: state_dim = env.observation_space.n # Discrete
-observation space one_hot = True # Requires one-hot encoding except Exception:
-state_dim = env.observation_space.shape # Continuous observation space one_hot
-= False # Does not require one-hot encoding try: action_dim =
-env.action_space.n # Discrete action space except Exception: action_dim =
-env.action_space.shape[0] # Continuous action space if INIT_HP
-['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
-dataset = h5py.File(INIT_HP['DATASET'], 'r') agent_pop = initialPopulation
-(algo=INIT_HP['ALGO'], # Algorithm state_dim=state_dim, # State dimension
-action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=INIT_HP['POP_SIZE'], # Population size
-device=torch.device("cuda")) ``` Next, create the tournament, mutations and
+names to store in memory device=device) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo='DQN', #
+Algorithm no_mutation=0.4, # No mutation architecture=0.2, # Architecture
+mutation new_layer_prob=0.2, # New layer mutation parameters=0.2, # Network
+parameters mutation activation=0, # Activation layer mutation rl_hp=0.2, #
+Learning HP mutation rl_hp_selection=['lr', 'batch_size'], # Learning HPs to
+choose from mutation_sd=0.1, # Mutation strength arch=NET_CONFIG['arch'], #
+Network architecture rand_seed=1, # Random seed device=device) max_episodes =
+1000 # Max training episodes max_steps = 500 # Max steps per episode #
+Exploration params eps_start = 1.0 # Max exploration eps_end = 0.1 # Min
+exploration eps_decay = 0.995 # Decay per episode epsilon = eps_start
+evo_epochs = 5 # Evolution frequency evo_loop = 1 # Number of evaluation
+episodes # TRAINING LOOP for idx_epi in range(max_episodes): for agent in pop:
+# Loop through population state = env.reset()[0] # Reset environment at start
+of episode score = 0 for idx_step in range(max_steps): if INIT_HP
+['CHANNELS_LAST']: state = np.moveaxis(state, [3], [1]) action =
+agent.getAction(state, epsilon) # Get next action from agent next_state,
+reward, done, _, _ = env.step(action) # Act in environment # Save experience to
+replay buffer if INIT_HP['CHANNELS_LAST']: memory.save2memoryVectEnvs( state,
+action, reward, np.moveaxis(next_state, [3], [1]), done) else:
+memory.save2memoryVectEnvs( state, action, reward, next_state, done) # Learn
+according to learning frequency if memory.counter % agent.learn_step == 0 and
+len(memory) >= agent.batch_size: experiences = memory.sample(agent.batch_size)
+# Sample replay buffer agent.learn(experiences) # Learn according to agent's RL
+algorithm state = next_state score += reward epsilon = max(eps_end,
+epsilon*eps_decay) # Update epsilon for exploration # Now evolve population if
+necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate population fitnesses =
+[agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps,
+loop=evo_loop) for agent in pop] print(f'Episode {idx_epi+1}/{max_episodes}')
+print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}') print(f'100
+fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}') #
+Tournament selection and population mutation elite, pop = tournament.select
+(pop) pop = mutations.mutation(pop) ``` ## Train an agent on data (Offline)
+Like with online RL, above, there are some meta-hyperparameters and settings
+that must be set before starting training. These are defined in INIT_HP, for
+general parameters, and MUTATION_PARAMS, which define the evolutionary
+probabilities, and NET_CONFIG, which defines the network architecture. For
+example: ```python INIT_HP = { 'ENV_NAME': 'CartPole-v1', # Gym environment
+name 'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', # Offline RL dataset
+'ALGO': 'CQN', # Algorithm 'DOUBLE': True, # Use double Q-learning # Swap image
+channels dimension from last to first [H, W, C] -> [C, H, W] 'CHANNELS_LAST':
+False, 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate 'EPISODES':
+2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training stop at avg
+score of last 100 episodes 'GAMMA': 0.99, # Discount factor 'MEMORY_SIZE':
+10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning frequency 'TAU':
+1e-3, # For soft update of target parameters 'TOURN_SIZE': 2, # Tournament size
+'ELITISM': True, # Elitism in tournament selection 'POP_SIZE': 6, # Population
+size 'EVO_EPOCHS': 20, # Evolution frequency 'POLICY_FREQ': 2, # Policy network
+update frequency 'WANDB': True # Log with Weights and Biases } ``` ```python
+MUTATION_PARAMS = { # Relative probabilities 'NO_MUT': 0.4, # No mutation
+'ARCH_MUT': 0.2, # Architecture mutation 'NEW_LAYER': 0.2, # New layer mutation
+'PARAMS_MUT': 0.2, # Network parameters mutation 'ACT_MUT': 0, # Activation
+layer mutation 'RL_HP_MUT': 0.2, # Learning HP mutation 'RL_HP_SELECTION':
+['lr', 'batch_size'], # Learning HPs to choose from 'MUT_SD': 0.1, # Mutation
+strength 'RAND_SEED': 1, # Random seed } ``` ```python NET_CONFIG = { 'arch':
+'mlp', # Network architecture 'h_size': [32, 32], # Actor hidden size } ```
+First, use utils.utils.initialPopulation to create a list of agents - our
+population that will evolve and mutate to the optimal hyperparameters.
+```python from agilerl.utils.utils import makeVectsEnvs, initialPopulation
+import torch import h5py import gymnasium as gym device = torch.device("cuda"
+if torch.cuda.is_available() else "cpu") env = makeVectEnvs(INIT_HP
+['ENV_NAME'], num_envs=1) try: state_dim = env.single_observation_space.n #
+Discrete observation space one_hot = True # Requires one-hot encoding except
+Exception: state_dim = env.single_observation_space.shape # Continuous
+observation space one_hot = False # Does not require one-hot encoding try:
+action_dim = env.single_action_space.n # Discrete action space except
+Exception: action_dim = env.single_action_space.shape[0] # Continuous action
+space if INIT_HP['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0],
+state_dim[1]) dataset = h5py.File(INIT_HP['DATASET'], 'r') agent_pop =
+initialPopulation(algo=INIT_HP['ALGO'], # Algorithm state_dim=state_dim, #
+State dimension action_dim=action_dim, # Action dimension one_hot=one_hot, #
+One-hot encoding net_config=NET_CONFIG, # Network configuration
+INIT_HP=INIT_HP, # Initial hyperparameters population_size=INIT_HP['POP_SIZE'],
+# Population size device=device) ``` Next, create the tournament, mutations and
 experience replay buffer objects that allow agents to share memory and
 efficiently perform evolutionary HPO. ```python from
 agilerl.components.replay_buffer import ReplayBuffer from
 agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
 import Mutations import torch field_names = ["state", "action", "reward",
 "next_state", "done"] memory = ReplayBuffer(action_dim=action_dim, # Number of
 agent actions memory_size=INIT_HP['MEMORY_SIZE'], # Max replay buffer size
-field_names=field_names, # Field names to store in memory device=torch.device
-("cuda")) tournament = TournamentSelection(tournament_size=INIT_HP
-['TOURN_SIZE'], # Tournament selection size elitism=INIT_HP['ELITISM'], #
-Elitism in tournament selection population_size=INIT_HP['POP_SIZE'], #
-Population size evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness
-scores mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
+field_names=field_names, # Field names to store in memory device=device)
+tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], #
+Tournament selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament
+selection population_size=INIT_HP['POP_SIZE'], # Population size
+evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness scores
+mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
 no_mutation=MUTATION_PARAMS['NO_MUT'], # No mutation
 architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
 new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], # New layer mutation
 parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
 activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
 rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
 rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
 from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
 ['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
-Random seed device=torch.device("cuda")) ``` The easiest training loop
-implementation is to use our training.train_offline.train() function. It
-requires the agent have functions getAction() and learn(). ```python from
+Random seed device=device) ``` The easiest training loop implementation is to
+use our training.train_offline.train() function. It requires the agent have
+functions getAction() and learn(). ```python from
 agilerl.training.train_offline import train trained_pop, pop_fitnesses = train
 (env=env, # Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment
 name dataset=dataset, # Offline dataset algo=INIT_HP['ALGO'], # Algorithm
 pop=agent_pop, # Population of agents memory=memory, # Replay buffer
-swap_channels=False, # Swap image channel from last to first n_episodes=INIT_HP
-['EPISODES'], # Max number of training episodes evo_epochs=INIT_HP
-['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of evaluation
-episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score for early
-stopping tournament=tournament, # Tournament selection object
-mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
-Biases tracking device=torch.device("cuda")) ``` ### Custom Offline Training
-Loop Alternatively, use a custom training loop. Combining all of the above:
-```python from agilerl.utils.utils import initialPopulation from
+swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image channel from last to first
+n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
+evo_epochs=INIT_HP['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of
+evaluation episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score
+for early stopping tournament=tournament, # Tournament selection object
+mutation=mutations, # Mutations object wb=INIT_HP['WANDB']) # Weights and
+Biases tracking ``` ### Custom Offline Training Loop Alternatively, use a
+custom training loop. Combining all of the above: ```python from
+agilerl.utils.utils import makeVectEnvs, initialPopulation from
 agilerl.components.replay_buffer import ReplayBuffer from
 agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
-import Mutations import gymnasium as gym import h5py import numpy as np import
-torch NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32],
+import Mutations import h5py import numpy as np import torch from tqdm import
+trange NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32],
 # Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
 'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
 Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
 update of target network parameters 'CHANNELS_LAST': False # Swap image
-channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
-initialPopulation(algo='CQN', # Algorithm state_dim=(4,), # State dimension
-action_dim=2, # Action dimension one_hot=False, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=6, # Population size device=torch.device
-("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=2, # Number of agent actions
+channels dimension from last to first [H, W, C] -> [C, H, W] } device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env = gym.make
+('CartPole-v1') # Create environment dataset = h5py.File('data/cartpole/
+cartpole_random_v1.1.0.h5', 'r') # Load dataset try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='CQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=6, # Population size device=device)
+field_names = ["state", "action", "reward", "next_state", "done"] memory =
+ReplayBuffer(action_dim=action_dim, # Number of agent actions
 memory_size=10000, # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=2, # Tournament selection size
-elitism=True, # Elitism in tournament selection population_size=6, # Population
-size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
-(algo='CQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
-Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
-# Network parameters mutation activation=0, # Activation layer mutation
-rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
-Learning HPs to choose from mutation_sd=0.1, # Mutation strength
-arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random seed
-device=torch.device("cuda")) max_episodes = 1000 # Max training episodes
-max_steps = 500 # Max steps per episode evo_epochs = 5 # Evolution frequency
-evo_loop = 1 # Number of evaluation episodes env = gym.make('CartPole-v1') #
-Create environment dataset = h5py.File('data/cartpole/
-cartpole_random_v1.1.0.h5', 'r') # Load dataset # Save transitions to replay
-buffer dataset_length = dataset['rewards'].shape[0] for i in range
-(dataset_length-1): state = dataset['observations'][i] next_state = dataset
-['observations'][i+1] if swap_channels: state = np.moveaxis(state, [3], [1])
-next_state = np.moveaxis(next_state, [3], [1]) action = dataset['actions'][i]
-reward = dataset['rewards'][i] done = bool(dataset['terminals'][i])
-memory.save2memory(state, action, reward, next_state, done) # TRAINING LOOP for
-idx_epi in range(max_episodes): for agent in pop: # Loop through population for
-idx_step in range(max_steps): experiences = memory.sample(agent.batch_size) #
-Sample replay buffer # Learn according to agent's RL algorithm agent.learn
-(experiences) # Now evolve population if necessary if (idx_epi+1) % evo_epochs
-== 0: # Evaluate population fitnesses = [agent.test(env, swap_channels=False,
+names to store in memory device=device) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo='CQN', #
+Algorithm no_mutation=0.4, # No mutation architecture=0.2, # Architecture
+mutation new_layer_prob=0.2, # New layer mutation parameters=0.2, # Network
+parameters mutation activation=0, # Activation layer mutation rl_hp=0.2, #
+Learning HP mutation rl_hp_selection=['lr', 'batch_size'], # Learning HPs to
+choose from mutation_sd=0.1, # Mutation strength arch=NET_CONFIG['arch'], #
+Network architecture rand_seed=1, # Random seed device=device) max_episodes =
+1000 # Max training episodes max_steps = 500 # Max steps per episode evo_epochs
+= 5 # Evolution frequency evo_loop = 1 # Number of evaluation episodes # Save
+transitions to replay buffer dataset_length = dataset['rewards'].shape[0] for i
+in trange(dataset_length-1): state = dataset['observations'][i] next_state =
+dataset['observations'][i+1] if INIT_HP['CHANNELS_LAST']: state = np.moveaxis
+(state, [3], [1]) next_state = np.moveaxis(next_state, [3], [1]) action =
+dataset['actions'][i] reward = dataset['rewards'][i] done = bool(dataset
+['terminals'][i]) # Save experience to replay buffer memory.save2memory(state,
+action, reward, next_state, done) # TRAINING LOOP for idx_epi in trange
+(max_episodes): for agent in pop: # Loop through population for idx_step in
+range(max_steps): experiences = memory.sample(agent.batch_size) # Sample replay
+buffer # Learn according to agent's RL algorithm agent.learn(experiences) # Now
+evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
+population fitnesses = [agent.test(env, swap_channels=False,
 max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
 {idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
 fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
 for agent in pop]}') # Tournament selection and population mutation elite, pop
 = tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
 a language environment (RLHF) We implement RLHF on Wordle, and use ILQL to
 finetune our model. To create your own language environment, see https://
@@ -315,9 +338,107 @@
 Due to the vast number of parameters and settings involved in training a Large
 Language Model (LLM) on human feedback, these are defined in configs. In order
 to finetune a model with RLHF, we need a trained model as a starting point. We
 can use behavioural cloning (BC, supervised learning) to build this first
 version of the model. To train your own model from scratch: ```bash python
 run_bc_lm.py ``` If you want to use pretrained model weights, these can be
 defined in configs/wordle/train_bc.yaml in model: load:. Similarly, to then run
-ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` View
-documentation.
+ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` ##
+Distributed training AgileRL can also be used for distributed training if you
+have multiple devices you want to take advantage of. We use the HuggingFace
+Accelerate library to implement this in an open manner, without hiding behind
+too many layers of abstraction. This should make implementations simple, but
+also highly customisable, by continuing to expose the PyTorch training loop
+beneath it all. To launch distributed training scripts in bash, use accelerate
+launch. To customise the distributed training properties, specify the key --
+config_file. An example config file has been provided at configs/accelerate/
+accelerate.yaml. Putting this all together, launching a distributed training
+script can be done as follows: ```bash accelerate_launch --config_file configs/
+accelerate/accelerate.yaml demo_online_distributed.py ``` There are some key
+considerations to bear in mind when implementing a distributed training run: *
+If you only want to execute something once, rather than repeating it for each
+process, e.g printing a statement, logging to W&B, then use if
+accelerator.is_main_process:. * Training happens in parallel on each device,
+meaning that steps in a RL environment happen on each device too. In order to
+count the number of global training steps taken, you must multiply the number
+of steps you have taken on a singular device by the number of devices (assuming
+they are equal). If you want to use distributed training to train more quickly,
+and normally you would train for 100,000 steps on one device, you can now train
+for just 25,000 steps if using four devices. Example distributed training loop:
+```python from agilerl.utils.utils import makeVectEnvs, initialPopulation from
+agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.components.replay_data import ReplayDataset from
+agilerl.components.sampler import Sampler from agilerl.hpo.tournament import
+TournamentSelection from agilerl.hpo.mutation import Mutations from accelerate
+import Accelerator import numpy as np import os from torch.utils.data import
+DataLoader from tqdm import trange if __name__ == '__main__': accelerator =
+Accelerator() NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } INIT_HP = { 'POPULATION_SIZE': 4, # Population
+size 'DOUBLE': True, # Use double Q-learning in DQN or CQN 'BATCH_SIZE': 128, #
+Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, # Discount factor
+'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft update of target
+network parameters 'POLICY_FREQ': 2, # DDPG target network update frequency vs
+policy network # Swap image channels dimension from last to first [H, W, C] ->
+[C, H, W] 'CHANNELS_LAST': False } env = makeVectEnvs('LunarLander-v2',
+num_envs=8) # Create environment try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='DQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=INIT_HP['POPULATION_SIZE'], #
+Population size accelerator=accelerator) # Accelerator field_names = ["state",
+"action", "reward", "next_state", "done"] memory = ReplayBuffer
+(action_dim=action_dim, # Number of agent actions memory_size=10000, # Max
+replay buffer size field_names=field_names) # Field names to store in memory
+replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE']) replay_dataloader
+= DataLoader(replay_dataset, batch_size=None) replay_dataloader =
+accelerator.prepare(replay_dataloader) sampler = Sampler(distributed=True,
+dataset=replay_dataset, dataloader=replay_dataloader) tournament =
+TournamentSelection(tournament_size=2, # Tournament selection size
+elitism=True, # Elitism in tournament selection population_size=INIT_HP
+['POPULATION_SIZE'], # Population size evo_step=1) # Evaluate using last N
+fitness scores mutations = Mutations(algo='DQN', # Algorithm no_mutation=0.4, #
+No mutation architecture=0.2, # Architecture mutation new_layer_prob=0.2, # New
+layer mutation parameters=0.2, # Network parameters mutation activation=0, #
+Activation layer mutation rl_hp=0.2, # Learning HP mutation rl_hp_selection=
+['lr', 'batch_size'], # Learning HPs to choose from mutation_sd=0.1, # Mutation
+strength arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random
+seed accelerator=accelerator) # Accelerator) max_episodes = 1000 # Max training
+episodes max_steps = 500 # Max steps per episode # Exploration params eps_start
+= 1.0 # Max exploration eps_end = 0.1 # Min exploration eps_decay = 0.995 #
+Decay per episode epsilon = eps_start evo_epochs = 5 # Evolution frequency
+evo_loop = 1 # Number of evaluation episodes accel_temp_models_path = 'models/
+{}'.format('LunarLander-v2') if accelerator.is_main_process: if not
+os.path.exists(accel_temp_models_path): os.makedirs(accel_temp_models_path)
+print(f'\nDistributed training on {accelerator.device}...') # TRAINING LOOP for
+idx_epi in trange(max_episodes): accelerator.wait_for_everyone() for agent in
+pop: # Loop through population state = env.reset()[0] # Reset environment at
+start of episode score = 0 for idx_step in range(max_steps): # Get next action
+from agent action = agent.getAction(state, epsilon) next_state, reward, done,
+_, _ = env.step( action) # Act in environment # Save experience to replay
+buffer memory.save2memoryVectEnvs( state, action, reward, next_state, done) #
+Learn according to learning frequency if memory.counter % agent.learn_step == 0
+and len( memory) >= agent.batch_size: # Sample dataloader experiences =
+sampler.sample(agent.batch_size) # Learn according to agent's RL algorithm
+agent.learn(experiences) state = next_state score += reward # Update epsilon
+for exploration epsilon = max(eps_end, epsilon * eps_decay) # Now evolve
+population if necessary if (idx_epi + 1) % evo_epochs == 0: # Evaluate
+population fitnesses = [ agent.test( env, swap_channels=False,
+max_steps=max_steps, loop=evo_loop) for agent in pop] if
+accelerator.is_main_process: print(f'Episode {idx_epi+1}/{max_episodes}') print
+(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}') print(f'100 fitness
+avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}') # Tournament
+selection and population mutation accelerator.wait_for_everyone() for model in
+pop: model.unwrap_models() accelerator.wait_for_everyone() if
+accelerator.is_main_process: elite, pop = tournament.select(pop) pop =
+mutations.mutation(pop) for pop_i, model in enumerate(pop):
+model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+accelerator.wait_for_everyone() if not accelerator.is_main_process: for pop_i,
+model in enumerate(pop): model.loadCheckpoint(f'{accel_temp_models_path}/DQN_
+{pop_i}.pt') accelerator.wait_for_everyone() for model in pop:
+model.wrap_models() ``` View documentation.
```

### Comparing `agilerl-0.1.6/PKG-INFO` & `agilerl-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agilerl
-Version: 0.1.6
+Version: 0.1.7
 Summary: AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps.
 License: Apache 2.0
 Author: Nick Ustaran-Anderegg
 Author-email: dev@agilerl.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,17 @@
 <div align="center">
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Documentation Status](https://readthedocs.org/projects/agilerl/badge/?version=latest)](https://agilerl.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/badge/agilerl)](https://pypi.python.org/pypi/agilerl/)
 [![Discord](https://dcbadge.vercel.app/api/server/eB8HyTA2ux?style=flat)](https://discord.gg/eB8HyTA2ux)
 
+**_NEW: AgileRL now supports distributed training with HuggingFace Accelerate!<br>
+Train even faster by taking full advantage of your entire compute stack._**
+
 </div>
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
   
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
@@ -60,14 +63,15 @@
   * [Get Started](#get-started)
   * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
   * [Train an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-online)
     + [Custom Online Training Loop](#custom-online-training-loop)
   * [Train an agent on data (Offline)](#train-an-agent-on-data-offline)
     + [Custom Offline Training Loop](#custom-offline-training-loop)
   * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
+  * [Distributed training](#distributed-training)
 
 ## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
 In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
@@ -86,22 +90,27 @@
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
 If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
 
 Demo:
 ```bash
-python demo.py
+python demo_online.py
+```
+or to demo distributed training:
+```bash
+accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
 ```
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
   * CQL
   * ILQL
+  * TD3
 
 ## Train an agent on a Gym environment (Online)
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
@@ -150,46 +159,45 @@
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16)
 try:
     state_dim = env.single_observation_space.n          # Discrete observation space
     one_hot = True                                      # Requires one-hot encoding
-except:
+except Exception:
     state_dim = env.single_observation_space.shape      # Continuous observation space
     one_hot = False                                     # Does not require one-hot encoding
 try:
     action_dim = env.single_action_space.n             # Discrete action space
-except:
+except Exception:
     action_dim = env.single_action_space.shape[0]      # Continuous action space
 
 if INIT_HP['CHANNELS_LAST']:
     state_dim = (state_dim[2], state_dim[0], state_dim[1])
 
 agent_pop = initialPopulation(algo=INIT_HP['ALGO'],                 # Algorithm
                               state_dim=state_dim,                  # State dimension
                               action_dim=action_dim,                # Action dimension
                               one_hot=one_hot,                      # One-hot encoding
                               net_config=NET_CONFIG,                # Network configuration
                               INIT_HP=INIT_HP,                      # Initial hyperparameters
                               population_size=INIT_HP['POP_SIZE'],  # Population size
-                              device=torch.device("cuda"))
+                              device=device)
 ```
 Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
 ```python
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
-import torch
 
 field_names = ["state", "action", "reward", "next_state", "done"]
 memory = ReplayBuffer(action_dim=action_dim,                # Number of agent actions
                       memory_size=INIT_HP['MEMORY_SIZE'],   # Max replay buffer size
                       field_names=field_names,              # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament selection size
                                  elitism=INIT_HP['ELITISM'],            # Elitism in tournament selection
                                  population_size=INIT_HP['POP_SIZE'],   # Population size
                                  evo_step=INIT_HP['EVO_EPOCHS'])        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo=INIT_HP['ALGO'],                                 # Algorithm
@@ -199,34 +207,33 @@
                       parameters=MUTATION_PARAMS['PARAMS_MUT'],             # Network parameters mutation
                       activation=MUTATION_PARAMS['ACT_MUT'],                # Activation layer mutation
                       rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
                       rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
                       mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
                       arch=NET_CONFIG['arch'],                              # Network architecture
                       rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 ```
 The easiest training loop implementation is to use our <code>training.train.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
 ```python
 from agilerl.training.train import train
 
-trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
-                                   env_name=INIT_HP['ENV_NAME'],        # Environment name
-                                   algo=INIT_HP['ALGO'],                # Algorithm
-                                   pop=agent_pop,                       # Population of agents
-                                   memory=memory,                       # Replay buffer
-                                   swap_channels=False,                 # Swap image channel from last to first
-                                   n_episodes=INIT_HP['EPISODES'],      # Max number of training episodes
-                                   evo_epochs=INIT_HP['EVO_EPOCHS'],    # Evolution frequency
-                                   evo_loop=1,                          # Number of evaluation episodes per agent
-                                   target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
-                                   tournament=tournament,               # Tournament selection object
-                                   mutation=mutations,                  # Mutations object
-                                   wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
-                                   device=torch.device("cuda"))
+trained_pop, pop_fitnesses = train(env=env,                                 # Gym-style environment
+                                   env_name=INIT_HP['ENV_NAME'],            # Environment name
+                                   algo=INIT_HP['ALGO'],                    # Algorithm
+                                   pop=agent_pop,                           # Population of agents
+                                   memory=memory,                           # Replay buffer
+                                   swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                   n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                   evo_epochs=INIT_HP['EVO_EPOCHS'],        # Evolution frequency
+                                   evo_loop=1,                              # Number of evaluation episodes per agent
+                                   target=INIT_HP['TARGET_SCORE'],          # Target score for early stopping
+                                   tournament=tournament,                   # Tournament selection object
+                                   mutation=mutations,                      # Mutations object
+                                   wb=INIT_HP['WANDB'])                     # Weights and Biases tracking
 ```
 
 ### Custom Online Training Loop
 Alternatively, use a custom training loop. Combining all of the above:
 
 ```python
 from agilerl.utils.utils import makeVectEnvs, initialPopulation
@@ -248,28 +255,46 @@
             'LR': 1e-3,             # Learning rate
             'GAMMA': 0.99,          # Discount factor
             'LEARN_STEP': 1,        # Learning frequency
             'TAU': 1e-3,            # For soft update of target network parameters
             'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
           }
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+env = makeVectEnvs('LunarLander-v2', num_envs=16)   # Create environment
+
+try:
+    state_dim = env.single_observation_space.n       # Discrete observation space
+    one_hot = True                            # Requires one-hot encoding
+except Exception:
+    state_dim = env.single_observation_space.shape   # Continuous observation space
+    one_hot = False                           # Does not require one-hot encoding
+try:
+    action_dim = env.single_action_space.n           # Discrete action space
+except Exception:
+    action_dim = env.single_action_space.shape[0]    # Continuous action space
+
+if INIT_HP['CHANNELS_LAST']:
+    state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
 pop = initialPopulation(algo='DQN',             # Algorithm
-                        state_dim=(8,),         # State dimension
-                        action_dim=4,           # Action dimension
-                        one_hot=False,          # One-hot encoding
+                        state_dim=state_dim,    # State dimension
+                        action_dim=action_dim,  # Action dimension
+                        one_hot=one_hot,        # One-hot encoding
                         net_config=NET_CONFIG,  # Network configuration
                         INIT_HP=INIT_HP,        # Initial hyperparameters
                         population_size=6,      # Population size
-                        device=torch.device("cuda"))
+                        device=device)
 
 field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=4,             # Number of agent actions
+memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                       memory_size=10000,        # Max replay buffer size
                       field_names=field_names,  # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=2, # Tournament selection size
                                  elitism=True,      # Elitism in tournament selection
                                  population_size=6, # Population size
                                  evo_step=1)        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo='DQN',                           # Algorithm
@@ -279,41 +304,46 @@
                       parameters=0.2,                       # Network parameters mutation
                       activation=0,                         # Activation layer mutation
                       rl_hp=0.2,                            # Learning HP mutation
                       rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
                       mutation_sd=0.1,                      # Mutation strength
                       arch=NET_CONFIG['arch'],              # Network architecture
                       rand_seed=1,                          # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 
 max_episodes = 1000 # Max training episodes
 max_steps = 500     # Max steps per episode
 
 # Exploration params
 eps_start = 1.0     # Max exploration
 eps_end = 0.1       # Min exploration
 eps_decay = 0.995   # Decay per episode
 epsilon = eps_start
 
 evo_epochs = 5      # Evolution frequency
 evo_loop = 1        # Number of evaluation episodes
 
-env = makeVectEnvs('LunarLander-v2', num_envs=16)   # Create environment
-
 # TRAINING LOOP
 for idx_epi in range(max_episodes):
     for agent in pop:   # Loop through population
         state = env.reset()[0]  # Reset environment at start of episode
         score = 0
         for idx_step in range(max_steps):
+            if INIT_HP['CHANNELS_LAST']:
+                state = np.moveaxis(state, [3], [1])
             action = agent.getAction(state, epsilon)    # Get next action from agent
             next_state, reward, done, _, _ = env.step(action)   # Act in environment
             
             # Save experience to replay buffer
-            memory.save2memoryVectEnvs(state, action, reward, next_state, done)
+            if INIT_HP['CHANNELS_LAST']:
+                memory.save2memoryVectEnvs(
+                    state, action, reward, np.moveaxis(next_state, [3], [1]), done)
+            else:
+                memory.save2memoryVectEnvs(
+                    state, action, reward, next_state, done)
 
             # Learn according to learning frequency
             if memory.counter % agent.learn_step == 0 and len(memory) >= agent.batch_size:
                 experiences = memory.sample(agent.batch_size) # Sample replay buffer
                 agent.learn(experiences)    # Learn according to agent's RL algorithm
             
             state = next_state
@@ -321,15 +351,15 @@
 
     epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
         
         # Evaluate population
-        fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
+        fitnesses = [agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
         # Tournament selection and population mutation
         elite, pop = tournament.select(pop)
@@ -380,59 +410,59 @@
 NET_CONFIG = {
     'arch': 'mlp',      # Network architecture
     'h_size': [32, 32], # Actor hidden size
 }
 ```
 First, use <code>utils.utils.initialPopulation</code> to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
 ```python
-from agilerl.utils.utils import initialPopulation
+from agilerl.utils.utils import makeVectsEnvs, initialPopulation
 import torch
 import h5py
 import gymnasium as gym
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-env = gym.make(INIT_HP['ENV_NAME'])
+env = makeVectEnvs(INIT_HP['ENV_NAME'], num_envs=1)
 try:
-    state_dim = env.observation_space.n       # Discrete observation space
-    one_hot = True                            # Requires one-hot encoding
+    state_dim = env.single_observation_space.n          # Discrete observation space
+    one_hot = True                                      # Requires one-hot encoding
 except Exception:
-    state_dim = env.observation_space.shape   # Continuous observation space
-    one_hot = False                           # Does not require one-hot encoding
+    state_dim = env.single_observation_space.shape      # Continuous observation space
+    one_hot = False                                     # Does not require one-hot encoding
 try:
-    action_dim = env.action_space.n           # Discrete action space
+    action_dim = env.single_action_space.n             # Discrete action space
 except Exception:
-    action_dim = env.action_space.shape[0]    # Continuous action space
+    action_dim = env.single_action_space.shape[0]      # Continuous action space
 
 if INIT_HP['CHANNELS_LAST']:
     state_dim = (state_dim[2], state_dim[0], state_dim[1])
 
 dataset = h5py.File(INIT_HP['DATASET'], 'r')
 
 agent_pop = initialPopulation(algo=INIT_HP['ALGO'],                 # Algorithm
                               state_dim=state_dim,                  # State dimension
                               action_dim=action_dim,                # Action dimension
                               one_hot=one_hot,                      # One-hot encoding
                               net_config=NET_CONFIG,                # Network configuration
                               INIT_HP=INIT_HP,                      # Initial hyperparameters
                               population_size=INIT_HP['POP_SIZE'],  # Population size
-                              device=torch.device("cuda"))
+                              device=device)
 ```
 Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
 ```python
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
 import torch
 
 field_names = ["state", "action", "reward", "next_state", "done"]
 memory = ReplayBuffer(action_dim=action_dim,                # Number of agent actions
                       memory_size=INIT_HP['MEMORY_SIZE'],   # Max replay buffer size
                       field_names=field_names,              # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament selection size
                                  elitism=INIT_HP['ELITISM'],            # Elitism in tournament selection
                                  population_size=INIT_HP['POP_SIZE'],   # Population size
                                  evo_step=INIT_HP['EVO_EPOCHS'])        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo=INIT_HP['ALGO'],                                 # Algorithm
@@ -442,49 +472,48 @@
                       parameters=MUTATION_PARAMS['PARAMS_MUT'],             # Network parameters mutation
                       activation=MUTATION_PARAMS['ACT_MUT'],                # Activation layer mutation
                       rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
                       rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
                       mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
                       arch=NET_CONFIG['arch'],                              # Network architecture
                       rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 ```
 The easiest training loop implementation is to use our <code>training.train_offline.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
 ```python
 from agilerl.training.train_offline import train
 
-trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
-                                   env_name=INIT_HP['ENV_NAME'],        # Environment name
-                                   dataset=dataset,                     # Offline dataset
-                                   algo=INIT_HP['ALGO'],                # Algorithm
-                                   pop=agent_pop,                       # Population of agents
-                                   memory=memory,                       # Replay buffer
-                                   swap_channels=False,                 # Swap image channel from last to first
-                                   n_episodes=INIT_HP['EPISODES'],      # Max number of training episodes
-                                   evo_epochs=INIT_HP['EVO_EPOCHS'],    # Evolution frequency
-                                   evo_loop=1,                          # Number of evaluation episodes per agent
-                                   target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
-                                   tournament=tournament,               # Tournament selection object
-                                   mutation=mutations,                  # Mutations object
-                                   wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
-                                   device=torch.device("cuda"))
+trained_pop, pop_fitnesses = train(env=env,                                 # Gym-style environment
+                                   env_name=INIT_HP['ENV_NAME'],            # Environment name
+                                   dataset=dataset,                         # Offline dataset
+                                   algo=INIT_HP['ALGO'],                    # Algorithm
+                                   pop=agent_pop,                           # Population of agents
+                                   memory=memory,                           # Replay buffer
+                                   swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                   n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                   evo_epochs=INIT_HP['EVO_EPOCHS'],        # Evolution frequency
+                                   evo_loop=1,                              # Number of evaluation episodes per agent
+                                   target=INIT_HP['TARGET_SCORE'],          # Target score for early stopping
+                                   tournament=tournament,                   # Tournament selection object
+                                   mutation=mutations,                      # Mutations object
+                                   wb=INIT_HP['WANDB'])                     # Weights and Biases tracking
 ```
 
 ### Custom Offline Training Loop
 Alternatively, use a custom training loop. Combining all of the above:
 
 ```python
-from agilerl.utils.utils import initialPopulation
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
-import gymnasium as gym
 import h5py
 import numpy as np
 import torch
+from tqdm import trange
 
 NET_CONFIG = {
                 'arch': 'mlp',       # Network architecture
                 'h_size': [32, 32],  # Actor hidden size
              }
 
 INIT_HP = {
@@ -493,28 +522,47 @@
             'LR': 1e-3,             # Learning rate
             'GAMMA': 0.99,          # Discount factor
             'LEARN_STEP': 1,        # Learning frequency
             'TAU': 1e-3,            # For soft update of target network parameters
             'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
           }
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+env = gym.make('CartPole-v1')   # Create environment
+dataset = h5py.File('data/cartpole/cartpole_random_v1.1.0.h5', 'r')  # Load dataset
+
+try:
+    state_dim = env.single_observation_space.n          # Discrete observation space
+    one_hot = True                                      # Requires one-hot encoding
+except Exception:
+    state_dim = env.single_observation_space.shape      # Continuous observation space
+    one_hot = False                                     # Does not require one-hot encoding
+try:
+    action_dim = env.single_action_space.n             # Discrete action space
+except Exception:
+    action_dim = env.single_action_space.shape[0]      # Continuous action space
+
+if INIT_HP['CHANNELS_LAST']:
+    state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
 pop = initialPopulation(algo='CQN',             # Algorithm
-                        state_dim=(4,),         # State dimension
-                        action_dim=2,           # Action dimension
-                        one_hot=False,          # One-hot encoding
+                        state_dim=state_dim,    # State dimension
+                        action_dim=action_dim,  # Action dimension
+                        one_hot=one_hot,        # One-hot encoding
                         net_config=NET_CONFIG,  # Network configuration
                         INIT_HP=INIT_HP,        # Initial hyperparameters
                         population_size=6,      # Population size
-                        device=torch.device("cuda"))
+                        device=device)
 
 field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=2,             # Number of agent actions
+memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                       memory_size=10000,        # Max replay buffer size
                       field_names=field_names,  # Field names to store in memory
-                      device=torch.device("cuda"))
+                      device=device)
 
 tournament = TournamentSelection(tournament_size=2, # Tournament selection size
                                  elitism=True,      # Elitism in tournament selection
                                  population_size=6, # Population size
                                  evo_step=1)        # Evaluate using last N fitness scores
 
 mutations = Mutations(algo='CQN',                           # Algorithm
@@ -524,41 +572,39 @@
                       parameters=0.2,                       # Network parameters mutation
                       activation=0,                         # Activation layer mutation
                       rl_hp=0.2,                            # Learning HP mutation
                       rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
                       mutation_sd=0.1,                      # Mutation strength
                       arch=NET_CONFIG['arch'],              # Network architecture
                       rand_seed=1,                          # Random seed
-                      device=torch.device("cuda"))
+                      device=device)
 
 max_episodes = 1000 # Max training episodes
 max_steps = 500     # Max steps per episode
 
 evo_epochs = 5      # Evolution frequency
 evo_loop = 1        # Number of evaluation episodes
 
-env = gym.make('CartPole-v1')   # Create environment
-
-dataset = h5py.File('data/cartpole/cartpole_random_v1.1.0.h5', 'r')  # Load dataset
-
 # Save transitions to replay buffer
 dataset_length = dataset['rewards'].shape[0]
-for i in range(dataset_length-1):
+for i in trange(dataset_length-1):
     state = dataset['observations'][i]
     next_state = dataset['observations'][i+1]
-    if swap_channels:
+    if INIT_HP['CHANNELS_LAST']:
         state = np.moveaxis(state, [3], [1])
         next_state = np.moveaxis(next_state, [3], [1])
     action = dataset['actions'][i]
     reward = dataset['rewards'][i]
     done = bool(dataset['terminals'][i])
+    # Save experience to replay buffer
     memory.save2memory(state, action, reward, next_state, done)
 
+
 # TRAINING LOOP
-for idx_epi in range(max_episodes):
+for idx_epi in trange(max_episodes):
     for agent in pop:   # Loop through population
         for idx_step in range(max_steps):
             experiences = memory.sample(agent.batch_size)   # Sample replay buffer
             # Learn according to agent's RL algorithm
             agent.learn(experiences)
 
     # Now evolve population if necessary
@@ -591,9 +637,200 @@
 If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
 
 Similarly, to then run ILQL and perform RLHF on the BC model:
 ```bash
 python run_ilql.py
 ```
 
+## Distributed training
+AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace 
+<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction. 
+This should make implementations simple, but also highly customisable, by continuing to expose the PyTorch training loop beneath it all.
+
+To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example 
+config file has been provided at <code>configs/accelerate/accelerate.yaml</code>.
+
+Putting this all together, launching a distributed training script can be done as follows:
+```bash
+accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
+```
+
+There are some key considerations to bear in mind when implementing a distributed training run:
+  * If you only want to execute something once, rather than repeating it for each process, e.g printing a statement, logging to W&B, then use <code>if accelerator.is_main_process:</code>.
+  * Training happens in parallel on each device, meaning that steps in a RL environment happen on each device too. In order to count the number of global training steps taken, you must multiply the number of steps you have taken on a singular device by the number of devices (assuming they are equal). If you want to use distributed training to train more quickly, and normally you would train for 100,000 steps on one device, you can now train for just 25,000 steps if using four devices.
+
+Example distributed training loop:
+
+```python
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
+from agilerl.components.replay_buffer import ReplayBuffer
+from agilerl.components.replay_data import ReplayDataset
+from agilerl.components.sampler import Sampler
+from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations
+from accelerate import Accelerator
+import numpy as np
+import os
+from torch.utils.data import DataLoader
+from tqdm import trange
+
+if __name__ == '__main__':
+
+    accelerator = Accelerator()
+
+    NET_CONFIG = {
+        'arch': 'mlp',       # Network architecture
+        'h_size': [32, 32],  # Actor hidden size
+    }
+
+    INIT_HP = {
+        'POPULATION_SIZE': 4,   # Population size
+        'DOUBLE': True,         # Use double Q-learning in DQN or CQN
+        'BATCH_SIZE': 128,      # Batch size
+        'LR': 1e-3,             # Learning rate
+        'GAMMA': 0.99,          # Discount factor
+        'LEARN_STEP': 1,        # Learning frequency
+        'TAU': 1e-3,            # For soft update of target network parameters
+        'POLICY_FREQ': 2,       # DDPG target network update frequency vs policy network
+        # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        'CHANNELS_LAST': False
+    }
+
+    env = makeVectEnvs('LunarLander-v2', num_envs=8)   # Create environment
+    try:
+        state_dim = env.single_observation_space.n          # Discrete observation space
+        one_hot = True                                      # Requires one-hot encoding
+    except Exception:
+        state_dim = env.single_observation_space.shape      # Continuous observation space
+        one_hot = False                                     # Does not require one-hot encoding
+    try:
+        action_dim = env.single_action_space.n             # Discrete action space
+    except Exception:
+        action_dim = env.single_action_space.shape[0]      # Continuous action space
+
+    if INIT_HP['CHANNELS_LAST']:
+        state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
+    pop = initialPopulation(algo='DQN',                 # Algorithm
+                            state_dim=state_dim,        # State dimension
+                            action_dim=action_dim,      # Action dimension
+                            one_hot=one_hot,            # One-hot encoding
+                            net_config=NET_CONFIG,      # Network configuration
+                            INIT_HP=INIT_HP,            # Initial hyperparameters
+                            population_size=INIT_HP['POPULATION_SIZE'], # Population size
+                            accelerator=accelerator)    # Accelerator
+
+    field_names = ["state", "action", "reward", "next_state", "done"]
+    memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
+                        memory_size=10000,        # Max replay buffer size
+                        field_names=field_names)  # Field names to store in memory
+    replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE'])
+    replay_dataloader = DataLoader(replay_dataset, batch_size=None)
+    replay_dataloader = accelerator.prepare(replay_dataloader)
+    sampler = Sampler(distributed=True, 
+                    dataset=replay_dataset, 
+                    dataloader=replay_dataloader)
+
+    tournament = TournamentSelection(tournament_size=2,  # Tournament selection size
+                                    elitism=True,      # Elitism in tournament selection
+                                    population_size=INIT_HP['POPULATION_SIZE'],  # Population size
+                                    evo_step=1)        # Evaluate using last N fitness scores
+
+    mutations = Mutations(algo='DQN',                           # Algorithm
+                        no_mutation=0.4,                      # No mutation
+                        architecture=0.2,                     # Architecture mutation
+                        new_layer_prob=0.2,                   # New layer mutation
+                        parameters=0.2,                       # Network parameters mutation
+                        activation=0,                         # Activation layer mutation
+                        rl_hp=0.2,                            # Learning HP mutation
+                        rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
+                        mutation_sd=0.1,                      # Mutation strength
+                        arch=NET_CONFIG['arch'],              # Network architecture
+                        rand_seed=1,                          # Random seed
+                        accelerator=accelerator)              # Accelerator)
+
+    max_episodes = 1000 # Max training episodes
+    max_steps = 500     # Max steps per episode
+
+    # Exploration params
+    eps_start = 1.0     # Max exploration
+    eps_end = 0.1       # Min exploration
+    eps_decay = 0.995   # Decay per episode
+    epsilon = eps_start
+
+    evo_epochs = 5      # Evolution frequency
+    evo_loop = 1        # Number of evaluation episodes
+
+    accel_temp_models_path = 'models/{}'.format('LunarLander-v2')
+    if accelerator.is_main_process:
+        if not os.path.exists(accel_temp_models_path):
+            os.makedirs(accel_temp_models_path)
+
+    print(f'\nDistributed training on {accelerator.device}...')
+
+    # TRAINING LOOP
+    for idx_epi in trange(max_episodes):
+        accelerator.wait_for_everyone()
+        for agent in pop:   # Loop through population
+            state = env.reset()[0]  # Reset environment at start of episode
+            score = 0
+            for idx_step in range(max_steps):
+                # Get next action from agent
+                action = agent.getAction(state, epsilon)
+                next_state, reward, done, _, _ = env.step(
+                    action)   # Act in environment
+
+                # Save experience to replay buffer
+                memory.save2memoryVectEnvs(
+                    state, action, reward, next_state, done)
+
+                # Learn according to learning frequency
+                if memory.counter % agent.learn_step == 0 and len(
+                        memory) >= agent.batch_size:
+                    # Sample dataloader
+                    experiences = sampler.sample(agent.batch_size)
+                    # Learn according to agent's RL algorithm
+                    agent.learn(experiences)
+
+                state = next_state
+                score += reward
+
+        # Update epsilon for exploration
+        epsilon = max(eps_end, epsilon * eps_decay)
+
+        # Now evolve population if necessary
+        if (idx_epi + 1) % evo_epochs == 0:
+
+            # Evaluate population
+            fitnesses = [
+                agent.test(
+                    env,
+                    swap_channels=False,
+                    max_steps=max_steps,
+                    loop=evo_loop) for agent in pop]
+
+            if accelerator.is_main_process:
+                print(f'Episode {idx_epi+1}/{max_episodes}')
+                print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
+                print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
+
+            # Tournament selection and population mutation
+            accelerator.wait_for_everyone()
+            for model in pop:
+                model.unwrap_models()
+            accelerator.wait_for_everyone()
+            if accelerator.is_main_process:
+                elite, pop = tournament.select(pop)
+                pop = mutations.mutation(pop)
+                for pop_i, model in enumerate(pop):
+                    model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+            accelerator.wait_for_everyone()
+            if not accelerator.is_main_process:
+                for pop_i, model in enumerate(pop):
+                    model.loadCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+            accelerator.wait_for_everyone()
+            for model in pop:
+                model.wrap_models()
+```
+
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agilerl Version: 0.1.6 Summary: AgileRL is a deep
+Metadata-Version: 2.1 Name: agilerl Version: 0.1.7 Summary: AgileRL is a deep
 reinforcement learning library focused on improving RL development through
 RLOps. License: Apache 2.0 Author: Nick Ustaran-Anderegg Author-email:
 dev@agilerl.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: accelerate
@@ -23,15 +23,17 @@
                     Join the Discord_Server to collaborate.
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
      opensource.org/licenses/Apache-2.0) [![Documentation Status](https://
        readthedocs.org/projects/agilerl/badge/?version=latest)](https://
     agilerl.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://
   static.pepy.tech/badge/agilerl)](https://pypi.python.org/pypi/agilerl/) [!
 [Discord](https://dcbadge.vercel.app/api/server/eB8HyTA2ux?style=flat)](https:/
-                            /discord.gg/eB8HyTA2ux)
+/discord.gg/eB8HyTA2ux) **_NEW: AgileRL now supports distributed training with
+                            HuggingFace Accelerate!
+  Train even faster by taking full advantage of your entire compute stack._**
 This is a Deep Reinforcement Learning library focused on improving development
 by introducing RLOps - MLOps for reinforcement learning. This library is
 initially focused on reducing the time taken for training models and
 hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for
 reinforcement learning.
 Evolutionary HPO has been shown to drastically reduce overall training times by
 automatically converging on optimal hyperparameters, without requiring numerous
@@ -46,282 +48,303 @@
                              optimization process.
 ## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
 * [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
 an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-
 online) + [Custom Online Training Loop](#custom-online-training-loop) * [Train
 an agent on data (Offline)](#train-an-agent-on-data-offline) + [Custom Offline
 Training Loop](#custom-offline-training-loop) * [Train an agent on a language
-environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) ##
-Benchmarks Reinforcement learning algorithms and libraries are usually
-benchmarked once the optimal hyperparameters for training are known, but it
-often takes hundreds or thousands of experiments to discover these. This is
-unrealistic and does not reflect the true, total time taken for training. What
-if we could remove the need to conduct all these prior experiments? In the
-charts below, a single AgileRL run, which automatically tunes hyperparameters,
-is benchmarked against Optuna's multiple training runs traditionally required
-for hyperparameter optimization, demonstrating the real time savings possible.
-Global steps is the sum of every step taken by any agent in the environment,
-including across an entire population.
+environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) *
+[Distributed training](#distributed-training) ## Benchmarks Reinforcement
+learning algorithms and libraries are usually benchmarked once the optimal
+hyperparameters for training are known, but it often takes hundreds or
+thousands of experiments to discover these. This is unrealistic and does not
+reflect the true, total time taken for training. What if we could remove the
+need to conduct all these prior experiments? In the charts below, a single
+AgileRL run, which automatically tunes hyperparameters, is benchmarked against
+Optuna's multiple training runs traditionally required for hyperparameter
+optimization, demonstrating the real time savings possible. Global steps is the
+sum of every step taken by any agent in the environment, including across an
+entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
-data.zip here. Demo: ```bash python demo.py ``` ## Algorithms implemented (more
-coming soon!) * DQN * DDPG * CQL * ILQL ## Train an agent on a Gym environment
-(Online) Before starting training, there are some meta-hyperparameters and
-settings that must be set. These are defined in INIT_HP, for general
-parameters, and MUTATION_PARAMS, which define the evolutionary probabilities,
-and NET_CONFIG, which defines the network architecture. For example: ```python
-INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN',
-# Algorithm 'DOUBLE': True, # Use double Q-learning 'CHANNELS_LAST': False, #
-Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
-'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate 'EPISODES': 2000, #
-Max no. episodes 'TARGET_SCORE': 200., # Early training stop at avg score of
-last 100 episodes 'GAMMA': 0.99, # Discount factor 'MEMORY_SIZE': 10000, # Max
-memory buffer size 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For
-soft update of target parameters 'TOURN_SIZE': 2, # Tournament size 'ELITISM':
-True, # Elitism in tournament selection 'POP_SIZE': 6, # Population size
-'EVO_EPOCHS': 20, # Evolution frequency 'POLICY_FREQ': 2, # Policy network
-update frequency 'WANDB': True # Log with Weights and Biases } ``` ```python
-MUTATION_PARAMS = { # Relative probabilities 'NO_MUT': 0.4, # No mutation
-'ARCH_MUT': 0.2, # Architecture mutation 'NEW_LAYER': 0.2, # New layer mutation
-'PARAMS_MUT': 0.2, # Network parameters mutation 'ACT_MUT': 0, # Activation
-layer mutation 'RL_HP_MUT': 0.2, # Learning HP mutation 'RL_HP_SELECTION':
-['lr', 'batch_size'], # Learning HPs to choose from 'MUT_SD': 0.1, # Mutation
-strength 'RAND_SEED': 1, # Random seed } ``` ```python NET_CONFIG = { 'arch':
-'mlp', # Network architecture 'h_size': [32, 32], # Actor hidden size } ```
-First, use utils.utils.initialPopulation to create a list of agents - our
-population that will evolve and mutate to the optimal hyperparameters.
-```python from agilerl.utils.utils import makeVectEnvs, initialPopulation
-import torch device = torch.device("cuda" if torch.cuda.is_available() else
-"cpu") env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16) try:
-state_dim = env.single_observation_space.n # Discrete observation space one_hot
-= True # Requires one-hot encoding except: state_dim =
-env.single_observation_space.shape # Continuous observation space one_hot =
-False # Does not require one-hot encoding try: action_dim =
-env.single_action_space.n # Discrete action space except: action_dim =
-env.single_action_space.shape[0] # Continuous action space if INIT_HP
-['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
-agent_pop = initialPopulation(algo=INIT_HP['ALGO'], # Algorithm
+data.zip here. Demo: ```bash python demo_online.py ``` or to demo distributed
+training: ```bash accelerate_launch --config_file configs/accelerate/
+accelerate.yaml demo_online_distributed.py ``` ## Algorithms implemented (more
+coming soon!) * DQN * DDPG * CQL * ILQL * TD3 ## Train an agent on a Gym
+environment (Online) Before starting training, there are some meta-
+hyperparameters and settings that must be set. These are defined in INIT_HP,
+for general parameters, and MUTATION_PARAMS, which define the evolutionary
+probabilities, and NET_CONFIG, which defines the network architecture. For
+example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment
+name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double Q-learning
+'CHANNELS_LAST': False, # Swap image channels dimension from last to first [H,
+W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate
+'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training
+stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount factor
+'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning
+frequency 'TAU': 1e-3, # For soft update of target parameters 'TOURN_SIZE': 2,
+# Tournament size 'ELITISM': True, # Elitism in tournament selection
+'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution frequency
+'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True # Log with
+Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative probabilities
+'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture mutation
+'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network parameters
+mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2, # Learning
+HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs to choose
+from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed } ```
+```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32,
+32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
+create a list of agents - our population that will evolve and mutate to the
+optimal hyperparameters. ```python from agilerl.utils.utils import
+makeVectEnvs, initialPopulation import torch device = torch.device("cuda" if
+torch.cuda.is_available() else "cpu") env = makeVectEnvs(env_name=INIT_HP
+['ENV_NAME'], num_envs=16) try: state_dim = env.single_observation_space.n #
+Discrete observation space one_hot = True # Requires one-hot encoding except
+Exception: state_dim = env.single_observation_space.shape # Continuous
+observation space one_hot = False # Does not require one-hot encoding try:
+action_dim = env.single_action_space.n # Discrete action space except
+Exception: action_dim = env.single_action_space.shape[0] # Continuous action
+space if INIT_HP['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0],
+state_dim[1]) agent_pop = initialPopulation(algo=INIT_HP['ALGO'], # Algorithm
 state_dim=state_dim, # State dimension action_dim=action_dim, # Action
 dimension one_hot=one_hot, # One-hot encoding net_config=NET_CONFIG, # Network
 configuration INIT_HP=INIT_HP, # Initial hyperparameters
-population_size=INIT_HP['POP_SIZE'], # Population size device=torch.device
-("cuda")) ``` Next, create the tournament, mutations and experience replay
-buffer objects that allow agents to share memory and efficiently perform
-evolutionary HPO. ```python from agilerl.components.replay_buffer import
-ReplayBuffer from agilerl.hpo.tournament import TournamentSelection from
-agilerl.hpo.mutation import Mutations import torch field_names = ["state",
-"action", "reward", "next_state", "done"] memory = ReplayBuffer
-(action_dim=action_dim, # Number of agent actions memory_size=INIT_HP
-['MEMORY_SIZE'], # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament
-selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament selection
-population_size=INIT_HP['POP_SIZE'], # Population size evo_step=INIT_HP
-['EVO_EPOCHS']) # Evaluate using last N fitness scores mutations = Mutations
-(algo=INIT_HP['ALGO'], # Algorithm no_mutation=MUTATION_PARAMS['NO_MUT'], # No
-mutation architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
+population_size=INIT_HP['POP_SIZE'], # Population size device=device) ``` Next,
+create the tournament, mutations and experience replay buffer objects that
+allow agents to share memory and efficiently perform evolutionary HPO.
+```python from agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
+import Mutations field_names = ["state", "action", "reward", "next_state",
+"done"] memory = ReplayBuffer(action_dim=action_dim, # Number of agent actions
+memory_size=INIT_HP['MEMORY_SIZE'], # Max replay buffer size
+field_names=field_names, # Field names to store in memory device=device)
+tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], #
+Tournament selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament
+selection population_size=INIT_HP['POP_SIZE'], # Population size
+evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness scores
+mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
+no_mutation=MUTATION_PARAMS['NO_MUT'], # No mutation
+architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
 new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], # New layer mutation
 parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
 activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
 rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
 rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
 from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
 ['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
-Random seed device=torch.device("cuda")) ``` The easiest training loop
-implementation is to use our training.train.train() function. It requires the
-agent have functions getAction() and learn(). ```python from
-agilerl.training.train import train trained_pop, pop_fitnesses = train(env=env,
-# Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment name
-algo=INIT_HP['ALGO'], # Algorithm pop=agent_pop, # Population of agents
-memory=memory, # Replay buffer swap_channels=False, # Swap image channel from
-last to first n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
+Random seed device=device) ``` The easiest training loop implementation is to
+use our training.train.train() function. It requires the agent have functions
+getAction() and learn(). ```python from agilerl.training.train import train
+trained_pop, pop_fitnesses = train(env=env, # Gym-style environment
+env_name=INIT_HP['ENV_NAME'], # Environment name algo=INIT_HP['ALGO'], #
+Algorithm pop=agent_pop, # Population of agents memory=memory, # Replay buffer
+swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image channel from last to first
+n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
 evo_epochs=INIT_HP['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of
 evaluation episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score
 for early stopping tournament=tournament, # Tournament selection object
-mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
-Biases tracking device=torch.device("cuda")) ``` ### Custom Online Training
-Loop Alternatively, use a custom training loop. Combining all of the above:
-```python from agilerl.utils.utils import makeVectEnvs, initialPopulation from
-agilerl.components.replay_buffer import ReplayBuffer from
-agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
-import Mutations import gymnasium as gym import numpy as np import torch
-NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32], #
-Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
-'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
-Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
-update of target network parameters 'CHANNELS_LAST': False # Swap image
-channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
-initialPopulation(algo='DQN', # Algorithm state_dim=(8,), # State dimension
-action_dim=4, # Action dimension one_hot=False, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=6, # Population size device=torch.device
-("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=4, # Number of agent actions
+mutation=mutations, # Mutations object wb=INIT_HP['WANDB']) # Weights and
+Biases tracking ``` ### Custom Online Training Loop Alternatively, use a custom
+training loop. Combining all of the above: ```python from agilerl.utils.utils
+import makeVectEnvs, initialPopulation from agilerl.components.replay_buffer
+import ReplayBuffer from agilerl.hpo.tournament import TournamentSelection from
+agilerl.hpo.mutation import Mutations import gymnasium as gym import numpy as
+np import torch NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-
+learning 'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA':
+0.99, # Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, #
+For soft update of target network parameters 'CHANNELS_LAST': False # Swap
+image channels dimension from last to first [H, W, C] -> [C, H, W] } device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env = makeVectEnvs
+('LunarLander-v2', num_envs=16) # Create environment try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='DQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=6, # Population size device=device)
+field_names = ["state", "action", "reward", "next_state", "done"] memory =
+ReplayBuffer(action_dim=action_dim, # Number of agent actions
 memory_size=10000, # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=2, # Tournament selection size
-elitism=True, # Elitism in tournament selection population_size=6, # Population
-size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
-(algo='DQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
-Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
-# Network parameters mutation activation=0, # Activation layer mutation
-rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
-Learning HPs to choose from mutation_sd=0.1, # Mutation strength
-arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random seed
-device=torch.device("cuda")) max_episodes = 1000 # Max training episodes
-max_steps = 500 # Max steps per episode # Exploration params eps_start = 1.0 #
-Max exploration eps_end = 0.1 # Min exploration eps_decay = 0.995 # Decay per
-episode epsilon = eps_start evo_epochs = 5 # Evolution frequency evo_loop = 1 #
-Number of evaluation episodes env = makeVectEnvs('LunarLander-v2', num_envs=16)
-# Create environment # TRAINING LOOP for idx_epi in range(max_episodes): for
-agent in pop: # Loop through population state = env.reset()[0] # Reset
-environment at start of episode score = 0 for idx_step in range(max_steps):
-action = agent.getAction(state, epsilon) # Get next action from agent
-next_state, reward, done, _, _ = env.step(action) # Act in environment # Save
-experience to replay buffer memory.save2memoryVectEnvs(state, action, reward,
-next_state, done) # Learn according to learning frequency if memory.counter %
-agent.learn_step == 0 and len(memory) >= agent.batch_size: experiences =
-memory.sample(agent.batch_size) # Sample replay buffer agent.learn(experiences)
-# Learn according to agent's RL algorithm state = next_state score += reward
-epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration #
-Now evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
-population fitnesses = [agent.test(env, swap_channels=False,
-max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
-{idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
-fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
-for agent in pop]}') # Tournament selection and population mutation elite, pop
-= tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
-data (Offline) Like with online RL, above, there are some meta-hyperparameters
-and settings that must be set before starting training. These are defined in
-INIT_HP, for general parameters, and MUTATION_PARAMS, which define the
-evolutionary probabilities, and NET_CONFIG, which defines the network
-architecture. For example: ```python INIT_HP = { 'ENV_NAME': 'CartPole-v1', #
-Gym environment name 'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', #
-Offline RL dataset 'ALGO': 'CQN', # Algorithm 'DOUBLE': True, # Use double Q-
-learning # Swap image channels dimension from last to first [H, W, C] -> [C, H,
-W] 'CHANNELS_LAST': False, 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
-Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
-Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
-factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
-Learning frequency 'TAU': 1e-3, # For soft update of target parameters
-'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
-selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
-frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
-Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
-probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
-mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
-parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
-# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
-to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
-} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
-[32, 32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
-create a list of agents - our population that will evolve and mutate to the
-optimal hyperparameters. ```python from agilerl.utils.utils import
-initialPopulation import torch import h5py import gymnasium as gym device =
-torch.device("cuda" if torch.cuda.is_available() else "cpu") env = gym.make
-(INIT_HP['ENV_NAME']) try: state_dim = env.observation_space.n # Discrete
-observation space one_hot = True # Requires one-hot encoding except Exception:
-state_dim = env.observation_space.shape # Continuous observation space one_hot
-= False # Does not require one-hot encoding try: action_dim =
-env.action_space.n # Discrete action space except Exception: action_dim =
-env.action_space.shape[0] # Continuous action space if INIT_HP
-['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
-dataset = h5py.File(INIT_HP['DATASET'], 'r') agent_pop = initialPopulation
-(algo=INIT_HP['ALGO'], # Algorithm state_dim=state_dim, # State dimension
-action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=INIT_HP['POP_SIZE'], # Population size
-device=torch.device("cuda")) ``` Next, create the tournament, mutations and
+names to store in memory device=device) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo='DQN', #
+Algorithm no_mutation=0.4, # No mutation architecture=0.2, # Architecture
+mutation new_layer_prob=0.2, # New layer mutation parameters=0.2, # Network
+parameters mutation activation=0, # Activation layer mutation rl_hp=0.2, #
+Learning HP mutation rl_hp_selection=['lr', 'batch_size'], # Learning HPs to
+choose from mutation_sd=0.1, # Mutation strength arch=NET_CONFIG['arch'], #
+Network architecture rand_seed=1, # Random seed device=device) max_episodes =
+1000 # Max training episodes max_steps = 500 # Max steps per episode #
+Exploration params eps_start = 1.0 # Max exploration eps_end = 0.1 # Min
+exploration eps_decay = 0.995 # Decay per episode epsilon = eps_start
+evo_epochs = 5 # Evolution frequency evo_loop = 1 # Number of evaluation
+episodes # TRAINING LOOP for idx_epi in range(max_episodes): for agent in pop:
+# Loop through population state = env.reset()[0] # Reset environment at start
+of episode score = 0 for idx_step in range(max_steps): if INIT_HP
+['CHANNELS_LAST']: state = np.moveaxis(state, [3], [1]) action =
+agent.getAction(state, epsilon) # Get next action from agent next_state,
+reward, done, _, _ = env.step(action) # Act in environment # Save experience to
+replay buffer if INIT_HP['CHANNELS_LAST']: memory.save2memoryVectEnvs( state,
+action, reward, np.moveaxis(next_state, [3], [1]), done) else:
+memory.save2memoryVectEnvs( state, action, reward, next_state, done) # Learn
+according to learning frequency if memory.counter % agent.learn_step == 0 and
+len(memory) >= agent.batch_size: experiences = memory.sample(agent.batch_size)
+# Sample replay buffer agent.learn(experiences) # Learn according to agent's RL
+algorithm state = next_state score += reward epsilon = max(eps_end,
+epsilon*eps_decay) # Update epsilon for exploration # Now evolve population if
+necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate population fitnesses =
+[agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps,
+loop=evo_loop) for agent in pop] print(f'Episode {idx_epi+1}/{max_episodes}')
+print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}') print(f'100
+fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}') #
+Tournament selection and population mutation elite, pop = tournament.select
+(pop) pop = mutations.mutation(pop) ``` ## Train an agent on data (Offline)
+Like with online RL, above, there are some meta-hyperparameters and settings
+that must be set before starting training. These are defined in INIT_HP, for
+general parameters, and MUTATION_PARAMS, which define the evolutionary
+probabilities, and NET_CONFIG, which defines the network architecture. For
+example: ```python INIT_HP = { 'ENV_NAME': 'CartPole-v1', # Gym environment
+name 'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', # Offline RL dataset
+'ALGO': 'CQN', # Algorithm 'DOUBLE': True, # Use double Q-learning # Swap image
+channels dimension from last to first [H, W, C] -> [C, H, W] 'CHANNELS_LAST':
+False, 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate 'EPISODES':
+2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training stop at avg
+score of last 100 episodes 'GAMMA': 0.99, # Discount factor 'MEMORY_SIZE':
+10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning frequency 'TAU':
+1e-3, # For soft update of target parameters 'TOURN_SIZE': 2, # Tournament size
+'ELITISM': True, # Elitism in tournament selection 'POP_SIZE': 6, # Population
+size 'EVO_EPOCHS': 20, # Evolution frequency 'POLICY_FREQ': 2, # Policy network
+update frequency 'WANDB': True # Log with Weights and Biases } ``` ```python
+MUTATION_PARAMS = { # Relative probabilities 'NO_MUT': 0.4, # No mutation
+'ARCH_MUT': 0.2, # Architecture mutation 'NEW_LAYER': 0.2, # New layer mutation
+'PARAMS_MUT': 0.2, # Network parameters mutation 'ACT_MUT': 0, # Activation
+layer mutation 'RL_HP_MUT': 0.2, # Learning HP mutation 'RL_HP_SELECTION':
+['lr', 'batch_size'], # Learning HPs to choose from 'MUT_SD': 0.1, # Mutation
+strength 'RAND_SEED': 1, # Random seed } ``` ```python NET_CONFIG = { 'arch':
+'mlp', # Network architecture 'h_size': [32, 32], # Actor hidden size } ```
+First, use utils.utils.initialPopulation to create a list of agents - our
+population that will evolve and mutate to the optimal hyperparameters.
+```python from agilerl.utils.utils import makeVectsEnvs, initialPopulation
+import torch import h5py import gymnasium as gym device = torch.device("cuda"
+if torch.cuda.is_available() else "cpu") env = makeVectEnvs(INIT_HP
+['ENV_NAME'], num_envs=1) try: state_dim = env.single_observation_space.n #
+Discrete observation space one_hot = True # Requires one-hot encoding except
+Exception: state_dim = env.single_observation_space.shape # Continuous
+observation space one_hot = False # Does not require one-hot encoding try:
+action_dim = env.single_action_space.n # Discrete action space except
+Exception: action_dim = env.single_action_space.shape[0] # Continuous action
+space if INIT_HP['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0],
+state_dim[1]) dataset = h5py.File(INIT_HP['DATASET'], 'r') agent_pop =
+initialPopulation(algo=INIT_HP['ALGO'], # Algorithm state_dim=state_dim, #
+State dimension action_dim=action_dim, # Action dimension one_hot=one_hot, #
+One-hot encoding net_config=NET_CONFIG, # Network configuration
+INIT_HP=INIT_HP, # Initial hyperparameters population_size=INIT_HP['POP_SIZE'],
+# Population size device=device) ``` Next, create the tournament, mutations and
 experience replay buffer objects that allow agents to share memory and
 efficiently perform evolutionary HPO. ```python from
 agilerl.components.replay_buffer import ReplayBuffer from
 agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
 import Mutations import torch field_names = ["state", "action", "reward",
 "next_state", "done"] memory = ReplayBuffer(action_dim=action_dim, # Number of
 agent actions memory_size=INIT_HP['MEMORY_SIZE'], # Max replay buffer size
-field_names=field_names, # Field names to store in memory device=torch.device
-("cuda")) tournament = TournamentSelection(tournament_size=INIT_HP
-['TOURN_SIZE'], # Tournament selection size elitism=INIT_HP['ELITISM'], #
-Elitism in tournament selection population_size=INIT_HP['POP_SIZE'], #
-Population size evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness
-scores mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
+field_names=field_names, # Field names to store in memory device=device)
+tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], #
+Tournament selection size elitism=INIT_HP['ELITISM'], # Elitism in tournament
+selection population_size=INIT_HP['POP_SIZE'], # Population size
+evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness scores
+mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
 no_mutation=MUTATION_PARAMS['NO_MUT'], # No mutation
 architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
 new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], # New layer mutation
 parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
 activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
 rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
 rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
 from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
 ['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
-Random seed device=torch.device("cuda")) ``` The easiest training loop
-implementation is to use our training.train_offline.train() function. It
-requires the agent have functions getAction() and learn(). ```python from
+Random seed device=device) ``` The easiest training loop implementation is to
+use our training.train_offline.train() function. It requires the agent have
+functions getAction() and learn(). ```python from
 agilerl.training.train_offline import train trained_pop, pop_fitnesses = train
 (env=env, # Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment
 name dataset=dataset, # Offline dataset algo=INIT_HP['ALGO'], # Algorithm
 pop=agent_pop, # Population of agents memory=memory, # Replay buffer
-swap_channels=False, # Swap image channel from last to first n_episodes=INIT_HP
-['EPISODES'], # Max number of training episodes evo_epochs=INIT_HP
-['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of evaluation
-episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score for early
-stopping tournament=tournament, # Tournament selection object
-mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
-Biases tracking device=torch.device("cuda")) ``` ### Custom Offline Training
-Loop Alternatively, use a custom training loop. Combining all of the above:
-```python from agilerl.utils.utils import initialPopulation from
+swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image channel from last to first
+n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
+evo_epochs=INIT_HP['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of
+evaluation episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score
+for early stopping tournament=tournament, # Tournament selection object
+mutation=mutations, # Mutations object wb=INIT_HP['WANDB']) # Weights and
+Biases tracking ``` ### Custom Offline Training Loop Alternatively, use a
+custom training loop. Combining all of the above: ```python from
+agilerl.utils.utils import makeVectEnvs, initialPopulation from
 agilerl.components.replay_buffer import ReplayBuffer from
 agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
-import Mutations import gymnasium as gym import h5py import numpy as np import
-torch NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32],
+import Mutations import h5py import numpy as np import torch from tqdm import
+trange NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32],
 # Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
 'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
 Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
 update of target network parameters 'CHANNELS_LAST': False # Swap image
-channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
-initialPopulation(algo='CQN', # Algorithm state_dim=(4,), # State dimension
-action_dim=2, # Action dimension one_hot=False, # One-hot encoding
-net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
-hyperparameters population_size=6, # Population size device=torch.device
-("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
-memory = ReplayBuffer(action_dim=2, # Number of agent actions
+channels dimension from last to first [H, W, C] -> [C, H, W] } device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env = gym.make
+('CartPole-v1') # Create environment dataset = h5py.File('data/cartpole/
+cartpole_random_v1.1.0.h5', 'r') # Load dataset try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='CQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=6, # Population size device=device)
+field_names = ["state", "action", "reward", "next_state", "done"] memory =
+ReplayBuffer(action_dim=action_dim, # Number of agent actions
 memory_size=10000, # Max replay buffer size field_names=field_names, # Field
-names to store in memory device=torch.device("cuda")) tournament =
-TournamentSelection(tournament_size=2, # Tournament selection size
-elitism=True, # Elitism in tournament selection population_size=6, # Population
-size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
-(algo='CQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
-Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
-# Network parameters mutation activation=0, # Activation layer mutation
-rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
-Learning HPs to choose from mutation_sd=0.1, # Mutation strength
-arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random seed
-device=torch.device("cuda")) max_episodes = 1000 # Max training episodes
-max_steps = 500 # Max steps per episode evo_epochs = 5 # Evolution frequency
-evo_loop = 1 # Number of evaluation episodes env = gym.make('CartPole-v1') #
-Create environment dataset = h5py.File('data/cartpole/
-cartpole_random_v1.1.0.h5', 'r') # Load dataset # Save transitions to replay
-buffer dataset_length = dataset['rewards'].shape[0] for i in range
-(dataset_length-1): state = dataset['observations'][i] next_state = dataset
-['observations'][i+1] if swap_channels: state = np.moveaxis(state, [3], [1])
-next_state = np.moveaxis(next_state, [3], [1]) action = dataset['actions'][i]
-reward = dataset['rewards'][i] done = bool(dataset['terminals'][i])
-memory.save2memory(state, action, reward, next_state, done) # TRAINING LOOP for
-idx_epi in range(max_episodes): for agent in pop: # Loop through population for
-idx_step in range(max_steps): experiences = memory.sample(agent.batch_size) #
-Sample replay buffer # Learn according to agent's RL algorithm agent.learn
-(experiences) # Now evolve population if necessary if (idx_epi+1) % evo_epochs
-== 0: # Evaluate population fitnesses = [agent.test(env, swap_channels=False,
+names to store in memory device=device) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo='CQN', #
+Algorithm no_mutation=0.4, # No mutation architecture=0.2, # Architecture
+mutation new_layer_prob=0.2, # New layer mutation parameters=0.2, # Network
+parameters mutation activation=0, # Activation layer mutation rl_hp=0.2, #
+Learning HP mutation rl_hp_selection=['lr', 'batch_size'], # Learning HPs to
+choose from mutation_sd=0.1, # Mutation strength arch=NET_CONFIG['arch'], #
+Network architecture rand_seed=1, # Random seed device=device) max_episodes =
+1000 # Max training episodes max_steps = 500 # Max steps per episode evo_epochs
+= 5 # Evolution frequency evo_loop = 1 # Number of evaluation episodes # Save
+transitions to replay buffer dataset_length = dataset['rewards'].shape[0] for i
+in trange(dataset_length-1): state = dataset['observations'][i] next_state =
+dataset['observations'][i+1] if INIT_HP['CHANNELS_LAST']: state = np.moveaxis
+(state, [3], [1]) next_state = np.moveaxis(next_state, [3], [1]) action =
+dataset['actions'][i] reward = dataset['rewards'][i] done = bool(dataset
+['terminals'][i]) # Save experience to replay buffer memory.save2memory(state,
+action, reward, next_state, done) # TRAINING LOOP for idx_epi in trange
+(max_episodes): for agent in pop: # Loop through population for idx_step in
+range(max_steps): experiences = memory.sample(agent.batch_size) # Sample replay
+buffer # Learn according to agent's RL algorithm agent.learn(experiences) # Now
+evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
+population fitnesses = [agent.test(env, swap_channels=False,
 max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
 {idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
 fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
 for agent in pop]}') # Tournament selection and population mutation elite, pop
 = tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
 a language environment (RLHF) We implement RLHF on Wordle, and use ILQL to
 finetune our model. To create your own language environment, see https://
@@ -331,9 +354,107 @@
 Due to the vast number of parameters and settings involved in training a Large
 Language Model (LLM) on human feedback, these are defined in configs. In order
 to finetune a model with RLHF, we need a trained model as a starting point. We
 can use behavioural cloning (BC, supervised learning) to build this first
 version of the model. To train your own model from scratch: ```bash python
 run_bc_lm.py ``` If you want to use pretrained model weights, these can be
 defined in configs/wordle/train_bc.yaml in model: load:. Similarly, to then run
-ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` View
-documentation.
+ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` ##
+Distributed training AgileRL can also be used for distributed training if you
+have multiple devices you want to take advantage of. We use the HuggingFace
+Accelerate library to implement this in an open manner, without hiding behind
+too many layers of abstraction. This should make implementations simple, but
+also highly customisable, by continuing to expose the PyTorch training loop
+beneath it all. To launch distributed training scripts in bash, use accelerate
+launch. To customise the distributed training properties, specify the key --
+config_file. An example config file has been provided at configs/accelerate/
+accelerate.yaml. Putting this all together, launching a distributed training
+script can be done as follows: ```bash accelerate_launch --config_file configs/
+accelerate/accelerate.yaml demo_online_distributed.py ``` There are some key
+considerations to bear in mind when implementing a distributed training run: *
+If you only want to execute something once, rather than repeating it for each
+process, e.g printing a statement, logging to W&B, then use if
+accelerator.is_main_process:. * Training happens in parallel on each device,
+meaning that steps in a RL environment happen on each device too. In order to
+count the number of global training steps taken, you must multiply the number
+of steps you have taken on a singular device by the number of devices (assuming
+they are equal). If you want to use distributed training to train more quickly,
+and normally you would train for 100,000 steps on one device, you can now train
+for just 25,000 steps if using four devices. Example distributed training loop:
+```python from agilerl.utils.utils import makeVectEnvs, initialPopulation from
+agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.components.replay_data import ReplayDataset from
+agilerl.components.sampler import Sampler from agilerl.hpo.tournament import
+TournamentSelection from agilerl.hpo.mutation import Mutations from accelerate
+import Accelerator import numpy as np import os from torch.utils.data import
+DataLoader from tqdm import trange if __name__ == '__main__': accelerator =
+Accelerator() NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } INIT_HP = { 'POPULATION_SIZE': 4, # Population
+size 'DOUBLE': True, # Use double Q-learning in DQN or CQN 'BATCH_SIZE': 128, #
+Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, # Discount factor
+'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft update of target
+network parameters 'POLICY_FREQ': 2, # DDPG target network update frequency vs
+policy network # Swap image channels dimension from last to first [H, W, C] ->
+[C, H, W] 'CHANNELS_LAST': False } env = makeVectEnvs('LunarLander-v2',
+num_envs=8) # Create environment try: state_dim =
+env.single_observation_space.n # Discrete observation space one_hot = True #
+Requires one-hot encoding except Exception: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
+env.single_action_space.n # Discrete action space except Exception: action_dim
+= env.single_action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1]) pop =
+initialPopulation(algo='DQN', # Algorithm state_dim=state_dim, # State
+dimension action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot
+encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
+Initial hyperparameters population_size=INIT_HP['POPULATION_SIZE'], #
+Population size accelerator=accelerator) # Accelerator field_names = ["state",
+"action", "reward", "next_state", "done"] memory = ReplayBuffer
+(action_dim=action_dim, # Number of agent actions memory_size=10000, # Max
+replay buffer size field_names=field_names) # Field names to store in memory
+replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE']) replay_dataloader
+= DataLoader(replay_dataset, batch_size=None) replay_dataloader =
+accelerator.prepare(replay_dataloader) sampler = Sampler(distributed=True,
+dataset=replay_dataset, dataloader=replay_dataloader) tournament =
+TournamentSelection(tournament_size=2, # Tournament selection size
+elitism=True, # Elitism in tournament selection population_size=INIT_HP
+['POPULATION_SIZE'], # Population size evo_step=1) # Evaluate using last N
+fitness scores mutations = Mutations(algo='DQN', # Algorithm no_mutation=0.4, #
+No mutation architecture=0.2, # Architecture mutation new_layer_prob=0.2, # New
+layer mutation parameters=0.2, # Network parameters mutation activation=0, #
+Activation layer mutation rl_hp=0.2, # Learning HP mutation rl_hp_selection=
+['lr', 'batch_size'], # Learning HPs to choose from mutation_sd=0.1, # Mutation
+strength arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random
+seed accelerator=accelerator) # Accelerator) max_episodes = 1000 # Max training
+episodes max_steps = 500 # Max steps per episode # Exploration params eps_start
+= 1.0 # Max exploration eps_end = 0.1 # Min exploration eps_decay = 0.995 #
+Decay per episode epsilon = eps_start evo_epochs = 5 # Evolution frequency
+evo_loop = 1 # Number of evaluation episodes accel_temp_models_path = 'models/
+{}'.format('LunarLander-v2') if accelerator.is_main_process: if not
+os.path.exists(accel_temp_models_path): os.makedirs(accel_temp_models_path)
+print(f'\nDistributed training on {accelerator.device}...') # TRAINING LOOP for
+idx_epi in trange(max_episodes): accelerator.wait_for_everyone() for agent in
+pop: # Loop through population state = env.reset()[0] # Reset environment at
+start of episode score = 0 for idx_step in range(max_steps): # Get next action
+from agent action = agent.getAction(state, epsilon) next_state, reward, done,
+_, _ = env.step( action) # Act in environment # Save experience to replay
+buffer memory.save2memoryVectEnvs( state, action, reward, next_state, done) #
+Learn according to learning frequency if memory.counter % agent.learn_step == 0
+and len( memory) >= agent.batch_size: # Sample dataloader experiences =
+sampler.sample(agent.batch_size) # Learn according to agent's RL algorithm
+agent.learn(experiences) state = next_state score += reward # Update epsilon
+for exploration epsilon = max(eps_end, epsilon * eps_decay) # Now evolve
+population if necessary if (idx_epi + 1) % evo_epochs == 0: # Evaluate
+population fitnesses = [ agent.test( env, swap_channels=False,
+max_steps=max_steps, loop=evo_loop) for agent in pop] if
+accelerator.is_main_process: print(f'Episode {idx_epi+1}/{max_episodes}') print
+(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}') print(f'100 fitness
+avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}') # Tournament
+selection and population mutation accelerator.wait_for_everyone() for model in
+pop: model.unwrap_models() accelerator.wait_for_everyone() if
+accelerator.is_main_process: elite, pop = tournament.select(pop) pop =
+mutations.mutation(pop) for pop_i, model in enumerate(pop):
+model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
+accelerator.wait_for_everyone() if not accelerator.is_main_process: for pop_i,
+model in enumerate(pop): model.loadCheckpoint(f'{accel_temp_models_path}/DQN_
+{pop_i}.pt') accelerator.wait_for_everyone() for model in pop:
+model.wrap_models() ``` View documentation.
```

