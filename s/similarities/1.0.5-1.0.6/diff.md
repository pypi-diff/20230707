# Comparing `tmp/similarities-1.0.5.tar.gz` & `tmp/similarities-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarities-1.0.5.tar", last modified: Mon Apr 17 07:03:40 2023, max compression
+gzip compressed data, was "similarities-1.0.6.tar", last modified: Fri Jul  7 10:30:47 2023, max compression
```

## Comparing `similarities-1.0.5.tar` & `similarities-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.578270 similarities-1.0.5/
--rw-r--r--   0 xuming     (501) staff       (20)    19179 2023-04-17 07:03:40.577900 similarities-1.0.5/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    14874 2023-04-16 03:33:18.000000 similarities-1.0.5/README.md
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-04-17 07:03:40.578392 similarities-1.0.5/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1562 2023-04-16 05:28:26.000000 similarities-1.0.5/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.566375 similarities-1.0.5/similarities/
--rw-r--r--   0 xuming     (501) staff       (20)      836 2022-12-11 03:55:29.000000 similarities-1.0.5/similarities/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6773 2022-03-11 13:33:50.000000 similarities-1.0.5/similarities/clip_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4874 2022-03-10 11:02:09.000000 similarities-1.0.5/similarities/data_loader.py
--rw-r--r--   0 xuming     (501) staff       (20)     6761 2022-03-11 09:18:28.000000 similarities-1.0.5/similarities/evaluation.py
--rw-r--r--   0 xuming     (501) staff       (20)     9577 2023-04-16 07:54:24.000000 similarities-1.0.5/similarities/fastsim.py
--rw-r--r--   0 xuming     (501) staff       (20)    17682 2023-04-16 06:28:41.000000 similarities-1.0.5/similarities/imagesim.py
--rw-r--r--   0 xuming     (501) staff       (20)    35902 2023-04-16 06:28:41.000000 similarities-1.0.5/similarities/literalsim.py
--rw-r--r--   0 xuming     (501) staff       (20)    10201 2023-04-16 06:54:36.000000 similarities-1.0.5/similarities/similarity.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.576458 similarities-1.0.5/similarities/utils/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-16 05:45:19.000000 similarities-1.0.5/similarities/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6929 2023-02-01 07:40:21.000000 similarities-1.0.5/similarities/utils/distance.py
--rw-r--r--   0 xuming     (501) staff       (20)     3010 2022-03-11 08:27:51.000000 similarities-1.0.5/similarities/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)    24585 2022-03-07 06:50:41.000000 similarities-1.0.5/similarities/utils/imagehash.py
--rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 similarities-1.0.5/similarities/utils/rank_bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)     2413 2022-09-26 07:54:49.000000 similarities-1.0.5/similarities/utils/tfidf.py
--rw-r--r--   0 xuming     (501) staff       (20)    11926 2023-04-16 05:28:26.000000 similarities-1.0.5/similarities/utils/util.py
--rw-r--r--   0 xuming     (501) staff       (20)      102 2023-04-16 05:28:26.000000 similarities-1.0.5/similarities/version.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-17 07:03:40.569503 similarities-1.0.5/similarities.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    19179 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      678 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-03-06 17:17:16.000000 similarities-1.0.5/similarities.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       55 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       13 2023-04-17 07:03:40.000000 similarities-1.0.5/similarities.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-07 10:30:47.911756 similarities-1.0.6/
+-rw-r--r--   0 xuming     (501) staff       (20)    19988 2023-07-07 10:30:47.911270 similarities-1.0.6/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    15659 2023-07-07 09:40:35.000000 similarities-1.0.6/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-07-07 10:30:47.911931 similarities-1.0.6/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1562 2023-04-16 05:28:26.000000 similarities-1.0.6/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-07 10:30:47.893770 similarities-1.0.6/similarities/
+-rw-r--r--   0 xuming     (501) staff       (20)      836 2022-12-11 03:55:29.000000 similarities-1.0.6/similarities/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7401 2023-07-07 10:30:14.000000 similarities-1.0.6/similarities/clip_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4874 2023-07-07 09:11:47.000000 similarities-1.0.6/similarities/data_loader.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6757 2023-07-07 09:29:26.000000 similarities-1.0.6/similarities/evaluation.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9572 2023-07-07 09:29:26.000000 similarities-1.0.6/similarities/fastsim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17796 2023-07-07 09:29:26.000000 similarities-1.0.6/similarities/imagesim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    35774 2023-07-07 09:29:26.000000 similarities-1.0.6/similarities/literalsim.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10352 2023-07-07 09:29:26.000000 similarities-1.0.6/similarities/similarity.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-07 10:30:47.909286 similarities-1.0.6/similarities/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-16 05:45:19.000000 similarities-1.0.6/similarities/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6929 2023-02-01 07:40:21.000000 similarities-1.0.6/similarities/utils/distance.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3010 2022-03-11 08:27:51.000000 similarities-1.0.6/similarities/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)    24585 2022-03-07 06:50:41.000000 similarities-1.0.6/similarities/utils/imagehash.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 similarities-1.0.6/similarities/utils/rank_bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2413 2022-09-26 07:54:49.000000 similarities-1.0.6/similarities/utils/tfidf.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11926 2023-04-16 05:28:26.000000 similarities-1.0.6/similarities/utils/util.py
+-rw-r--r--   0 xuming     (501) staff       (20)      102 2023-07-07 09:38:00.000000 similarities-1.0.6/similarities/version.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-07 10:30:47.898249 similarities-1.0.6/similarities.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    19988 2023-07-07 10:30:47.000000 similarities-1.0.6/similarities.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      678 2023-07-07 10:30:47.000000 similarities-1.0.6/similarities.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-07 10:30:47.000000 similarities-1.0.6/similarities.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-03-06 17:17:16.000000 similarities-1.0.6/similarities.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       55 2023-07-07 10:30:47.000000 similarities-1.0.6/similarities.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       13 2023-07-07 10:30:47.000000 similarities-1.0.6/similarities.egg-info/top_level.txt
```

### Comparing `similarities-1.0.5/PKG-INFO` & `similarities-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarities
-Version: 1.0.5
+Version: 1.0.6
 Summary: Similarities is a toolkit for compute similarity scores between two sets of strings.
 Home-page: https://github.com/shibing624/similarities
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [![PyPI version](https://badge.fury.io/py/similarities.svg)](https://badge.fury.io/py/similarities)
         [![Downloads](https://pepy.tech/badge/similarities)](https://pepy.tech/project/similarities)
@@ -114,14 +114,17 @@
         python3 setup.py install
         ```
         
         # Usage
         
         ### 1. 文本语义相似度计算
         
+        example: [examples/text_similarity_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_similarity_demo.py)
+        
+        
         ```python
         from similarities import Similarity
         
         m = Similarity()
         r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
         print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
         ```
@@ -129,27 +132,24 @@
         Similarity的默认方法：
         ```python
         Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
                    model_name_or_path="shibing624/text2vec-base-chinese",
                    max_seq_length=128)
         ```
         
-        > 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
-        
-        > corpus表示：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
-        
-        > model_name_or_path表示：模型名称或者模型路径，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
-        
-        > max_seq_length表示：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
+        - 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
+        - `corpus`：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
+        - `model_name_or_path`：模型名称或者模型路径，默认会从HF model hub下载并使用中文语义匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，如果是多语言景，可以替换为多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)
+        - `max_seq_length`：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
         
         ### 2. 文本语义匹配搜索
         
         一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
         
-        example: [examples/base_demo.py](./examples/base_demo.py)
+        example: [examples/text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
         from similarities import Similarity
         
@@ -214,29 +214,31 @@
         	我什么时候开通了花呗: 0.7212
         	中央情报局局长访问以色列叙利亚会谈: 0.2517
         ```
         
         > 余弦`score`的值范围[-1, 1]，值越大，表示该query与corpus的文本越相似。
         
         
-        #### 英文语义相似度计算和匹配搜索
+        #### 多语言文本语义相似度计算和匹配搜索
+        
+        多语言：包括中、英、韩、日、德、意等多国语言
         
-        example: [examples/base_english_demo.py](./examples/base_english_demo.py)
+        example: [examples/text_semantic_search_multilingual_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_multilingual_demo.py)
         
-        ### 3. 快速近似语义匹配搜索
+        ### 3. 快速近似文本语义匹配搜索
         
         支持Annoy、Hnswlib的近似语义匹配搜索，常用于百万数据集的匹配搜索任务。
         
-        example: [examples/fast_sim_demo.py](./examples/fast_sim_demo.py)
+        example: [examples/fast_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/fast_text_semantic_search_demo.py)
         
         ### 4. 基于字面的文本相似度计算和匹配搜索
         
         支持同义词词林（Cilin）、知网Hownet、词向量（WordEmbedding）、Tfidf、SimHash、BM25等算法的相似度计算和字面匹配搜索，常用于文本匹配冷启动。
         
-        example: [examples/literal_sim_demo.py](./examples/literal_sim_demo.py)
+        example: [examples/literal_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/literal_text_semantic_search_demo.py)
         
         ```python
         from similarities.literalsim import SimHashSimilarity, TfidfSimilarity, BM25Similarity, \
             WordEmbeddingSimilarity, CilinSimilarity, HownetSimilarity
         
         text1 = "如何更换花呗绑定银行卡"
         text2 = "花呗更改绑定银行卡"
@@ -281,15 +283,15 @@
         ...
         ```
         
         ### 5. 图像相似度计算和匹配搜索
         
         支持[CLIP](similarities/imagesim.py)、pHash、SIFT等算法的图像相似度计算和匹配搜索。
         
-        example: [examples/image_demo.py](./examples/image_demo.py)
+        example: [examples/image_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/image_semantic_search_demo.py)
         
         ```python
         import sys
         import glob
         from PIL import Image
         
         sys.path.append('..')
@@ -348,15 +350,15 @@
         	data/image8-like-image1.png: 0.9327
         ```
         
         ![image_sim](docs/image_sim.png)
         
         ### 6. 图文互搜
         
-        CLIP 模型不仅支持以图搜图，还支持图文互搜：
+        CLIP 模型不仅支持以图搜图，还支持中英文图文互搜：
         ```python
         import sys
         import glob
         from PIL import Image
         sys.path.append('..')
         from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
         
@@ -431,14 +433,15 @@
         
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [liuhuanyong/SentenceSimilarity](https://github.com/liuhuanyong/SentenceSimilarity)
         - [shibing624/text2vec](https://github.com/shibing624/text2vec)
         - [qwertyforce/image_search](https://github.com/qwertyforce/image_search)
         - [ImageHash - Official Github repository](https://github.com/JohannesBuchner/imagehash)
         - [openai/CLIP](https://github.com/openai/CLIP)
+        
 Keywords: similarities,Chinese Text Similarity Calculation Tool,similarity,word2vec
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `similarities-1.0.5/README.md` & `similarities-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,17 @@
 python3 setup.py install
 ```
 
 # Usage
 
 ### 1. 文本语义相似度计算
 
+example: [examples/text_similarity_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_similarity_demo.py)
+
+
 ```python
 from similarities import Similarity
 
 m = Similarity()
 r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
 print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
 ```
@@ -121,27 +124,24 @@
 Similarity的默认方法：
 ```python
 Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
            model_name_or_path="shibing624/text2vec-base-chinese",
            max_seq_length=128)
 ```
 
-> 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
-
-> corpus表示：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
-
-> model_name_or_path表示：模型名称或者模型路径，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
-
-> max_seq_length表示：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
+- 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
+- `corpus`：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
+- `model_name_or_path`：模型名称或者模型路径，默认会从HF model hub下载并使用中文语义匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，如果是多语言景，可以替换为多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)
+- `max_seq_length`：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
 
 ### 2. 文本语义匹配搜索
 
 一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
 
-example: [examples/base_demo.py](./examples/base_demo.py)
+example: [examples/text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
 from similarities import Similarity
 
@@ -206,29 +206,31 @@
 	我什么时候开通了花呗: 0.7212
 	中央情报局局长访问以色列叙利亚会谈: 0.2517
 ```
 
 > 余弦`score`的值范围[-1, 1]，值越大，表示该query与corpus的文本越相似。
 
 
-#### 英文语义相似度计算和匹配搜索
+#### 多语言文本语义相似度计算和匹配搜索
+
+多语言：包括中、英、韩、日、德、意等多国语言
 
-example: [examples/base_english_demo.py](./examples/base_english_demo.py)
+example: [examples/text_semantic_search_multilingual_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_multilingual_demo.py)
 
-### 3. 快速近似语义匹配搜索
+### 3. 快速近似文本语义匹配搜索
 
 支持Annoy、Hnswlib的近似语义匹配搜索，常用于百万数据集的匹配搜索任务。
 
-example: [examples/fast_sim_demo.py](./examples/fast_sim_demo.py)
+example: [examples/fast_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/fast_text_semantic_search_demo.py)
 
 ### 4. 基于字面的文本相似度计算和匹配搜索
 
 支持同义词词林（Cilin）、知网Hownet、词向量（WordEmbedding）、Tfidf、SimHash、BM25等算法的相似度计算和字面匹配搜索，常用于文本匹配冷启动。
 
-example: [examples/literal_sim_demo.py](./examples/literal_sim_demo.py)
+example: [examples/literal_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/literal_text_semantic_search_demo.py)
 
 ```python
 from similarities.literalsim import SimHashSimilarity, TfidfSimilarity, BM25Similarity, \
     WordEmbeddingSimilarity, CilinSimilarity, HownetSimilarity
 
 text1 = "如何更换花呗绑定银行卡"
 text2 = "花呗更改绑定银行卡"
@@ -273,15 +275,15 @@
 ...
 ```
 
 ### 5. 图像相似度计算和匹配搜索
 
 支持[CLIP](similarities/imagesim.py)、pHash、SIFT等算法的图像相似度计算和匹配搜索。
 
-example: [examples/image_demo.py](./examples/image_demo.py)
+example: [examples/image_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/image_semantic_search_demo.py)
 
 ```python
 import sys
 import glob
 from PIL import Image
 
 sys.path.append('..')
@@ -340,15 +342,15 @@
 	data/image8-like-image1.png: 0.9327
 ```
 
 ![image_sim](docs/image_sim.png)
 
 ### 6. 图文互搜
 
-CLIP 模型不仅支持以图搜图，还支持图文互搜：
+CLIP 模型不仅支持以图搜图，还支持中英文图文互搜：
 ```python
 import sys
 import glob
 from PIL import Image
 sys.path.append('..')
 from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
 
@@ -422,8 +424,8 @@
 # Reference
 
 - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
 - [liuhuanyong/SentenceSimilarity](https://github.com/liuhuanyong/SentenceSimilarity)
 - [shibing624/text2vec](https://github.com/shibing624/text2vec)
 - [qwertyforce/image_search](https://github.com/qwertyforce/image_search)
 - [ImageHash - Official Github repository](https://github.com/JohannesBuchner/imagehash)
-- [openai/CLIP](https://github.com/openai/CLIP)
+- [openai/CLIP](https://github.com/openai/CLIP)
```

### Comparing `similarities-1.0.5/setup.py` & `similarities-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/__init__.py` & `similarities-1.0.6/similarities/__init__.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/clip_model.py` & `similarities-1.0.6/similarities/clip_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: CLIP model for text and image embeddings
-model url: https://huggingface.co/openai/clip-vit-base-patch32
 """
 from typing import List, Union
 
 import numpy as np
 import torch
 import torch.nn.functional
-import transformers
 from PIL import Image
 from torch import nn
 from tqdm import trange
+from transformers import ChineseCLIPProcessor, ChineseCLIPModel, CLIPProcessor, CLIPModel
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 class CLIPModel(nn.Module):
-    def __init__(self, model_name: str = "openai/clip-vit-base-patch32", processor_name=None):
-        super(CLIPModel, self).__init__()
+    """
+    CLIP model for text and image embeddings
+
+    Args:
+        model_name: str, default "OFA-Sys/chinese-clip-vit-base-patch16"
+            chinese model url: https://huggingface.co/OFA-Sys/chinese-clip-vit-base-patch16
+            english model url: https://huggingface.co/openai/clip-vit-base-patch32
+        processor_name: str, default None
+    """
 
+    def __init__(self, model_name: str = "OFA-Sys/chinese-clip-vit-base-patch16", processor_name=None):
+        super(CLIPModel, self).__init__()
+        self.model_name = model_name
         if processor_name is None:
             processor_name = model_name
-
-        self.model = transformers.CLIPModel.from_pretrained(model_name)
-        self.processor = transformers.CLIPProcessor.from_pretrained(processor_name)
+        if 'chinese' in model_name:
+            self.processor = ChineseCLIPProcessor.from_pretrained(processor_name)
+            self.model = ChineseCLIPModel.from_pretrained(model_name)
+        else:
+            self.model = CLIPModel.from_pretrained(model_name)
+            self.processor = CLIPProcessor.from_pretrained(processor_name)
 
     def __str__(self):
-        return f"CLIPModel({self.model})"
+        return f"model_name: {self.model_name} CLIPModel({self.model})"
 
     def forward(self, features):
         image_embeds = []
         text_embeds = []
 
         if 'pixel_values' in features:
             vision_outputs = self.model.vision_model(pixel_values=features['pixel_values'])
```

### Comparing `similarities-1.0.5/similarities/data_loader.py` & `similarities-1.0.6/similarities/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 refer: https://github.com/UKPLab/beir/blob/main/beir/datasets/data_loader.py
 """
-from typing import Dict, Tuple
-from tqdm.autonotebook import tqdm
+import csv
 import json
 import os
-import csv
+from typing import Dict, Tuple
+
 from loguru import logger
+from tqdm.autonotebook import tqdm
 
 
 class SearchDataLoader:
 
     def __init__(self, data_folder: str = None, prefix: str = None, corpus_file: str = "corpus.jsonl",
                  query_file: str = "queries.jsonl",
                  qrels_folder: str = "qrels", qrels_file: str = ""):
@@ -40,15 +41,15 @@
         self.check(fIn=self.corpus_file, ext="jsonl")
         self.check(fIn=self.query_file, ext="jsonl")
         self.check(fIn=self.qrels_file, ext="tsv")
 
         if not len(self.corpus):
             logger.info("Loading Corpus...")
             self._load_corpus()
-            logger.info(f"Loaded {len(self.corpus)} Documents." )
+            logger.info(f"Loaded {len(self.corpus)} Documents.")
             logger.info(f"Doc Example: {list(self.corpus.values())[0]}")
 
         if not len(self.queries):
             logger.info("Loading Queries...")
             self._load_queries()
 
         if os.path.exists(self.qrels_file):
```

### Comparing `similarities-1.0.5/similarities/evaluation.py` & `similarities-1.0.6/similarities/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
 
     return top_k_acc
 
 
 def evaluate(
         qrels: Dict[str, Dict[str, int]],
         results: Dict[str, Dict[str, float]],
-        k_values: List[int] = (1, 3, 5, 10, 100)) -> Tuple[
-    Dict[str, float], Dict[str, float], Dict[str, float], Dict[str, float]]:
+        k_values: List[int] = (1, 3, 5, 10, 100)
+) -> Tuple[Dict[str, float], Dict[str, float], Dict[str, float], Dict[str, float]]:
     try:
         import pytrec_eval
     except ImportError:
         raise ImportError("Please install pytrec_eval to use this function, eg. `pip install pytrec_eval`")
 
     ndcg = {}
     _map = {}
```

### Comparing `similarities-1.0.5/similarities/fastsim.py` & `similarities-1.0.6/similarities/fastsim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
 """
-from typing import List, Union, Tuple, Dict
 import os
+from typing import List, Union, Dict
+
 from loguru import logger
+
 from similarities.similarity import Similarity
 
 
 class AnnoySimilarity(Similarity):
     """
     Computes cosine similarities between word embeddings and retrieves most
     similar query for a given docs with Annoy.
```

### Comparing `similarities-1.0.5/similarities/imagesim.py` & `similarities-1.0.6/similarities/imagesim.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 
 class ClipSimilarity(SimilarityABC):
     """
     Compute CLIP similarity between two images and retrieves most
     similar image for a given image corpus.
 
     CLIP: https://github.com/openai/CLIP.git
+    english model: openai/clip-vit-base-patch32
+    chinese model: OFA-Sys/chinese-clip-vit-base-patch16
     """
 
     def __init__(
             self,
             corpus: Union[List[Image.Image], Dict[str, Image.Image]] = None,
-            model_name_or_path='openai/clip-vit-base-patch32'
+            model_name_or_path='OFA-Sys/chinese-clip-vit-base-patch16'
     ):
         self.clip_model = CLIPModel(model_name_or_path)  # load the CLIP model
         self.score_functions = {'cos_sim': cos_sim, 'dot': dot_score}
         self.corpus = {}
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
```

### Comparing `similarities-1.0.5/similarities/literalsim.py` & `similarities-1.0.6/similarities/literalsim.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from typing import List, Union, Dict
 
 import jieba
 import jieba.analyse
 import jieba.posseg
 import numpy as np
 from loguru import logger
-from tqdm import tqdm
 from text2vec import Word2Vec
+from tqdm import tqdm
 
 from similarities.similarity import SimilarityABC
 from similarities.utils.distance import string_hash, hamming_distance, longest_match_size
 from similarities.utils.rank_bm25 import BM25Okapi
 from similarities.utils.tfidf import TFIDF, load_stopwords, default_stopwords_file
 from similarities.utils.util import cos_sim, semantic_search
 
@@ -32,15 +32,15 @@
     """
     Compute SimHash similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         self.corpus = {}
-        
+
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
@@ -67,15 +67,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = []
         for sentence in tqdm(corpus_texts, desc="Computing corpus SimHash"):
             corpus_embeddings.append(self.simhash(sentence))
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
@@ -194,15 +194,15 @@
     Compute TFIDF similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        
+
         self.corpus_embeddings = []
         self.tfidf = TFIDF()
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
@@ -230,15 +230,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = []
         for sentence in tqdm(corpus_texts, desc="Computing corpus TFIDF"):
             corpus_embeddings.append(self.tfidf.get_tfidf(sentence))
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
@@ -290,15 +290,15 @@
     Compute BM25OKapi similarity between two sentences and retrieves most
     similar sentence for a given corpus.
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        
+
         self.bm25 = None
         self.default_stopwords = load_stopwords(default_stopwords_file)
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
@@ -326,15 +326,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_seg = [jieba.lcut(d) for d in corpus_texts]
         corpus_seg = [[w for w in doc if (w.strip().lower() not in self.default_stopwords) and
                        len(w.strip()) > 0] for doc in corpus_seg]
         self.bm25 = BM25Okapi(corpus_seg)
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
@@ -381,15 +381,15 @@
         if isinstance(model_name_or_path, str):
             self.keyedvectors = Word2Vec(model_name_or_path)
         elif hasattr(model_name_or_path, "encode"):
             self.keyedvectors = model_name_or_path
         else:
             raise ValueError("model_name_or_path must be ~text2vec.Word2Vec or Word2Vec model name")
         self.corpus = {}
-        
+
         self.corpus_embeddings = []
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
@@ -416,15 +416,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start computing corpus embeddings, new docs: {len(corpus_new)}")
         corpus_texts = list(corpus_new.values())
         corpus_embeddings = self._get_vector(corpus_texts, show_progress_bar=True).tolist()
         if self.corpus_embeddings:
             self.corpus_embeddings += corpus_embeddings
         else:
             self.corpus_embeddings = corpus_embeddings
@@ -475,15 +475,15 @@
     """
     default_cilin_path = os.path.join(pwd_path, 'data/cilin.txt')
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None, cilin_path: str = default_cilin_path):
         super().__init__()
         self.cilin_dict = self.load_cilin_dict(cilin_path)  # Cilin(词林) semantic dictionary
         self.corpus = {}
-        
+
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -509,15 +509,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     @staticmethod
     def load_cilin_dict(path):
         """加载词林语义词典"""
         sem_dict = {}
@@ -632,15 +632,15 @@
     similar sentence for a given corpus.
     """
     default_hownet_path = os.path.join(pwd_path, 'data/hownet.txt')
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None, hownet_path: str = default_hownet_path):
         self.hownet_dict = self.load_hownet_dict(hownet_path)  # semantic dictionary
         self.corpus = {}
-        
+
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -666,15 +666,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     @staticmethod
     def load_hownet_dict(path):
         """加载Hownet语义词典"""
         hownet_dict = {}
@@ -762,15 +762,15 @@
     similar sentence for a given corpus.
     不考虑文本字符位置顺序，基于相同字符数占比计算相似度
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        
+
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -796,15 +796,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     def similarity(self, a: Union[str, List[str]], b: Union[str, List[str]]):
         """
         Compute Chars similarity between two texts.
         :param a:
@@ -858,15 +858,15 @@
     similar sentence for a given corpus.
     考虑文本字符位置顺序，基于最长公共子串占比计算相似度
     """
 
     def __init__(self, corpus: Union[List[str], Dict[str, str]] = None):
         super().__init__()
         self.corpus = {}
-        
+
         if corpus is not None:
             self.add_corpus(corpus)
 
     def __len__(self):
         """Get length of corpus."""
         return len(self.corpus)
 
@@ -892,15 +892,15 @@
                 if doc not in list(self.corpus.values()):
                     corpus_new[start_id + id] = doc
         else:
             for id, doc in corpus.items():
                 if doc not in list(self.corpus.values()):
                     corpus_new[id] = doc
         self.corpus.update(corpus_new)
-        
+
         logger.info(f"Start add new docs: {len(corpus_new)}")
         logger.info(f"Add {len(corpus)} docs, total: {len(self.corpus)}")
 
     def similarity(self, a: Union[str, List[str]], b: Union[str, List[str]],
                    min_same_len: int = 70, min_same_len_score: float = 0.9):
         """
         Compute Chars similarity between two texts.
```

### Comparing `similarities-1.0.5/similarities/similarity.py` & `similarities-1.0.6/similarities/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 @description:
 
 Compute similarity:
 1. Compute the similarity between two sentences
 2. Retrieves most similar sentence of a query against a corpus of documents.
 """
 
-import os
 import json
+import os
 from typing import List, Union, Dict
 
 import numpy as np
 from loguru import logger
 from text2vec import SentenceModel
 
 from similarities.utils.util import cos_sim, semantic_search, dot_score
@@ -73,28 +73,35 @@
 
     The index supports adding new documents dynamically.
     """
 
     def __init__(
             self,
             corpus: Union[List[str], Dict[str, str]] = None,
-            model_name_or_path="sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
+            model_name_or_path="shibing624/text2vec-base-chinese",
+            encoder_type="MEAN",
             max_seq_length=128,
+            device=None,
     ):
         """
         Initialize the similarity object.
         :param model_name_or_path: Transformer model name or path, like:
             'sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2', 'bert-base-uncased', 'bert-base-chinese',
              'shibing624/text2vec-base-chinese', ...
             model in HuggingFace Model Hub and release from https://github.com/shibing624/text2vec
         :param corpus: Corpus of documents to use for similarity queries.
         :param max_seq_length: Max sequence length for sentence model.
         """
         if isinstance(model_name_or_path, str):
-            self.sentence_model = SentenceModel(model_name_or_path, max_seq_length=max_seq_length)
+            self.sentence_model = SentenceModel(
+                model_name_or_path,
+                encoder_type=encoder_type,
+                max_seq_length=max_seq_length,
+                device=device
+            )
         elif hasattr(model_name_or_path, "encode"):
             self.sentence_model = model_name_or_path
         else:
             raise ValueError("model_name_or_path is transformers model name or path")
         self.score_functions = {'cos_sim': cos_sim, 'dot': dot_score}
         self.corpus = {}
         self.corpus_embeddings = []
```

### Comparing `similarities-1.0.5/similarities/utils/distance.py` & `similarities-1.0.6/similarities/utils/distance.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/utils/get_file.py` & `similarities-1.0.6/similarities/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/utils/imagehash.py` & `similarities-1.0.6/similarities/utils/imagehash.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/utils/rank_bm25.py` & `similarities-1.0.6/similarities/utils/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/utils/tfidf.py` & `similarities-1.0.6/similarities/utils/tfidf.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities/utils/util.py` & `similarities-1.0.6/similarities/utils/util.py`

 * *Files identical despite different names*

### Comparing `similarities-1.0.5/similarities.egg-info/PKG-INFO` & `similarities-1.0.6/similarities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarities
-Version: 1.0.5
+Version: 1.0.6
 Summary: Similarities is a toolkit for compute similarity scores between two sets of strings.
 Home-page: https://github.com/shibing624/similarities
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [![PyPI version](https://badge.fury.io/py/similarities.svg)](https://badge.fury.io/py/similarities)
         [![Downloads](https://pepy.tech/badge/similarities)](https://pepy.tech/project/similarities)
@@ -114,14 +114,17 @@
         python3 setup.py install
         ```
         
         # Usage
         
         ### 1. 文本语义相似度计算
         
+        example: [examples/text_similarity_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_similarity_demo.py)
+        
+        
         ```python
         from similarities import Similarity
         
         m = Similarity()
         r = m.similarity('如何更换花呗绑定银行卡', '花呗更改绑定银行卡')
         print(f"similarity score: {float(r)}")  # similarity score: 0.855146050453186
         ```
@@ -129,27 +132,24 @@
         Similarity的默认方法：
         ```python
         Similarity(corpus: Union[List[str], Dict[str, str]] = None, 
                    model_name_or_path="shibing624/text2vec-base-chinese",
                    max_seq_length=128)
         ```
         
-        > 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
-        
-        > corpus表示：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
-        
-        > model_name_or_path表示：模型名称或者模型路径，默认使用中文表征式匹配模型`shibing624/text2vec-base-chinese`，可以替换为多语言表征模型`sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
-        
-        > max_seq_length表示：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
+        - 返回值：余弦值`score`范围是[-1, 1]，值越大越相似
+        - `corpus`：搜索用的doc集，仅搜索时需要，输入格式：句子列表`List[str]`或者{corpus_id: sentence}的`Dict[str, str]`格式
+        - `model_name_or_path`：模型名称或者模型路径，默认会从HF model hub下载并使用中文语义匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，如果是多语言景，可以替换为多语言匹配模型[shibing624/text2vec-base-multilingual](https://huggingface.co/shibing624/text2vec-base-multilingual)
+        - `max_seq_length`：输入句子的最大长度，最大为匹配模型支持的最大长度，BERT系列是512
         
         ### 2. 文本语义匹配搜索
         
         一般在文档候选集中找与query最相似的文本，常用于QA场景的问句相似匹配、文本相似检索等任务。
         
-        example: [examples/base_demo.py](./examples/base_demo.py)
+        example: [examples/text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
         from similarities import Similarity
         
@@ -214,29 +214,31 @@
         	我什么时候开通了花呗: 0.7212
         	中央情报局局长访问以色列叙利亚会谈: 0.2517
         ```
         
         > 余弦`score`的值范围[-1, 1]，值越大，表示该query与corpus的文本越相似。
         
         
-        #### 英文语义相似度计算和匹配搜索
+        #### 多语言文本语义相似度计算和匹配搜索
+        
+        多语言：包括中、英、韩、日、德、意等多国语言
         
-        example: [examples/base_english_demo.py](./examples/base_english_demo.py)
+        example: [examples/text_semantic_search_multilingual_demo.py](https://github.com/shibing624/similarities/blob/main/examples/text_semantic_search_multilingual_demo.py)
         
-        ### 3. 快速近似语义匹配搜索
+        ### 3. 快速近似文本语义匹配搜索
         
         支持Annoy、Hnswlib的近似语义匹配搜索，常用于百万数据集的匹配搜索任务。
         
-        example: [examples/fast_sim_demo.py](./examples/fast_sim_demo.py)
+        example: [examples/fast_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/fast_text_semantic_search_demo.py)
         
         ### 4. 基于字面的文本相似度计算和匹配搜索
         
         支持同义词词林（Cilin）、知网Hownet、词向量（WordEmbedding）、Tfidf、SimHash、BM25等算法的相似度计算和字面匹配搜索，常用于文本匹配冷启动。
         
-        example: [examples/literal_sim_demo.py](./examples/literal_sim_demo.py)
+        example: [examples/literal_text_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/literal_text_semantic_search_demo.py)
         
         ```python
         from similarities.literalsim import SimHashSimilarity, TfidfSimilarity, BM25Similarity, \
             WordEmbeddingSimilarity, CilinSimilarity, HownetSimilarity
         
         text1 = "如何更换花呗绑定银行卡"
         text2 = "花呗更改绑定银行卡"
@@ -281,15 +283,15 @@
         ...
         ```
         
         ### 5. 图像相似度计算和匹配搜索
         
         支持[CLIP](similarities/imagesim.py)、pHash、SIFT等算法的图像相似度计算和匹配搜索。
         
-        example: [examples/image_demo.py](./examples/image_demo.py)
+        example: [examples/image_semantic_search_demo.py](https://github.com/shibing624/similarities/blob/main/examples/image_semantic_search_demo.py)
         
         ```python
         import sys
         import glob
         from PIL import Image
         
         sys.path.append('..')
@@ -348,15 +350,15 @@
         	data/image8-like-image1.png: 0.9327
         ```
         
         ![image_sim](docs/image_sim.png)
         
         ### 6. 图文互搜
         
-        CLIP 模型不仅支持以图搜图，还支持图文互搜：
+        CLIP 模型不仅支持以图搜图，还支持中英文图文互搜：
         ```python
         import sys
         import glob
         from PIL import Image
         sys.path.append('..')
         from similarities.imagesim import ImageHashSimilarity, SiftSimilarity, ClipSimilarity
         
@@ -431,14 +433,15 @@
         
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [liuhuanyong/SentenceSimilarity](https://github.com/liuhuanyong/SentenceSimilarity)
         - [shibing624/text2vec](https://github.com/shibing624/text2vec)
         - [qwertyforce/image_search](https://github.com/qwertyforce/image_search)
         - [ImageHash - Official Github repository](https://github.com/JohannesBuchner/imagehash)
         - [openai/CLIP](https://github.com/openai/CLIP)
+        
 Keywords: similarities,Chinese Text Similarity Calculation Tool,similarity,word2vec
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `similarities-1.0.5/similarities.egg-info/SOURCES.txt` & `similarities-1.0.6/similarities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

