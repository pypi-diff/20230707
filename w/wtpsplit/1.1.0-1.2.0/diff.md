# Comparing `tmp/wtpsplit-1.1.0.tar.gz` & `tmp/wtpsplit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtpsplit-1.1.0.tar", last modified: Sat Jun 17 09:54:08 2023, max compression
+gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-8ira0x3h/wtpsplit-1.2.0.tar", last modified: Fri Jul  7 09:49:14 2023, max compression
```

## Comparing `wtpsplit-1.1.0.tar` & `wtpsplit-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     1076 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/LICENSE
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      268 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/PKG-INFO
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    11432 2023-06-17 09:52:02.000000 wtpsplit-1.1.0/README.md
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       73 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/pyproject.toml
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       97 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/setup.cfg
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      494 2023-06-17 09:53:23.000000 wtpsplit-1.1.0/setup.py
-drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit/
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    14249 2023-06-17 09:52:37.000000 wtpsplit-1.1.0/wtpsplit/__init__.py
-drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit/data/
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     3434 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/language_info.csv
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    38208 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/punctuation.json
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      408 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/punctuation.txt
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     7560 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/extract.py
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    40289 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/models.py
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     5814 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/utils.py
-drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit.egg-info/
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      268 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/PKG-INFO
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      381 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/SOURCES.txt
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)        1 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/dependency_links.txt
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       49 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/requires.txt
--rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)        9 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/LICENSE
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    11432 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/README.md
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-04 15:41:03.000000 wtpsplit-1.2.0/pyproject.toml
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/setup.cfg
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-04 16:15:49.000000 wtpsplit-1.2.0/setup.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.404911 wtpsplit-1.2.0/wtpsplit/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14285 2023-07-04 16:15:58.000000 wtpsplit-1.2.0/wtpsplit/__init__.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-04 15:39:28.000000 wtpsplit-1.2.0/wtpsplit/configs.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/wtpsplit/data/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/language_info.csv
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/punctuation.json
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.0/wtpsplit/data/punctuation.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5146 2023-07-04 15:54:05.000000 wtpsplit-1.2.0/wtpsplit/extract.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-04 16:15:50.000000 wtpsplit-1.2.0/wtpsplit/models.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6374 2023-07-04 16:15:57.000000 wtpsplit-1.2.0/wtpsplit/utils.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-07 09:49:14.408911 wtpsplit-1.2.0/wtpsplit.egg-info/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/requires.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-07 09:49:14.000000 wtpsplit-1.2.0/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.1.0/LICENSE` & `wtpsplit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.1.0/README.md` & `wtpsplit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.1.0/wtpsplit/__init__.py` & `wtpsplit-1.2.0/wtpsplit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,25 @@
+import math
 import os
 from pathlib import Path
+import contextlib
 
-# to register models for AutoModel
-import wtpsplit.models  # noqa
-
+# avoid the "None of PyTorch, TensorFlow, etc. have been found" warning.
+with contextlib.redirect_stderr(open(os.devnull, "w")):
+    import transformers  # noqa
 
-import math
 import numpy as np
-
-import torch
-from transformers import AutoModelForTokenClassification
-from transformers.utils.hub import cached_file
 import skops.io as sio
+from transformers import AutoConfig, AutoModelForTokenClassification
+from transformers.utils.hub import cached_file
 
-from wtpsplit.extract import extract
-from wtpsplit.utils import Constants, encode, indices_to_sentences
-
-__version__ = "1.1.0"
-
-
-class ORTWrapper:
-    def __init__(self, model, ort_session):
-        self.model = model
-        self.ort_session = ort_session
-
-    @property
-    def device(self):
-        return self.model.device
-
-    @property
-    def config(self):
-        return self.model.config
-
-    def __call__(self, input_ids, attention_mask, position_ids):
-        inputs_embeds = self.model.get_input_embeddings()(input_ids)
-
-        logits = self.ort_session.run(
-            ["logits"],
-            {
-                "attention_mask": attention_mask.detach().numpy(),
-                "position_ids": position_ids.detach().numpy(),
-                "inputs_embeds": inputs_embeds.detach().numpy(),
-            },
-        )[0]
+from wtpsplit.extract import ORTWrapper, PyTorchWrapper, extract
+from wtpsplit.utils import Constants, indices_to_sentences, sigmoid
 
-        return {"logits": torch.from_numpy(logits).to(self.model.device)}
+__version__ = "1.2.0"
 
 
 class WtP:
     def __init__(
         self,
         model_name_or_model,
         from_pretrained_kwargs=None,
@@ -60,28 +31,24 @@
         self.model_name_or_model = model_name_or_model
         self.ort_providers = ort_providers
         self.ort_kwargs = ort_kwargs
 
         mixture_path = None
 
         if isinstance(model_name_or_model, (str, Path)):
-            model_name_or_model = str(model_name_or_model)
-            is_local = os.path.isdir(model_name_or_model)
+            model_name = str(model_name_or_model)
+            is_local = os.path.isdir(model_name)
 
             if not is_local and hub_prefix is not None:
-                model_name_to_fetch = f"{hub_prefix}/{model_name_or_model}"
+                model_name_to_fetch = f"{hub_prefix}/{model_name}"
             else:
-                model_name_to_fetch = model_name_or_model
-
-            model = AutoModelForTokenClassification.from_pretrained(
-                model_name_to_fetch, **(from_pretrained_kwargs or {})
-            )
+                model_name_to_fetch = model_name
 
             if is_local:
-                model_path = Path(model_name_or_model)
+                model_path = Path(model_name)
                 mixture_path = model_path / "mixture.skops"
                 if not mixture_path.exists():
                     mixture_path = None
                 onnx_path = model_path / "model.onnx"
                 if not onnx_path.exists():
                     onnx_path = None
             else:
@@ -98,46 +65,65 @@
 
             if ort_providers is not None:
                 if onnx_path is None:
                     raise ValueError(
                         "Could not find an ONNX model in the model directory. Try `use_ort=False` to run with PyTorch."
                     )
 
-                import onnxruntime as ort
+                try:
+                    import onnxruntime as ort  # noqa
+                except ModuleNotFoundError:
+                    raise ValueError("Please install `onnxruntime` to use WtP with an ONNX model.")
+
+                # to register models for AutoConfig
+                import wtpsplit.configs  # noqa
 
                 self.model = ORTWrapper(
-                    model, ort.InferenceSession(onnx_path, providers=ort_providers, **(ort_kwargs or {}))
+                    AutoConfig.from_pretrained(model_name_to_fetch, **(from_pretrained_kwargs or {})),
+                    ort.InferenceSession(str(onnx_path), providers=ort_providers, **(ort_kwargs or {})),
                 )
             else:
-                self.model = model
+                # to register models for AutoConfig
+                try:
+                    import torch  # noqa
+                except ModuleNotFoundError:
+                    raise ValueError("Please install `torch` to use WtP with a PyTorch model.")
+
+                import wtpsplit.models  # noqa
+
+                self.model = PyTorchWrapper(
+                    AutoModelForTokenClassification.from_pretrained(
+                        model_name_to_fetch, **(from_pretrained_kwargs or {})
+                    )
+                )
         else:
             if ort_providers is not None:
                 raise ValueError("You can only use onnxruntime with a model directory, not a model object.")
 
             self.model = model_name_or_model
 
         if mixtures is not None:
             self.mixtures = mixtures
         elif mixture_path is not None:
             self.mixtures = sio.load(
                 mixture_path,
-                ["numpy.float32", "numpy.float64"],
+                ["numpy.float32", "numpy.float64", "sklearn.linear_model._logistic.LogisticRegression"],
             )
         else:
             self.mixtures = None
 
     def __getattr__(self, name):
         return getattr(self.model, name)
 
     def predict_proba(
         self,
         text_or_texts,
         lang_code: str = None,
         style: str = None,
-        stride=64,
+        stride=256,
         block_size: int = 512,
         batch_size=32,
         pad_last_batch: bool = False,
         remove_whitespace_before_inference: bool = False,
         outer_batch_size=1000,
         return_paragraph_probabilities=False,
         verbose: bool = False,
@@ -226,26 +212,26 @@
                     space_positions.append(text_space_positions)
                 else:
                     input_text = text
 
                 input_texts.append(input_text)
 
             outer_batch_logits = extract(
-                [encode(text) for text in outer_batch_texts],
+                outer_batch_texts,
                 self.model,
                 lang_code=lang_code,
                 stride=stride,
                 block_size=block_size,
                 batch_size=batch_size,
                 pad_last_batch=pad_last_batch,
                 verbose=verbose,
             )
 
             def newline_probability_fn(logits):
-                return torch.sigmoid(logits.float()[:, Constants.NEWLINE_INDEX]).numpy()
+                return sigmoid(logits[:, Constants.NEWLINE_INDEX])
 
             for i, (text, logits) in enumerate(zip(outer_batch_texts, outer_batch_logits)):
                 if style is not None:
                     sentence_probs = clf.predict_proba(logits)[:, 1]
                     newline_probs = newline_probability_fn(logits)
                 else:
                     sentence_probs = newline_probs = newline_probability_fn(logits)
@@ -311,15 +297,15 @@
                 pad_last_batch=pad_last_batch,
                 remove_whitespace_before_inference=remove_whitespace_before_inference,
                 outer_batch_size=outer_batch_size,
                 paragraph_threshold=paragraph_threshold,
                 do_paragraph_segmentation=do_paragraph_segmentation,
                 verbose=verbose,
             )
-        
+
     def get_threshold(self, lang_code: str, style: str, return_punctuation_threshold: bool = False):
         try:
             _, _, punctuation_threshold, threshold = self.mixtures[lang_code][style]
         except KeyError:
             raise ValueError(f"Could not find a mixture for the style '{style}' and language '{lang_code}'.")
 
         if return_punctuation_threshold:
```

### Comparing `wtpsplit-1.1.0/wtpsplit/data/language_info.csv` & `wtpsplit-1.2.0/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.1.0/wtpsplit/data/punctuation.json` & `wtpsplit-1.2.0/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.1.0/wtpsplit/models.py` & `wtpsplit-1.2.0/wtpsplit/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import copy
 import math
 from typing import Optional, Tuple, Union
 
 import torch
 from torch import nn
-from transformers import AutoConfig, AutoModel, AutoModelForTokenClassification, CanineConfig
-from transformers.models.bert.modeling_bert import (
-    BertConfig,
-    BertEncoder,
-    BertForTokenClassification,
-    BertModel,
-    BertPooler,
-)
+from transformers import AutoModel, AutoModelForTokenClassification
+from transformers.models.bert.modeling_bert import BertEncoder, BertForTokenClassification, BertModel, BertPooler
 from transformers.models.canine.modeling_canine import (
     _PRIMES,
     ACT2FN,
     BaseModelOutput,
     CanineAttention,
     CanineEmbeddings,
     CanineEncoder,
@@ -29,103 +23,101 @@
     CanineSelfAttention,
     CanineSelfOutput,
     CharactersToMolecules,
     ConvProjection,
     TokenClassifierOutput,
 )
 
+from wtpsplit.configs import BertCharConfig, LACanineConfig
 from wtpsplit.utils import Constants
 
 
-class LACanineConfig(CanineConfig):
-    model_type = "la-canine"
-
-    def __init__(
-        self,
-        n_languages=None,
-        ngram_order=1,
-        bottleneck_factor=2,
-        language_adapter="on",
-        lookahead=None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-
-        self.n_languages = n_languages
-        self.ngram_order = ngram_order
-        self.language_adapter = language_adapter  # 'on', 'off', 'shared'
-        self.bottleneck_factor = bottleneck_factor
-
-        self.lookahead = lookahead
-        self.lookahead_block_size = 1
-
-
-class BertCharConfig(BertConfig):
-    model_type = "bert-char"
-
-    def __init__(
-        self,
-        num_hash_buckets=8192,
-        num_hash_functions=8,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-
-        self.num_hash_buckets = num_hash_buckets
-        self.num_hash_functions = num_hash_functions
-
-
 # added n-gram representations
 class LACanineEmbeddings(CanineEmbeddings):
     def __init__(self, config):
         super().__init__(config)
 
         self.ngram_order = getattr(config, "ngram_order", 1)
+        if self.ngram_order > 1:
+            raise NotImplementedError("n-gram representations are not implemented.")
 
         shard_embedding_size = config.hidden_size // config.num_hash_functions
         for j in range(2, self.ngram_order + 1):
             for i in range(config.num_hash_functions):
                 name = f"HashBucketCodepointEmbedder_{i}_{j}"
                 setattr(
                     self,
                     name,
                     nn.Embedding(config.num_hash_buckets, shard_embedding_size),
                 )
 
-    def _embed_hash_buckets(self, input_ids, embedding_size: int, num_hashes: int, num_buckets: int):
+    def _embed_hash_buckets(self, input_ids=None, hashed_ids=None):
+        embedding_size = self.config.hidden_size
+        num_hashes = self.config.num_hash_functions
+        num_buckets = self.config.num_hash_buckets
+
+        assert (input_ids is None) + (
+            hashed_ids is None
+        ) == 1, "Either `input_ids` or `hashed_ids` must be provided (and not both!)."
+
         """Converts IDs (e.g. codepoints) into embeddings via multiple hashing."""
         if embedding_size % num_hashes != 0:
             raise ValueError(f"Expected `embedding_size` ({embedding_size}) % `num_hashes` ({num_hashes}) == 0")
 
         if num_hashes > len(_PRIMES):
             raise ValueError(f"`num_hashes` must be <= {len(_PRIMES)}")
 
         embedding_shards = []
         for i in range(num_hashes):
             name = f"HashBucketCodepointEmbedder_{i}"
 
-            hash_ids = (input_ids + 1) * _PRIMES[i]
+            hash_ids = ((input_ids + 1) * _PRIMES[i]) % num_buckets if hashed_ids is None else hashed_ids[:, :, i]
 
-            shard_embeddings = getattr(self, name)(hash_ids % num_buckets)
+            shard_embeddings = getattr(self, name)(hash_ids)
+            embedding_shards.append(shard_embeddings)
 
-            for j in range(2, self.ngram_order + 1):
-                name = f"HashBucketCodepointEmbedder_{i}_{j}"
+        return torch.cat(embedding_shards, dim=-1)
+
+    def forward(
+        self,
+        input_ids: Optional[torch.LongTensor] = None,
+        hashed_ids: Optional[torch.LongTensor] = None,
+        token_type_ids: Optional[torch.LongTensor] = None,
+        position_ids: Optional[torch.LongTensor] = None,
+        inputs_embeds: Optional[torch.FloatTensor] = None,
+        **kwargs,
+    ) -> torch.FloatTensor:
+        if input_ids is not None:
+            input_shape = input_ids.size()
+        elif hashed_ids is not None:
+            input_shape = hashed_ids.size()[:-1]
+        else:
+            input_shape = inputs_embeds.size()[:-1]
 
-                prev_hash_ids = hash_ids.clone()
+        seq_length = input_shape[1]
 
-                hash_ids[:-1] = (input_ids[:-1] + prev_hash_ids[1:] + 1) * _PRIMES[i]
-                shard_embeddings += getattr(self, name)(hash_ids % num_buckets)
+        if position_ids is None:
+            position_ids = self.position_ids[:, :seq_length]
 
-            embedding_shards.append(shard_embeddings)
+        if token_type_ids is None:
+            token_type_ids = torch.zeros(input_shape, dtype=torch.long, device=self.position_ids.device)
 
-        return torch.cat(embedding_shards, dim=-1)
+        if inputs_embeds is None:
+            inputs_embeds = self._embed_hash_buckets(input_ids, hashed_ids)
+
+        token_type_embeddings = self.token_type_embeddings(token_type_ids)
+
+        embeddings = inputs_embeds + token_type_embeddings
 
-    def forward(self, *args, **kwargs):
-        kwargs.pop("past_key_values_length", None)
-        return super().forward(*args, **kwargs)
+        if self.position_embedding_type == "absolute":
+            position_embeddings = self.char_position_embeddings(position_ids)
+            embeddings += position_embeddings
+        embeddings = self.LayerNorm(embeddings)
+        embeddings = self.dropout(embeddings)
+        return embeddings
 
 
 class LACanineSelfAttention(CanineSelfAttention):
     def __init__(self, config):
         super(CanineSelfAttention, self).__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
             raise ValueError(
@@ -693,15 +685,17 @@
             inputs_embeds=inputs_embeds,
         )
 
         # Contextualize character embeddings using shallow Transformer.
         # We use a 3D attention mask for the local attention.
         # `input_char_encoding`: shape (batch_size, char_seq_len, char_dim)
         if attention_mask.ndim == 2:
-            char_attention_mask = self._create_3d_attention_mask_from_input_mask(input_ids, attention_mask)
+            char_attention_mask = self._create_3d_attention_mask_from_input_mask(
+                input_ids or inputs_embeds, attention_mask
+            )
         else:
             char_attention_mask = attention_mask
         init_chars_encoder_outputs = self.initial_char_encoder(
             input_char_embeddings,
             language_ids=language_ids,
             attention_mask=char_attention_mask,
             output_attentions=output_attentions,
@@ -826,20 +820,30 @@
         token_type_ids: Optional[torch.LongTensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         head_mask: Optional[torch.FloatTensor] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
+        hashed_ids: Optional[torch.Tensor] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple, TokenClassifierOutput]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
+        inputs_embeds = self.canine.char_embeddings(
+            input_ids=input_ids,
+            hashed_ids=hashed_ids,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
+            inputs_embeds=inputs_embeds,
+        )
+        input_ids = None
+
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         outputs = self.canine(
             input_ids,
             language_ids=language_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
@@ -928,31 +932,39 @@
         token_type_ids: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
         head_mask: Optional[torch.Tensor] = None,
         inputs_embeds: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
+        hashed_ids: Optional[torch.Tensor] = None,
         language_ids=None,
         return_dict: Optional[bool] = None,
     ):
+        inputs_embeds = self.bert.embeddings(
+            input_ids=input_ids,
+            hashed_ids=hashed_ids,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
+            inputs_embeds=inputs_embeds,
+        )
+        input_ids = None
+
         return super().forward(
             input_ids,
             attention_mask,
             token_type_ids,
             position_ids,
             head_mask,
             inputs_embeds,
             labels,
             output_attentions,
             output_hidden_states,
             return_dict,
         )
 
 
-AutoConfig.register("la-canine", LACanineConfig)
 AutoModel.register(LACanineConfig, LACanineModel)
 AutoModelForTokenClassification.register(LACanineConfig, LACanineForTokenClassification)
 
-AutoConfig.register("bert-char", BertCharConfig)
 AutoModel.register(BertCharConfig, BertCharModel)
 AutoModelForTokenClassification.register(BertCharConfig, BertCharForTokenClassification)
```

### Comparing `wtpsplit-1.1.0/wtpsplit/utils.py` & `wtpsplit-1.2.0/wtpsplit/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import json
 import os
 import random
 from dataclasses import dataclass, field
+from cached_property import cached_property
 from pathlib import Path
 from typing import List
-from functools import cached_property
 
+import numpy as np
 import pandas as pd
 
+# same as in CANINE
+PRIMES = [31, 43, 59, 61, 73, 97, 103, 113, 137, 149, 157, 173, 181, 193, 211, 223]
+
 
 class ConstantsClass:
     NEWLINE_INDEX = 0
     AUX_OFFSET = 1
 
     @cached_property
     def ROOT_DIR(self):
@@ -69,18 +73,34 @@
 
     for c in label_args.newline_chars:
         label_dict[ord(c)] = 1 + Constants.NEWLINE_INDEX
 
     return label_dict
 
 
+def sigmoid(x):
+    return 1 / (1 + np.exp(-x))
+
+
 def encode(text):
     return [ord(c) for c in text]
 
 
+def hash_encode(encoding, num_hashes=8, num_buckets=8192):
+    if num_hashes > len(PRIMES):
+        raise ValueError(f"`num_hashes` must be <= {len(PRIMES)}")
+
+    hash_ids = np.zeros((len(encoding), num_hashes), dtype=np.int64)
+    for i in range(num_hashes):
+        shard_ids = (encoding + 1) * PRIMES[i]
+        hash_ids[:, i] = shard_ids % num_buckets
+
+    return hash_ids
+
+
 def label(input_ids, label_dict):
     return [label_dict.get(input_id, 0) for input_id in input_ids[1:]] + [0]
 
 
 def lang_code_to_lang(lang_code):
     from iso639 import languages
```

