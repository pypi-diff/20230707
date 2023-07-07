# Comparing `tmp/tibert-0.0.3.tar.gz` & `tmp/tibert-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibert-0.0.3.tar", max compression
+gzip compressed data, was "tibert-0.1.0.tar", max compression
```

## Comparing `tibert-0.0.3.tar` & `tibert-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.0.3/LICENSE
--rw-r--r--   0        0        0     5929 2023-07-04 12:51:01.410790 tibert-0.0.3/README.md
--rw-r--r--   0        0        0      600 2023-07-04 15:09:36.658247 tibert-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.0.3/tibert/__init__.py
--rw-r--r--   0        0        0    50015 2023-07-04 15:08:45.449549 tibert-0.0.3/tibert/bertcoref.py
--rw-r--r--   0        0        0     3176 2023-07-04 12:16:01.266205 tibert-0.0.3/tibert/predict.py
--rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.0.3/tibert/run_train.py
--rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.0.3/tibert/score.py
--rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.0.3/tibert/train.py
--rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.0.3/tibert/utils.py
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 tibert-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 10:22:09.254266 tibert-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6443 2023-07-07 08:20:25.534883 tibert-0.1.0/README.md
+-rw-r--r--   0        0        0      600 2023-07-07 08:29:00.050394 tibert-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-07-04 12:15:55.862129 tibert-0.1.0/tibert/__init__.py
+-rw-r--r--   0        0        0    50015 2023-07-04 15:08:45.449549 tibert-0.1.0/tibert/bertcoref.py
+-rw-r--r--   0        0        0     3594 2023-07-07 08:24:50.126587 tibert-0.1.0/tibert/predict.py
+-rw-r--r--   0        0        0     2298 2023-07-04 10:26:10.637292 tibert-0.1.0/tibert/run_train.py
+-rw-r--r--   0        0        0     4530 2023-07-04 12:16:20.738479 tibert-0.1.0/tibert/score.py
+-rw-r--r--   0        0        0     5792 2023-07-04 10:26:09.773280 tibert-0.1.0/tibert/train.py
+-rw-r--r--   0        0        0     4417 2023-07-04 12:40:38.986271 tibert-0.1.0/tibert/utils.py
+-rw-r--r--   0        0        0     7305 1970-01-01 00:00:00.000000 tibert-0.1.0/PKG-INFO
```

### Comparing `tibert-0.0.3/LICENSE` & `tibert-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/README.md` & `tibert-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,30 @@
 results in:
 
 `>>> (0 Sli ) did not want the earpods . (0 He ) didn't like them .`
 
 `>>> (0 Princess Liana ) felt sad , because (1 Zarth Arn ) was gone . (0 The princess) went to sleep .`
 
 
+## Using Coreference Chains
+
+The coreference chains predicted can be accessed using the `.coref_chains` attribute:
+
+```python
+annotated_doc = predict_coref_simple(
+    "Princess Liana felt sad, because Zarth Arn was gone. The princess went to sleep.",
+    model,
+    tokenizer
+)
+print(annotated_doc.coref_chains)
+```
+
+`>>>[[Mention(tokens=['The', 'princess'], start_idx=11, end_idx=13), Mention(tokens=['Princess', 'Liana'], start_idx=0, end_idx=2)], [Mention(tokens=['Zarth', 'Arn'], start_idx=6, end_idx=8)]]`
+
+
 ## Training a model
 
 Aside from the `tibert.train.train_coref_model` function, it is possible to train a model from the command line. Training a model requires installing the `sacred` library. Here is the most basic example:
 
 ```sh
 python -m tibert.run_train with\
        dataset_path=/path/to/litbank/repository\
```

### Comparing `tibert-0.0.3/pyproject.toml` & `tibert-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibert"
-version = "0.0.3"
+version = "0.1.0"
 description = "BERT for Coreference Resolution"
 authors = ["Arthur Amalvy <arthur.amalvy@univ-avignon.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "tibert" }
 ]
```

### Comparing `tibert-0.0.3/tibert/bertcoref.py` & `tibert-0.1.0/tibert/bertcoref.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/tibert/predict.py` & `tibert-0.1.0/tibert/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Literal, List
+from typing import TYPE_CHECKING, Literal, List, Union, cast
 from transformers import PreTrainedTokenizerFast
 import torch
 from tqdm import tqdm
 from torch.utils.data.dataloader import DataLoader
 from sacremoses import MosesTokenizer
 
 if TYPE_CHECKING:
@@ -11,46 +11,55 @@
         CoreferenceDocument,
         BertCoreferenceResolutionOutput,
         BertForCoreferenceResolution,
     )
 
 
 def predict_coref(
-    documents: List[str],
+    documents: List[Union[str, List[str]]],
     model: BertForCoreferenceResolution,
     tokenizer: PreTrainedTokenizerFast,
     batch_size: int = 1,
     quiet: bool = False,
     device_str: Literal["cpu", "cuda", "auto"] = "auto",
 ) -> List[CoreferenceDocument]:
     """Predict coreference chains for a list of documents.
 
-    :param documents: A list of tokenized documents.
+    :param documents: A list of documents, tokenized or not.  If
+        documents are not tokenized, MosesTokenizer will tokenize them
+        automatically.
     :param tokenizer:
     :param batch_size:
-    :param quiet: If ``True``, will report progress using
-        ``tqdm``.
+    :param quiet: If ``True``, will report progress using ``tqdm``.
 
     :return: a list of ``CoreferenceDocument``, with annotated
-                coreference chains.
+             coreference chains.
     """
     from tibert import (
         CoreferenceDataset,
         CoreferenceDocument,
         DataCollatorForSpanClassification,
     )
 
     if device_str == "auto":
         device_str = "cuda" if torch.cuda.is_available() else "cpu"
     device = torch.device(device_str)
 
-    m_tokenizer = MosesTokenizer(lang="en")
-    tokenized_documents = [
-        m_tokenizer.tokenize(text, escape=False) for text in documents
-    ]
+    if len(documents) == 0:
+        return []
+
+    # Tokenized input sentence if needed
+    if isinstance(documents[0], str):
+        m_tokenizer = MosesTokenizer(lang="en")
+        tokenized_documents = [
+            m_tokenizer.tokenize(text, escape=False) for text in documents
+        ]
+    else:
+        tokenized_documents = documents
+    tokenized_documents = cast(List[List[str]], tokenized_documents)
 
     dataset = CoreferenceDataset(
         [CoreferenceDocument(doc, []) for doc in tokenized_documents],
         tokenizer,
         model.config.max_span_size,
     )
     data_collator = DataCollatorForSpanClassification(tokenizer, model.config.max_span_size)  # type: ignore
@@ -89,13 +98,16 @@
             ]
             preds += out_docs
 
     return preds
 
 
 def predict_coref_simple(
-    text: str, model, tokenizer, device_str: Literal["cpu", "cuda", "auto"] = "auto"
+    text: Union[str, List[str]],
+    model,
+    tokenizer,
+    device_str: Literal["cpu", "cuda", "auto"] = "auto",
 ) -> CoreferenceDocument:
     annotated_docs = predict_coref(
         [text], model, tokenizer, batch_size=1, device_str=device_str, quiet=True
     )
     return annotated_docs[0]
```

### Comparing `tibert-0.0.3/tibert/run_train.py` & `tibert-0.1.0/tibert/run_train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/tibert/score.py` & `tibert-0.1.0/tibert/score.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/tibert/train.py` & `tibert-0.1.0/tibert/train.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/tibert/utils.py` & `tibert-0.1.0/tibert/utils.py`

 * *Files identical despite different names*

### Comparing `tibert-0.0.3/PKG-INFO` & `tibert-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibert
-Version: 0.0.3
+Version: 0.1.0
 Summary: BERT for Coreference Resolution
 License: GPL-3.0-only
 Author: Arthur Amalvy
 Author-email: arthur.amalvy@univ-avignon.fr
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -93,14 +93,30 @@
 results in:
 
 `>>> (0 Sli ) did not want the earpods . (0 He ) didn't like them .`
 
 `>>> (0 Princess Liana ) felt sad , because (1 Zarth Arn ) was gone . (0 The princess) went to sleep .`
 
 
+## Using Coreference Chains
+
+The coreference chains predicted can be accessed using the `.coref_chains` attribute:
+
+```python
+annotated_doc = predict_coref_simple(
+    "Princess Liana felt sad, because Zarth Arn was gone. The princess went to sleep.",
+    model,
+    tokenizer
+)
+print(annotated_doc.coref_chains)
+```
+
+`>>>[[Mention(tokens=['The', 'princess'], start_idx=11, end_idx=13), Mention(tokens=['Princess', 'Liana'], start_idx=0, end_idx=2)], [Mention(tokens=['Zarth', 'Arn'], start_idx=6, end_idx=8)]]`
+
+
 ## Training a model
 
 Aside from the `tibert.train.train_coref_model` function, it is possible to train a model from the command line. Training a model requires installing the `sacred` library. Here is the most basic example:
 
 ```sh
 python -m tibert.run_train with\
        dataset_path=/path/to/litbank/repository\
```

