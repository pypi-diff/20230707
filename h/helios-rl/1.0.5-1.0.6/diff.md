# Comparing `tmp/helios-rl-1.0.5.tar.gz` & `tmp/helios-rl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-rl-1.0.5.tar", last modified: Fri Jul  7 11:15:12 2023, max compression
+gzip compressed data, was "helios-rl-1.0.6.tar", last modified: Fri Jul  7 11:17:03 2023, max compression
```

## Comparing `helios-rl-1.0.5.tar` & `helios-rl-1.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.386366 helios-rl-1.0.5/
--rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.5/LICENSE
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:15:12.385765 helios-rl-1.0.5/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.5/README.md
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.328154 helios-rl-1.0.5/helios_rl/
--rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.336044 helios-rl-1.0.5/helios_rl/adapters/
--rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/adapters/__init__.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.344927 helios-rl-1.0.5/helios_rl/agents/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/agent_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.5/helios_rl/agents/neural_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/random_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/agents/table_q_agent.py
--rw-r--r--   0 p97070po   (502) staff       (20)    20101 2023-07-07 11:13:22.000000 helios-rl-1.0.5/helios_rl/analysis.py
--rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/config.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/config_local.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.357143 helios-rl-1.0.5/helios_rl/encoders/
--rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/__init__.py
--rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/encoder_abstract.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/observable_objects_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/poss_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/poss_state_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/encoders/prior_actions_encoded.py
--rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.5/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.362232 helios-rl-1.0.5/helios_rl/environment_setup/
--rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/helios_info.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/imports.py
--rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/environment_setup/results_table.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.369856 helios-rl-1.0.5/helios_rl/evaluation/
--rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/combined_variance_visual.py
--rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/convergence_measure.py
--rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/evaluation/tabular_output.py
--rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.5/helios_rl/evaluation/visual_output.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.384281 helios-rl-1.0.5/helios_rl/experiments/
--rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/experience_sampling.py
--rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instr_input.py
--rw-r--r--   0 p97070po   (502) staff       (20)    32072 2023-07-05 17:06:07.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search.py
--rw-r--r--   0 p97070po   (502) staff       (20)    27274 2023-07-03 19:04:14.000000 helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search_mlp.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.5/helios_rl/experiments/standard.py
--rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/supervised_instruction_following.py
--rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.5/helios_rl/experiments/unsupervised_instruction_following.py
-drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:15:12.334032 helios-rl-1.0.5/helios_rl.egg-info/
--rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/PKG-INFO
--rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/SOURCES.txt
--rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/dependency_links.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/requires.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-07 11:15:12.000000 helios-rl-1.0.5/helios_rl.egg-info/top_level.txt
--rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-07 11:15:12.386572 helios-rl-1.0.5/setup.cfg
--rw-r--r--   0 p97070po   (502) staff       (20)      767 2023-07-07 11:14:38.000000 helios-rl-1.0.5/setup.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:03.021063 helios-rl-1.0.6/
+-rw-r--r--   0 p97070po   (502) staff       (20)    35821 2023-05-19 11:01:03.000000 helios-rl-1.0.6/LICENSE
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:17:03.020406 helios-rl-1.0.6/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     2749 2023-05-19 10:54:09.000000 helios-rl-1.0.6/README.md
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:02.977809 helios-rl-1.0.6/helios_rl/
+-rw-r--r--   0 p97070po   (502) staff       (20)      533 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:02.984449 helios-rl-1.0.6/helios_rl/adapters/
+-rw-r--r--   0 p97070po   (502) staff       (20)      715 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/adapters/__init__.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:02.990859 helios-rl-1.0.6/helios_rl/agents/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/agents/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      536 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/agents/agent_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     8310 2023-06-07 16:46:15.000000 helios-rl-1.0.6/helios_rl/agents/neural_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      548 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/agents/random_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     7770 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/agents/table_q_agent.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20101 2023-07-07 11:16:43.000000 helios-rl-1.0.6/helios_rl/analysis.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     3039 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/config.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2391 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/config_local.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:02.999258 helios-rl-1.0.6/helios_rl/encoders/
+-rw-r--r--   0 p97070po   (502) staff       (20)     1498 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/__init__.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      804 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/encoder_abstract.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1674 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/observable_objects_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1424 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/poss_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1562 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/poss_state_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1647 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/encoders/prior_actions_encoded.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     2055 2023-05-22 10:54:48.000000 helios-rl-1.0.6/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:03.002792 helios-rl-1.0.6/helios_rl/environment_setup/
+-rw-r--r--   0 p97070po   (502) staff       (20)     6105 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/environment_setup/helios_info.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1645 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/environment_setup/imports.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     4842 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/environment_setup/results_table.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:03.007327 helios-rl-1.0.6/helios_rl/evaluation/
+-rw-r--r--   0 p97070po   (502) staff       (20)     3228 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/evaluation/combined_variance_visual.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     6246 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/evaluation/convergence_measure.py
+-rw-r--r--   0 p97070po   (502) staff       (20)      358 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/evaluation/tabular_output.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    20998 2023-07-03 10:46:56.000000 helios-rl-1.0.6/helios_rl/evaluation/visual_output.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:03.019033 helios-rl-1.0.6/helios_rl/experiments/
+-rw-r--r--   0 p97070po   (502) staff       (20)        0 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/experiments/experience_sampling.py
+-rw-r--r--   0 p97070po   (502) staff       (20)     1238 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/experiments/helios_instr_input.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    32072 2023-07-05 17:06:07.000000 helios-rl-1.0.6/helios_rl/experiments/helios_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27468 2023-05-22 11:07:35.000000 helios-rl-1.0.6/helios_rl/experiments/helios_instruction_search.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    27274 2023-07-03 19:04:14.000000 helios-rl-1.0.6/helios_rl/experiments/helios_instruction_search_mlp.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15554 2023-06-07 16:46:13.000000 helios-rl-1.0.6/helios_rl/experiments/standard.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    15901 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/experiments/supervised_instruction_following.py
+-rw-r--r--   0 p97070po   (502) staff       (20)    10752 2023-05-17 13:39:38.000000 helios-rl-1.0.6/helios_rl/experiments/unsupervised_instruction_following.py
+drwxr-xr-x   0 p97070po   (502) staff       (20)        0 2023-07-07 11:17:02.983469 helios-rl-1.0.6/helios_rl.egg-info/
+-rw-r--r--   0 p97070po   (502) staff       (20)      293 2023-07-07 11:17:02.000000 helios-rl-1.0.6/helios_rl.egg-info/PKG-INFO
+-rw-r--r--   0 p97070po   (502) staff       (20)     1477 2023-07-07 11:17:02.000000 helios-rl-1.0.6/helios_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)        1 2023-07-07 11:17:02.000000 helios-rl-1.0.6/helios_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       66 2023-07-07 11:17:02.000000 helios-rl-1.0.6/helios_rl.egg-info/requires.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       10 2023-07-07 11:17:02.000000 helios-rl-1.0.6/helios_rl.egg-info/top_level.txt
+-rw-r--r--   0 p97070po   (502) staff       (20)       38 2023-07-07 11:17:03.021241 helios-rl-1.0.6/setup.cfg
+-rw-r--r--   0 p97070po   (502) staff       (20)      767 2023-07-07 11:16:46.000000 helios-rl-1.0.6/setup.py
```

### Comparing `helios-rl-1.0.5/LICENSE` & `helios-rl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/README.md` & `helios-rl-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/__init__.py` & `helios-rl-1.0.6/helios_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/adapters/__init__.py` & `helios-rl-1.0.6/helios_rl/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/agents/agent_abstract.py` & `helios-rl-1.0.6/helios_rl/agents/agent_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/agents/neural_q_agent.py` & `helios-rl-1.0.6/helios_rl/agents/neural_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/agents/random_agent.py` & `helios-rl-1.0.6/helios_rl/agents/random_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/agents/table_q_agent.py` & `helios-rl-1.0.6/helios_rl/agents/table_q_agent.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/analysis.py` & `helios-rl-1.0.6/helios_rl/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from helios_rl.evaluation.visual_output import VisualOutput
 from helios_rl.evaluation.tabular_output import TabularOutput
 class Analysis:
     """Calls the Local Environment function and produces analysis reports & figures."""
     def __init__(self, window_size) -> None:
         self.window_size = window_size
-        self.timeout = 30
+        self.timeout = 10
     
     # Training Plots
     def train_report(self, training_results:pd.DataFrame(), save_dir:str, show_figures:str):
         """Produces visual and tabular analysis of individual training results."""
         if not os.path.exists(save_dir):
             os.mkdir(save_dir)
```

### Comparing `helios-rl-1.0.5/helios_rl/config.py` & `helios-rl-1.0.6/helios_rl/config.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/config_local.py` & `helios-rl-1.0.6/helios_rl/config_local.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/__init__.py` & `helios-rl-1.0.6/helios_rl/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/encoder_abstract.py` & `helios-rl-1.0.6/helios_rl/encoders/encoder_abstract.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/observable_objects_encoded.py` & `helios-rl-1.0.6/helios_rl/encoders/observable_objects_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/poss_actions_encoded.py` & `helios-rl-1.0.6/helios_rl/encoders/poss_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/poss_state_encoded.py` & `helios-rl-1.0.6/helios_rl/encoders/poss_state_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/prior_actions_encoded.py` & `helios-rl-1.0.6/helios_rl/encoders/prior_actions_encoded.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py` & `helios-rl-1.0.6/helios_rl/encoders/sentence_transformer_MiniLM_L6v2.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/environment_setup/helios_info.py` & `helios-rl-1.0.6/helios_rl/environment_setup/helios_info.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/environment_setup/imports.py` & `helios-rl-1.0.6/helios_rl/environment_setup/imports.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/environment_setup/results_table.py` & `helios-rl-1.0.6/helios_rl/environment_setup/results_table.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/evaluation/combined_variance_visual.py` & `helios-rl-1.0.6/helios_rl/evaluation/combined_variance_visual.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/evaluation/convergence_measure.py` & `helios-rl-1.0.6/helios_rl/evaluation/convergence_measure.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/evaluation/visual_output.py` & `helios-rl-1.0.6/helios_rl/evaluation/visual_output.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/helios_instr_input.py` & `helios-rl-1.0.6/helios_rl/experiments/helios_instr_input.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_following.py` & `helios-rl-1.0.6/helios_rl/experiments/helios_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search.py` & `helios-rl-1.0.6/helios_rl/experiments/helios_instruction_search.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/helios_instruction_search_mlp.py` & `helios-rl-1.0.6/helios_rl/experiments/helios_instruction_search_mlp.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/standard.py` & `helios-rl-1.0.6/helios_rl/experiments/standard.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/supervised_instruction_following.py` & `helios-rl-1.0.6/helios_rl/experiments/supervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl/experiments/unsupervised_instruction_following.py` & `helios-rl-1.0.6/helios_rl/experiments/unsupervised_instruction_following.py`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/helios_rl.egg-info/SOURCES.txt` & `helios-rl-1.0.6/helios_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-rl-1.0.5/setup.py` & `helios-rl-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='helios-rl',
-    version='1.0.5',
+    version='1.0.6',
     packages=[
         'helios_rl', 
         'helios_rl.adapters', 
         'helios_rl.agents', 
         'helios_rl.encoders', 
         'helios_rl.environment_setup', 
         'helios_rl.evaluation',
```

