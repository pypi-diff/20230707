# Comparing `tmp/helios-rl-1.0.4.tar.gz` & `tmp/helios-rl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-rl-1.0.4.tar", last modified: Wed Jul  5 17:06:29 2023, max compression
+gzip compressed data, was "helios-rl-1.0.5.tar", last modified: Fri Jul  7 11:15:12 2023, max compression
```

## Comparing `helios-rl-1.0.4.tar` & `helios-rl-1.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.425464 helios-rl-1.0.4/
--rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.4/LICENSE
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-05 17:06:29.424810 helios-rl-1.0.4/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.4/README.md
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.375344 helios-rl-1.0.4/helios_rl/
--rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.382510 helios-rl-1.0.4/helios_rl/adapters/
--rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/adapters/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.389560 helios-rl-1.0.4/helios_rl/agents/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/agents/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/agents/agent_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.4/helios_rl/agents/neural_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/agents/random_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/agents/table_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)    19502 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/analysis.py
--rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/config.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/config_local.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.399550 helios-rl-1.0.4/helios_rl/encoders/
--rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/encoder_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/observable_objects_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/poss_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/poss_state_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/encoders/prior_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.4/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.404109 helios-rl-1.0.4/helios_rl/environment_setup/
--rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/environment_setup/helios_info.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/environment_setup/imports.py
--rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/environment_setup/results_table.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.409848 helios-rl-1.0.4/helios_rl/evaluation/
--rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/evaluation/combined_variance_visual.py
--rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/evaluation/convergence_measure.py
--rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/evaluation/tabular_output.py
--rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.4/helios_rl/evaluation/visual_output.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.423258 helios-rl-1.0.4/helios_rl/experiments/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/experiments/experience_sampling.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/experiments/helios_instr_input.py
--rw-r--r--   0 p97070po   (502) staff       (20)    32072 2023-07-05 17:06:07.000000 helios-rl-1.0.4/helios_rl/experiments/helios_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.4/helios_rl/experiments/helios_instruction_search.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27274 2023-07-03 19:04:14.000000 helios-rl-1.0.4/helios_rl/experiments/helios_instruction_search_mlp.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.4/helios_rl/experiments/standard.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/experiments/supervised_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.4/helios_rl/experiments/unsupervised_instruction_following.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-05 17:06:29.381459 helios-rl-1.0.4/helios_rl.egg-info/
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-05 17:06:29.000000 helios-rl-1.0.4/helios_rl.egg-info/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-05 17:06:29.000000 helios-rl-1.0.4/helios_rl.egg-info/SOURCES.txt
--rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-05 17:06:29.000000 helios-rl-1.0.4/helios_rl.egg-info/dependency_links.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-05 17:06:29.000000 helios-rl-1.0.4/helios_rl.egg-info/requires.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-05 17:06:29.000000 helios-rl-1.0.4/helios_rl.egg-info/top_level.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-05 17:06:29.425691 helios-rl-1.0.4/setup.cfg
--rw-r--r--   0 p97070po   (502) staff       (20)      767 2023-07-05 17:06:07.000000 helios-rl-1.0.4/setup.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.386366 helios-rl-1.0.5/
+-rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.5/LICENSE
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:15:12.385765 helios-rl-1.0.5/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.5/README.md
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.328154 helios-rl-1.0.5/helios_rl/
+-rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.336044 helios-rl-1.0.5/helios_rl/adapters/
+-rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/adapters/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.344927 helios-rl-1.0.5/helios_rl/agents/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/agent_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.5/helios_rl/agents/neural_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/random_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/table_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20101 2023-07-07 11:13:22.000000 helios-rl-1.0.5/helios_rl/analysis.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/config.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/config_local.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.357143 helios-rl-1.0.5/helios_rl/encoders/
+-rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/encoder_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/observable_objects_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/poss_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/poss_state_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/prior_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.5/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.362232 helios-rl-1.0.5/helios_rl/environment_setup/
+-rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/helios_info.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/imports.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/results_table.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.369856 helios-rl-1.0.5/helios_rl/evaluation/
+-rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/combined_variance_visual.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/convergence_measure.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/tabular_output.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.5/helios_rl/evaluation/visual_output.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.384281 helios-rl-1.0.5/helios_rl/experiments/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/experience_sampling.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instr_input.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    32072 2023-07-05 17:06:07.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27274 2023-07-03 19:04:14.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search_mlp.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.5/helios_rl/experiments/standard.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/supervised_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/unsupervised_instruction_following.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.334032 helios-rl-1.0.5/helios_rl.egg-info/
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/requires.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/top_level.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-07 11:15:12.386572 helios-rl-1.0.5/setup.cfg
+-rw-r--r--   0 p97070po   (502) staff       (20)      767 2023-07-07 11:14:38.000000 helios-rl-1.0.5/setup.py
```

### Comparing `helios-rl-1.0.4/LICENSE` & `helios-rl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/README.md` & `helios-rl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/__init__.py` & `helios-rl-1.0.5/helios_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/adapters/__init__.py` & `helios-rl-1.0.5/helios_rl/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/agents/agent_abstract.py` & `helios-rl-1.0.5/helios_rl/agents/agent_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/agents/neural_q_agent.py` & `helios-rl-1.0.5/helios_rl/agents/neural_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/agents/random_agent.py` & `helios-rl-1.0.5/helios_rl/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/agents/table_q_agent.py` & `helios-rl-1.0.5/helios_rl/agents/table_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/analysis.py` & `helios-rl-1.0.5/helios_rl/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-
+import multiprocessing
 import os
 
 import warnings
 warnings.filterwarnings("ignore")
 
 from helios_rl.evaluation.visual_output import VisualOutput
 from helios_rl.evaluation.tabular_output import TabularOutput
 class Analysis:
     """Calls the Local Environment function and produces analysis reports & figures."""
     def __init__(self, window_size) -> None:
         self.window_size = window_size
+        self.timeout = 30
     
     # Training Plots
     def train_report(self, training_results:pd.DataFrame(), save_dir:str, show_figures:str):
         """Produces visual and tabular analysis of individual training results."""
         if not os.path.exists(save_dir):
             os.mkdir(save_dir)
         
@@ -27,15 +28,22 @@
         VisualAnalysis.episode_reward_dist_graph()
         VisualAnalysis.average_reward_graph()
         VisualAnalysis.rolling_average_reward_graph()
         VisualAnalysis.avg_return_dist_graph()
         VisualAnalysis.number_actions_graph()
         VisualAnalysis.number_actions_dist_graph()
         VisualAnalysis.runtime_per_episode_graph()
-        VisualAnalysis.runtime_dist_graph()
+        # Catch runtime issues for dist plot
+        p = multiprocessing.Process(target=VisualAnalysis.runtime_dist_graph(), name="runtime_dist_graph")
+        p.start()
+        p.join(self.timeout)
+        if p.is_alive():
+            print('function terminated')
+            p.terminate()
+            p.join()
         
         TableOutput = TabularOutput(training_results, save_dir)
         TableOutput.save_results()
         return training_results[training_results['episode']==np.max(training_results['episode'])]['cumulative_reward'].iloc[0]
         
     def training_variance_report(self, save_dir:str, show_figures:str):
         """Extracts individual training reports from folders in save_dir and produces summary report if agent types match."""
@@ -202,15 +210,22 @@
         VisualAnalysis.episode_reward_dist_graph()
         VisualAnalysis.average_reward_graph()
         VisualAnalysis.rolling_average_reward_graph()
         VisualAnalysis.avg_return_dist_graph()
         VisualAnalysis.number_actions_graph()
         VisualAnalysis.number_actions_dist_graph()
         VisualAnalysis.runtime_per_episode_graph()
-        VisualAnalysis.runtime_dist_graph()
+        # Catch runtime issues for dist plot
+        p = multiprocessing.Process(target=VisualAnalysis.runtime_dist_graph(), name="runtime_dist_graph")
+        p.start()
+        p.join(self.timeout)
+        if p.is_alive():
+            print('function terminated')
+            p.terminate()
+            p.join()
 
         TableOutput = TabularOutput(test_results, save_dir)
         TableOutput.save_results()
         return test_results[test_results['episode']==np.max(test_results['episode'])]['cumulative_reward'].iloc[0]
 
     def testing_variance_report(self, save_dir:str, show_figures:str):
         """Extracts individual training reports from folders in save_dir and produces summary report if agent types match."""
```

### Comparing `helios-rl-1.0.4/helios_rl/config.py` & `helios-rl-1.0.5/helios_rl/config.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/config_local.py` & `helios-rl-1.0.5/helios_rl/config_local.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/__init__.py` & `helios-rl-1.0.5/helios_rl/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/encoder_abstract.py` & `helios-rl-1.0.5/helios_rl/encoders/encoder_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/observable_objects_encoded.py` & `helios-rl-1.0.5/helios_rl/encoders/observable_objects_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/poss_actions_encoded.py` & `helios-rl-1.0.5/helios_rl/encoders/poss_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/poss_state_encoded.py` & `helios-rl-1.0.5/helios_rl/encoders/poss_state_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/prior_actions_encoded.py` & `helios-rl-1.0.5/helios_rl/encoders/prior_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py` & `helios-rl-1.0.5/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/environment_setup/helios_info.py` & `helios-rl-1.0.5/helios_rl/environment_setup/helios_info.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/environment_setup/imports.py` & `helios-rl-1.0.5/helios_rl/environment_setup/imports.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/environment_setup/results_table.py` & `helios-rl-1.0.5/helios_rl/environment_setup/results_table.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/evaluation/combined_variance_visual.py` & `helios-rl-1.0.5/helios_rl/evaluation/combined_variance_visual.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/evaluation/convergence_measure.py` & `helios-rl-1.0.5/helios_rl/evaluation/convergence_measure.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/evaluation/visual_output.py` & `helios-rl-1.0.5/helios_rl/evaluation/visual_output.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/helios_instr_input.py` & `helios-rl-1.0.5/helios_rl/experiments/helios_instr_input.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/helios_instruction_following.py` & `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/helios_instruction_search.py` & `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/helios_instruction_search_mlp.py` & `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search_mlp.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/standard.py` & `helios-rl-1.0.5/helios_rl/experiments/standard.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/supervised_instruction_following.py` & `helios-rl-1.0.5/helios_rl/experiments/supervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl/experiments/unsupervised_instruction_following.py` & `helios-rl-1.0.5/helios_rl/experiments/unsupervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/helios_rl.egg-info/SOURCES.txt` & `helios-rl-1.0.5/helios_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.4/setup.py` & `helios-rl-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='helios-rl',
-    version='1.0.4',
+    version='1.0.5',
     packages=[
         'helios_rl', 
         'helios_rl.adapters', 
         'helios_rl.agents', 
         'helios_rl.encoders', 
         'helios_rl.environment_setup', 
         'helios_rl.evaluation',
```

