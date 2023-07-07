# Comparing `tmp/dataporter-0.1.4.tar.gz` & `tmp/dataporter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataporter-0.1.4.tar", max compression
+gzip compressed data, was "dataporter-0.1.5.tar", max compression
```

## Comparing `dataporter-0.1.4.tar` & `dataporter-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.4/README.md
--rw-r--r--   0        0        0      177 2023-06-14 11:19:16.055673 dataporter-0.1.4/dataporter/__init__.py
--rw-r--r--   0        0        0     6351 2023-06-30 11:00:53.891585 dataporter-0.1.4/dataporter/csv2sql.py
--rw-r--r--   0        0        0     3582 2023-06-14 13:44:28.242148 dataporter-0.1.4/dataporter/sql2csv.py
--rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.4/dataporter/sql_schema2txt.py
--rw-r--r--   0        0        0      502 2023-06-30 12:13:53.746523 dataporter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 dataporter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.5/README.md
+-rw-r--r--   0        0        0      225 2023-07-07 12:27:43.595700 dataporter-0.1.5/dataporter/__init__.py
+-rw-r--r--   0        0        0     4752 2023-07-07 13:14:56.566444 dataporter-0.1.5/dataporter/csv2csv.py
+-rw-r--r--   0        0        0     7001 2023-07-07 12:14:47.084091 dataporter-0.1.5/dataporter/csv2sql.py
+-rw-r--r--   0        0        0     3598 2023-07-07 11:52:32.112896 dataporter-0.1.5/dataporter/sql2csv.py
+-rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.5/dataporter/sql_schema2txt.py
+-rw-r--r--   0        0        0      373 2023-07-07 12:03:48.359884 dataporter-0.1.5/dataporter/utils.py
+-rw-r--r--   0        0        0      577 2023-07-07 12:28:59.493693 dataporter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 dataporter-0.1.5/PKG-INFO
```

### Comparing `dataporter-0.1.4/dataporter/csv2sql.py` & `dataporter-0.1.5/dataporter/csv2sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,48 @@
-from typing import List, Literal, Optional, Any
+from typing import List, Literal, Optional, Any, Iterable
 from loguru import logger
 from fire import Fire
 import pandas as pd
 from sqlalchemy import create_engine, text, exc
 from sqlalchemy.orm import sessionmaker
+from dataporter.utils import exec_multi_expr
 
 
-def _exec_multi_expr(df: pd.DataFrame, exprs: List[str], debug: bool = False) -> pd.DataFrame:
-    for expr in exprs:
-        if debug:
-            logger.info("exec expr: {}", expr)
-        df = pd.eval(expr=expr, target=df)
-
-        if debug:
-            logger.info("result: {}", df)
+def insert(trunk_df: Iterable[pd.DataFrame], pandas_exprs: List[str] | None, debug: bool, sql_data_exists: Literal["append", "fail", "replace"], ignore_error: bool, table_name: str, conn, index: bool):
+    for i, df in enumerate(trunk_df):
+        if pandas_exprs:
+            df = exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
+        df: pd.DataFrame
+        logger.info(f"writing trunk {len(df)} line...")
+
+        if sql_data_exists == 'append':
+            # if exist strategy is append, all trunk always append
+            current_data_exist = 'append'
+        elif sql_data_exists == 'fail':
+            # if exist strategy is fail, it should failed in first trunk
+            # in later trunk, it should be append
+            if i == 0:
+                current_data_exist = 'fail'
+            else:
+                current_data_exist = 'append'
+        elif sql_data_exists == 'replace':
+            if i == 0:
+                current_data_exist = 'replace'
+            else:
+                current_data_exist = 'append'
+        else:
+            raise ValueError(f"cannot parse current_data_exist value:{sql_data_exists}")
 
-    return df
+        with logger.catch(message="write to db error, loss chunk.", reraise=not ignore_error):
+            df.to_sql(
+                name=table_name,
+                con=conn,
+                index=index,
+                if_exists=current_data_exist,
+            )
 
 
 def csv2sql(
     sql_uri: str,
     table_name: str,
     filename: str,
     header: List[int] | Literal["infer"] | None = "infer",
@@ -31,35 +54,37 @@
     lineterminator: Optional[str] = None,
     sql_schema_file: str | None = None,
     sql_data_exists: Literal["fail", "replace", "append"] = "fail",
     read_chunk_size: Optional[int] = None,
     pandas_exprs: List[str] | None = None,
     debug: bool = False,
     ignore_error: bool = False,
+    insert_in_transaction: bool = True,
     **sql_kwargs: Any
 ):
     """
     convert csv to sql table.
     :param sql_uri: database uri, according to sqlalchemy uri, according to sqlalchemy uri, e.g. "mysql+pymysql://username:pass@host:port/database.
     :param table_name: csv data insert table name.
     :param filename: source csv filename.
-    :param header: default first line, also can provide by 'xxx,yyy,bbb' format.
+    :param header: default first line.
     :param names: specify the headers of csv file, e.g. 'a,b,c,d'.
     :param sep: sep symbol, ',' default.
     :param index: if generate index in result.
     :param quotechar: quote char, '"' default.
     :param escapechar: escape char, None default.
     :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
     :param sql_data_exists: action on data exist in sql db, can be 'fail' or 'replace' or 'append', default 'fail'.
     :param sql_schema_file: schema on create table, default None (auto generate with no index).
     :param read_chunk_line: if csv file is large, to reduce the memory usage, read csv to memory by trunk of lines.
-    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['expr1 xxxxx','expr2 xxx']".
+    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['df.drop([\"xxxx\"], axis=1)','expr2 xxx']".
     :param debug: if debug mod on, will print every result after exec pandas exprs.
     :param ignore_error: if ignore sql insert error, it may cause loss chunks of data.
+    :param insert_in_transaction: if insert data to db in transaction, default True.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
 
     Session = sessionmaker(engine)
     # handle sql schema
     # if replace, drop table and create according to schema
     # if append or fail, try create table if not exist according to schema
@@ -97,15 +122,15 @@
             names=names,
             header=header,
             quotechar=quotechar,
             escapechar=escapechar,
             lineterminator=lineterminator,
         )
         if pandas_exprs:
-            df = _exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
+            df = exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
         with engine.begin() as conn:
             df.to_sql(
                 name=table_name, con=conn, if_exists=sql_data_exists, index=index
             )
             logger.info(f"inserted {len(df)} rows")
     else:
         logger.info("converting csv to sql...")
@@ -116,46 +141,39 @@
             iterator=True,
             names=names,
             header=header,
             quotechar=quotechar,
             escapechar=escapechar,
             lineterminator=lineterminator,
         )
-        with engine.begin() as conn:
-            for i, df in enumerate(trunk_df):
-                if pandas_exprs:
-                    df = _exec_multi_expr(df, exprs=pandas_exprs, debug=debug)
-                df: pd.DataFrame
-                logger.info(f"writing trunk {len(df)} line...")
-
-                if sql_data_exists == 'append':
-                    # if exist strategy is append, all trunk always append
-                    current_data_exist = 'append'
-                elif sql_data_exists == 'fail':
-                    # if exist strategy is fail, it should failed in first trunk
-                    # in later trunk, it should be append
-                    if i == 0:
-                        current_data_exist = 'fail'
-                    else:
-                        current_data_exist = 'append'
-                elif sql_data_exists == 'replace':
-                    if i == 0:
-                        current_data_exist = 'replace'
-                    else:
-                        current_data_exist = 'append'
-                else:
-                    raise ValueError(f"cannot parse current_data_exist value:{sql_data_exists}")
+        if insert_in_transaction:
+            with engine.begin() as conn:
+                insert(
+                    trunk_df=trunk_df,
+                    pandas_exprs=pandas_exprs,
+                    debug=debug,
+                    sql_data_exists=sql_data_exists,
+                    ignore_error=ignore_error,
+                    table_name=table_name,
+                    conn=conn,
+                    index=index
+                )
+        else:
+            with engine.connect() as conn:
+                insert(
+                    trunk_df=trunk_df,
+                    pandas_exprs=pandas_exprs,
+                    debug=debug,
+                    sql_data_exists=sql_data_exists,
+                    ignore_error=ignore_error,
+                    table_name=table_name,
+                    conn=conn,
+                    index=index
+                )
 
-                with logger.catch(message="write to db error, loss chunk.", reraise=not ignore_error):
-                    df.to_sql(
-                        name=table_name,
-                        con=conn,
-                        index=index,
-                        if_exists=current_data_exist,
-                    )
 
         logger.info("done.")
 
 
 def main():
     Fire(csv2sql)
```

### Comparing `dataporter-0.1.4/dataporter/sql2csv.py` & `dataporter-0.1.5/dataporter/sql2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     :param header: if contains header in result.
     :param sep: sep symbol, ',' default.
     :param quotechar: quote char, '"' default.
     :param escapechar: escape char, None default.
     :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param read_chunk_size: if sql table is large, to reduce the memory usage, read sql to memory by trunk of lines, then write to local csv.
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
-    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['expr1 xxxxx','expr2 xxx']".
+    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['df.drop([\"xxxx\"], axis=1)','expr2 xxx']".
     :param debug: if debug mod on, will print every result after exec pandas exprs.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
     if read_chunk_size is None:
         with engine.begin() as conn:
             df = pd.read_sql(sql, conn)
         if pandas_exprs:
```

### Comparing `dataporter-0.1.4/dataporter/sql_schema2txt.py` & `dataporter-0.1.5/dataporter/sql_schema2txt.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.4/PKG-INFO` & `dataporter-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dataporter
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: convert csv to csv/sql or convert sql to csv
 Author: AuthorPlaceholder
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
```

