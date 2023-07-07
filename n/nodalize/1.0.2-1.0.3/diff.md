# Comparing `tmp/nodalize-1.0.2-py3-none-any.whl.zip` & `tmp/nodalize-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 66712 bytes, number of entries: 43
+Zip file size: 70418 bytes, number of entries: 44
 -rw-r--r--  2.0 unx      102 b- defN 23-Jun-04 09:32 nodalize/__init__.py
--rw-r--r--  2.0 unx    13455 b- defN 23-Jun-14 20:31 nodalize/datanode.py
+-rw-r--r--  2.0 unx    13425 b- defN 23-Jun-19 13:57 nodalize/datanode.py
 -rw-r--r--  2.0 unx     6443 b- defN 23-Jun-15 16:57 nodalize/dependency.py
 -rw-r--r--  2.0 unx     2673 b- defN 23-Jun-04 09:22 nodalize/dependency_loader.py
 -rw-r--r--  2.0 unx       58 b- defN 22-Sep-01 17:05 nodalize/calculators/__init__.py
 -rw-r--r--  2.0 unx     9656 b- defN 23-Jun-10 15:25 nodalize/calculators/calculator.py
 -rw-r--r--  2.0 unx    14888 b- defN 23-Jun-04 17:18 nodalize/calculators/dask_calculator.py
 -rw-r--r--  2.0 unx    12382 b- defN 23-Jun-04 17:19 nodalize/calculators/pandas_calculator.py
 -rw-r--r--  2.0 unx    13967 b- defN 23-Jun-10 15:25 nodalize/calculators/polars_calculator.py
@@ -18,28 +18,29 @@
 -rw-r--r--  2.0 unx     4082 b- defN 23-Jun-14 20:26 nodalize/custom_dependencies/date.py
 -rw-r--r--  2.0 unx     5542 b- defN 23-Jun-14 20:25 nodalize/custom_dependencies/lag.py
 -rw-r--r--  2.0 unx     4308 b- defN 23-Jun-14 20:26 nodalize/custom_dependencies/window.py
 -rw-r--r--  2.0 unx       30 b- defN 22-Sep-01 17:05 nodalize/data_management/__init__.py
 -rw-r--r--  2.0 unx     8113 b- defN 23-Jun-11 17:07 nodalize/data_management/data_manager.py
 -rw-r--r--  2.0 unx     6112 b- defN 23-Jun-10 15:10 nodalize/data_management/database_data_manager.py
 -rw-r--r--  2.0 unx    13798 b- defN 23-Jun-11 17:07 nodalize/data_management/delta_lake_data_manager.py
+-rw-r--r--  2.0 unx    15253 b- defN 23-Jun-19 13:30 nodalize/data_management/duckdb_data_manager.py
 -rw-r--r--  2.0 unx    29878 b- defN 23-Jun-10 15:26 nodalize/data_management/kdb_data_manager.py
 -rw-r--r--  2.0 unx     8213 b- defN 23-Jun-10 15:25 nodalize/data_management/local_file_data_manager.py
 -rw-r--r--  2.0 unx     8415 b- defN 23-Jun-10 15:25 nodalize/data_management/s3_file_data_manager.py
--rw-r--r--  2.0 unx    15158 b- defN 23-Jun-10 15:24 nodalize/data_management/sqlite_data_manager.py
+-rw-r--r--  2.0 unx    15019 b- defN 23-Jun-19 13:15 nodalize/data_management/sqlite_data_manager.py
 -rw-r--r--  2.0 unx       47 b- defN 22-Sep-01 17:05 nodalize/orchestration/__init__.py
--rw-r--r--  2.0 unx     2899 b- defN 23-Jun-04 09:32 nodalize/orchestration/calculator_factory.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jun-19 13:56 nodalize/orchestration/calculator_factory.py
 -rw-r--r--  2.0 unx    12816 b- defN 23-Jun-15 16:25 nodalize/orchestration/coordinator.py
 -rw-r--r--  2.0 unx     1784 b- defN 23-Jun-04 09:21 nodalize/orchestration/data_manager_factory.py
 -rw-r--r--  2.0 unx     3790 b- defN 23-Jun-04 09:22 nodalize/orchestration/data_node_cache.py
 -rw-r--r--  2.0 unx       37 b- defN 22-Sep-01 17:05 nodalize/tools/__init__.py
 -rw-r--r--  2.0 unx     1942 b- defN 23-Apr-16 11:18 nodalize/tools/dates.py
 -rw-r--r--  2.0 unx     1772 b- defN 22-Dec-30 16:50 nodalize/tools/static_func_tools.py
 -rw-r--r--  2.0 unx     4112 b- defN 22-Sep-01 17:05 nodalize/tools/tree.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-22 14:42 sandbox/__init__.py
--rw-r--r--  2.0 unx       81 b- defN 23-Jun-10 14:57 sandbox/test_anything.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6033 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3907 b- defN 23-Jun-15 17:17 nodalize-1.0.2.dist-info/RECORD
-43 files, 255508 bytes uncompressed, 60372 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 12:06 sandbox/test_anything.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Jul-07 12:08 nodalize-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6135 b- defN 23-Jul-07 12:08 nodalize-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 12:08 nodalize-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-07 12:08 nodalize-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4011 b- defN 23-Jul-07 12:08 nodalize-1.0.3.dist-info/RECORD
+44 files, 271283 bytes uncompressed, 63908 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -63,14 +63,17 @@
 
 Filename: nodalize/data_management/database_data_manager.py
 Comment: 
 
 Filename: nodalize/data_management/delta_lake_data_manager.py
 Comment: 
 
+Filename: nodalize/data_management/duckdb_data_manager.py
+Comment: 
+
 Filename: nodalize/data_management/kdb_data_manager.py
 Comment: 
 
 Filename: nodalize/data_management/local_file_data_manager.py
 Comment: 
 
 Filename: nodalize/data_management/s3_file_data_manager.py
@@ -108,23 +111,23 @@
 
 Filename: sandbox/__init__.py
 Comment: 
 
 Filename: sandbox/test_anything.py
 Comment: 
 
-Filename: nodalize-1.0.2.dist-info/LICENSE
+Filename: nodalize-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: nodalize-1.0.2.dist-info/METADATA
+Filename: nodalize-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: nodalize-1.0.2.dist-info/WHEEL
+Filename: nodalize-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: nodalize-1.0.2.dist-info/top_level.txt
+Filename: nodalize-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: nodalize-1.0.2.dist-info/RECORD
+Filename: nodalize-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nodalize/datanode.py

```diff
@@ -52,22 +52,22 @@
 
         Args:
             dependencies: dictionary of dependency definitions
         """
         self._dependency_definitions = dependencies
 
     @property
-    def calculator_type(self) -> str:
+    def calculator_type(self) -> Optional[str]:
         """
         Return name of calculator to use.
 
         Returns:
             calculator name
         """
-        raise AssertionError("Calculator type not defined")
+        return None
 
     @property
     def calculator(self) -> Calculator:
         """
         Get calculator.
 
         Returns:
```

## nodalize/data_management/sqlite_data_manager.py

```diff
@@ -207,15 +207,15 @@
         Convert value to sqlite.
 
         Args:
             t: value type
             v: value
 
         Returns:
-            KDB value as string
+            sqlite value as string
         """
         if v is None:
             return "NULL"
 
         if t == int:
             if np.isnan(v):
                 return "NULL"
@@ -354,20 +354,15 @@
         key_columns_list = ",".join(key_columns)
 
         if columns is None:
             columns = list(schema.keys())
         else:
             columns = columns[:]
 
-        column_list2 = ", ".join([f"A.{col}" for col in columns])
-
-        for col in key_columns:
-            if col not in columns:
-                columns.append(col)
-        column_list = ", ".join(columns)
+        column_list = ", ".join([f"A.{col}" for col in columns])
 
         if batch_ids is not None:
             if filters is None:
                 filters = [[(column_names.BATCH_ID, "in", batch_ids)]]
             else:
                 for f in filters:
                     f.append((column_names.BATCH_ID, "in", batch_ids))
@@ -385,19 +380,19 @@
         joins.append(f"A.{column_names.INSERTED_DATETIME}=B.{max_datetime_col_name}")
         joins_list = " AND ".join(joins)
 
         cte_name = generate_random_name(10)
 
         query = f"""
 WITH [{cte_name}] AS (
-    SELECT {column_list}, MAX({column_names.INSERTED_DATETIME}) AS {max_datetime_col_name}
+    SELECT {key_columns_list}, MAX({column_names.INSERTED_DATETIME}) AS {max_datetime_col_name}
     FROM [{table_name}]
     GROUP BY {key_columns_list}
 )
-SELECT {column_list2}
+SELECT {column_list}
 FROM [{table_name}] A
 INNER JOIN [{cte_name}] B on {joins_list}
 {sql_filter}
 """
 
         logging.info(f"Running Sqlite query: {query}")
         with sqlite3.connect(self._location) as conn:
```

## nodalize/orchestration/calculator_factory.py

```diff
@@ -12,24 +12,30 @@
         Initialize factory.
 
         Args:
             application_name: name of the application
         """
         self._application_name = application_name
         self._calculators = {}  # type: Dict[str, Calculator]
+        self._default_calculator = None  # type: Optional[Calculator]
 
     def set_calculator(
-        self, identifier: str, calculator: Optional[Calculator] = None, **kwargs: Any
+        self,
+        identifier: str,
+        calculator: Optional[Calculator] = None,
+        default: bool = False,
+        **kwargs: Any,
     ) -> Calculator:
         """
         Define calculator, which can then be accessed by name.
 
         Args:
             identifier: unique identifier
             calculator: instance of calculator - if None, then will use default calculator
+            default: set calculator as default
             kwargs: optional parameters to pass to calculator initializer
 
         Returns:
             calculator added to cache
         """
         if calculator is None:
             if identifier == "pandas":
@@ -54,31 +60,39 @@
                 calculator = PolarsCalculator(self._application_name, **kwargs)
             else:
                 raise ValueError(
                     f"{identifier} not defined, available identifiers are: pandas, pyarrow, pandas, dask"
                 )
 
         self._calculators[identifier] = calculator
+        if default:
+            self._default_calculator = calculator
         return calculator
 
-    def get_calculator(self, calculator_type: str) -> Calculator:
+    def get_calculator(self, calculator_type: Optional[str] = None) -> Calculator:
         """
         Get existing calculator based on identifier.
 
         Args:
-            calculator_type: type of calculator needed
+            calculator_type: type of calculator needed. If none, then return default one.
 
         Returns:
             instance of calculator
         """
-        calculator = self._calculators.get(calculator_type)
-
-        if calculator is None:
-            try:
-                calculator = self.set_calculator(calculator_type)
-            except Exception:
-                pass
+        if calculator_type is None:
+            if self._default_calculator is not None:
+                return self._default_calculator
+            else:
+                raise AssertionError("No default calculator defined")
+        else:
+            calculator = self._calculators.get(calculator_type)
+
+            if calculator is None:
+                try:
+                    calculator = self.set_calculator(calculator_type)
+                except Exception:
+                    pass
 
-        if calculator is None:
-            raise ValueError(f"No calculator defined for {calculator_type}.")
+            if calculator is None:
+                raise ValueError(f"No calculator defined for {calculator_type}.")
 
         return calculator
```

## sandbox/test_anything.py

```diff
@@ -1,6 +0,0 @@
-00000000: 6672 6f6d 206e 6f64 616c 697a 652e 636f  from nodalize.co
-00000010: 6e73 7461 6e74 7320 696d 706f 7274 2063  nstants import c
-00000020: 6f6c 756d 6e5f 6e61 6d65 730a 0a63 6f6c  olumn_names..col
-00000030: 756d 6e5f 6e61 6d65 732e 4441 5441 5f44  umn_names.DATA_D
-00000040: 4154 4520 3d20 224d 7944 6174 6522 0a0a  ATE = "MyDate"..
-00000050: 0a                                       .
```

## Comparing `nodalize-1.0.2.dist-info/LICENSE` & `nodalize-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nodalize-1.0.2.dist-info/METADATA` & `nodalize-1.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nodalize
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework to organize data transformation flow.
 Home-page: https://github.com/Ron-Ldn/nodalize
 Author: Ronan Mouquet
 Author-email: ronan.mouquet@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nodalize
-Nodalize is a flexible framework for Python projects to easily create and maintain data pipelines. The dependency orchestration is automated and all accesses to the data store are abstracted. The phylosophy is to make developers focus on their business logic.
+Nodalize is a flexible framework for Python projects to easily create and maintain data pipelines. The dependency orchestration is automated and all accesses to the data store are abstracted. Developers can focus on their business logic.
 
-Nodalize supports multiple data storage technologies and allows to easily plug customized ones.
+Nodalize supports multiple data storage technologies and allows to easily plug in bespoke ones.
 
-Finally, Nodalize handle multiple dataframe-based calculation frameworks, so that each pipeline can be built with the most convenient tool (Pandas, PySpark, etc.).
+Finally, Nodalize handle multiple dataframe-based calculation frameworks, so that each pipeline can be built with the most convenient tool (Pandas, Polars, PySpark, etc.).
 
 
 ## Illustration
 Let's start with an example. We assume that we have a data set called "BaseDataSet" with 3 columns "Id", "Numerator" and "Denominator". We can create a derived data set applying some transformations using Python code such as below.
 
 ```python
 class EnrichedDataSet(DataNode):
@@ -141,14 +141,21 @@
 
 [Working with time series](docs/time_series.md)
 
 [Loading data with lookback](docs/data_lookback.md)
 
 [Cascading calculations](docs/cascading.md)
 
+[Retry and fallback](docs/retry_fallback.md)
+
+## API
+[Compute nodes](docs/compute.md)
+
+[Define node](docs/node.md)
+
 ## Customization
 [Manage your own data store](docs/custom_data_manager.md)
 
 [Create your own calculator](docs/custom_calculator.md)
 
 ## Development
 [How to contribute](docs/development.md)
```

## Comparing `nodalize-1.0.2.dist-info/RECORD` & `nodalize-1.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 nodalize/__init__.py,sha256=BmDtEafssUfgezj0dhPKSbCnWmNVlvUz6OFORPwPvnA,102
-nodalize/datanode.py,sha256=D19iM-CoZyqWLf4jQj8gq9KUenFbxdJRwm8ppos4yro,13455
+nodalize/datanode.py,sha256=s4l7PAn8zXmgEimKWtNmLc7VY1IzV7oRIGRZw_SFDGc,13425
 nodalize/dependency.py,sha256=S9maNUsa5KHhbaT1GRa0I8CjSIJz26prQ5AsdmG-Eww,6443
 nodalize/dependency_loader.py,sha256=GKlg71LFXLp12HiK1yjvsKKCMqFVEJXdn11rGwd69Rs,2673
 nodalize/calculators/__init__.py,sha256=UuTx55ZtSkzjuC_A77uWYb6WTAFtoaJCGuWYI57L9IU,58
 nodalize/calculators/calculator.py,sha256=uOACNqM3Qr1sAfYIbothYKxFShCM8xCkHYSw04rEz1Y,9656
 nodalize/calculators/dask_calculator.py,sha256=PdgValqvy5V2ZBTrsdOAzuqPZYguxaSG58FLwX9WjBo,14888
 nodalize/calculators/pandas_calculator.py,sha256=pEVYEzzzcQs8rMrFY95obqx349kUCB4FPMSDVpW3XF0,12382
 nodalize/calculators/polars_calculator.py,sha256=e5QJKy8A4E1IWG6EqNguR3_ETn4kiLqOe8wqsGVGI3M,13967
@@ -17,27 +17,28 @@
 nodalize/custom_dependencies/date.py,sha256=sdunubeJGOBs2OAdPFWqrif05U3EYkPQzlKdpP3lFK8,4082
 nodalize/custom_dependencies/lag.py,sha256=xYY8TYkTeAQi8XqljotjgA0vC5QBuFrQVdSGXCCYeIE,5542
 nodalize/custom_dependencies/window.py,sha256=b2ZqgI14GfMfV4TC7GnCSV89nJQjtRtKJ2fzt2gpD5k,4308
 nodalize/data_management/__init__.py,sha256=VBY2rHLAPf15SEIzpS2NjOIm2oLEGW1qXSQsTj-JKuQ,30
 nodalize/data_management/data_manager.py,sha256=FUzuu6SrCedIM90lEZ9ju55NKW_z5v4cA7I3MsVWbL4,8113
 nodalize/data_management/database_data_manager.py,sha256=jVJ7akf2tQGYuKBa8uL0Ocqjtvn5zBpe-USQIaiObH0,6112
 nodalize/data_management/delta_lake_data_manager.py,sha256=Umb3Nu7WuXPhgJSfKvj6oenSqBP81P2uRsyNbsXH-4Y,13798
+nodalize/data_management/duckdb_data_manager.py,sha256=YkM5JWU4ZOo_6OFbmPMmVvAlO0oCBHcyImK17Hy0_co,15253
 nodalize/data_management/kdb_data_manager.py,sha256=UBTzIhnncadfZ8YKJss0a3cFvrTVznmt_KgpdkbA7k4,29878
 nodalize/data_management/local_file_data_manager.py,sha256=3NudiFcGQmlYrHRHhMwQyVwf4ZJCF2Nz7pu7IxLSj-o,8213
 nodalize/data_management/s3_file_data_manager.py,sha256=KpLMPflzpxE1QLXLSeR5jz9l3jK01m6Kf-cg24pTUUM,8415
-nodalize/data_management/sqlite_data_manager.py,sha256=kAdaTvWRm7QurO4c5tDDXhCtNQUsuSWXT4Po2j4XwO0,15158
+nodalize/data_management/sqlite_data_manager.py,sha256=m82MelxqZ95esHYFaEZ74azoCms6HyUYL2eg-KY7ujk,15019
 nodalize/orchestration/__init__.py,sha256=QE8--MA0Su_FC-SGDKl5cffA2CST6Nf0AOEoBH_eRO0,47
-nodalize/orchestration/calculator_factory.py,sha256=zRigEqh86zJmAJrKfWrwn9A58JKGsAViuS4FfVFt2vg,2899
+nodalize/orchestration/calculator_factory.py,sha256=yd_gUNwN7Zwmx0ewoy9Zu7vAAvcwXYLQS1wLYdQR8n8,3465
 nodalize/orchestration/coordinator.py,sha256=ulF4nnUr0scW_hOI_EOvyWydG_qc3I4WvVAJYcIRcyM,12816
 nodalize/orchestration/data_manager_factory.py,sha256=MlUXqUstl0OFHmzxkwsssAJBofPwg1GSl6bM6B_hTvo,1784
 nodalize/orchestration/data_node_cache.py,sha256=sDBxAALhC5kykWQjcjzYxtUQVPAIpM9jpvh3cN456VA,3790
 nodalize/tools/__init__.py,sha256=t0FXjajsgg9zvYX5RZhatciX_tr8651HVfknbs0GEIM,37
 nodalize/tools/dates.py,sha256=BOJ3JKqxBUFkyUi6PkXsyTXOxIw5je9aLm7p0FVxkNQ,1942
 nodalize/tools/static_func_tools.py,sha256=XMMF22Ttq_aIceG9k8qlM1I42e2Wxl1ib_YJxD7jeYo,1772
 nodalize/tools/tree.py,sha256=L-xcKZ6P7EVr6j6DPj0fadzN8cJ7faJZgILPLniV4I0,4112
 sandbox/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sandbox/test_anything.py,sha256=P_sAKUwuWtO-D4saI3NSNxOtPwWh_vkZuqy_OmfbUzk,81
-nodalize-1.0.2.dist-info/LICENSE,sha256=JSLRq56-S2ilfHCBH-UGSgrmg1Wpdsgz7Ju9IkY9Qtc,1060
-nodalize-1.0.2.dist-info/METADATA,sha256=ZVRnz_BAI1E46Jzj9u9HErsFI7mvsogaG7mpUocxuC8,6033
-nodalize-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nodalize-1.0.2.dist-info/top_level.txt,sha256=PkmomGh5hRDE5vnV0L74Ke3gk-7n0Pj5qyNLXvGV3s0,17
-nodalize-1.0.2.dist-info/RECORD,,
+sandbox/test_anything.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nodalize-1.0.3.dist-info/LICENSE,sha256=JSLRq56-S2ilfHCBH-UGSgrmg1Wpdsgz7Ju9IkY9Qtc,1060
+nodalize-1.0.3.dist-info/METADATA,sha256=29R3TTr3-DSH-mFVfMOT6aYdoB-ZuiGQ5ifL85KZsvw,6135
+nodalize-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nodalize-1.0.3.dist-info/top_level.txt,sha256=PkmomGh5hRDE5vnV0L74Ke3gk-7n0Pj5qyNLXvGV3s0,17
+nodalize-1.0.3.dist-info/RECORD,,
```

