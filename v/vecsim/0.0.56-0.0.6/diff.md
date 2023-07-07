# Comparing `tmp/vecsim-0.0.56.tar.gz` & `tmp/vecsim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecsim-0.0.56.tar", last modified: Sun Feb 12 13:25:19 2023, max compression
+gzip compressed data, was "vecsim-0.0.6.tar", last modified: Fri Jul  7 16:27:51 2023, max compression
```

## Comparing `vecsim-0.0.56.tar` & `vecsim-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 13:25:19.226996 vecsim-0.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-12 13:25:05.000000 vecsim-0.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-12 13:25:19.226996 vecsim-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-12 13:25:05.000000 vecsim-0.0.56/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 13:25:19.226996 vecsim-0.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-12 13:25:05.000000 vecsim-0.0.56/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 13:25:19.226996 vecsim-0.0.56/vecsim/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-12 13:25:05.000000 vecsim-0.0.56/vecsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20637 2023-02-12 13:25:05.000000 vecsim-0.0.56/vecsim/similarity_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 13:25:19.226996 vecsim-0.0.56/vecsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-12 13:25:19.000000 vecsim-0.0.56/vecsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-12 13:25:19.000000 vecsim-0.0.56/vecsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 13:25:19.000000 vecsim-0.0.56/vecsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-12 13:25:19.000000 vecsim-0.0.56/vecsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-12 13:25:19.000000 vecsim-0.0.56/vecsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.552754 vecsim-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 16:27:39.000000 vecsim-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-07 16:27:51.552754 vecsim-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-07 16:27:39.000000 vecsim-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:27:51.552754 vecsim-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 16:27:39.000000 vecsim-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.548754 vecsim-0.0.6/vecsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 16:27:39.000000 vecsim-0.0.6/vecsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24114 2023-07-07 16:27:39.000000 vecsim-0.0.6/vecsim/similarity_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:27:51.552754 vecsim-0.0.6/vecsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 16:27:51.000000 vecsim-0.0.6/vecsim.egg-info/top_level.txt
```

### Comparing `vecsim-0.0.56/LICENSE` & `vecsim-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vecsim-0.0.56/PKG-INFO` & `vecsim-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vecsim
-Version: 0.0.56
+Version: 0.0.6
 Summary: Vector Similarity Search Engine
 Home-page: https://github.com/argmaxml/vecsim
 Author: ArgmaxML
 Author-email: ugoren@argmax.ml
 Keywords: vector-similarity,faiss,hnsw,redis,matching,ranking,elasticsearch,search,embedding
 Description-Content-Type: text/markdown
 Provides-Extra: faiss
 Provides-Extra: redis
 Provides-Extra: elasticsearch
+Provides-Extra: pinecone
 Provides-Extra: postgres
 License-File: LICENSE
 
 # VecSim - A unified interface for similarity servers
 A standard, light-weight interface to all popular similarity servers.
 
 ## The problems we are trying to solve:
```

### Comparing `vecsim-0.0.56/README.md` & `vecsim-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vecsim-0.0.56/setup.py` & `vecsim-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,11 +26,12 @@
     url='https://github.com/argmaxml/vecsim',
     keywords=['vector-similarity','faiss','hnsw','redis','matching','ranking','elasticsearch','search','embedding'],
     classifiers=[],
     extras_require = {
         'faiss': ['faiss-cpu>=1.7.1'],
         'redis': ['redis>=4.3.0'],
         'elasticsearch': ['elasticsearch>=8.5.0'],
+        'pinecone': ['pinecone-client>=2.2.0'],
         'postgres': ['psycopg2-binary~=2.9.3',"SQLAlchemy~=1.3.22"],
 
     }
 )
```

### Comparing `vecsim-0.0.56/vecsim/similarity_helpers.py` & `vecsim-0.0.6/vecsim/similarity_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import sys, json
 from typing import Dict
 import numpy as np
 import collections
+import itertools
 from sklearn.neighbors import NearestNeighbors
 available_engines = {"sklearn"}
 try:
     import faiss
     available_engines.add("faiss")
 except Exception:
     faiss = None
 try:
+    import pinecone
+    available_engines.add("pinecone")
+except Exception:
+    pinecone = None
+try:
     from redis import Redis
     from redis.commands.search.field import VectorField
     from redis.commands.search.field import TextField
     from redis.commands.search.field import TagField
     from redis.commands.search.query import Query
     from redis.commands.search.result import Result
     available_engines.add("redis")
@@ -513,8 +519,95 @@
         self.indices = collections.defaultdict(lambda:self.cls(**self.cls_args))
 
 class FaissIVFPQIndex(BaseIndex):
     def __init__(self, metric:str, dim:int, **kwargs):
         BaseIndex.__init__(self, metric, dim)
         self.cls = FaissIVFPQIndexUnpartitioned
         self.cls_args={"metric":self.metric,"dim":self.dim}
-        self.indices = collections.defaultdict(lambda:self.cls(**self.cls_args))
+        self.indices = collections.defaultdict(lambda:self.cls(**self.cls_args))
+
+## Pinecone
+class PineconeIndex(BaseIndex):
+    def __init__(self, metric:str, dim:int, pinecone_credentials, index_name="vecsim",**kwargs):
+        self.index_name = index_name
+        self.partitions = set()
+        if metric == "cosine":
+            metric = 'cosine'
+        elif metric in ['ip', 'dot']:
+            metric = 'dotproduct'
+        elif metric == 'l2':
+            metric = 'euclidean'
+        else:
+            raise TypeError(str(metric) + " is not supported")
+        pinecone.init(**pinecone_credentials)
+        try:
+            pinecone.describe_index(index_name)
+        except:
+            pinecone.create_index(index_name, dimension=dim, metric=metric, **kwargs)
+        self.index = pinecone.Index(index_name)
+
+    def _get_data_chunks(self, iterable, batch_size=100):
+        """A helper function to break an iterable into chunks of size batch_size."""
+        it = iter(iterable)
+        chunk = tuple(itertools.islice(it, batch_size))
+        while chunk:
+            yield chunk
+            chunk = tuple(itertools.islice(it, batch_size))
+
+    def add_items(self, data, ids, partition=None):
+        # Support for adding items to multiple partitions
+        if type(partition)==np.str_:
+            partition = str(partition)
+        if hasattr(partition, "__iter__") and type(partition)!=str:
+            data = np.array(data)
+            ids = np.array(ids)
+            ps = set(partition)
+            partition = np.array(partition)
+            for p in ps:
+                self.add_items(data[partition==p], ids[partition==p], p)
+            return
+        self.partitions.add(partition)
+        if partition is not None:
+            data_generator = map(lambda i: (
+                ids[i], 
+                [float(item) for item in data[i]],
+                {"partition": partition}
+                ), range(len(ids)))
+        else:
+            data_generator = map(lambda i: (
+                            str(ids[i]), 
+                            [float(item) for item in data[i]]
+                            ), range(len(ids)))
+            
+        for ids_vectors_chunk in self._get_data_chunks(data_generator, batch_size=100):
+            self.index.upsert(vectors=list(ids_vectors_chunk))
+
+    
+    def search(self, data, k=1,partition=None):
+        if partition is not None and partition not in self.partitions:
+            raise Exception(f"Partition {partition} does not exist")
+        query_args = {
+            "vector": [float(i) for i in data],
+            "top_k": k,
+        }
+        if partition:
+            query_args["filter"] = {"partition": {"$eq": partition}}
+        response = self.index.query(**query_args)
+        matches = response['matches']
+        ids = [x["id"] for x in matches]
+        scores = [x["score"] for x in matches]
+        return scores, ids
+    
+    def get_items(self, ids):
+        """Get items by id"""
+        if not isinstance(ids, list):
+            ids = [ids]
+        res = self.index.fetch(ids)
+        return [np.array(res['vectors'][x]["values"]) for x in res['vectors'].keys()]
+
+    def get_current_count(self):
+        """Get number of items in index"""
+        index_stats = self.index.describe_index_stats()
+        return index_stats['total_vector_count']
+    
+
+
```

### Comparing `vecsim-0.0.56/vecsim.egg-info/PKG-INFO` & `vecsim-0.0.6/vecsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vecsim
-Version: 0.0.56
+Version: 0.0.6
 Summary: Vector Similarity Search Engine
 Home-page: https://github.com/argmaxml/vecsim
 Author: ArgmaxML
 Author-email: ugoren@argmax.ml
 Keywords: vector-similarity,faiss,hnsw,redis,matching,ranking,elasticsearch,search,embedding
 Description-Content-Type: text/markdown
 Provides-Extra: faiss
 Provides-Extra: redis
 Provides-Extra: elasticsearch
+Provides-Extra: pinecone
 Provides-Extra: postgres
 License-File: LICENSE
 
 # VecSim - A unified interface for similarity servers
 A standard, light-weight interface to all popular similarity servers.
 
 ## The problems we are trying to solve:
```

