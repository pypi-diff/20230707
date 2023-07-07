# Comparing `tmp/vecsim-0.0.6.tar.gz` & `tmp/vecsim-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecsim-0.0.6.tar", last modified: Fri Jul  7 16:27:51 2023, max compression
+gzip compressed data, was "vecsim-0.0.61.tar", last modified: Fri Jul  7 16:36:09 2023, max compression
```

## Comparing `vecsim-0.0.6.tar` & `vecsim-0.0.61.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.552754 vecsim-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 16:27:39.000000 vecsim-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-07 16:27:51.552754 vecsim-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-07 16:27:39.000000 vecsim-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:27:51.552754 vecsim-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 16:27:39.000000 vecsim-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.548754 vecsim-0.0.6/vecsim/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 16:27:39.000000 vecsim-0.0.6/vecsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24114 2023-07-07 16:27:39.000000 vecsim-0.0.6/vecsim/similarity_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.552754 vecsim-0.0.6/vecsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:36:09.929467 vecsim-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 16:35:58.000000 vecsim-0.0.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-07 16:36:09.929467 vecsim-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-07 16:35:58.000000 vecsim-0.0.61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:36:09.929467 vecsim-0.0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 16:35:58.000000 vecsim-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:36:09.929467 vecsim-0.0.61/vecsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 16:35:58.000000 vecsim-0.0.61/vecsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24114 2023-07-07 16:35:58.000000 vecsim-0.0.61/vecsim/similarity_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:36:09.929467 vecsim-0.0.61/vecsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-07 16:36:09.000000 vecsim-0.0.61/vecsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 16:36:09.000000 vecsim-0.0.61/vecsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:36:09.000000 vecsim-0.0.61/vecsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 16:36:09.000000 vecsim-0.0.61/vecsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 16:36:09.000000 vecsim-0.0.61/vecsim.egg-info/top_level.txt
```

### Comparing `vecsim-0.0.6/LICENSE` & `vecsim-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `vecsim-0.0.6/PKG-INFO` & `vecsim-0.0.61/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecsim
-Version: 0.0.6
+Version: 0.0.61
 Summary: Vector Similarity Search Engine
 Home-page: https://github.com/argmaxml/vecsim
 Author: ArgmaxML
 Author-email: ugoren@argmax.ml
 Keywords: vector-similarity,faiss,hnsw,redis,matching,ranking,elasticsearch,search,embedding
 Description-Content-Type: text/markdown
 Provides-Extra: faiss
@@ -23,14 +23,15 @@
 1. **Partitions** - In most cases, pre-filtering is needed prior to querying, we abstract this concept away.
 
 ## Supported engines:
 1. Scikit-learn, via [NearestNeighbors](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html)
 1. [RediSearch](https://redis.io/docs/stack/search/reference/vectors/)
 1. [Faiss](https://github.com/facebookresearch/faiss)
 1. [ElasticSearch](https://www.elastic.co)
+1. [Pinecone](https://www.pinecone.io)
 
 
 ## QuickStart example
 ```python
 import numpy as np
 # Import a similarity server of your choice:
 # SKlearn (best for small datasets or testing)
```

### Comparing `vecsim-0.0.6/README.md` & `vecsim-0.0.61/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 1. **Partitions** - In most cases, pre-filtering is needed prior to querying, we abstract this concept away.
 
 ## Supported engines:
 1. Scikit-learn, via [NearestNeighbors](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html)
 1. [RediSearch](https://redis.io/docs/stack/search/reference/vectors/)
 1. [Faiss](https://github.com/facebookresearch/faiss)
 1. [ElasticSearch](https://www.elastic.co)
+1. [Pinecone](https://www.pinecone.io)
 
 
 ## QuickStart example
 ```python
 import numpy as np
 # Import a similarity server of your choice:
 # SKlearn (best for small datasets or testing)
```

### Comparing `vecsim-0.0.6/setup.py` & `vecsim-0.0.61/setup.py`

 * *Files identical despite different names*

### Comparing `vecsim-0.0.6/vecsim/similarity_helpers.py` & `vecsim-0.0.61/vecsim/similarity_helpers.py`

 * *Files identical despite different names*

### Comparing `vecsim-0.0.6/vecsim.egg-info/PKG-INFO` & `vecsim-0.0.61/vecsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecsim
-Version: 0.0.6
+Version: 0.0.61
 Summary: Vector Similarity Search Engine
 Home-page: https://github.com/argmaxml/vecsim
 Author: ArgmaxML
 Author-email: ugoren@argmax.ml
 Keywords: vector-similarity,faiss,hnsw,redis,matching,ranking,elasticsearch,search,embedding
 Description-Content-Type: text/markdown
 Provides-Extra: faiss
@@ -23,14 +23,15 @@
 1. **Partitions** - In most cases, pre-filtering is needed prior to querying, we abstract this concept away.
 
 ## Supported engines:
 1. Scikit-learn, via [NearestNeighbors](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html)
 1. [RediSearch](https://redis.io/docs/stack/search/reference/vectors/)
 1. [Faiss](https://github.com/facebookresearch/faiss)
 1. [ElasticSearch](https://www.elastic.co)
+1. [Pinecone](https://www.pinecone.io)
 
 
 ## QuickStart example
 ```python
 import numpy as np
 # Import a similarity server of your choice:
 # SKlearn (best for small datasets or testing)
```

