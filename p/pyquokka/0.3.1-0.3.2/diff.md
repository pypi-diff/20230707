# Comparing `tmp/pyquokka-0.3.1-py3-none-any.whl.zip` & `tmp/pyquokka-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 312156 bytes, number of entries: 48
+Zip file size: 312626 bytes, number of entries: 48
 -rw-rw-r--  2.0 unx      309 b- defN 23-Jun-27 05:10 pyquokka/__init__.py
 -rw-rw-r--  2.0 unx     4291 b- defN 23-Apr-19 05:39 pyquokka/catalog.py
 -rw-rw-r--  2.0 unx      372 b- defN 23-Jun-06 17:55 pyquokka/common_startup.sh
--rw-rw-r--  2.0 unx    28239 b- defN 23-Apr-16 23:17 pyquokka/coordinator.py
--rw-rw-r--  2.0 unx    48433 b- defN 23-Jun-22 19:44 pyquokka/core.py
+-rw-rw-r--  2.0 unx    28801 b- defN 23-Jul-04 05:25 pyquokka/coordinator.py
+-rw-rw-r--  2.0 unx    48433 b- defN 23-Jul-05 16:34 pyquokka/core.py
 -rw-rw-r--  2.0 unx    51863 b- defN 23-Jun-14 21:42 pyquokka/dataset.py
 -rw-rw-r--  2.0 unx   101812 b- defN 23-May-16 03:36 pyquokka/datastream.py
 -rw-rw-r--  2.0 unx     1438 b- defN 22-Nov-11 18:24 pyquokka/debugger.py
--rw-rw-r--  2.0 unx    84360 b- defN 23-Jun-27 15:11 pyquokka/df.py
+-rw-rw-r--  2.0 unx    84362 b- defN 23-Jul-06 22:54 pyquokka/df.py
 -rw-rw-r--  2.0 unx      230 b- defN 23-Jun-01 06:12 pyquokka/disk_setup.sh
 -rw-rw-r--  2.0 unx    37360 b- defN 23-Apr-16 23:19 pyquokka/executors.py
 -rw-rw-r--  2.0 unx    12657 b- defN 23-Mar-28 22:05 pyquokka/expression.py
 -rw-rw-r--  2.0 unx    17483 b- defN 23-Mar-26 21:54 pyquokka/flight.py
 -rw-rw-r--  2.0 unx     3098 b- defN 23-May-11 02:45 pyquokka/hbq.py
 -rwxrwxr-x  2.0 unx   368480 b- defN 23-Apr-11 05:32 pyquokka/ldb.so
 -rw-rw-r--  2.0 unx      274 b- defN 23-Mar-25 18:43 pyquokka/leader_start_ray.sh
 -rw-rw-r--  2.0 unx      619 b- defN 23-Mar-25 18:43 pyquokka/leader_startup.sh
 -rw-rw-r--  2.0 unx    31410 b- defN 23-Jun-14 20:46 pyquokka/logical.py
--rw-rw-r--  2.0 unx     8530 b- defN 23-Jun-27 06:14 pyquokka/orderedstream.py
+-rw-rw-r--  2.0 unx     8705 b- defN 23-Jul-06 22:53 pyquokka/orderedstream.py
 -rw-rw-r--  2.0 unx     1009 b- defN 23-May-18 17:31 pyquokka/placement_strategy.py
 -rw-rw-r--  2.0 unx     3717 b- defN 23-Mar-29 00:48 pyquokka/quokka_dataset.py
 -rw-rw-r--  2.0 unx    20581 b- defN 23-Jun-05 23:12 pyquokka/quokka_runtime.py
 -rw-rw-r--  2.0 unx    93718 b- defN 22-Oct-04 03:50 pyquokka/redis.conf
 -rw-rw-r--  2.0 unx    15525 b- defN 23-Jun-02 03:36 pyquokka/sql.py
 -rw-rw-r--  2.0 unx    16471 b- defN 23-Mar-27 22:47 pyquokka/sql_utils.py
 -rw-rw-r--  2.0 unx     2371 b- defN 22-Jul-15 20:59 pyquokka/state.py
@@ -32,19 +32,19 @@
 -rw-rw-r--  2.0 unx     4081 b- defN 23-Jan-25 17:17 pyquokka/windowtypes.py
 -rw-rw-r--  2.0 unx     1231 b- defN 23-Jun-22 05:22 pyquokka/dataset/__init__.py
 -rw-rw-r--  2.0 unx      652 b- defN 23-Jun-22 05:25 pyquokka/dataset/base_dataset.py
 -rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-22 18:00 pyquokka/dataset/crypto_dataset.py
 -rw-rw-r--  2.0 unx    11209 b- defN 23-Jun-29 03:12 pyquokka/dataset/ordered_readers.py
 -rw-rw-r--  2.0 unx    36345 b- defN 23-Jun-22 18:00 pyquokka/dataset/unordered_readers.py
 -rw-rw-r--  2.0 unx      192 b- defN 23-Jun-27 05:11 pyquokka/executors/__init__.py
--rw-rw-r--  2.0 unx      811 b- defN 23-May-11 02:45 pyquokka/executors/base_executor.py
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jul-04 17:50 pyquokka/executors/base_executor.py
 -rw-rw-r--  2.0 unx     8198 b- defN 23-Jun-27 06:13 pyquokka/executors/cep_executors.py
--rw-rw-r--  2.0 unx    20679 b- defN 23-Jun-12 19:32 pyquokka/executors/sql_executors.py
--rw-rw-r--  2.0 unx    17185 b- defN 23-May-11 02:45 pyquokka/executors/ts_executors.py
+-rw-rw-r--  2.0 unx    20679 b- defN 23-Jul-01 23:10 pyquokka/executors/sql_executors.py
+-rw-rw-r--  2.0 unx    18649 b- defN 23-Jul-06 22:58 pyquokka/executors/ts_executors.py
 -rw-rw-r--  2.0 unx     5209 b- defN 23-May-19 06:44 pyquokka/executors/vector_executors.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      971 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       53 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3908 b- defN 23-Jun-29 06:48 pyquokka-0.3.1.dist-info/RECORD
-48 files, 1140727 bytes uncompressed, 306048 bytes compressed:  73.2%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      971 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       53 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3908 b- defN 23-Jul-06 23:05 pyquokka-0.3.2.dist-info/RECORD
+48 files, 1142972 bytes uncompressed, 306518 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -120,26 +120,26 @@
 
 Filename: pyquokka/executors/ts_executors.py
 Comment: 
 
 Filename: pyquokka/executors/vector_executors.py
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/LICENSE
+Filename: pyquokka-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/METADATA
+Filename: pyquokka-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/WHEEL
+Filename: pyquokka-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/entry_points.txt
+Filename: pyquokka-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/top_level.txt
+Filename: pyquokka-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyquokka-0.3.1.dist-info/RECORD
+Filename: pyquokka-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyquokka/coordinator.py

```diff
@@ -133,29 +133,40 @@
         # you need to figure out what is the first stage to execute
         self.ast = self.AST.to_dict(self.r)
         self.r.set("finish-execution",  0)
         self.r.set("current-execution-stage", min(self.ast.values()))
         execute_handles = {worker : self.node_handles[worker].execute.remote() for worker in self.node_handles}
         execute_handles_list = list(execute_handles.values())
         
+        stage_timer = time.time()
+
         while True:
             time.sleep(0.01)
 
             try:
                 finished, unfinished = ray.wait(execute_handles_list, timeout= 0.01)
                 # print("finished", finished, "unfinished", unfinished)
                 assert len(unfinished) == len(execute_handles_list), "no execute method should terminate on its own" + str(ray.get(finished))
 
                 self.update_undone()                
                 if len(self.undone) == 0:
                     # wipe task manager state after execution of a TaskGraph.
                     self.r.set("finish-execution",  1)
                     assert all(ray.get(execute_handles_list))
+                    old_stage = self.r.get("current-execution-stage")
+                    print("STAGE {} took {} seconds".format(old_stage, time.time() - stage_timer))
                     return
+                
+                old_stage = self.r.get("current-execution-stage")
                 self.update_execution_stage()
+                new_stage = self.r.get("current-execution-stage")
+                if new_stage != old_stage:
+                    print("STAGE {} took {} seconds".format(old_stage, time.time() - stage_timer))
+                    stage_timer = time.time()
+                    
 
             except ray.exceptions.RayActorError:
                 print("detected failure")
                 self.r.set("recovery-lock", 1)
 
                 start = time.time()
                 while True:
```

## pyquokka/df.py

```diff
@@ -59,15 +59,15 @@
             >>> cluster = manager.from_json("my_cluster.json")
 
         """
 
         self.sql_config= {"optimize_joins" : True, "s3_csv_materialize_threshold" : 10 * 1048576, "disk_csv_materialize_threshold" : 1048576,
                       "s3_parquet_materialize_threshold" : 10 * 1048576, "disk_parquet_materialize_threshold" : 1048576}
         self.exec_config = {"hbq_path": "/data/", "fault_tolerance": False, "memory_limit": 0.1, "max_pipeline_batches": 30, 
-                        "checkpoint_interval": None, "checkpoint_bucket": "quokka-checkpoint", "batch_attempt": 20, "max_pipeline": 3}
+                        "checkpoint_interval": None, "checkpoint_bucket": "quokka-checkpoint", "batch_attempt": 20, "max_pipeline": 300}
 
         self.latest_node_id = 0
         self.nodes = {}
         self.cluster = LocalCluster() if cluster is None else cluster
         if type(self.cluster) == LocalCluster:
             if self.exec_config["fault_tolerance"]:
                 print("Fault tolerance is not supported in local mode, turning it off")
```

## pyquokka/orderedstream.py

```diff
@@ -134,23 +134,27 @@
         else:
             assert left_by is not None and right_by is not None
         
         assert left_by in self.schema
         assert right_by in right.schema
 
         new_schema = self.schema.copy()
-        if self.materialized:
-            schema_mapping = {col: {-1: col} for col in self.schema}
-        else:
-            schema_mapping = {col: {0: col} for col in self.schema}
-
-        if right.materialized:
-            right_table_id = -1
-        else:
-            right_table_id = 1
+        # if self.materialized:
+        #     schema_mapping = {col: {-1: col} for col in self.schema}
+        # else:
+        #     schema_mapping = {col: {0: col} for col in self.schema}
+
+        schema_mapping = schema_mapping = {col: {0: col} for col in self.schema}
+
+        # if right.materialized:
+        #     right_table_id = -1
+        # else:
+        #     right_table_id = 1
+        
+        right_table_id = 1
 
         rename_dict = {}
 
         # import pdb;pdb.set_trace()
 
         right_cols = right.schema
         for col in right_cols:
@@ -166,15 +170,15 @@
             else:
                 new_schema.append(col)
                 schema_mapping[col] = {right_table_id: col}
         
         if len(rename_dict) > 0:
             right = right.rename(rename_dict)
 
-
+        # print("new schema", new_schema)
         executor = SortedAsofExecutor(left_on, right_on, left_by, right_by, suffix)
 
         return self.quokka_context.new_stream(
                 sources={0: self, 1: right},
                 partitioners={0: HashPartitioner(
                     left_by), 1: HashPartitioner(right_by)},
                 node=StatefulNode(
```

## pyquokka/executors/base_executor.py

```diff
@@ -1,8 +1,9 @@
 import os
+# os.environ["POLARS_MAX_THREADS"] = "2" 
 import polars
 import pandas as pd
 os.environ['ARROW_DEFAULT_MEMORY_POOL'] = 'system'
 import redis
 import pyarrow as pa
 import time
 import os, psutil
```

## pyquokka/executors/ts_executors.py

```diff
@@ -283,14 +283,49 @@
                         ORDER BY TIME_COL
                         RANGE unbounded preceding
                     )
                 """.replace("TIME_COL", self.time_col).replace("BY_COL", self.by_col).replace("AGG_FUNCS", aggregations)).arrow()
         
             return result
 
+class BroadcastAsofJoinExecutor(Executor):
+    # batch func here expects a list of dfs. This is a quark of the fact that join results could be a list of dfs.
+    # batch func must return a list of dfs too
+    def __init__(self, small_quotes, time_col_trades = 'time', time_col_quotes = 'time', symbol_col_trades = 'symbol', symbol_col_quotes = 'symbol', suffix = "_right"):
+
+        self.suffix = suffix
+
+        assert type(small_table) == polars.DataFrame
+        self.state = small_table
+
+        self.time_col_trades = time_col_trades
+        self.time_col_quotes = time_col_quotes
+        self.symbol_col_trades = symbol_col_trades
+        self.symbol_col_quotes = symbol_col_quotes
+        
+        assert self.small_on in self.state.columns
+    
+    def checkpoint(self, conn, actor_id, channel_id, seq):
+        pass
+    
+    def restore(self, conn, actor_id, channel_id, seq):
+        pass
+
+    # the execute function signature does not change. stream_id will be a [0 - (length of InputStreams list - 1)] integer
+    def execute(self,batches, stream_id, executor_id):
+        # state compaction
+        batches = [polars.from_arrow(i) for i in batches if i is not None and len(i) > 0]
+        if len(batches) == 0:
+            return
+        batch = polars.concat(batches)
+        return batch.join(self.state, left_on = self.big_on, right_on = self.small_on, how = self.how, suffix = self.suffix)
+        
+    def done(self,executor_id):
+        return
+
 class SortedAsofExecutor(Executor):
     def __init__(self, time_col_trades = 'time', time_col_quotes = 'time', symbol_col_trades = 'symbol', symbol_col_quotes = 'symbol', suffix = "_right") -> None:
         self.trade_state = None
         self.quote_state = None
         self.join_state = None
         self.time_col_trades = time_col_trades
         self.time_col_quotes = time_col_quotes
```

## Comparing `pyquokka-0.3.1.dist-info/LICENSE` & `pyquokka-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyquokka-0.3.1.dist-info/METADATA` & `pyquokka-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquokka
-Version: 0.3.1
+Version: 0.3.2
 Summary: Quokka
 Author: Tony Wang
 Author-email: zihengw@stanford.edu
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `pyquokka-0.3.1.dist-info/RECORD` & `pyquokka-0.3.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 pyquokka/__init__.py,sha256=pBsjKUKy3Fdy47TuKyvWUGKAppifFP4F64l_ZuSwV80,309
 pyquokka/catalog.py,sha256=XczH9nRAjYE0eWvPdoI_sQE1N85vflPouzjpIe0lqOA,4291
 pyquokka/common_startup.sh,sha256=km_6KjJKJtmTovnLdKjUMeg3uuvuLmSuPQhlpYpw0xs,372
-pyquokka/coordinator.py,sha256=s7yjNB_F6bEoWoko_5cTfN0BAyH9AcYm2PKIbqJexhI,28239
+pyquokka/coordinator.py,sha256=71ODvs3io8rQYDnUxmL8yBJ-K10Cwmbi_sHc4rZRJB4,28801
 pyquokka/core.py,sha256=mJ7LW5GRsnccv_Zy7DrVyo3zUj4XozKG-yUn2bZQ9u8,48433
 pyquokka/dataset.py,sha256=8oE4Z0uHmnnbFlqxvg2buvQtlp--j_QiHkgGEhsgTH8,51863
 pyquokka/datastream.py,sha256=qeqpWiI9tVcJbfec41uE6f-KhzAWu31B-Z3zB3EjO0s,101812
 pyquokka/debugger.py,sha256=Yi1CqGHbV2y2bszUhKuxcQ561vugc6hs6xfnpJ8HIjU,1438
-pyquokka/df.py,sha256=q_LzMlihNADynd5ORFUjJxIjLGyahY7qQvHPguZUCnM,84360
+pyquokka/df.py,sha256=UI_JoROzRLcWTCHwZiwhPAcuMiwfz9MFY1E6P3SodlA,84362
 pyquokka/disk_setup.sh,sha256=4ZKHTrju2mQo-v8509xhGaEkacP_lBIzX8QYZkTLEhQ,230
 pyquokka/executors.py,sha256=dVzy3_WbsMtbAWay2UlEgE1GmxEVbT6Fz1X9i2elboY,37360
 pyquokka/expression.py,sha256=SmJxvGrSgW3ra8EU5SLGbQ8AxbJ2bPxKHLvbXpQ-8WY,12657
 pyquokka/flight.py,sha256=ri1aEXtn4s2_ACD8PfU5EIy_fA7FlNrM61WuUjQ9Pl8,17483
 pyquokka/hbq.py,sha256=V3nE2IcIIclxxdDyXRdzuV7_y_DRa90B_aVaa6aU9tg,3098
 pyquokka/ldb.so,sha256=SO70uhXN219Ns5RNIEePv1fs0qRSksc6yq2eN0tucw8,368480
 pyquokka/leader_start_ray.sh,sha256=vyZi-Utmj7r8Qr43YmOQq3uIuAN5Nn4F61MIszzdit4,274
 pyquokka/leader_startup.sh,sha256=yOP5vjuLS9D2WtcozcFewXQB84p8jm8IcyltYcuWNss,619
 pyquokka/logical.py,sha256=1qv8igMqQT_GWk9eUQdMzAO2LervMD7d3D_XbHARSeI,31410
-pyquokka/orderedstream.py,sha256=Kg7h8yimNlqQX_KX8c-fbtrYPD9qoUyoSpwwcGB1lN4,8530
+pyquokka/orderedstream.py,sha256=gFeiBP8Rk-CO77ZZetudhcs1IBflT0s5F2bYq6EzLXk,8705
 pyquokka/placement_strategy.py,sha256=0ISmKzf5d4Hxs8RvNXWyvPSCuybIsNxG8nbJgBV6NRk,1009
 pyquokka/quokka_dataset.py,sha256=_b7L8zWCimtiR3kMbCZWLH4g-w3SZ-J8gw8bjqhv-lA,3717
 pyquokka/quokka_runtime.py,sha256=D8FdK_4504DWO_YDsaa8rFn5FbKM_5d_07s4Ichrmaw,20581
 pyquokka/redis.conf,sha256=Hk0GU-BnDDpMZ6Gmit1-Ct_iyO7ttCvzyfz5PLFVkJY,93718
 pyquokka/sql.py,sha256=T5YcwnIElhQa3s9xPqR6D9P3B4o8Fz7ctJlKWNQh9i4,15525
 pyquokka/sql_utils.py,sha256=1vWMrQft37so5KtOLlsqLk8MpaFB0XO9Ib9XwQEuw90,16471
 pyquokka/state.py,sha256=wGt5uh_ZS-xV-HqVgWmdTZUnQoabpvSOHiQXOejg7L4,2371
@@ -31,18 +31,18 @@
 pyquokka/windowtypes.py,sha256=zPh9QgwSQ3E00eNQM8jk2iQZNMuzAQ3eoaFDm1H5NGk,4081
 pyquokka/dataset/__init__.py,sha256=n2qlwH9kIaV9FXeK9yrFGTomb_XXdJEGcRMdBCq8Unw,1231
 pyquokka/dataset/base_dataset.py,sha256=lx8vlk6VI0jXpofm69iq-aOgooc8MQwXC5pRE78s1lg,652
 pyquokka/dataset/crypto_dataset.py,sha256=gn58ljIXLJs7pt2NIuNnAcDzRDgjotntcek3w0IGSU8,3553
 pyquokka/dataset/ordered_readers.py,sha256=vkOsw0HGdJJLyt4vWevQ8cLNawcxCL0obRPMhSy2TH4,11209
 pyquokka/dataset/unordered_readers.py,sha256=w_aFkXgTmTJnpg6P9oL7-s1EtnXiVt30hN0Kp-Uupxk,36345
 pyquokka/executors/__init__.py,sha256=jGnveyusBOz39mkcih7C0eN1WlOudDZ2sTSEiuMvs_s,192
-pyquokka/executors/base_executor.py,sha256=clVkP0wf03OMG7x9vMdzRPTviT5DE6rQv3n6E81bZM4,811
+pyquokka/executors/base_executor.py,sha256=D0AoYZ4UB3EEktuawYXaXr8t2toaItiTDNX5QgDsC8c,853
 pyquokka/executors/cep_executors.py,sha256=9eqdDZbvvcu5WO2Nu_WlcK4wjXJkscfRr2pNw-fxNZM,8198
 pyquokka/executors/sql_executors.py,sha256=DG9AXg1Zl3XsBzKeUfXQxu9Q3zLk9Cb1RMwoj-FsLck,20679
-pyquokka/executors/ts_executors.py,sha256=KPRjeMap_PogESYfqYpCBrLyVgRKVrGxWQYICQRehEo,17185
+pyquokka/executors/ts_executors.py,sha256=EGDkYmL1aV8jnDh7TxqMzfQiEh34wyjW_wnsLEfpbW8,18649
 pyquokka/executors/vector_executors.py,sha256=etRjJ93u0l5h4hwUeIUdUcLKgmWJhtITLzBJQZMm_Qc,5209
-pyquokka-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pyquokka-0.3.1.dist-info/METADATA,sha256=WkPIEDmg5ffMQ6Alasq-Xid5GMEyAiqgcJ06l9T4oJ4,971
-pyquokka-0.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyquokka-0.3.1.dist-info/entry_points.txt,sha256=EuS_cN6o5rCqK6wFXMnnaQBY-2jSlNWpZxP41mHMbAU,53
-pyquokka-0.3.1.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
-pyquokka-0.3.1.dist-info/RECORD,,
+pyquokka-0.3.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pyquokka-0.3.2.dist-info/METADATA,sha256=t8BKHFmyl3knCOut5Kf6PG9VVkO_aXvw1mX9e4b2T_Y,971
+pyquokka-0.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyquokka-0.3.2.dist-info/entry_points.txt,sha256=EuS_cN6o5rCqK6wFXMnnaQBY-2jSlNWpZxP41mHMbAU,53
+pyquokka-0.3.2.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
+pyquokka-0.3.2.dist-info/RECORD,,
```

