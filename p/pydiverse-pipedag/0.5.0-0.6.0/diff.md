# Comparing `tmp/pydiverse_pipedag-0.5.0.tar.gz` & `tmp/pydiverse_pipedag-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.5.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.6.0.tar", max compression
```

## Comparing `pydiverse_pipedag-0.5.0.tar` & `pydiverse_pipedag-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,69 @@
--rw-r--r--   0        0        0     1517 2023-06-28 08:54:22.346858 pydiverse_pipedag-0.5.0/LICENSE
--rw-r--r--   0        0        0     7229 2023-06-28 08:54:22.346858 pydiverse_pipedag-0.5.0/docs/package/README.md
--rw-r--r--   0        0        0     3212 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      355 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       88 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5334 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      357 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    11773 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2541 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      768 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3671 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0        0 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    21262 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7661 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    63798 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0    24570 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/sql_hooks.py
--rw-r--r--   0        0        0      171 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8461 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0     2257 2023-06-28 08:54:22.350858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0    43657 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0    12122 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table_cache.py
--rw-r--r--   0        0        0      397 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     8094 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    26404 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      243 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    13669 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    16460 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     3501 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5626 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     7731 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      332 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     2789 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     6536 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1447 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1703 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0      124 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8938 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     5422 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     9875 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2062 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    17445 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      177 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1093 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     2927 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4349 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1553 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2811 2023-06-28 08:54:22.354858 pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     8857 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-07-07 14:19:45.678347 pydiverse_pipedag-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7229 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/docs/package/README.md
+-rw-r--r--   0        0        0     3262 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      413 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5334 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13278 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2541 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      768 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3671 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    22728 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3106 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6503 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6800 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0       67 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    37136 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0      956 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0     3013 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0     7776 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     3706 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    20048 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4250 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    42398 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8579 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     7916 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    26249 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      279 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    13716 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    16460 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     3501 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5848 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     7731 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      368 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     2789 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     6536 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1447 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1734 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2700 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      160 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8991 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     5431 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     9875 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2074 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    16812 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3298 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     4349 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     8890 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.0/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.5.0/LICENSE` & `pydiverse_pipedag-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/docs/package/README.md` & `pydiverse_pipedag-0.6.0/docs/package/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         # print final sql statements
         print_sql: true
 
       local_table_cache:
         store_input: true
         store_output: true
         use_stored_input_as_cache: true
-        class: "pydiverse.pipedag.backend.table_cache.ParquetTableCache"
+        class: "pydiverse.pipedag.backend.table.cache.ParquetTableCache"
         args:
           base_path: "/tmp/pipedag/table_cache"
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
       args:
         base_path: "/tmp/pipedag/blobs"
```

### Comparing `pydiverse_pipedag-0.5.0/pyproject.toml` & `pydiverse_pipedag-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.5.0"
+version = "0.6.0"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -33,14 +33,15 @@
 packaging = ">=21.3"
 python-box = ">=6.1.0"
 PyYAML = ">=6.0"
 pyarrow = ">=11.0.0"
 cryptography = ">=41.0.1"
 pydot = ">=1.4.2"
 click = "^8.1.3"
+pyparsing = ">=3.0"
 
 filelock = { version = ">=3.7.1", optional = true }
 kazoo = { version = ">=2.8.0", optional = true }
 dask = { version = ">=2022.1.0", optional = true }
 
 
 [tool.poetry.extras]
@@ -50,15 +51,14 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 pytest-mock = ">=3.10.0"
 pytest-timeout = ">=2.1.0"
 
 black = { version = "23.3.0", extras = ["d"] }
-isort = "^5.10.1"
 ruff = "^0.0.270"
 pre-commit = ">=2.20.0"
 
 kazoo = ">=2.8.0"
 dask = ">=2022.1.0"
 psycopg2 = ">=2.9.3"
 duckdb = "^0.8.1"
@@ -66,15 +66,14 @@
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 # Table Hooks
 pydiverse-transform = "^0.1.3"
-ibis = ">=3.2.0"
 ibis-framework = { version = ">=5.1.0", extras = ["mssql", "postgres"] }
 polars = ">=0.16.18"
 tidypolars = { version = "^0.2.19", python = "<3.11" }
 connectorx = [
     { version = ">=0.3.1", python = "<3.11" },
     { version = "0.3.2a5", python = "==3.11" }  # Latest full release is broken - unpin when 0.3.2 released
 ]
@@ -113,29 +112,31 @@
 [tool.ruff]
 select = [
     "F",
     "E",
     "UP",
     "W",
     "I001",
+    "I002",
     "B",
     "A",
 ]
 ignore = [
     "B028",
 ]
 extend-exclude = ["docs/*"]
 ignore-init-module-imports = true
 fix = true
 target-version = "py38"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
-"src/pydiverse/pipedag/backend/table/util/sql_ddl.py" = ["F811"]
+"src/pydiverse/pipedag/backend/table/sql/ddl.py" = ["F811"]
 "tests/*" = ["F403", "F405"]
 
 [tool.ruff.isort]
 known-first-party = ["pydiverse"]
+required-imports = ["from __future__ import annotations"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/_typing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, TypeVar, Union
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Blob, Table
-    from pydiverse.pipedag.backend import BaseTableStore
+    from pydiverse.pipedag.backend.table.base import BaseTableStore, TableHookResolver
 
 
 def decorator_hint(decorator: Callable) -> Callable:
     # Used to fix incorrect type hints in pycharm
     return decorator
 
 
 T = TypeVar("T")
 CallableT = TypeVar("CallableT", bound=Callable)
 StoreT = TypeVar("StoreT", bound="BaseTableStore")
+TableHookResolverT = TypeVar("TableHookResolverT", bound="TableHookResolver")
 
 # Materializable
 MPrimitives = Union[int, float, bool, str]
 MTypes = Union["Table", "Blob"]
 
 BaseMaterializable = Union[MPrimitives, MTypes]
 Materializable = Union[
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
 import hashlib
 import threading
 import time
+import warnings
 from abc import ABC, abstractmethod
 from typing import Any
 
 import sqlalchemy as sa
 
 from pydiverse.pipedag import ConfigContext, Stage
 from pydiverse.pipedag.backend.lock.base import BaseLockManager, Lockable, LockState
-from pydiverse.pipedag.backend.table.util import engine_dispatch
-from pydiverse.pipedag.backend.table.util.sql_ddl import (
+from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateSchema,
     Schema,
-    ibm_db_sa_fix_name,
 )
 from pydiverse.pipedag.errors import LockError
 
 
 class DatabaseLockManager(BaseLockManager):
     """Lock manager based on database locking mechanisms
 
@@ -27,14 +26,31 @@
     level (where each stage can be locked and unlocked individually), or only on
     the instance level (where the entire instance including all stages get locked and
     unlocked together).
 
     The database specific lock implementations can be found at the end of the file.
     """
 
+    __registered_dialects: dict[str, type[DatabaseLockManager]] = {}
+    _dialect_name: str
+
+    def __new__(cls, engine: sa.Engine, *args, **kwargs):
+        if cls != DatabaseLockManager:
+            return super().__new__(cls)
+
+        # If calling DatabaseLockManager(engine), then we want to dynamically
+        # instantiate the correct dialect specific subclass based on the engine dialect.
+        dialect = engine.dialect.name
+        dialect_specific_cls = DatabaseLockManager.__registered_dialects.get(
+            dialect, cls
+        )
+        return super(DatabaseLockManager, dialect_specific_cls).__new__(
+            dialect_specific_cls
+        )
+
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
         assert (
             len(config) == 0
         ), "DatabaseLockManager doesn't take any additional arguments"
 
         cfg_context = ConfigContext.get()
@@ -47,46 +63,70 @@
         table_store = config_context.store.table_store
         if not isinstance(table_store, SQLTableStore):
             raise TypeError("Table Store must be a subclass of SQLTableStore")
 
         engine = table_store.get_engine_for_locking()
         instance_id = config_context.instance_id
         lock_schema = table_store.get_lock_schema()
+        create_lock_schema = not table_store.avoid_drop_create_schema
 
-        return cls(engine, instance_id, lock_schema)
+        return cls(engine, instance_id, lock_schema, create_lock_schema)
 
     def __init__(
-        self, engine: sa.Engine, instance_id: str, lock_schema: Schema | None = None
+        self,
+        engine: sa.Engine,
+        instance_id: str,
+        lock_schema: Schema | None = None,
+        create_lock_schema: bool = True,
     ):
         super().__init__()
 
         self.engine = engine
         self.instance_id = instance_id
         self.lock_schema = lock_schema
+        self.create_lock_schema = create_lock_schema
 
         # Stage level locking
         self.connection = None
         self.locks: dict[Lockable, Lock] = {}
 
         # Instance level locking
         self.il_lock: Lock | None = None
         self.il_locks: set[Lockable] = set()
         self.__il_threading_lock = threading.Lock()
 
         # Prepare database
         self.prepare()
 
-    @engine_dispatch
+    def __init_subclass__(cls, **kwargs):
+        # Whenever a new subclass if DatabaseLockManager is defined, it must contain the
+        # `_dialect_name` attribute. This allows us to dynamically instantiate it
+        # when DatabaseLockManager SQLTableStore(engine, ...) based on the dialect
+        # of the engine (see __new__).
+        dialect_name = getattr(cls, "_dialect_name", None)
+        if dialect_name is None:
+            raise ValueError(
+                "All subclasses of DatabaseLockManager must have a `_dialect_name`"
+                f"attribute. But {cls.__name__}._dialect_name is None."
+            )
+
+        if dialect_name in DatabaseLockManager.__registered_dialects:
+            warnings.warn(
+                f"Already registered a DatabaseLockManager for dialect {dialect_name}"
+            )
+        DatabaseLockManager.__registered_dialects[dialect_name] = cls
+
     def prepare(self):
-        ...
+        pass
 
-    @prepare.dialect("mssql")
-    @prepare.dialect("ibm_db_sa")
-    def __prepare(self):
+    def _prepare_create_lock_schema(self):
         # Create the lock schema
+        if not self.create_lock_schema:
+            return
+
         # If two lock managers do this concurrently, this action might fail. Thus,
         # we retry a second time to ensure the schema exists.
         with self.engine.connect() as conn:
             exception = None
             for _ in range(3):
                 try:
                     with conn.begin():
@@ -100,15 +140,15 @@
 
     def dispose(self):
         self.engine.dispose()
         super().dispose()
 
     @property
     def supports_stage_level_locking(self):
-        return self.engine.dialect.name not in ["ibm_db_sa"]
+        raise NotImplementedError
 
     def acquire(self, lockable: Lockable):
         if self.supports_stage_level_locking:
             lock = self.get_lock_object(lockable)
             self.logger.info(f"Locking '{lockable}'")
             if not lock.acquire():
                 raise LockError(f"Failed to acquire lock '{lockable}'")
@@ -147,42 +187,19 @@
                 self.il_locks.remove(lockable)
                 self.set_lock_state(lockable, LockState.UNLOCKED)
 
                 if len(self.il_locks) == 0:
                     self.logger.info("Unlocking at instance level")
                     self.il_lock.release()
 
-    @engine_dispatch
     def get_lock_object(self, lockable: Lockable):
-        raise NotImplementedError(f"Dialect '{self.engine.dialect}' not supported")
-
-    @get_lock_object.dialect("postgresql")
-    def __get_lock_object(self, lockable: Lockable):
-        if self.connection is None:
-            self.connection = self.engine.connect()
-
-        name = self.lock_name(lockable)
-        return PostgresLock(name, self.connection)
-
-    @get_lock_object.dialect("mssql")
-    def __get_lock_object(self, lockable: Lockable):
-        if self.connection is None:
-            self.connection = self.engine.connect()
-
-        name = self.lock_name(lockable)
-        database, _ = self.lock_schema.get().split(".")
-        return MSSqlLock(name, database, self.connection)
+        raise NotImplementedError(f"Dialect '{self.engine.dialect.name}' not supported")
 
-    @engine_dispatch
     def get_instance_level_lock(self):
-        raise NotImplementedError(f"Dialect '{self.engine.dialect}' not supported")
-
-    @get_instance_level_lock.dialect("ibm_db_sa")
-    def __get_instance_level_lock(self):
-        return DB2Lock("instance_lock", self.lock_schema.get(), self.engine)
+        raise NotImplementedError(f"Dialect '{self.engine.dialect.name}' not supported")
 
     def lock_name(self, lock: Lockable):
         if isinstance(lock, Stage):
             return self.instance_id + "#" + lock.name
         elif isinstance(lock, str):
             return self.instance_id + "#" + lock
         else:
@@ -218,47 +235,57 @@
         digest = hashlib.sha256(name.encode("utf-8")).digest()
         self._id = int.from_bytes(digest[:8], byteorder="big", signed=True)
 
         self._connection = connection
         self._locked = False
 
     def acquire(self) -> bool:
-        result = self._connection.execute(
-            sa.text(f"SELECT pg_catalog.pg_advisory_lock({self._id})")
+        result = self._connection.exec_driver_sql(
+            f"SELECT pg_catalog.pg_advisory_lock({self._id})"
         ).scalar()
         result = False if result is False else True
         self._locked = result
         return result
 
     def release(self) -> bool:
-        result = self._connection.execute(
-            sa.text(f"SELECT pg_catalog.pg_advisory_unlock({self._id})")
+        result = self._connection.exec_driver_sql(
+            f"SELECT pg_catalog.pg_advisory_unlock({self._id})"
         ).scalar()
         self._locked = False
         return False if result is False else True
 
     @property
     def locked(self) -> bool:
         return self._locked
 
 
+class PostgresLockManager(DatabaseLockManager):
+    _dialect_name = "postgresql"
+    supports_stage_level_locking = True
+
+    def get_lock_object(self, lockable: Lockable):
+        if self.connection is None:
+            self.connection = self.engine.connect()
+
+        name = self.lock_name(lockable)
+        return PostgresLock(name, self.connection)
+
+
 class MSSqlLock(Lock):
     """
     Locking based on application resource locks.
     https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-getapplock-transact-sql?view=sql-server-ver15
     """
 
-    def __init__(self, name: str, database: str, connection: sa.Connection):
+    def __init__(self, name: str, connection: sa.Connection):
         self.name = name
-        self._database = database
         self._connection = connection
         self._locked = False
 
     def acquire(self) -> bool:
-        self._connection.execute(sa.text(f"USE [{self._database}]"))
         result = self._connection.execute(
             sa.text(
                 """
                 DECLARE @result int
                 EXEC @result =
                     sp_getapplock
                         @Resource = :lock_name,
@@ -270,15 +297,14 @@
             {"lock_name": self.name},
         ).scalar()
         result = result >= 0
         self._locked = result
         return result
 
     def release(self) -> bool:
-        self._connection.execute(sa.text(f"USE [{self._database}]"))
         result = self._connection.execute(
             sa.text(
                 """
                 DECLARE @result int
                 EXEC @result =
                     sp_releaseapplock
                         @Resource = :lock_name,
@@ -293,14 +319,26 @@
         return result
 
     @property
     def locked(self) -> bool:
         return self._locked
 
 
+class MSSqlLockManager(DatabaseLockManager):
+    _dialect_name = "mssql"
+    supports_stage_level_locking = True
+
+    def get_lock_object(self, lockable: Lockable):
+        if self.connection is None:
+            self.connection = self.engine.connect()
+
+        name = self.lock_name(lockable)
+        return MSSqlLock(name, self.connection)
+
+
 class DB2Lock(Lock):
     """
     Locking based on 'LOCK TABLE' statements.
     https://www.ibm.com/docs/en/db2-for-zos/13?topic=statements-lock-table
 
     These locks can only be released by committing a transaction. Therefor it is
     not suitable for fine grain locking.
@@ -311,41 +349,35 @@
         self._connection = None
         self._locked = False
 
         self.table = table
         self.schema = schema
 
     def acquire(self) -> bool:
-        table = self._engine.dialect.identifier_preparer.quote_identifier(
-            ibm_db_sa_fix_name(self.table)
-        )
-        schema = self._engine.dialect.identifier_preparer.format_schema(
-            ibm_db_sa_fix_name(self.schema)
-        )
+        table = self._engine.dialect.identifier_preparer.quote(self.table)
+        schema = self._engine.dialect.identifier_preparer.format_schema(self.schema)
 
         # CREATE TABLE IF NOT EXISTS
         with self._engine.begin() as conn:
-            conn.execute(
-                sa.text(
-                    f"""
-                    BEGIN
-                        DECLARE CONTINUE HANDLER FOR SQLSTATE '42710' BEGIN END;
-                        EXECUTE IMMEDIATE 'CREATE TABLE {schema}.{table} (x int)';
-                    END
-                    """
-                )
+            conn.exec_driver_sql(
+                f"""
+                BEGIN
+                    DECLARE CONTINUE HANDLER FOR SQLSTATE '42710' BEGIN END;
+                    EXECUTE IMMEDIATE 'CREATE TABLE {schema}.{table} (x int)';
+                END
+                """
             )
 
         # LOCK TABLE
         if self._connection is None:
             self._connection = self._engine.connect()
             self._connection.begin()
 
-        self._connection.execute(
-            sa.text(f"LOCK TABLE {schema}.{table} IN EXCLUSIVE MODE")
+        self._connection.exec_driver_sql(
+            f"LOCK TABLE {schema}.{table} IN EXCLUSIVE MODE"
         )
 
         self._locked = True
         return True
 
     def release(self) -> bool:
         if self._connection is None:
@@ -354,7 +386,18 @@
         self._connection.close()
         self._locked = False
         return True
 
     @property
     def locked(self) -> bool:
         return self._locked
+
+
+class DB2LockManager(DatabaseLockManager):
+    _dialect_name = "ibm_db_sa"
+    supports_stage_level_locking = False
+
+    def prepare(self):
+        self._prepare_create_lock_schema()
+
+    def get_instance_level_lock(self):
+        return DB2Lock("instance_lock", self.lock_schema.get(), self.engine)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 from __future__ import annotations
 
-from abc import ABC, ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
+from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, Generic
 
 import structlog
 from typing_extensions import Self
 
-from pydiverse.pipedag._typing import StoreT, T
+from pydiverse.pipedag._typing import T, TableHookResolverT
 from pydiverse.pipedag.context import RunContext, TaskContext
 from pydiverse.pipedag.materialize.cache import CacheManager
 from pydiverse.pipedag.materialize.container import RawSql, Table
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.util import Disposable, requires
 from pydiverse.pipedag.util.hashing import stable_hash
-from pydiverse.pipedag.util.naming import NameDisambiguator
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Stage
+    from pydiverse.pipedag.backend.table.cache.base import BaseTableCache
     from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 
 
-class _TableStoreMeta(ABCMeta):
-    """TableStore Metaclass
-
-    Add the `_REGISTERED_TABLES`, `_M_TABLE_CACHE` and `_R_TABLE_CACHE`
-    attributes to all table stores.
-    """
-
-    def __new__(mcs, name, bases, attrs, **kwargs):
-        cls = super().__new__(mcs, name, bases, attrs, **kwargs)
-
-        cls._REGISTERED_TABLES = []
-        cls._M_TABLE_CACHE = {}
-        cls._R_TABLE_CACHE = {}
-
-        return cls
-
-
-class TableHookResolver(Disposable, metaclass=_TableStoreMeta):
-    _REGISTERED_TABLES: list[TableHook]
-    _M_TABLE_CACHE: dict[type, TableHook]
-    _R_TABLE_CACHE: dict[type, TableHook]
+class TableHookResolver:
+    _registered_table_hooks: list[type[TableHook]] = []
+    _m_hook_cache: dict[type, type[TableHook]] = {}
+    _r_hook_cache: dict[type, type[TableHook]] = {}
+    _hook_subclass_cache: dict[type, type[TableHook]] = {}
 
     @classmethod
     def register_table(cls, *requirements: Any):
         """Decorator to register a `TableHook`
 
         Each table store should be able to handle tables of various different
         types (e.g. a pandas dataframe, a sqlalchemy select statement, a
@@ -67,60 +52,94 @@
             def XTableHook(TableHook):
                 ...
 
         :param requirements: The requirements which must be satisfied to register
             the decorated class.
         """
 
+        # `cls` is very likely a subclass of TableHookResolver
+        # -> Add the hook related attributes to subclass to allow registering
+        #    new hooks without interfering with the superclass.
+        if "_registered_table_hooks" not in cls.__dict__:
+            cls._registered_table_hooks = []
+            cls._m_hook_cache = {}
+            cls._r_hook_cache = {}
+            cls._hook_subclass_cache = {}
+
         def decorator(hook_cls):
             if not all(requirements):
                 return requires(
                     False,
                     Exception(f"Not all requirements met for {hook_cls.__name__}"),
                 )(hook_cls)
 
             # Register the hook
-            cls._REGISTERED_TABLES.append(hook_cls)
-            cls._M_TABLE_CACHE.clear()
-            cls._R_TABLE_CACHE.clear()
+            cls._registered_table_hooks.append(hook_cls)
+            cls._m_hook_cache.clear()
+            cls._r_hook_cache.clear()
+            cls._hook_subclass_cache.clear()
             return hook_cls
 
         return decorator
 
-    def get_m_table_hook(self: Self, type_: type[T]) -> TableHook[Self]:
+    def __registered_tables(self) -> Iterable[type[TableHook]]:
+        # Walk up the hierarchy of super classes and return each registered
+        # table hook in reverse order
+        for cls in type(self).__mro__:
+            if "_registered_table_hooks" in cls.__dict__:
+                yield from cls._registered_table_hooks[::-1]  # noqa
+
+    def get_m_table_hook(self: Self, type_: type[T]) -> type[TableHook[Self]]:
         """Get a table hook that can materialize the specified type"""
-        if type_ in self._M_TABLE_CACHE:
-            return self._M_TABLE_CACHE[type_]
-        for hook in self._REGISTERED_TABLES:
+        if type_ in self._m_hook_cache:
+            return self._m_hook_cache[type_]
+
+        for hook in self.__registered_tables():
             if hook.can_materialize(type_):
-                self._M_TABLE_CACHE[type_] = hook
+                self._m_hook_cache[type_] = hook
                 return hook
+
         raise TypeError(f"Can't materialize Table with underlying type {type_}")
 
-    def get_r_table_hook(self: Self, type_: type[T] | tuple | dict) -> TableHook[Self]:
+    def get_r_table_hook(
+        self: Self, type_: type[T] | tuple | dict
+    ) -> type[TableHook[Self]]:
         """Get a table hook that can retrieve the specified type"""
         if isinstance(type_, tuple):
             type_ = type_[0]
         elif isinstance(type_, dict):
             type_ = type_["type"]
 
-        if type_ in self._R_TABLE_CACHE:
-            return self._R_TABLE_CACHE[type_]
-        for hook in self._REGISTERED_TABLES:
+        if type_ in self._r_hook_cache:
+            return self._r_hook_cache[type_]
+
+        for hook in self.__registered_tables():
             if hook.can_retrieve(type_):
-                self._R_TABLE_CACHE[type_] = hook
+                self._r_hook_cache[type_] = hook
                 return hook
+
         raise TypeError(f"Can't retrieve Table as type {type_}")
 
+    def get_hook_subclass(self, type_: type[TableHook[T]]) -> type[TableHook[T]]:
+        """Finds a table hook that is a subclass of the provided type"""
+        if type_ in self._hook_subclass_cache:
+            return self._hook_subclass_cache[type_]
+
+        for hook in self.__registered_tables():
+            if issubclass(hook, type_):
+                self._hook_subclass_cache[type_] = hook
+                return hook
+
+        return type_
+
     def store_table(
         self,
         table: Table,
         task: MaterializingTask | None,
         task_info: TaskInfo | None,
-        use_transaction_name=True,
     ):
         """Stores a table in the associated transaction stage
 
         The store must convert the table object (`table.obj`) to the correct
         internal type. This means, that in some cases it first has to
         evaluate a lazy object. For example: if a sql based table store
         receives a sql query to store, it has to execute it first.
@@ -132,25 +151,20 @@
         # In case of deferred operations, inform run context that stage
         # isn't 100% cache valid anymore.
         if task is not None:
             RunContext.get().set_stage_has_changed(task.stage)
 
         # Materialize
         hook = self.get_m_table_hook(type(table.obj))
-        stage_name = (
-            table.stage.transaction_name if use_transaction_name else table.stage.name
-        )
-        hook.materialize(self, table, stage_name, task_info)
+        hook.materialize(self, table, table.stage.transaction_name, task_info)
 
     def retrieve_table_obj(
         self,
         table: Table,
         as_type: type[T],
-        namer: NameDisambiguator | None = None,
-        use_transaction_name=True,
     ) -> T:
         """Loads a table from the store
 
         Retrieves the table from the store, converts it to the correct
         If the stage hasn't yet been committed, the table must be retrieved
         from the transaction, else it must be retrieved from the committed
         stage.
@@ -162,25 +176,21 @@
         if as_type is None:
             raise TypeError(
                 "Missing 'as_type' argument. You must specify a type to be able "
                 "to dematerialize a Table."
             )
 
         hook = self.get_r_table_hook(as_type)
-        stage_name = (
-            table.stage.current_name if use_transaction_name else table.stage.name
-        )
-
         try:
-            return hook.retrieve(self, table, stage_name, as_type, namer)
+            return hook.retrieve(self, table, table.stage.current_name, as_type)
         except Exception as e:
             raise RuntimeError(f"Failed to retrieve table '{table}'") from e
 
 
-class BaseTableStore(TableHookResolver):
+class BaseTableStore(TableHookResolver, Disposable):
     """Table store base class
 
     The table store is responsible for storing and retrieving various types
     of tabular data. Additionally, it also has to manage all task metadata,
     This includes storing it, but also cleaning up stale metadata.
 
     A store must use a table's name (`table.name`) and stage (`table.stage`)
@@ -201,14 +211,15 @@
     or cache) with the 'transaction schema'. This is usually done by renaming
     them.
 
     """
 
     def __init__(self):
         self.logger = structlog.get_logger(logger_name=type(self).__name__)
+        self.local_table_cache: BaseTableCache | None = None
 
     def setup(self):
         """Setup function
 
         This function gets called at the beginning of a flow run.
         Unlike the __init__ method, a lock is acquired before
         the setup method gets called to prevent race conditions.
@@ -238,14 +249,24 @@
 
         Additionally, the metadata associated with the transaction schema should
         replace the metadata of the base schema. The latter can be discarded.
         """
 
     # Materialize
 
+    def store_table(
+        self,
+        table: Table,
+        task: MaterializingTask | None,
+        task_info: TaskInfo | None,
+    ):
+        super().store_table(table, task, task_info)
+        if self.local_table_cache:
+            self.local_table_cache.store_table(table, task, task_info)
+
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage
 
         This method is overridden by actual table stores that can handle raw SQL.
         """
 
         raise NotImplementedError(
@@ -317,18 +338,26 @@
 
         table_cache_info = CacheManager.raw_sql_cache_lookup(
             self, task_info.task_cache_info, raw_sql, query_hash
         )
         if not table_cache_info.is_cache_valid():
             TaskContext.get().is_cache_valid = False
             RunContext.get().set_stage_has_changed(task.stage)
-            prev_tables = self.list_tables(raw_sql.stage, include_everything=True)
+
+            prev_objects = self.get_objects_in_stage(raw_sql.stage)
             self.execute_raw_sql(raw_sql)
-            post_tables = self.list_tables(raw_sql.stage, include_everything=True)
-            table_cache_info.store_raw_sql_metadata(self, prev_tables, post_tables)
+            post_objects = self.get_objects_in_stage(raw_sql.stage)
+
+            # Object names must be sorted to ensure that we can identify the task
+            # again in the future even if the objects get returned in a different order.
+            prev_objects = sorted(prev_objects)
+
+            prev_objects_set = set(prev_objects)
+            new_objects = [o for o in post_objects if o in prev_objects_set]
+            table_cache_info.store_raw_sql_metadata(self, prev_objects, new_objects)
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
         raw_sql.cache_key = CacheManager.lazy_table_cache_key(
             task_info.task_cache_info.get_task_cache_key(), query_hash
         )
 
@@ -371,14 +400,33 @@
     @abstractmethod
     def delete_table_from_transaction(self, table: Table):
         """Delete a table from the transaction
 
         If the table doesn't exist in the transaction stage, fail silently.
         """
 
+    def retrieve_table_obj(
+        self,
+        table: Table,
+        as_type: type[T],
+    ) -> T:
+        if self.local_table_cache:
+            obj = self.local_table_cache.retrieve_table_obj(table, as_type)
+            if obj is not None:
+                return obj
+
+        obj = super().retrieve_table_obj(table, as_type)
+
+        if self.local_table_cache:
+            t = table.copy_without_obj()
+            t.obj = obj
+            self.local_table_cache.store_input(t, task=None, task_info=None)
+
+        return obj
+
     # Metadata
 
     @abstractmethod
     def store_task_metadata(self, metadata: TaskMetadata, stage: Stage):
         """Stores the metadata of a task
 
         The metadata must always be stored in such a way that it is
@@ -460,33 +508,29 @@
         raise NotImplementedError(
             "This table store does not support executing raw sql statements"
         )
 
     # Utility
 
     @abstractmethod
-    def list_tables(self, stage: Stage, *, include_everything=False) -> list[str]:
+    def get_objects_in_stage(self, stage: Stage) -> list[str]:
         """
-        List all tables that were generated in a stage.
+        List all objects that are in the current stage.
 
-        It may also include other objects database objects like views, stored
-        procedures, functions, etc. which makes the name `list_tables` too specific.
-        But the predominant idea is that tasks produce tables in stages and thus the
-        storyline of callers is much nicer to read. In the end we might need everything
-        to recover the full cache output which was produced by a RawSQL statement
-        (we want to be compatible with legacy sql code as a starting point).
+        This may include tables but also other database objects like views, stored
+        procedures, functions etc. This function is used to calculate a diff on the
+        table store to determine which objects were produced (or could have been used
+        to produce those objects) when executing RawSQL.
 
         :param stage: the stage
-        :param include_everything: If True, we might include stored procedures,
-            functions and other database objects that have a schema associated name.
-        :return: list of tables [and other objects]
+        :return: list of object names in the stage at the current point in time.
         """
 
 
-class TableHook(Generic[StoreT], ABC):
+class TableHook(Generic[TableHookResolverT], ABC):
     """Base class to define how to handle a specific table
 
     For more information, take a look at the `BaseTableStore.register_table`
     documentation.
     """
 
     __slots__ = ()
@@ -509,15 +553,15 @@
         `retrieve` method MUST be implemented for the type.
         """
 
     @classmethod
     @abstractmethod
     def materialize(
         cls,
-        store: StoreT,
+        store: TableHookResolverT,
         table: Table,
         stage_name: str,
         task_info: TaskInfo,
     ) -> None:
         """Materialize a table object
 
         :param store: The store which called this method
@@ -527,28 +571,26 @@
         :param task_info: Information about task execution
         """
 
     @classmethod
     @abstractmethod
     def retrieve(
         cls,
-        store: StoreT,
+        store: TableHookResolverT,
         table: Table,
         stage_name: str,
         as_type: type[T] | tuple | dict[str, Any],
-        namer: NameDisambiguator | None = None,
     ) -> T:
         """Retrieve a table from the store
 
         :param store: The store in which the table is stored
         :param table: The table which should get retrieved
         :param stage_name: The name of the stage from which te table should
             be retrieved
         :param as_type: The type as which the table is to be retrieved
-        :param namer: Helper object which ensures unique alias names
         :return: The retrieved table (converted to the correct type)
         """
 
     @classmethod
     def auto_table(cls, obj: T) -> Table[T]:
         """Wrap an object inside a `Table`
 
@@ -558,15 +600,15 @@
 
         :param obj: The object which should get wrapped inside a `Table`
         :return: The `Table` object which wraps `obj`
         """
         return Table(obj)
 
     @classmethod
-    def lazy_query_str(cls, store: StoreT, obj) -> str:
+    def lazy_query_str(cls, store: TableHookResolverT, obj) -> str:
         """String that represents the associated object
 
         Can either be a literal query string (e.g. SQL query), or a string that
         uniquely represents the query in some other way. Used for computing
         the cache key for materializing tasks with `lazy=True`.
 
         :raises TypeError: if the type doesn't support lazy queries.
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,31 +116,16 @@
     ) -> LazyTableMetadata:
         try:
             cache_key = query_hash + task_hash
             return self.lazy_table_metadata[stage.name][cache_key]
         except (TypeError, KeyError):
             raise CacheError("Couldn't find metadata for lazy table") from None
 
-    def list_tables(self, stage, *, include_everything=False):
-        """
-        List all tables that were generated in a stage.
-
-        It may also include other objects database objects like views, stored
-        procedures, functions, etc. which makes the name `list_tables` too specific.
-        But the predominant idea is that tasks produce tables in stages and thus the
-        storyline of callers is much nicer to read. In the end we might need everything
-        to recover the full cache output which was produced by a RawSQL statement
-        (we want to be compatible with legacy sql code as a starting point).
-
-        :param stage: the stage
-        :param include_everything: If True, we might include stored procedures,
-            functions and other database objects that have a schema associated name.
-        :return: list of tables [and other objects]
-        """
-        return self.store[stage.transaction_name].keys()
+    def get_objects_in_stage(self, stage):
+        return list(self.store[stage.transaction_name].keys())
 
 
 @DictTableStore.register_table(pd)
 class PandasTableHook(TableHook[DictTableStore]):
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(type_, pd.DataFrame)
@@ -159,15 +144,15 @@
     ):
         _ = task_info
         if table.name is not None:
             table.obj.attrs["name"] = table.name
         store.store[stage_name][table.name] = table.obj
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type, namer):
+    def retrieve(cls, store, table, stage_name, as_type):
         return store.store[stage_name][table.name].copy()
 
     @classmethod
     def auto_table(cls, obj: pd.DataFrame):
         if name := obj.attrs.get("name"):
             return Table(obj, name)
         return super().auto_table(obj)
@@ -204,17 +189,17 @@
         from pydiverse.transform.core.verbs import collect
 
         table.obj = table.obj >> collect()
         # noinspection PyTypeChecker
         return PandasTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
-    def retrieve(cls, store, table, stage_name, as_type, namer):
+    def retrieve(cls, store, table, stage_name, as_type):
         from pydiverse.transform.eager import PandasTableImpl
 
-        df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame, namer)
+        df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame)
         return pdt.Table(PandasTableImpl(table.name, df))
 
     @classmethod
     def auto_table(cls, obj: pdt.Table):
         # noinspection PyProtectedMember
         return Table(obj, obj._impl.name)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 from __future__ import annotations
 
-import itertools
 import json
-import re
 import textwrap
-import time
+import warnings
 from collections.abc import Iterable
 from contextlib import contextmanager
 from typing import Any
 
 import sqlalchemy as sa
 import sqlalchemy.exc
 import sqlalchemy.sql.elements
 
 from pydiverse.pipedag import Stage, Table
 from pydiverse.pipedag.backend.table.base import BaseTableStore
-from pydiverse.pipedag.backend.table.util import engine_dispatch
-from pydiverse.pipedag.backend.table.util.sql_ddl import (
+from pydiverse.pipedag.backend.table.sql.ddl import (
     AddIndex,
     AddPrimaryKey,
-    ChangeColumnNullable,
-    ChangeColumnTypes,
     CopyTable,
     CreateAlias,
     CreateDatabase,
     CreateSchema,
-    CreateViewAsSelect,
     DropAlias,
-    DropFunction,
-    DropProcedure,
     DropSchema,
+    DropSchemaContent,
     DropTable,
-    DropView,
     RenameSchema,
     RenameTable,
     Schema,
-    ibm_db_sa_fix_name,
     split_ddl_statement,
 )
 from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.context.context import ConfigContext, StageCommitTechnique
 from pydiverse.pipedag.context.run_context import DeferredTableStoreOp
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.container import RawSql
@@ -60,281 +51,225 @@
     transaction. If all tasks inside a stage succeed, swaps the schemas by
     renaming them.
     """
 
     METADATA_SCHEMA = "pipedag_metadata"
     LOCK_SCHEMA = "pipedag_locks"
 
+    __registered_dialects: dict[str, type[SQLTableStore]] = {}
+    _dialect_name: str
+
+    def __new__(cls, engine_url: str, *args, **kwargs):
+        if cls != SQLTableStore:
+            return super().__new__(cls)
+
+        # If calling SQLTableStore(engine_url), then we want to dynamically instantiate
+        # the correct dialect specific subclass based on the dialect found in the url.
+        dialect = sa.engine.make_url(engine_url).get_dialect().name
+        dialect_specific_cls = SQLTableStore.__registered_dialects.get(dialect, cls)
+        return super(SQLTableStore, dialect_specific_cls).__new__(dialect_specific_cls)
+
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
         config = config.copy()
         engine_url = config.pop("url")
         return cls(engine_url, **config)
 
     def __init__(
         self,
         engine_url: str,
         *,
         create_database_if_not_exists: bool = False,
         schema_prefix: str = "",
         schema_suffix: str = "",
         avoid_drop_create_schema: bool = False,
-        disable_pytsql: bool = False,
-        pytsql_isolate_top_level_statements: bool = True,
         print_materialize: bool = False,
         print_sql: bool = False,
         no_db_locking: bool = True,
-        unlogged_tables: bool = False,
     ):
         """
         Construct table store.
 
         :param engine_url:
             URL for SQLAlchemy engine
         :param create_database_if_not_exists:
             whether to create database if it does not exist
         :param schema_prefix:
-            prefix string for schemas (dot is interpreted as database.schema)
+            prefix string for schemas
         :param schema_suffix:
-            suffix string for schemas (dot is interpreted as database.schema)
+            suffix string for schemas
         :param avoid_drop_create_schema
             avoid creating and dropping schemas
-        :param disable_pytsql:
-            whether to disable the use of pytsql (dialect mssql only)
-        :param pytsql_isolate_top_level_statements:
-            forward pytsql executes() parameter
         :param print_materialize:
             whether to print select statements before materialization
         :param print_sql:
             whether to print final SQL statements (except for metadata)
         :param no_db_locking:
             speed up database by telling it we will not rely on it's locking mechanisms
-        :param unlogged_tables:
-            whether to use UNLOGGED tables or not (dialect postgresql only)
         """
         super().__init__()
 
         self.create_database_if_not_exists = create_database_if_not_exists
         self.schema_prefix = schema_prefix
         self.schema_suffix = schema_suffix
-        self.disable_pytsql = disable_pytsql
         self.avoid_drop_create_schema = avoid_drop_create_schema
-        self.pytsql_isolate_top_level_statements = pytsql_isolate_top_level_statements
         self.print_materialize = print_materialize
         self.print_sql = print_sql
         self.no_db_locking = no_db_locking
-        self.unlogged_tables = unlogged_tables
-        self.metadata_schema = self.get_schema(self.METADATA_SCHEMA)
 
+        self.metadata_schema = self.get_schema(self.METADATA_SCHEMA)
         self.engine_url = sa.engine.make_url(engine_url)
         self.engine = self._create_engine()
-        self.engines_other = dict()  # i.e. for IBIS connection
+
+        # Dict where hooks are allowed to store values that should get cached
+        self.hook_cache = {}
 
         self._init_database()
 
         # Set up metadata tables and schema
-        from sqlalchemy import CLOB, BigInteger, Boolean, Column, DateTime, String
-
-        if self.engine.dialect.name == "ibm_db_sa":
-            clob_type = CLOB  # VARCHAR(MAX) does not exist
-        else:
-            clob_type = String  # VARCHAR(MAX)s
-
-        self.sql_metadata = sa.MetaData()
-
-        # Stage Table is unique for stage
-        # (we currently cannot version changes of this metadata table when using
-        # stage_commit_tequnique=read_views)
-
-        def autoincrement_pk(name: str, seq_name: str):
-            if self.engine.dialect.name == "duckdb":
-                sequence = sqlalchemy.Sequence(
-                    f"{seq_name}_{name}_seq", schema=self.metadata_schema.get()
-                )
-                return Column(
-                    name,
-                    BigInteger,
-                    sequence,
-                    server_default=sequence.next_value(),
-                    primary_key=True,
-                )
-
-            return Column(name, BigInteger, primary_key=True, autoincrement=True)
-
-        self.stage_table = sa.Table(
-            "stages",
-            self.sql_metadata,
-            autoincrement_pk("id", "stages"),
-            Column("stage", String(64)),
-            Column("cur_transaction_name", String(256)),
-            schema=self.metadata_schema.get(),
-        )
+        self.sql_metadata = sa.MetaData(schema=self.metadata_schema.get())
 
         # Store version number for metadata table schema evolution.
         # We disable caching in case of version mismatch.
         self.disable_caching = False
-        self.metadata_version = "0.3.0"  # Increase version if metadata table changes
+        self.metadata_version = "0.3.1"  # Increase version if metadata table changes
         self.version_table = sa.Table(
             "metadata_version",
             self.sql_metadata,
-            Column("version", String(32)),
-            schema=self.metadata_schema.get(),
+            sa.Column("version", sa.String(32)),
+        )
+
+        # Stage Table is unique for stage
+        self.stage_table = sa.Table(
+            "stages",
+            self.sql_metadata,
+            self._metadata_pk("id", "stages"),
+            sa.Column("stage", sa.String(64)),
+            sa.Column("cur_transaction_name", sa.String(256)),
         )
 
         # Task Table is unique for stage * in_transaction_schema
         self.tasks_table = sa.Table(
             "tasks",
             self.sql_metadata,
-            autoincrement_pk("id", "tasks"),
-            Column("name", String(128)),
-            Column("stage", String(64)),
-            Column("version", String(64)),
-            Column("timestamp", DateTime),
-            Column("run_id", String(20)),
-            Column("position_hash", String(20)),
-            Column("input_hash", String(20)),
-            Column("cache_fn_hash", String(20)),
-            Column("output_json", clob_type),
-            Column("in_transaction_schema", Boolean),
-            schema=self.metadata_schema.get(),
+            self._metadata_pk("id", "tasks"),
+            sa.Column("name", sa.String(128)),
+            sa.Column("stage", sa.String(64)),
+            sa.Column("version", sa.String(64)),
+            sa.Column("timestamp", sa.DateTime()),
+            sa.Column("run_id", sa.String(20)),
+            sa.Column("position_hash", sa.String(20)),
+            sa.Column("input_hash", sa.String(20)),
+            sa.Column("cache_fn_hash", sa.String(20)),
+            sa.Column("output_json", sa.Text()),
+            sa.Column("in_transaction_schema", sa.Boolean()),
         )
 
         # Lazy Cache Table is unique for stage * in_transaction_schema
         self.lazy_cache_table = sa.Table(
             "lazy_tables",
             self.sql_metadata,
-            autoincrement_pk("id", "lazy_tables"),
-            Column("name", String(128)),
-            Column("stage", String(64)),
-            Column("query_hash", String(20)),
-            Column("task_hash", String(20)),
-            Column("in_transaction_schema", Boolean),
-            schema=self.metadata_schema.get(),
+            self._metadata_pk("id", "lazy_tables"),
+            sa.Column("name", sa.String(128)),
+            sa.Column("stage", sa.String(64)),
+            sa.Column("query_hash", sa.String(20)),
+            sa.Column("task_hash", sa.String(20)),
+            sa.Column("in_transaction_schema", sa.Boolean()),
         )
 
         # Sql Cache Table is unique for stage * in_transaction_schema
         self.raw_sql_cache_table = sa.Table(
-            "raw_sql_tables",
+            "raw_sql",
             self.sql_metadata,
-            autoincrement_pk("id", "raw_sql_tables"),
-            Column("prev_tables", String(256)),
-            Column("tables", String(256)),
-            Column("stage", String(64)),
-            Column("query_hash", String(20)),
-            Column("task_hash", String(20)),
-            Column("in_transaction_schema", Boolean),
-            schema=self.metadata_schema.get(),
+            self._metadata_pk("id", "raw_sql"),
+            sa.Column("prev_objects", sa.Text()),
+            sa.Column("new_objects", sa.Text()),
+            sa.Column("stage", sa.String(64)),
+            sa.Column("query_hash", sa.String(20)),
+            sa.Column("task_hash", sa.String(20)),
+            sa.Column("in_transaction_schema", sa.Boolean()),
         )
 
         self.logger.info(
             "Initialized SQL Table Store",
             engine_url=self.engine_url.render_as_string(hide_password=True),
             schema_prefix=self.schema_prefix,
             schema_suffix=self.schema_suffix,
         )
 
-    @engine_dispatch
+    def __init_subclass__(cls, **kwargs):
+        # Whenever a new subclass if SQLTableStore is defined, it must contain the
+        # `_dialect_name` attribute. This allows us to dynamically instantiate it
+        # when calling SQLTableStore(engine_url, ...) based on the dialect name found
+        # in the engine url (see __new__).
+        dialect_name = getattr(cls, "_dialect_name", None)
+        if dialect_name is None:
+            raise ValueError(
+                "All subclasses of SQLTableStore must have a `_dialect_name` attribute."
+                f" But {cls.__name__}._dialect_name is None."
+            )
+
+        if dialect_name in SQLTableStore.__registered_dialects:
+            warnings.warn(
+                f"Already registered a SQLTableStore for dialect {dialect_name}"
+            )
+        SQLTableStore.__registered_dialects[dialect_name] = cls
+
+    def _metadata_pk(self, name: str, table_name: str):
+        return sa.Column(name, sa.BigInteger(), primary_key=True)
+
     def _init_database(self):
         if not self.create_database_if_not_exists:
             return
 
         raise NotImplementedError(
-            "create_database_if_not_exists is only implemented for this engine"
+            "create_database_if_not_exists is not implemented for this engine"
         )
 
-    @_init_database.dialect("postgresql")
-    def _init_database_postgresql(self):
+    def _init_database_with_database(
+        self, database: str, execution_options: dict = None
+    ):
         if not self.create_database_if_not_exists:
             return
 
+        if execution_options is None:
+            execution_options = {}
+
         try:
             # Check if database exists
             with self.engine.connect() as conn:
-                conn.execute(sa.text("SELECT 1"))
+                conn.exec_driver_sql("SELECT 1")
             return
         except sa.exc.DBAPIError:
             # Database doesn't exist
             pass
 
         # Create new database using temporary engine object
-        postgres_db_url = self.engine_url.set(database="postgres")
-        tmp_engine = sa.create_engine(postgres_db_url)
+        tmp_db_url = self.engine_url.set(database=database)
+        tmp_engine = sa.create_engine(tmp_db_url, execution_options=execution_options)
 
         try:
             with tmp_engine.connect() as conn:
-                conn.execute(sa.text("COMMIT"))
                 conn.execute(CreateDatabase(self.engine_url.database))
         except sa.exc.DBAPIError:
             # This happens if multiple instances try to create the database
             # at the same time.
             with self.engine.connect() as conn:
                 # Verify database actually exists
-                conn.execute(sa.text("SELECT 1"))
-
-    @_init_database.dialect("duckdb")
-    def _init_database_duckdb(self):
-        # Duckdb already creates the database file automatically
-        pass
+                conn.exec_driver_sql("SELECT 1")
 
     def _create_engine(self):
-        engine = sa.create_engine(self.engine_url)
-
-        if engine.dialect.name == "mssql":
-            engine.dispose()
-            # this is needed to allow for CREATE DATABASE statements
-            # (we don't rely on database transactions anyways)
-            engine = sa.create_engine(
-                self.engine_url, connect_args={"autocommit": True}
-            )
-
-            if "." in self.schema_prefix and "." in self.schema_suffix:
-                raise AttributeError(
-                    "Config Error: It is not allowed to have a dot in both"
-                    " schema_prefix and schema_suffix for SQL Server / mssql database:"
-                    f' schema_prefix="{self.schema_prefix}","'
-                    f' schema_suffix="{self.schema_suffix}"'
-                )
-
-            if (self.schema_prefix + self.schema_suffix).count(".") != 1:
-                raise AttributeError(
-                    "Config Error: There must be exactly dot in both schema_prefix and"
-                    " schema_suffix together for SQL Server / mssql database:"
-                    f' schema_prefix="{self.schema_prefix}",'
-                    f' schema_suffix="{self.schema_suffix}"'
-                )
-
-        # if engine.dialect.name == "ibm_db_sa":
-        #     engine.dispose()
-        #     # switch to READ STABILITY isolation level to avoid unnecessary deadlock
-        #     # victims in case of background operations when reflecting columns
-        #     engine = sa.create_engine(
-        #         engine_url, execution_options={"isolation_level": "RS"}
-        #     )
-        # sqlalchemy 2 has create_engine().execution_options()
-
-        return engine
+        # future=True enables SQLAlchemy 2.0 behaviour with version 1.4
+        return sa.create_engine(self.engine_url, future=True)
 
     @contextmanager
-    @engine_dispatch
     def engine_connect(self) -> sa.Connection:
-        if self.engine.dialect.name == "ibm_db_sa":
-            conn = self.engine.connect()
-        else:
-            # sqlalchemy 2.0 uses this (except for dialect ibm_db_sa)
-            conn = (
-                self.engine.connect()
-            )  # .execution_options(isolation_level="AUTOCOMMIT")
-        try:
+        with self.engine.connect() as conn:
             yield conn
-        finally:
-            try:
-                # sqlalchemy 2.0 + ibm_db_sa needs this
-                conn.commit()
-            except AttributeError:
-                pass
+            conn.commit()
 
     def get_schema(self, name):
         return Schema(name, self.schema_prefix, self.schema_suffix)
 
     def _execute(self, query, conn: sa.engine.Connection):
         if self.print_sql:
             if isinstance(query, str):
@@ -350,182 +285,78 @@
             return conn.execute(sa.text(query))
         else:
             return conn.execute(query)
 
     def execute(self, query, *, conn: sa.engine.Connection = None):
         if conn is None:
             with self.engine_connect() as conn:
-                if isinstance(query, str):
-                    return self.execute(sa.text(query), conn=conn)
-                else:
-                    return self.execute(query, conn=conn)
+                return self.execute(query, conn=conn)
 
         if isinstance(query, sa.schema.DDLElement):
             # Some custom DDL statements contain multiple statements.
             # They are all seperated using a special seperator.
             query_str = str(
                 query.compile(self.engine, compile_kwargs={"literal_binds": True})
             )
-            try:
-                # sqlalchemy 2.0 + ibm_db_sa needs this
-                conn.commit()
-            except AttributeError:
-                # sqlalchemy 1.x does not have this function and does not need it
-                pass
+
             with conn.begin():
                 for part in split_ddl_statement(query_str):
                     self._execute(part, conn)
             return
 
         return self._execute(query, conn)
 
-    @engine_dispatch
-    def name_adj(self, name: str):
-        # some dialects need to replace all lowercase names by uppercase because
-        # they create uppercase table names by default
-        return name
-
-    @name_adj.dialect("ibm_db_sa")
-    def _name_adj_ibm_db_sa(self, name: str):
-        # DB2 creates tables uppercase if all lowercase given
-        return name.upper() if name.islower() else name
-
     def add_indexes(
         self, table: Table, schema: Schema, *, early_not_null_possible: bool = False
     ):
         if table.primary_key is not None:
             key = table.primary_key
             if isinstance(key, str):
                 key = [key]
             self.add_primary_key(
                 table.name, schema, key, early_not_null_possible=early_not_null_possible
             )
         if table.indexes is not None:
             for index in table.indexes:
                 self.add_index(table.name, schema, index)
 
-    @engine_dispatch
     def add_primary_key(
         self,
         table_name: str,
         schema: Schema,
         key_columns: list[str],
         *,
         name: str | None = None,
         early_not_null_possible: bool = False,
     ):
         _ = early_not_null_possible  # only used for some dialects
         self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
 
-    @engine_dispatch
     def add_index(
         self,
         table_name: str,
         schema: Schema,
         index_columns: list[str],
         name: str | None = None,
     ):
         self.execute(AddIndex(table_name, schema, index_columns, name))
 
-    @add_primary_key.dialect("mssql")
-    def _add_primary_key_mssql(
-        self,
-        table_name: str,
-        schema: Schema,
-        key_columns: list[str],
-        *,
-        name: str | None = None,
-        early_not_null_possible: bool = False,
-    ):
-        _ = early_not_null_possible  # not needed for this dialect
-        sql_types = self.reflect_sql_types(key_columns, table_name, schema)
-        # impose some varchar(max) limit to allow use in primary key / index
-        # TODO: consider making cap_varchar_max a config option
-        self.execute(
-            ChangeColumnTypes(
-                table_name,
-                schema,
-                key_columns,
-                sql_types,
-                nullable=False,
-                cap_varchar_max=1024,
-            )
-        )
-        self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
-
-    @add_index.dialect("mssql")
-    def _add_index_mssql(
-        self, table_name: str, schema: Schema, index: list[str], name: str | None = None
-    ):
-        sql_types = self.reflect_sql_types(index, table_name, schema)
-        if any(
-            [
-                isinstance(_type, sa.String) and _type.length is None
-                for _type in sql_types
-            ]
-        ):
-            # impose some varchar(max) limit to allow use in primary key / index
-            self.execute(
-                ChangeColumnTypes(
-                    table_name, schema, index, sql_types, cap_varchar_max=1024
-                )
-            )
-        self.execute(AddIndex(table_name, schema, index, name))
-
-    @add_primary_key.dialect("ibm_db_sa")
-    def _add_primary_key_ibm_db_sa(
-        self,
-        table_name: str,
-        schema: Schema,
-        key_columns: list[str],
-        *,
-        name: str | None = None,
-        early_not_null_possible: bool = False,
-    ):
-        if not early_not_null_possible:
-            for retry_iteration in range(4):
-                # retry operation since it might have been terminated as a
-                # deadlock victim
-                try:
-                    self.execute(
-                        ChangeColumnNullable(
-                            table_name, schema, key_columns, nullable=False
-                        )
-                    )
-                    break
-                except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
-                    if retry_iteration == 3:
-                        raise
-                    time.sleep(retry_iteration * retry_iteration * 1.1)
-        self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
-
-    # @add_index.dialect("ibm_db_sa")
-    # def _add_index_ibm_db_sa(
-    #     self, table_name: str, schema: Schema, index: list[str],
-    #     name: str | None = None
-    # ):
-    #     self.execute(AddIndex(table_name, schema, index, name))
-
     def copy_indexes(
         self, src_table: str, src_schema: Schema, dest_table: str, dest_schema: Schema
     ):
         inspector = sa.inspect(self.engine)
-        pk_constraint = inspector.get_pk_constraint(
-            self.name_adj(src_table), schema=self.name_adj(src_schema.get())
-        )
+        pk_constraint = inspector.get_pk_constraint(src_table, schema=src_schema.get())
         if len(pk_constraint["constrained_columns"]) > 0:
             self.add_primary_key(
                 dest_table,
                 dest_schema,
                 pk_constraint["constrained_columns"],
                 name=pk_constraint["name"],
             )
-        indexes = inspector.get_indexes(
-            self.name_adj(src_table), schema=self.name_adj(src_schema.get())
-        )
+        indexes = inspector.get_indexes(src_table, schema=src_schema.get())
         for index in indexes:
             if len(index["include_columns"]) > 0:
                 self.logger.warning(
                     "Perfect index recreation in caching is not net implemented",
                     table=dest_table,
                     schema=dest_schema.get(),
                     include_columns=index["include_columns"],
@@ -544,77 +375,28 @@
                 dest_table, dest_schema, index["column_names"], index["name"]
             )
 
     def reflect_sql_types(
         self, col_names: Iterable[str], table_name: str, schema: Schema
     ):
         inspector = sa.inspect(self.engine)
-        columns = inspector.get_columns(
-            self.name_adj(table_name), schema=self.name_adj(schema.get())
-        )
+        columns = inspector.get_columns(table_name, schema=schema.get())
         types = {d["name"]: d["type"] for d in columns}
         sql_types = [types[col] for col in col_names]
         return sql_types
 
     @staticmethod
     def format_sql_string(query_str: str) -> str:
         return textwrap.dedent(query_str).strip()
 
-    @engine_dispatch
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage"""
         for statement in raw_sql.sql.split(";"):
             self.execute(statement)
 
-    @execute_raw_sql.dialect("mssql")
-    def _execute_raw_sql_mssql(self, raw_sql: RawSql):
-        if self.disable_pytsql:
-            return self._execute_raw_sql_mssql_fallback(raw_sql)
-        return self._execute_raw_sql_mssql_pytsql(raw_sql)
-
-    def _execute_raw_sql_mssql_fallback(self, raw_sql: RawSql):
-        """Alternative to using pytsql for splitting SQL statement.
-
-        Known Problems:
-        - DECLARE statements will not be available across GO
-        """
-        last_use_statement = None
-        for statement in re.split(r"\bGO\b", raw_sql.sql, flags=re.IGNORECASE):
-            statement = statement.strip()
-            if statement == "":
-                # allow GO at end of script
-                continue
-
-            if re.match(r"\bUSE\b", statement):
-                last_use_statement = statement
-
-            with self.engine_connect() as conn:
-                if last_use_statement is not None:
-                    self.execute(last_use_statement, conn=conn)
-                self.execute(statement, conn=conn)
-
-    def _execute_raw_sql_mssql_pytsql(self, raw_sql: RawSql):
-        """Use pytsql for executing T-SQL scripts containing many GO statements."""
-        # noinspection PyUnresolvedReferences,PyPackageRequirements
-        import pytsql
-
-        sql_string = raw_sql.sql
-        if self.print_sql:
-            print_query_string = self.format_sql_string(sql_string)
-            max_length = 5000
-            if len(print_query_string) >= max_length:
-                print_query_string = print_query_string[:max_length] + " [...]"
-            self.logger.info("Executing sql", query=print_query_string)
-
-        pytsql.executes(
-            sql_string,
-            self.engine,
-            isolate_top_level_statements=self.pytsql_isolate_top_level_statements,
-        )
-
     def setup(self):
         super().setup()
         if not self.avoid_drop_create_schema:
             self.execute(CreateSchema(self.metadata_schema, if_not_exists=True))
         with self.engine_connect() as conn:
             try:
                 version = conn.execute(
@@ -643,67 +425,40 @@
                 "Disabled caching due to metadata version mismatch",
                 version=version,
                 expected_version=self.metadata_version,
             )
 
     def dispose(self):
         self.engine.dispose()
+        self.hook_cache = None
         super().dispose()
 
     def init_stage(self, stage: Stage):
         stage_commit_technique = ConfigContext.get().stage_commit_technique
         if stage_commit_technique == StageCommitTechnique.SCHEMA_SWAP:
             return self._init_stage_schema_swap(stage)
         if stage_commit_technique == StageCommitTechnique.READ_VIEWS:
             return self._init_stage_read_views(stage)
         raise ValueError(f"Invalid stage commit technique: {stage_commit_technique}")
 
-    @engine_dispatch
-    def drop_all_dialect_specific(self, schema: Schema):
-        pass
-
-    @drop_all_dialect_specific.dialect("ibm_db_sa")
-    def _drop_all_dialect_specific_ibm_db_sa(self, schema: Schema):
-        with self.engine_connect() as conn:
-            alias_names = conn.execute(
-                sa.text(
-                    "SELECT NAME FROM SYSIBM.SYSTABLES WHERE CREATOR ="
-                    f" '{ibm_db_sa_fix_name(schema.get())}' and TYPE='A'"
-                )
-            ).all()
-        alias_names = [row[0] for row in alias_names]
-        for alias in alias_names:
-            self.execute(DropAlias(alias, schema))
-
-    @engine_dispatch
     def _init_stage_schema_swap(self, stage: Stage):
         schema = self.get_schema(stage.name)
         transaction_schema = self.get_schema(stage.transaction_name)
 
         cs_base = CreateSchema(schema, if_not_exists=True)
         ds_trans = DropSchema(
             transaction_schema, if_exists=True, cascade=True, engine=self.engine
         )
         cs_trans = CreateSchema(transaction_schema, if_not_exists=False)
 
         with self.engine_connect() as conn:
             if self.avoid_drop_create_schema:
-                # empty tansaction_schema by deleting all tables and views
-                # Attention: similar code in sql_ddl.py:visit_drop_schema_ibm_db_sa
-                # for drop.cascade=True
-                inspector = sa.inspect(self.engine)
-                for table in inspector.get_table_names(
-                    schema=self.name_adj(transaction_schema.get())
-                ):
-                    self.execute(DropTable(table, schema=transaction_schema))
-                for view in inspector.get_view_names(
-                    schema=self.name_adj(transaction_schema.get())
-                ):
-                    self.execute(DropView(view, schema=transaction_schema))
-                self.drop_all_dialect_specific(schema=transaction_schema)
+                self.execute(
+                    DropSchemaContent(transaction_schema, self.engine), conn=conn
+                )
             else:
                 self.execute(cs_base, conn=conn)
                 self.execute(ds_trans, conn=conn)
                 self.execute(cs_trans, conn=conn)
 
             if not self.disable_caching:
                 for table in [
@@ -713,86 +468,14 @@
                 ]:
                     conn.execute(
                         table.delete()
                         .where(table.c.stage == stage.name)
                         .where(table.c.in_transaction_schema)
                     )
 
-    @_init_stage_schema_swap.dialect("mssql")
-    def _init_stage_schema_swap_mssql(self, stage: Stage):
-        if "." not in self.schema_suffix:
-            return self._init_stage_schema_swap.original(self, stage)
-
-        schema = self.get_schema(stage.name)
-        transaction_schema = self.get_schema(stage.transaction_name)
-
-        cs_base = CreateSchema(schema, if_not_exists=True)
-        cs_trans = CreateSchema(transaction_schema, if_not_exists=True)
-
-        # TODO: detect whether tmp_schema exists and rename it as base or
-        #       transaction schema if one is missing
-        database, trans_schema_only = transaction_schema.get().split(".")
-
-        # don't drop/create databases, just replace the schema underneath
-        # (files will keep name on renaming)
-        with self.engine_connect() as conn:
-            if not self.avoid_drop_create_schema:
-                self.execute(cs_base, conn=conn)
-                self.execute(cs_trans, conn=conn)
-            self.execute(f"USE [{database}]", conn=conn)
-            # clear tables in schema
-            self.execute(
-                f"""
-                EXEC sp_MSforeachtable
-                  @command1 = 'DROP TABLE ?'
-                , @whereand = 'AND SCHEMA_NAME(schema_id) = ''{trans_schema_only}'' '
-                """,
-                conn=conn,
-            )
-
-            # clear views and stored procedures
-            for view in self.get_view_names(transaction_schema.get()):
-                self.execute(
-                    DropView(view, transaction_schema, if_exists=True), conn=conn
-                )
-
-            modules = self._get_mssql_sql_modules(transaction_schema.get())
-            for name, _type in modules.items():
-                _type = _type.strip()
-                if _type == "P":
-                    self.execute(
-                        DropProcedure(name, transaction_schema, if_exists=True),
-                        conn=conn,
-                    )
-                elif _type == "FN":
-                    self.execute(
-                        DropFunction(name, transaction_schema, if_exists=True),
-                        conn=conn,
-                    )
-
-            synonyms = self._get_mssql_sql_synonyms(transaction_schema.get())
-            for name in synonyms.keys():
-                self.execute(
-                    DropAlias(name, transaction_schema, if_exists=True),
-                    conn=conn,
-                )
-
-            # Clear metadata
-            if not self.disable_caching:
-                for table in [
-                    self.tasks_table,
-                    self.lazy_cache_table,
-                    self.raw_sql_cache_table,
-                ]:
-                    conn.execute(
-                        table.delete()
-                        .where(table.c.stage == stage.name)
-                        .where(table.c.in_transaction_schema)
-                    )
-
     def _init_stage_read_views(self, stage: Stage):
         try:
             with self.engine_connect() as conn:
                 metadata_rows = (
                     conn.execute(
                         self.stage_table.select().where(
                             self.stage_table.c.stage == stage.name
@@ -842,49 +525,43 @@
         self.engine.dispose()
 
         # We might want to also append ', conn.begin()' to the with statement,
         # but this collides with the inner conn.begin() used to execute
         # statement parts as one transaction. This is solvable via complex code,
         # but we typically don't want to rely on database transactions anyways.
         with self.engine_connect() as conn:
-            # TODO: for mssql try to find schema does not exist and then move
-            #       the forgotten tmp schema there
-            assert not self.avoid_drop_create_schema, (
-                "The option avoid_drop_create_schema is currently not supported in "
-                "combination with dialect mssql"
+            # TODO: self.avoid_drop_create_schema is currently being ignored...
+            self.execute(
+                DropSchema(
+                    tmp_schema, if_exists=True, cascade=True, engine=self.engine
+                ),
+                conn=conn,
+            )
+            self.execute(RenameSchema(schema, tmp_schema, self.engine), conn=conn)
+            self.execute(
+                RenameSchema(transaction_schema, schema, self.engine), conn=conn
             )
             self.execute(
-                DropSchema(tmp_schema, if_exists=True, cascade=True), conn=conn
+                RenameSchema(tmp_schema, transaction_schema, self.engine), conn=conn
             )
-            # TODO: in case "." is in self.schema_prefix, we need to implement
-            #       schema renaming by creating the new schema and moving
-            #       table objects over
-            self.execute(RenameSchema(schema, tmp_schema), conn=conn)
-            self.execute(RenameSchema(transaction_schema, schema), conn=conn)
-            self.execute(RenameSchema(tmp_schema, transaction_schema), conn=conn)
 
             self._commit_stage_update_metadata(stage, conn=conn)
 
     def _commit_stage_read_views(self, stage: Stage):
         dest_schema = self.get_schema(stage.name)
         src_schema = self.get_schema(stage.transaction_name)
 
         with self.engine_connect() as conn:
-            # Delete all read views in visible (destination) schema
-            views = self.get_view_names(dest_schema.get())
-            for view in views:
-                self.execute(DropView(view, schema=dest_schema), conn=conn)
-            self.drop_all_dialect_specific(schema=dest_schema)
-
-            # Create views for all tables in transaction schema
-            src_meta = sa.MetaData()
-            src_meta.reflect(bind=self.engine, schema=src_schema.get())
-            self._create_read_views(
-                conn, dest_schema, src_schema, src_meta.tables.values()
-            )
+            # Clear contents of destination schema
+            self.execute(DropSchemaContent(dest_schema, self.engine), conn=conn)
+
+            # Create aliases for all tables in transaction schema
+            inspector = sa.inspect(self.engine)
+            for table in inspector.get_table_names(schema=src_schema.get()):
+                self.execute(CreateAlias(table, src_schema, table, dest_schema))
 
             # Update metadata
             stage_metadata_exists = (
                 conn.execute(
                     sa.select(1).where(self.stage_table.c.stage == stage.name)
                 ).scalar()
                 == 1
@@ -902,43 +579,14 @@
                         stage=stage.name,
                         cur_transaction_name=stage.transaction_name,
                     )
                 )
 
             self._commit_stage_update_metadata(stage, conn=conn)
 
-    @engine_dispatch
-    def _create_read_views(
-        self,
-        conn,
-        dest_schema: Schema,
-        src_schema: Schema,
-        src_tables: Iterable[sa.Table],
-    ):
-        _ = src_schema  # only needed by other dialects
-        for table in src_tables:
-            self.execute(
-                CreateViewAsSelect(
-                    table.name, dest_schema, sa.select("*").select_from(table)
-                ),
-                conn=conn,
-            )
-
-    @_create_read_views.dialect("ibm_db_sa")
-    def _create_read_views_ibm_db_sa(
-        self, conn, dest_schema, src_schema: Schema, src_tables: Iterable[sa.Table]
-    ):
-        # Instead of views create aliases which can be locked like tables and
-        # have primary keys
-        for table in src_tables:
-            self.execute(
-                CreateAlias(table.name, src_schema, table.name, dest_schema),
-                conn=conn,
-            )
-
     def _commit_stage_update_metadata(self, stage: Stage, conn: sa.engine.Connection):
         if not self.disable_caching:
             for table in [
                 self.tasks_table,
                 self.lazy_cache_table,
                 self.raw_sql_cache_table,
             ]:
@@ -969,22 +617,19 @@
         if RunContext.get().has_stage_changed(table.stage):
             self._copy_table(table, from_schema, from_name)
         else:
             self._deferred_copy_table(table, from_schema, from_name)
 
     def _copy_table(self, table: Table, from_schema: Schema, from_name: str):
         """Copies the table immediately"""
-        has_table = sa.inspect(self.engine).has_table(
-            self.name_adj(from_name), schema=self.name_adj(from_schema.get())
-        )
+        inspector = sa.inspect(self.engine)
+        has_table = inspector.has_table(from_name, schema=from_schema.get())
 
         if not has_table:
-            available_tables = sa.inspect(self.engine).get_table_names(
-                self.name_adj(from_schema.get())
-            )
+            available_tables = inspector.get_table_names(from_schema.get())
             msg = (
                 f"Can't copy table '{from_name}' (schema: '{from_schema}') to "
                 f"transaction because no such table exists.\n"
                 f"Tables in schema: {available_tables}"
             )
             self.logger.error(msg)
             raise CacheError(msg)
@@ -1017,21 +662,18 @@
         tables from their old names to their new names.
 
         Otherwise, we copy the tables to the transaction schema in the background,
         and once we're ready to commit, we replace the aliases with the copied tables.
         """
         assert from_schema == self.get_schema(table.stage.name)
 
-        has_table = sa.inspect(self.engine).has_table(
-            self.name_adj(from_name), schema=self.name_adj(from_schema.get())
-        )
+        inspector = sa.inspect(self.engine)
+        has_table = inspector.has_table(from_name, schema=from_schema.get())
         if not has_table:
-            available_tables = sa.inspect(self.engine).get_table_names(
-                self.name_adj(from_schema.get())
-            )
+            available_tables = inspector.get_table_names(from_schema.get())
             msg = (
                 f"Can't deferred copy table '{from_name}' (schema: '{from_schema}') to "
                 f"transaction because no such table exists.\n"
                 f"Tables in schema: {available_tables}"
             )
             self.logger.error(msg)
             raise CacheError(msg)
@@ -1117,162 +759,102 @@
 
     def _rename_table(self, from_name: str, to_name: str, schema: Schema):
         if from_name == to_name:
             return
         self.logger.info("RENAME", fr=from_name, to=to_name)
         self.execute(RenameTable(from_name, to_name, schema))
 
-    @engine_dispatch
-    def get_view_names(self, schema: str, *, include_everything=False) -> list[str]:
-        """
-        List all views that are present in a schema.
-
-        It may also include other database objects like stored procedures, functions,
-        etc. which makes the name `get_view_names` too specific. But sqlalchemy
-        only allows reading views for all dialects thus the storyline of dialect
-        agnostic callers is much nicer to read. In the end we might need everything
-        to recover the full cache output which was produced by a RawSQL statement
-        (we want to be compatible with legacy sql code as a starting point).
-        :param schema: the schema
-        :param include_everything: If True, we might include stored procedures,
-            functions and other database objects that have a schema associated name.
-            Currently, this only makes a difference for dialect=mssql.
-        :return: list of view names [and other objects]
-        """
-        _ = include_everything  # not used in this implementation
-        inspector = sa.inspect(self.engine)
-        return inspector.get_view_names(self.name_adj(schema))
-
-    @get_view_names.dialect("mssql")
-    def _get_view_names_mssql(self, schema: str, *, include_everything=False):
-        if not include_everything:
-            return self.get_view_names.original(
-                self, schema, include_everything=include_everything
-            )
-        return list(self._get_mssql_sql_modules(schema).keys())
-
-    # noinspection SqlDialectInspection
-    def _get_mssql_sql_modules(self, schema: str):
-        with self.engine_connect() as conn:
-            database, schema_only = schema.split(".")
-            self.execute(f"USE {database}", conn=conn)
-            # include stored procedures in view names because they can also be recreated
-            # based on sys.sql_modules.description
-            sql = (
-                "select obj.name, obj.type from sys.sql_modules as mod "
-                "left join sys.objects as obj on mod.object_id=obj.object_id "
-                "left join sys.schemas as schem on schem.schema_id=obj.schema_id "
-                f"where schem.name='{schema_only}'"
-            )
-            rows = self.execute(sql, conn=conn).fetchall()
-        return {row[0]: row[1] for row in rows}
-
-    # noinspection SqlDialectInspection
-    def _get_mssql_sql_synonyms(self, schema: str):
-        with self.engine_connect() as conn:
-            database, schema_only = schema.split(".")
-            self.execute(f"USE {database}", conn=conn)
-            # include stored procedures in view names because they can also be recreated
-            # based on sys.sql_modules.description
-            sql = (
-                "select syn.name, syn.type from sys.synonyms as syn "
-                "left join sys.schemas as schem on schem.schema_id=syn.schema_id "
-                f"where schem.name='{schema_only}'"
-            )
-            rows = self.execute(sql, conn=conn).fetchall()
-        return {row[0]: row[1] for row in rows}
-
     def copy_raw_sql_tables_to_transaction(
         self, metadata: RawSqlMetadata, target_stage: Stage
     ):
+        inspector = sa.inspect(self.engine)
         src_schema = self.get_schema(metadata.stage)
         dest_schema = self.get_schema(target_stage.transaction_name)
 
-        views = set(self.get_view_names(src_schema.get(), include_everything=True))
-        new_tables = set(metadata.tables) - set(metadata.prev_tables)
+        # New tables (AND other objects)
+        new_objects = set(metadata.new_objects) - set(metadata.prev_objects)
+        tables_in_schema = set(inspector.get_table_names(src_schema.get()))
+        objects_in_schema = self._get_all_objects_in_schema(src_schema)
+
+        tables_to_copy = new_objects & tables_in_schema
+        objects_to_copy = {
+            k: v
+            for k, v in objects_in_schema.items()
+            if k in new_objects and k not in tables_to_copy
+        }
 
-        tables_to_copy = new_tables - set(views)
-        for table_name in tables_to_copy:
-            try:
-                # TODO: implement deferred execution in RunContextServer so
-                # no data is copied if a stage is 100% cache valid
-                self.execute(
-                    CopyTable(
-                        table_name,
+        try:
+            with self.engine_connect() as conn:
+                for name in tables_to_copy:
+                    self.execute(
+                        CopyTable(
+                            name,
+                            src_schema,
+                            name,
+                            dest_schema,
+                        ),
+                        conn=conn,
+                    )
+                    self.copy_indexes(
+                        name,
                         src_schema,
-                        table_name,
+                        name,
                         dest_schema,
                     )
-                )
-                self.copy_indexes(
-                    table_name,
-                    src_schema,
-                    table_name,
-                    dest_schema,
-                )
-            except Exception as _e:
-                msg = (
-                    f"Failed to copy raw sql generated table {table_name} (schema:"
-                    f" '{src_schema}') to transaction."
-                )
-                self.logger.exception(
-                    msg
-                    + " This error is treated as cache-lookup-failure and thus we can"
-                    " continue."
-                )
-                raise CacheError(msg) from _e
 
-        views_to_copy = new_tables & set(views)
-        for view_name in views_to_copy:
-            self._copy_view_to_transaction(view_name, src_schema, dest_schema)
-
-    @engine_dispatch
-    def _copy_view_to_transaction(
-        self, view_name: str, src_schema: Schema, dest_schema: Schema
-    ):
-        raise NotImplementedError("Only implemented for mssql.")
+                for name, obj_metadata in objects_to_copy.items():
+                    self._copy_object_to_transaction(
+                        name, obj_metadata, src_schema, dest_schema, conn
+                    )
 
-    # noinspection SqlDialectInspection
-    @_copy_view_to_transaction.dialect("mssql")
-    def _copy_view_to_transaction_mssql(
-        self, view_name: str, src_schema: Schema, dest_schema: Schema
-    ):
-        src_database, src_schema_only = src_schema.get().split(".")
-        dest_database, dest_schema_only = dest_schema.get().split(".")
+        except Exception as _e:
+            msg = (
+                f"Failed to copy raw sql generated object {name} (schema:"
+                f" '{src_schema}') to transaction."
+            )
+            self.logger.exception(
+                msg + " This error is treated as cache-lookup-failure."
+            )
+            raise CacheError(msg) from _e
 
-        with self.engine_connect() as conn:
-            self.execute(f"USE {src_database}", conn=conn)
-            view_sql = self.execute(
-                f"""
-                SELECT definition
-                FROM sys.sql_modules
-                WHERE [object_id] = OBJECT_ID('[{src_schema_only}].[{view_name}]');
-                """,
-                conn=conn,
-            ).first()
+    def _get_all_objects_in_schema(self, schema: Schema) -> dict[str, Any]:
+        """List all objects that are present in a schema.
 
-            if view_sql is None:
-                msg = f"No SQL query associated with view {view_name} found."
-                raise ValueError(msg)
-            view_sql = view_sql[0]
-
-            # Update view SQL so that it references the destination schema
-            if src_schema_only != dest_schema_only:
-                names_product = itertools.product(
-                    [src_schema_only, f"[{src_schema_only}]"],
-                    [view_name, f"[{view_name}]"],
-                )
-                for schema, view in names_product:
-                    view_sql.replace(
-                        f"{schema}.{view}",
-                        f"[{dest_schema_only}].[{view_name}]",
-                    )
+        This may include things like views, stored procedures, functions, etc.
 
-            self.execute(f"USE {dest_database}", conn=conn)
-            self.execute(view_sql, conn=conn)
+        :param schema: the schema
+        :return: a dictionary where the keys are the names of the objects, and the
+            values are any other (dialect specific) information that might be useful.
+        """
+
+        # Because SQLAlchemy only provides limited capabilities to inspect objects
+        # inside a schema, we limit ourselves to tables and views.
+        inspector = sa.inspect(self.engine)
+        tables = inspector.get_table_names(schema.get())
+        views = inspector.get_view_names(schema.get())
+        return {name: None for name in tables + views}
+
+    def _copy_object_to_transaction(
+        self,
+        name: str,
+        metadata: Any,
+        src_schema: Schema,
+        dest_schema: Schema,
+        conn: sa.Connection,
+    ):
+        """Copy a generic object from one schema to another.
+
+        :param name: name of the object to be copied
+        :param metadata:
+            additional information as returned by `get_all_objects_in_schema`
+        :param src_schema: the schema in which the object is
+        :param dest_schema: the schema into which the object should be copied
+        """
+        dialect = self.engine.dialect.name
+        raise NotImplementedError(f"Not implemented for dialect '{dialect}'.")
 
     def delete_table_from_transaction(self, table: Table):
         self.execute(
             DropTable(
                 table.name,
                 self.get_schema(table.stage.transaction_name),
                 if_exists=True,
@@ -1426,16 +1008,16 @@
         )
 
     def store_raw_sql_metadata(self, metadata: RawSqlMetadata):
         if not self.disable_caching:
             with self.engine_connect() as conn:
                 conn.execute(
                     self.raw_sql_cache_table.insert().values(
-                        prev_tables=json.dumps(metadata.prev_tables),
-                        tables=json.dumps(metadata.tables),
+                        prev_objects=json.dumps(metadata.prev_objects),
+                        new_objects=json.dumps(metadata.new_objects),
                         stage=metadata.stage,
                         query_hash=metadata.query_hash,
                         task_hash=metadata.task_hash,
                         in_transaction_schema=True,
                     )
                 )
 
@@ -1469,58 +1051,27 @@
         except sa.exc.MultipleResultsFound:
             raise CacheError("Multiple results found for raw sql cache key") from None
 
         if result is None:
             raise CacheError("No result found for raw sql cache key")
 
         return RawSqlMetadata(
-            prev_tables=json.loads(result.prev_tables),
-            tables=json.loads(result.tables),
+            prev_objects=json.loads(result.prev_objects),
+            new_objects=json.loads(result.new_objects),
             stage=result.stage,
             query_hash=result.query_hash,
             task_hash=result.task_hash,
         )
 
-    @engine_dispatch
-    def resolve_aliases(self, table_name, schema):
-        return table_name, schema
-
-    @resolve_aliases.dialect("ibm_db_sa")
-    def resolve_aliases_ibm_db_sa(self, table_name, schema):
-        with self.engine_connect() as conn:
-            return _resolve_alias_ibm_db_sa(conn, table_name, schema)
-
-    @resolve_aliases.dialect("mssql")
-    def resolve_aliases_mssql(self, table_name, schema):
-        with self.engine_connect() as conn:
-            return _resolve_alias_mssql(conn, table_name, schema)
-
-    def list_tables(self, stage: Stage, *, include_everything=False):
-        """
-        List all tables that were generated in a stage.
-
-        It may also include other objects database objects like views, stored
-        procedures, functions, etc. which makes the name `list_tables` too specific.
-        But the predominant idea is that tasks produce tables in stages and thus the
-        storyline of callers is much nicer to read. In the end we might need everything
-        to recover the full cache output which was produced by a RawSQL statement
-        (we want to be compatible with legacy sql code as a starting point).
-
-        :param stage: the stage
-        :param include_everything: If True, we might include stored procedures,
-            functions and other database objects that have a schema associated name.
-        :return: list of tables [and other objects]
-        """
-        inspector = sa.inspect(self.engine)
-        schema = self.get_schema(stage.transaction_name).get()
+    def resolve_alias(self, table: str, schema: str) -> tuple[str, str]:
+        return table, schema
 
-        table_names = inspector.get_table_names(self.name_adj(schema))
-        view_names = self.get_view_names(schema, include_everything=include_everything)
-
-        return table_names + view_names
+    def get_objects_in_stage(self, stage: Stage):
+        schema = self.get_schema(stage.transaction_name)
+        return list(self._get_all_objects_in_schema(schema).keys())
 
     def get_stage_hash(self, stage: Stage) -> str:
         """Compute hash that represents entire stage's output metadata."""
         # We only need to look in tasks_table since the output_json column is updated
         # after evaluating lazy output objects for cache validity. This is the same
         # information we use for producing input_hash of downstream tasks.
         if self.disable_caching:
@@ -1542,79 +1093,12 @@
     def get_engine_for_locking(self) -> sa.Engine:
         return self._create_engine()
 
     def get_lock_schema(self) -> Schema:
         return self.get_schema(self.LOCK_SCHEMA)
 
 
-def _resolve_alias_ibm_db_sa(conn, table_name: str, schema: str, *, _iteration=0):
-    # TODO: consider speeding this up by caching information for complete schemas
-    #  instead of running at least two queries per source table; Ultimately problem can
-    #  also be fixed by upstream contribution to ibm_db_sa
-
-    # we need to resolve aliases since pandas.read_sql_table does not work for them
-    # and sa.Table does not auto-reflect columns
-    table_name = ibm_db_sa_fix_name(table_name)
-    schema = ibm_db_sa_fix_name(schema)
-    tbl = sa.Table("SYSTABLES", sa.MetaData(), schema="SYSIBM", autoload_with=conn)
-    query = (
-        sa.select(tbl.c.base_name, tbl.c.base_schema)
-        .select_from(tbl)
-        .where(
-            (tbl.c.creator == schema) & (tbl.c.name == table_name) & (tbl.c.TYPE == "A")
-        )
-    )
-    for retry_iteration in range(4):
-        # retry operation since it might have been terminated as a deadlock victim
-        try:
-            row = conn.execute(query).mappings().one_or_none()
-            break
-        except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
-            if retry_iteration == 3:
-                raise
-            time.sleep(retry_iteration * retry_iteration)
-    if row is not None:
-        assert _iteration < 3, f"Unexpected recursion looking up {schema}.{table_name}"
-        table_name, schema = _resolve_alias_ibm_db_sa(
-            conn, row["base_name"], row["base_schema"], _iteration=_iteration + 1
-        )
-    return table_name, schema
-
-
-def _resolve_alias_mssql(conn, table_name: str, schema: str, *, _iteration=0):
-    # TODO: consider speeding this up by caching information for complete schemas
-    #  instead of running at least two queries per source table; Ultimately problem can
-    #  also be fixed by upstream contribution to ibm_db_sa
-
-    # we need to resolve aliases since pandas.read_sql_table does not work for them
-    # and sa.Table does not auto-reflect columns
-    database, schema_only = schema.split(".")
-    conn.execute(sa.text(f"USE [{database}]"))
-    # include stored procedures in view names because they can also be recreated
-    # based on sys.sql_modules.description
-    sql = (
-        "select syn.base_object_name from sys.synonyms as syn left join sys.schemas as"
-        f" schem on schem.schema_id=syn.schema_id where schem.name='{schema_only}' and"
-        f" syn.name='{table_name}' and syn.type='SN'"
-    )
-    row = conn.execute(sa.text(sql)).mappings().one_or_none()
-    if row is not None:
-        parts = row["base_object_name"].split(".")
-        assert len(parts) == 3, (
-            "Unexpected number of '.' delimited parts when looking up synonym for "
-            f"{schema}.{table_name}: {row['base_object_name']}"
-        )
-        assert _iteration < 3, f"Unexpected recursion looking up {schema}.{table_name}"
-        parts = [
-            part[1:-1] if part.startswith("[") and part.endswith("]") else part
-            for part in parts
-        ]
-        schema = ".".join(parts[0:2])
-        table_name = parts[2]
-        table_name, schema = _resolve_alias_mssql(
-            conn, table_name, schema, _iteration=_iteration + 1
-        )
-    return table_name, schema
-
-
 # Load SQLTableStore Hooks
-from pydiverse.pipedag.backend.table.sql_hooks import *  # noqa
+import pydiverse.pipedag.backend.table.sql.hooks  # noqa
+
+# Load SQLTableStore dialect specific subclasses
+import pydiverse.pipedag.backend.table.sql.dialects  # noqa
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/sql_hooks.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,32 @@
 import re
 import time
 import warnings
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
-import sqlalchemy.dialects
+import sqlalchemy.exc
 from packaging.version import Version
 
+from pydiverse.pipedag import ConfigContext
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import TableHook
-from pydiverse.pipedag.backend.table.sql import SQLTableStore
+from pydiverse.pipedag.backend.table.sql.ddl import (
+    CreateTableAsSelect,
+    Schema,
+)
+from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import (
     DType,
     PandasDTypeBackend,
-    classmethod_engine_argument_dispatch,
-)
-from pydiverse.pipedag.backend.table.util.sql_ddl import (
-    ChangeTableLogged,
-    CreateTableAsSelect,
-    Schema,
-    ibm_db_sa_fix_name,
 )
+from pydiverse.pipedag.context import TaskContext
 from pydiverse.pipedag.materialize import Table
 from pydiverse.pipedag.materialize.core import TaskInfo
-from pydiverse.pipedag.util.naming import NameDisambiguator
 
 # region SQLALCHEMY
 
 
 @SQLTableStore.register_table()
 class SQLAlchemyTableHook(TableHook[SQLTableStore]):
     @classmethod
@@ -71,45 +69,39 @@
         store.execute(
             CreateTableAsSelect(
                 table.name,
                 schema,
                 obj,
                 early_not_null=table.primary_key,
                 source_tables=source_tables,
-                unlogged=store.unlogged_tables,
             )
         )
         store.add_indexes(table, schema, early_not_null_possible=True)
 
     @classmethod
     def retrieve(
-        cls, store, table, stage_name, as_type: type[sa.Table], namer=None
+        cls, store, table, stage_name, as_type: type[sa.Table]
     ) -> sa.sql.selectable.Selectable:
-        table_name = table.name
         schema = store.get_schema(stage_name).get()
-        table_name, schema = store.resolve_aliases(table_name, schema)
-        tbl = None
+        table_name, schema = store.resolve_alias(table.name, schema)
+        alias_name = TaskContext.get().name_disambiguator.get_name(table_name)
+
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
-                alias_name = (
-                    namer.get_name(table_name) if namer is not None else table_name
-                )
-                tbl = sa.Table(
+                return sa.Table(
                     table_name,
                     sa.MetaData(),
                     schema=schema,
                     autoload_with=store.engine,
                 ).alias(alias_name)
-                break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
-        return tbl
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
         if isinstance(obj, sa.sql.selectable.FromClause):
             query = sa.select("*").select_from(obj)
         else:
             query = obj
@@ -128,14 +120,24 @@
 # endregion
 
 # region PANDAS
 
 
 @SQLTableStore.register_table(pd)
 class PandasTableHook(TableHook[SQLTableStore]):
+    """
+    Allows overriding the default dtype backend to use by setting the `dtype_backend`
+    argument in the `hook_args` section of the table store config:
+    ::
+
+        hook_args:
+          pandas:
+            dtype_backend: "arrow" | "numpy"
+    """
+
     pd_version = Version(pd.__version__)
 
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(type_, pd.DataFrame)
 
     @classmethod
@@ -190,209 +192,81 @@
                 df[col] = df[col].astype(object)
 
         cls._execute_materialize(
             df,
             store=store,
             table=table,
             schema=schema,
-            engine=store.engine,
             dtypes=dtypes,
         )
         store.add_indexes(table, schema)
 
-    @classmethod_engine_argument_dispatch
+    @classmethod
     def _execute_materialize(
         cls,
         df: pd.DataFrame,
         store: SQLTableStore,
         table: Table[pd.DataFrame],
         schema: Schema,
-        engine: sa.Engine,
         dtypes: dict[str, DType],
     ):
         dtypes = {name: dtype.to_sql() for name, dtype in dtypes.items()}
         if table.type_map:
             dtypes.update(table.type_map)
 
         df.to_sql(
             table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-            chunksize=100_000,
-        )
-
-    @_execute_materialize.dialect("postgresql")
-    def _execute_materialize_postgres(
-        cls,
-        df: pd.DataFrame,
-        store: SQLTableStore,
-        table: Table[pd.DataFrame],
-        schema: Schema,
-        engine: sa.Engine,
-        dtypes: dict[str, DType],
-    ):
-        import csv
-        from io import StringIO
-
-        dtypes = {name: dtype.to_sql() for name, dtype in dtypes.items()}
-        if table.type_map:
-            dtypes.update(table.type_map)
-
-        # Create empty table
-        df[:0].to_sql(
-            table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-        )
-
-        if store.unlogged_tables:
-            with engine.connect() as conn:
-                conn.execute(ChangeTableLogged(table.name, schema, False))
-
-        # COPY data
-        # TODO: For python 3.12, there is csv.QUOTE_STRINGS
-        #       This would make everything a bit safer, because then we could represent
-        #       the string "\\N" (backslash + capital n).
-        s_buf = StringIO()
-        df.to_csv(
-            s_buf,
-            na_rep="\\N",
-            header=False,
-            index=False,
-            quoting=csv.QUOTE_MINIMAL,
-        )
-        s_buf.seek(0)
-
-        dbapi_conn = engine.raw_connection()
-        try:
-            with dbapi_conn.cursor() as cur:
-                sql = (
-                    f"COPY {schema.get()}.{table.name} FROM STDIN"
-                    " WITH (FORMAT CSV, NULL '\\N')"
-                )
-                cur.copy_expert(sql=sql, file=s_buf)
-            dbapi_conn.commit()
-        finally:
-            dbapi_conn.close()
-
-    @_execute_materialize.dialect("mssql")
-    def _execute_materialize_mssql(
-        cls,
-        df: pd.DataFrame,
-        store: SQLTableStore,
-        table: Table[pd.DataFrame],
-        schema: Schema,
-        engine: sa.Engine,
-        dtypes: dict[str, DType],
-    ):
-        dtypes = ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
-            {
-                name: sa.dialects.mssql.DATETIME2()
-                for name, dtype in dtypes.items()
-                if dtype == DType.DATETIME
-            }
-        )
-
-        if table.type_map:
-            dtypes.update(table.type_map)
-
-        df.to_sql(
-            table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-            chunksize=100_000,
-        )
-
-    @_execute_materialize.dialect("ibm_db_sa")
-    def _execute_materialize_ibm_db_sa(
-        cls,
-        df: pd.DataFrame,
-        store: SQLTableStore,
-        table: Table[pd.DataFrame],
-        schema: Schema,
-        engine: sa.Engine,
-        dtypes: dict[str, DType],
-    ):
-        # Default string target is CLOB which can't be used for indexing.
-        # -> Convert indexed string columns to VARCHAR(256)
-        index_columns = set()
-        if indexes := table.indexes:
-            index_columns |= {col for index in indexes for col in index}
-        if primary_key := table.primary_key:
-            index_columns |= set(primary_key)
-
-        dtypes = ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
-            {
-                name: (
-                    sa.String(length=256)
-                    if name in index_columns
-                    else sa.String(length=32_672)
-                )
-                for name, dtype in dtypes.items()
-                if dtype == DType.STRING
-            }
-        )
-
-        if table.type_map:
-            dtypes.update(table.type_map)
-
-        df.to_sql(
-            ibm_db_sa_fix_name(table.name),
-            engine,
+            store.engine,
             schema=schema.get(),
             index=False,
             dtype=dtypes,
             chunksize=100_000,
         )
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         as_type: type[pd.DataFrame] | tuple | dict,
-        namer: NameDisambiguator | None = None,
     ) -> pd.DataFrame:
         # Config
         if PandasTableHook.pd_version >= Version("2.0"):
             backend_str = "arrow"
         else:
             backend_str = "numpy"
 
+        if hook_args := ConfigContext.get().table_hook_args.get("pandas", None):
+            if dtype_backend := hook_args.get("dtype_backend", None):
+                backend_str = dtype_backend
+
         if isinstance(as_type, tuple):
             backend_str = as_type[1]
         elif isinstance(as_type, dict):
             backend_str = as_type["backend"]
 
         backend = PandasDTypeBackend(backend_str)
 
         # Retrieve
         query, dtypes = cls._build_retrieve_query(store, table, stage_name, backend)
-        dataframe = cls._execute_query_retrieve(query, dtypes, store.engine, backend)
+        dataframe = cls._execute_query_retrieve(store, query, dtypes, backend)
         return dataframe
 
     @classmethod
     def _build_retrieve_query(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         backend: PandasDTypeBackend,
     ) -> tuple[Any, dict[str, DType]]:
         engine = store.engine
         schema = store.get_schema(stage_name).get()
-        table_name = table.name
-        table_name, schema = store.resolve_aliases(table_name, schema)
+        table_name, schema = store.resolve_alias(table.name, schema)
 
         sql_table = sa.Table(
             table_name,
             sa.MetaData(),
             schema=schema,
             autoload_with=engine,
         ).alias("tbl")
@@ -449,27 +323,27 @@
                     (col > max_val, max_val),
                     else_=col,
                 ).label(name)
                 res_cols[name] = clamped_col
 
         return res_cols, res_dtypes
 
-    @classmethod_engine_argument_dispatch
+    @classmethod
     def _execute_query_retrieve(
         cls,
+        store: SQLTableStore,
         query: Any,
         dtypes: dict[str, DType],
-        engine: sa.Engine,
         backend: PandasDTypeBackend,
     ) -> pd.DataFrame:
         dtypes = {
             name: dtype.to_pandas(backend=backend) for name, dtype in dtypes.items()
         }
 
-        with engine.connect() as conn:
+        with store.engine.connect() as conn:
             if PandasTableHook.pd_version >= Version("2.0"):
                 df = pd.read_sql(query, con=conn, dtype=dtypes)
             else:
                 df = pd.read_sql(query, con=conn)
                 for col, dtype in dtypes.items():
                     df[col] = df[col].astype(dtype)
 
@@ -520,34 +394,33 @@
             store.logger.info(
                 f"Writing table '{schema.get()}.{table.name}'", table_obj=table.obj
             )
 
         dtypes = dict(zip(df.columns, map(DType.from_polars, df.dtypes)))
 
         pd_df = df.to_pandas(use_pyarrow_extension_array=True, zero_copy_only=True)
-        return PandasTableHook.materialize_(
+        hook = store.get_hook_subclass(PandasTableHook)
+        return hook.materialize_(
             df=pd_df,
             dtypes=dtypes,
             store=store,
             table=table,
             schema=schema,
         )
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         as_type: type[polars.dataframe.DataFrame],
-        namer: NameDisambiguator | None = None,
     ) -> polars.dataframe.DataFrame:
         schema = store.get_schema(stage_name).get()
-        table_name = table.name
-        table_name, schema = store.resolve_aliases(table_name, schema)
+        table_name, schema = store.resolve_alias(table.name, schema)
         connection_uri = store.engine_url.render_as_string(hide_password=False)
         df = polars.read_database(
             f'SELECT * FROM {schema}."{table_name}"', connection_uri
         )
         return df
 
     @classmethod
@@ -580,26 +453,28 @@
         table: Table[tidypolars.Tibble],
         stage_name,
         task_info: TaskInfo | None,
     ):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = t.to_polars()
-        PolarsTableHook.materialize(store, table, stage_name, task_info)
+
+        hook = store.get_hook_subclass(PolarsTableHook)
+        return hook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         as_type: type[tidypolars.Tibble],
-        namer: NameDisambiguator | None = None,
     ) -> tidypolars.Tibble:
-        df = PolarsTableHook.retrieve(store, table, stage_name, as_type, namer)
+        hook = store.get_hook_subclass(PolarsTableHook)
+        df = hook.retrieve(store, table, stage_name, as_type)
         return tidypolars.from_polars(df)
 
     @classmethod
     def auto_table(cls, obj: tidypolars.Tibble):
         # currently, we don't know how to store a table name inside tidypolars tibble
         return super().auto_table(obj)
 
@@ -638,39 +513,40 @@
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         t = table.obj
         table = table.copy_without_obj()
         if isinstance(t._impl, PandasTableImpl):
             table.obj = t >> collect()
-            return PandasTableHook.materialize(store, table, stage_name, task_info)
+            hook = store.get_hook_subclass(PandasTableHook)
+            return hook.materialize(store, table, stage_name, task_info)
         if isinstance(t._impl, SQLTableImpl):
             table.obj = t._impl.build_select()
-            return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
+            hook = store.get_hook_subclass(SQLAlchemyTableHook)
+            return hook.materialize(store, table, stage_name, task_info)
         raise NotImplementedError
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         as_type: type[T],
-        namer: NameDisambiguator | None = None,
     ) -> T:
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         if issubclass(as_type, PandasTableImpl):
-            df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame, namer)
+            hook = store.get_hook_subclass(PandasTableHook)
+            df = hook.retrieve(store, table, stage_name, pd.DataFrame)
             return pdt.Table(PandasTableImpl(table.name, df))
         if issubclass(as_type, SQLTableImpl):
-            sa_tbl = SQLAlchemyTableHook.retrieve(
-                store, table, stage_name, sa.Table, namer
-            )
+            hook = store.get_hook_subclass(SQLAlchemyTableHook)
+            sa_tbl = hook.retrieve(store, table, stage_name, sa.Table)
             return pdt.Table(SQLTableImpl(store.engine, sa_tbl))
         raise NotImplementedError
 
     @classmethod
     def auto_table(cls, obj: pdt.Table):
         return Table(obj, obj._impl.name)
 
@@ -687,111 +563,91 @@
 
 # endregion
 
 # region IBIS
 
 
 try:
-    # optional dependency to ibis
     import ibis
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     ibis = None
 
 
 @SQLTableStore.register_table(ibis)
 class IbisTableHook(TableHook[SQLTableStore]):
-    @staticmethod
-    def get_con(store):
-        # TODO: move this function to a better ibis specific place
-        con = store.engines_other.get("ibis")
-        if con is None:
-            url = store.engine_url
-            dialect = store.engine.dialect.name
-            if dialect == "postgresql":
-                con = ibis.postgres.connect(
-                    host=url.host,
-                    user=url.username,
-                    password=url.password,
-                    port=url.port,
-                    database=url.database,
-                )
-            elif dialect == "mssql":
-                con = ibis.mssql.connect(
-                    host=url.host,
-                    user=url.username,
-                    password=url.password,
-                    port=url.port,
-                    database=url.database,
-                )
-            else:
-                raise RuntimeError(
-                    f"initializing ibis for {dialect} is not supported, yet "
-                    "-- supported: postgresql, mssql"
-                )
-            store.engines_other["ibis"] = con
-        return con
+    @classmethod
+    def conn(cls, store: SQLTableStore):
+        if conn := store.hook_cache.get((cls, "conn")):
+            return conn
+        conn = cls._conn(store)
+        store.hook_cache[(cls, "conn")] = conn
+        return conn
+
+    @classmethod
+    def _conn(cls, store: SQLTableStore):
+        return ibis.connect(store.engine_url.render_as_string(hide_password=False))
 
     @classmethod
     def can_materialize(cls, type_) -> bool:
         # Operations on a table like mutate() or join() don't change the type
-        return issubclass(type_, ibis.expr.types.Table)
+        return issubclass(type_, ibis.api.Table)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
-        return issubclass(type_, ibis.expr.types.Table)
+        return issubclass(type_, ibis.api.Table)
 
     @classmethod
     def materialize(
         cls,
         store,
-        table: Table[ibis.expr.types.Table],
+        table: Table[ibis.api.Table],
         stage_name,
         task_info: TaskInfo | None,
     ):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = sa.text(cls.lazy_query_str(store, t))
-        return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
+
+        sa_hook = store.get_hook_subclass(SQLAlchemyTableHook)
+        return sa_hook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
-        as_type: type[ibis.expr.types.Table],
-        namer: NameDisambiguator | None = None,
-    ) -> ibis.expr.types.Table:
-        con = cls.get_con(store)
-        table_name = table.name
+        as_type: type[ibis.api.Table],
+    ) -> ibis.api.Table:
+        conn = cls.conn(store)
         schema = store.get_schema(stage_name).get()
-        table_name, schema = store.resolve_aliases(table_name, schema)
+        table_name, schema = store.resolve_alias(table.name, schema)
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
-                tbl = con.table(
+                tbl = conn.table(
                     table_name,
                     schema=schema,
                 )
                 break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
         else:
             raise Exception
         return tbl
 
     @classmethod
-    def auto_table(cls, obj: ibis.expr.types.Table):
+    def auto_table(cls, obj: ibis.api.Table):
         if obj.has_name():
             return Table(obj, obj.get_name())
         else:
             return super().auto_table(obj)
 
     @classmethod
-    def lazy_query_str(cls, store, obj: ibis.expr.types.Table) -> str:
-        return str(ibis.to_sql(obj, cls.get_con(store).name))
+    def lazy_query_str(cls, store, obj: ibis.api.Table) -> str:
+        return str(ibis.to_sql(obj, cls.conn(store).name))
 
 
 # endregion
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,17 @@
         if isinstance(type_, sa.SmallInteger):
             return DType.INT16
         if isinstance(type_, sa.BigInteger):
             return DType.INT64
         if isinstance(type_, sa.Integer):
             return DType.INT32
         if isinstance(type_, sa.Numeric):
+            precision = type_.precision or 53
+            if precision <= 24:
+                return DType.FLOAT32
             return DType.FLOAT64
         if isinstance(type_, sa.String):
             return DType.STRING
         if isinstance(type_, sa.Boolean):
             return DType.BOOLEAN
         if isinstance(type_, sa.Date):
             return DType.DATE
@@ -188,16 +191,16 @@
             DType.INT16: sa.SmallInteger(),
             DType.INT32: sa.Integer(),
             DType.INT64: sa.BigInteger(),
             DType.UINT8: sa.SmallInteger(),
             DType.UINT16: sa.Integer(),
             DType.UINT32: sa.BigInteger(),
             DType.UINT64: sa.BigInteger(),
-            DType.FLOAT32: sa.Float(),
-            DType.FLOAT64: sa.Double(),
+            DType.FLOAT32: sa.Float(24),
+            DType.FLOAT64: sa.Float(53),
             DType.STRING: sa.String(),
             DType.BOOLEAN: sa.Boolean(),
             DType.DATE: sa.Date(),
             DType.TIME: sa.Time(),
             DType.DATETIME: sa.DateTime(),
         }[self]
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import copy
 import re
 
+import pyparsing as pp
 import sqlalchemy as sa
 from attr import frozen
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.schema import DDLElement
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import TextClause
 
 __all__ = [
     "Schema",
     "CreateSchema",
     "DropSchema",
     "RenameSchema",
+    "DropSchemaContent",
     "CreateTableAsSelect",
     "CreateViewAsSelect",
     "CreateAlias",
     "CopyTable",
     "RenameTable",
     "DropTable",
     "CreateDatabase",
@@ -26,16 +28,16 @@
     "DropFunction",
     "DropProcedure",
     "DropView",
     "AddPrimaryKey",
     "AddIndex",
     "ChangeColumnNullable",
     "ChangeColumnTypes",
+    "ChangeTableLogged",
     "split_ddl_statement",
-    "ibm_db_sa_fix_name",
 ]
 
 
 @frozen
 class Schema:
     name: str
     prefix: str
@@ -63,17 +65,24 @@
         self.if_exists = if_exists
         self.cascade = cascade
 
         self.engine = engine
 
 
 class RenameSchema(DDLElement):
-    def __init__(self, from_: Schema, to: Schema):
+    def __init__(self, from_: Schema, to: Schema, engine: sa.Engine):
         self.from_ = from_
         self.to = to
+        self.engine = engine
+
+
+class DropSchemaContent(DDLElement):
+    def __init__(self, schema: Schema, engine: sa.Engine):
+        self.schema = schema
+        self.engine = engine
 
 
 class CreateDatabase(DDLElement):
     def __init__(self, database: str, if_not_exists=False):
         self.database = database
         self.if_not_exists = if_not_exists
 
@@ -310,61 +319,40 @@
     text.append(schema)
     return " ".join(text)
 
 
 # noinspection SqlDialectInspection
 @compiles(CreateSchema, "mssql")
 def visit_create_schema_mssql(create: CreateSchema, compiler, **kw):
-    # For SQL Server we support two modes:  using databases as schemas,
-    # or schemas as schemas.
     _ = kw
-    if "." in create.schema.name:
-        raise AttributeError(
-            "We currently do not support dots in schema names "
-            " when working with mssql database"
-        )
-    full_name = create.schema.get()
-    # it was already checked that there is exactly one dot in schema prefix + suffix
-    database_name, schema_name = full_name.split(".")
-    database = compiler.preparer.format_schema(database_name)
-    schema = compiler.preparer.format_schema(schema_name)
-    create_schema = f"CREATE SCHEMA {schema}"
-    create_database = f"CREATE DATABASE {database}"
+    schema = compiler.preparer.format_schema(create.schema.get())
     if create.if_not_exists:
-        create_database = f"""
-            IF NOT EXISTS (
-                SELECT * FROM sys.databases WHERE name = N'{database_name}'
-            )
-            BEGIN {create_database} END"""
-        create_schema = f"""
-            IF NOT EXISTS (
-                SELECT * FROM sys.schema WHERE name = N'{schema_name}'
-            )
-            BEGIN {create_schema} END"""
-
-    if "." in create.schema.prefix:
-        # With prefix like "my_db." we create our stages as schemas
-        # Attention: we have to rely on a preceding USE statement
-        #            for correct prefix database
-        return create_schema
+        unquoted_schema = create.schema.get()
+        return f"""
+        IF NOT EXISTS (
+            SELECT 1 FROM sys.schemas WHERE name = N'{unquoted_schema}'
+        )
+        BEGIN EXEC('CREATE SCHEMA {schema}') END
+        """
     else:
-        # With suffix like ".dbo" we create our stages as databases
-        return create_database
+        return f"CREATE SCHEMA {schema}"
 
 
 @compiles(CreateSchema, "ibm_db_sa")
 def visit_create_schema_ibm_db_sa(create: CreateSchema, compiler, **kw):
     """For IBM DB2 we need to jump through extra hoops for if_exists=True."""
     _ = kw
     schema = compiler.preparer.format_schema(create.schema.get())
     if create.if_not_exists:
-        return (
-            "BEGIN\ndeclare continue handler for sqlstate '42710' begin end;\n"
-            f"execute immediate 'CREATE SCHEMA {schema}';\nEND"
-        )
+        return f"""
+        BEGIN
+            declare continue handler for sqlstate '42710' begin end;
+            execute immediate 'CREATE SCHEMA {schema}';
+        END
+        """
     else:
         return f"CREATE SCHEMA {schema}"
 
 
 @compiles(DropSchema)
 def visit_drop_schema(drop: DropSchema, compiler, **kw):
     _ = kw
@@ -377,67 +365,45 @@
         text.append("CASCADE")
     return " ".join(text)
 
 
 @compiles(DropSchema, "mssql")
 def visit_drop_schema_mssql(drop: DropSchema, compiler, **kw):
     _ = kw
-    full_name = drop.schema.get()
-    # it was already checked that there is exactly one dot in schema prefix + suffix
-    database_name, schema_name = full_name.split(".")
-    if "." in drop.schema.prefix:
-        # With prefix like "my_db." we create our stages as schemas
-        # Attention: we have to rely on a preceding USE statement
-        #            for correct prefix database
-        text = ["DROP SCHEMA"]
-        name = compiler.preparer.format_schema(schema_name)
-    else:
-        # With suffix like ".dbo" we create our stages as databases
-        text = ["DROP DATABASE"]
-        name = compiler.preparer.format_schema(database_name)
+    schema = compiler.preparer.format_schema(drop.schema.get())
+    statements = []
+
+    if drop.cascade:
+        if drop.engine is None:
+            raise ValueError(
+                "Using DropSchema with cascade=True for mssql requires passing"
+                " the engine kwarg to DropSchema."
+            )
+
+        statements.append(DropSchemaContent(drop.schema, drop.engine))
+
+    text = ["DROP SCHEMA"]
     if drop.if_exists:
         text.append("IF EXISTS")
-    text.append(name)
-    return " ".join(text)
+    text.append(schema)
+    statements.append(" ".join(text))
+
+    return join_ddl_statements(statements, compiler, **kw)
 
 
-# noinspection SqlDialectInspection
 @compiles(DropSchema, "ibm_db_sa")
 def visit_drop_schema_ibm_db_sa(drop: DropSchema, compiler, **kw):
-    """
-    Because IBM DB2 doesn't support CASCADE, we must manually drop all tables in
-    the schema first.
-    """
     statements = []
     if drop.cascade:
         if drop.engine is None:
             raise ValueError(
                 "Using DropSchema with cascade=True for ibm_db2 requires passing"
                 " the engine kwarg to DropSchema."
             )
-
-        add_statements = []
-        # see SQLTableStore._init_stage_schema_swap()
-        inspector = sa.inspect(drop.engine)
-        for table in inspector.get_table_names(schema=drop.schema.get()):
-            add_statements.append(DropTable(table, schema=drop.schema))
-        for view in inspector.get_view_names(schema=drop.schema.get()):
-            add_statements.append(DropView(view, schema=drop.schema))
-        # see SQLTableStore.drop_all_dialect_specific()
-        with drop.engine.connect() as conn:
-            alias_names = conn.execute(
-                sa.text(
-                    "SELECT NAME FROM SYSIBM.SYSTABLES WHERE CREATOR ="
-                    f" '{ibm_db_sa_fix_name(drop.schema.get())}' and TYPE='A'"
-                ),
-            ).all()
-        alias_names = [row[0] for row in alias_names]
-        for alias in alias_names:
-            add_statements.append(DropAlias(alias, drop.schema))
-        statements += [compiler.process(stmt) for stmt in add_statements]
+        statements.append(DropSchemaContent(drop.schema, drop.engine))
 
     # Compile DROP SCHEMA statement
     schema = compiler.preparer.format_schema(drop.schema.get())
     if drop.if_exists:
         # Add error handler to cache the case that the schema doesn't exist
         statements.append(
             f"""
@@ -459,35 +425,146 @@
     from_ = compiler.preparer.format_schema(rename.from_.get())
     to = compiler.preparer.format_schema(rename.to.get())
     return "ALTER SCHEMA " + from_ + " RENAME TO " + to
 
 
 @compiles(RenameSchema, "mssql")
 def visit_rename_schema_mssql(rename: RenameSchema, compiler, **kw):
+    # MSSql doesn't support renaming schemas, but it allows you to move objects from
+    # one schema to another.
+    # https://stackoverflow.com/questions/17571233/how-to-change-schema-of-all-tables-views-and-stored-procedures-in-mssql
+    # https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-schema-transact-sql?view=sql-server-ver16
+    from pydiverse.pipedag.backend.table.sql.reflection import (
+        PipedagMSSqlReflection,
+    )
+
     _ = kw
-    if rename.from_.prefix != rename.to.prefix:
-        raise AttributeError(
-            "We currently do not support varying schema prefixes for mssql database"
-        )
-    from_full_name = rename.from_.get()
-    to_full_name = rename.to.get()
-    # it was already checked that there is exactly one dot in schema prefix + suffix
-    from_database_name, from_schema_name = from_full_name.split(".")
-    to_database_name, to_schema_name = to_full_name.split(".")
-    if "." in rename.from_.prefix:
-        # With prefix like "my_db." we create our stages as schemas
-        raise NotImplementedError(
-            "There is not SCHEMA rename expression for mssql. "
-            "Needs to be addressed on higher level!"
-        )
-    else:
-        # With suffix like ".dbo" we create our stages as databases
-        from_name = compiler.preparer.format_schema(from_database_name)
-        to_name = compiler.preparer.format_schema(to_database_name)
-        return f"ALTER DATABASE {from_name} MODIFY NAME = {to_name}"
+    from_ = compiler.preparer.format_schema(rename.from_.get())
+    to = compiler.preparer.format_schema(rename.to.get())
+
+    inspector = sa.inspect(rename.engine)
+
+    # Reflect to get objects which we want to move
+    names_to_move = []
+    names_to_redefine = []
+
+    table_names = inspector.get_table_names(schema=rename.from_.get())
+    view_names = inspector.get_view_names(schema=rename.from_.get())
+    alias_names = PipedagMSSqlReflection.get_alias_names(
+        rename.engine, schema=rename.from_.get()
+    )
+    procedure_names = PipedagMSSqlReflection.get_procedure_names(
+        rename.engine, schema=rename.from_.get()
+    )
+    function_names = PipedagMSSqlReflection.get_function_names(
+        rename.engine, schema=rename.from_.get()
+    )
+
+    names_to_move.extend(table_names)
+    names_to_move.extend(alias_names)
+    names_to_redefine.extend(view_names)
+    names_to_redefine.extend(procedure_names)
+    names_to_redefine.extend(function_names)
+
+    if not (names_to_move or names_to_redefine):
+        return ""
+
+    # Produce statement
+    statements = []
+
+    statements.append(CreateSchema(rename.to, if_not_exists=True))
+    for name in names_to_move:
+        name = compiler.preparer.quote(name)
+        statements.append(f"ALTER SCHEMA {to} TRANSFER {from_}.{name}")
+
+    # Recreate views, procedures and functions, but replace all references to the
+    # old schema name with the new schema name
+    with rename.engine.connect() as conn:
+        for name in names_to_redefine:
+            definition = _mssql_update_definition(conn, name, rename.from_, rename.to)
+            statements.append(definition)
+
+    for view in view_names:
+        statements.append(DropView(view, rename.from_))
+    for procedure in procedure_names:
+        statements.append(DropProcedure(procedure, rename.from_))
+    for function in function_names:
+        statements.append(DropFunction(function, rename.from_))
+
+    statements.append(DropSchema(rename.from_))
+    return join_ddl_statements(statements, compiler, **kw)
+
+
+@compiles(DropSchemaContent)
+def visit_drop_schema_content(drop: DropSchemaContent, compiler, **kw):
+    _ = kw
+    schema = drop.schema
+    engine = drop.engine
+    inspector = sa.inspect(engine)
+
+    statements = []
+
+    for table in inspector.get_table_names(schema=schema.get()):
+        statements.append(DropTable(table, schema=schema))
+    for view in inspector.get_view_names(schema=schema.get()):
+        statements.append(DropView(view, schema=schema))
+
+    return join_ddl_statements(statements, compiler, **kw)
+
+
+@compiles(DropSchemaContent, "mssql")
+def visit_drop_schema_content_mssql(drop: DropSchemaContent, compiler, **kw):
+    from pydiverse.pipedag.backend.table.sql.reflection import (
+        PipedagMSSqlReflection,
+    )
+
+    _ = kw
+    schema = drop.schema
+    engine = drop.engine
+    inspector = sa.inspect(engine)
+
+    statements = []
+
+    for table in inspector.get_table_names(schema=schema.get()):
+        statements.append(DropTable(table, schema=schema))
+    for view in inspector.get_view_names(schema=schema.get()):
+        statements.append(DropView(view, schema=schema))
+    for alias in PipedagMSSqlReflection.get_alias_names(engine, schema=schema.get()):
+        statements.append(DropAlias(alias, schema=drop.schema))
+    for procedure in PipedagMSSqlReflection.get_procedure_names(
+        engine, schema=schema.get()
+    ):
+        statements.append(DropProcedure(procedure, schema=schema))
+    for function in PipedagMSSqlReflection.get_function_names(
+        engine, schema=schema.get()
+    ):
+        statements.append(DropFunction(function, schema=schema))
+
+    return join_ddl_statements(statements, compiler, **kw)
+
+
+@compiles(DropSchemaContent, "ibm_db_sa")
+def visit_drop_schema_content_ibm_db2(drop: DropSchemaContent, compiler, **kw):
+    from pydiverse.pipedag.backend.table.sql.reflection import PipedagDB2Reflection
+
+    _ = kw
+    schema = drop.schema
+    engine = drop.engine
+    inspector = sa.inspect(engine)
+
+    statements = []
+
+    for table in inspector.get_table_names(schema=schema.get()):
+        statements.append(DropTable(table, schema=schema))
+    for view in inspector.get_view_names(schema=schema.get()):
+        statements.append(DropView(view, schema=schema))
+    for alias in PipedagDB2Reflection.get_alias_names(engine, schema=schema.get()):
+        statements.append(DropAlias(alias, schema=drop.schema))
+
+    return join_ddl_statements(statements, compiler, **kw)
 
 
 @compiles(CreateDatabase)
 def visit_create_database(create: CreateDatabase, compiler, **kw):
     _ = kw
     database = compiler.preparer.format_schema(create.database)
     text = ["CREATE DATABASE"]
@@ -510,15 +587,15 @@
     ret = " ".join(text)
     raise NotImplementedError(
         f"Disable for now for safety reasons (not yet needed): {ret}"
     )
 
 
 def _visit_create_obj_as_select(create, compiler, _type, kw, *, prefix="", suffix=""):
-    name = compiler.preparer.quote_identifier(create.name)
+    name = compiler.preparer.quote(create.name)
     schema = compiler.preparer.format_schema(create.schema.get())
     kw["literal_binds"] = True
     select = compiler.sql_compiler.process(create.query, **kw)
     return f"CREATE {_type} {schema}.{name} AS\n{prefix}{select}{suffix}"
 
 
 @compiles(CreateTableAsSelect)
@@ -534,41 +611,26 @@
         return _visit_create_obj_as_select(create, compiler, "UNLOGGED TABLE", kw)
     else:
         return _visit_create_obj_as_select(create, compiler, "TABLE", kw)
 
 
 @compiles(CreateTableAsSelect, "mssql")
 def visit_create_table_as_select_mssql(create: CreateTableAsSelect, compiler, **kw):
-    name = compiler.preparer.quote_identifier(create.name)
-    full_name = create.schema.get()
-    # it was already checked that there is exactly one dot in schema prefix + suffix
-    database_name, schema_name = full_name.split(".")
-    database = compiler.preparer.format_schema(database_name)
-    schema = compiler.preparer.format_schema(schema_name)
+    name = compiler.preparer.quote(create.name)
+    schema = compiler.preparer.format_schema(create.schema.get())
 
     kw["literal_binds"] = True
     select = compiler.sql_compiler.process(create.query, **kw)
 
-    return insert_into_in_query(select, database, schema, name)
-
-
-def ref_ibm_db_sa(tbl: dict[str, str], compiler):
-    return (
-        f"{compiler.preparer.quote_identifier(ibm_db_sa_fix_name(tbl['schema']))}."
-        f"{compiler.preparer.quote_identifier(ibm_db_sa_fix_name(tbl['name']))}"
-    )
+    return insert_into_in_query(select, schema, name)
 
 
 # noinspection SqlDialectInspection
 @compiles(CreateTableAsSelect, "ibm_db_sa")
 def visit_create_table_as_select_ibm_db_sa(create: CreateTableAsSelect, compiler, **kw):
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    create = copy.deepcopy(create)
-    create.name = ibm_db_sa_fix_name(create.name)
-
     prepare_statement = _visit_create_obj_as_select(
         create, compiler, "TABLE", kw, prefix="(", suffix=") DEFINITION ONLY"
     )
 
     if create.early_not_null is not None:
         not_null_cols = create.early_not_null
         if isinstance(not_null_cols, str):
@@ -581,20 +643,24 @@
                 nullable=False,
             ),
             compiler,
         )
     else:
         not_null_statements = []
 
-    name = compiler.preparer.quote_identifier(create.name)
-    schema = compiler.preparer.format_schema(create.schema.get())
+    preparer = compiler.preparer
+    name = preparer.quote(create.name)
+    schema = preparer.format_schema(create.schema.get())
 
     lock_statements = [f"LOCK TABLE {schema}.{name} IN EXCLUSIVE MODE"]
     if create.source_tables is not None:
-        src_tables = [f"{ref_ibm_db_sa(tbl, compiler)}" for tbl in create.source_tables]
+        src_tables = [
+            f"{preparer.format_schema(tbl['schema'])}.{preparer.quote(tbl['name'])}"
+            for tbl in create.source_tables
+        ]
         lock_statements += [f"LOCK TABLE {ref} IN SHARE MODE" for ref in src_tables]
 
     kw["literal_binds"] = True
     select = compiler.sql_compiler.process(create.query, **kw)
     create_statement = f"INSERT INTO {schema}.{name}\n{select}"
 
     return join_ddl_statements(
@@ -608,24 +674,16 @@
 
 
 @compiles(CreateViewAsSelect)
 def visit_create_view_as_select(create: CreateViewAsSelect, compiler, **kw):
     return _visit_create_obj_as_select(create, compiler, "VIEW", kw)
 
 
-@compiles(CreateViewAsSelect, "ibm_db_sa")
-def visit_create_view_as_select_ibm_db_sa(create: CreateViewAsSelect, compiler, **kw):
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    create = copy.deepcopy(create)
-    create.name = ibm_db_sa_fix_name(create.name)
-    return _visit_create_obj_as_select(create, compiler, "VIEW", kw)
-
-
-def insert_into_in_query(select_sql, database, schema, table):
-    into = f"INTO {database}.{schema}.{table}"
+def insert_into_in_query(select_sql, schema, table):
+    into = f"INTO {schema}.{table}"
     into_point = None
     # insert INTO before first FROM, WHERE, GROUP BY, WINDOW, HAVING,
     #                          ORDER BY, UNION, EXCEPT, INTERSECT
     for marker in [
         "FROM",
         "WHERE",
         r"GROUP\s*BY",
@@ -651,76 +709,53 @@
         if into_point is not None
         else select_sql + " " + into
     )
 
 
 @compiles(CreateAlias)
 def visit_create_alias(create_alias: CreateAlias, compiler, **kw):
-    query = sa.select("*").select_from(
-        sa.Table(
-            create_alias.from_name, sa.MetaData(), schema=create_alias.from_schema.get()
-        )
-    )
-    return visit_create_view_as_select(
-        CreateViewAsSelect(create_alias.to_name, create_alias.to_schema, query),
-        compiler,
-        **kw,
+    from_name = compiler.preparer.quote(create_alias.from_name)
+    from_schema = compiler.preparer.format_schema(create_alias.from_schema.get())
+    query = sa.select("*").select_from(sa.text(f"{from_schema}.{from_name}"))
+    return compiler.process(
+        CreateViewAsSelect(create_alias.to_name, create_alias.to_schema, query), **kw
     )
 
 
 @compiles(CreateAlias, "mssql")
 def visit_create_alias(create_alias: CreateAlias, compiler, **kw):
-    from_name = compiler.preparer.quote_identifier(
-        ibm_db_sa_fix_name(create_alias.from_name)
-    )
-    from_database, from_schema = _get_mssql_database_schema(
-        create_alias.from_schema, compiler
-    )
-    to_name = compiler.preparer.quote_identifier(
-        ibm_db_sa_fix_name(create_alias.to_name)
-    )
-    to_database, to_schema = _get_mssql_database_schema(
-        create_alias.to_schema, compiler
-    )
+    from_name = compiler.preparer.quote(create_alias.from_name)
+    from_schema = compiler.preparer.format_schema(create_alias.from_schema.get())
+    to_name = compiler.preparer.quote(create_alias.to_name)
+    to_schema = compiler.preparer.format_schema(create_alias.to_schema.get())
 
-    statements = [f"USE {to_database}"]
     text = ["CREATE"]
     if create_alias.or_replace:
         text.append("OR REPLACE")
-    text.append(
-        f"SYNONYM {to_schema}.{to_name} FOR {from_database}.{from_schema}.{from_name}"
-    )
-    statements.append(" ".join(text))
-    return join_ddl_statements(statements, compiler, **kw)
+    text.append(f"SYNONYM {to_schema}.{to_name} FOR {from_schema}.{from_name}")
+    return " ".join(text)
 
 
 @compiles(CreateAlias, "ibm_db_sa")
 def visit_create_alias(create_alias: CreateAlias, compiler, **kw):
-    from_name = compiler.preparer.quote_identifier(
-        ibm_db_sa_fix_name(create_alias.from_name)
-    )
-    from_schema = compiler.preparer.format_schema(
-        ibm_db_sa_fix_name(create_alias.from_schema.get())
-    )
-    to_name = compiler.preparer.quote_identifier(
-        ibm_db_sa_fix_name(create_alias.to_name)
-    )
-    to_schema = compiler.preparer.format_schema(
-        ibm_db_sa_fix_name(create_alias.to_schema.get())
-    )
+    from_name = compiler.preparer.quote(create_alias.from_name)
+    from_schema = compiler.preparer.format_schema(create_alias.from_schema.get())
+    to_name = compiler.preparer.quote(create_alias.to_name)
+    to_schema = compiler.preparer.format_schema(create_alias.to_schema.get())
+
     text = ["CREATE"]
     if create_alias.or_replace:
         text.append("OR REPLACE")
     text.append(f"ALIAS {to_schema}.{to_name} FOR TABLE {from_schema}.{from_name}")
     return " ".join(text)
 
 
 @compiles(CopyTable)
 def visit_copy_table(copy_table: CopyTable, compiler, **kw):
-    from_name = compiler.preparer.quote_identifier(copy_table.from_name)
+    from_name = compiler.preparer.quote(copy_table.from_name)
     from_schema = compiler.preparer.format_schema(copy_table.from_schema.get())
     query = sa.select("*").select_from(sa.text(f"{from_schema}.{from_name}"))
     create = CreateTableAsSelect(
         copy_table.to_name,
         copy_table.to_schema,
         query,
         early_not_null=copy_table.early_not_null,
@@ -728,527 +763,354 @@
             dict(name=copy_table.from_name, schema=copy_table.from_schema.get())
         ],
     )
     return compiler.process(create, **kw)
 
 
 # noinspection SqlDialectInspection
-@compiles(CopyTable, "mssql")
-def visit_copy_table_mssql(copy_table: CopyTable, compiler, **kw):
-    from_name = compiler.preparer.quote_identifier(copy_table.from_name)
-    database, schema = _get_mssql_database_schema(copy_table.from_schema, compiler)
-    query = sa.text(f"SELECT * FROM {database}.{schema}.{from_name}")
-    create = CreateTableAsSelect(
-        copy_table.to_name,
-        copy_table.to_schema,
-        query,
-        early_not_null=copy_table.early_not_null,
-    )
-    return compiler.process(create, **kw)
-
-
-@compiles(CopyTable, "ibm_db_sa")
-def visit_copy_table_ibm_db_sa(copy_table: CopyTable, compiler, **kw):
-    copy_table = copy.deepcopy(copy_table)
-    copy_table.from_name = ibm_db_sa_fix_name(copy_table.from_name)
-    copy_table.to_name = ibm_db_sa_fix_name(copy_table.to_name)
-    return visit_copy_table(copy_table, compiler, **kw)
-
-
-# noinspection SqlDialectInspection
 @compiles(RenameTable)
 def visit_rename_table(rename_table: RenameTable, compiler, **kw):
     _ = kw
-    from_table = compiler.preparer.quote_identifier(rename_table.from_name)
-    to_table = compiler.preparer.quote_identifier(rename_table.to_name)
+    from_table = compiler.preparer.quote(rename_table.from_name)
+    to_table = compiler.preparer.quote(rename_table.to_name)
     schema = compiler.preparer.format_schema(rename_table.schema.get())
     return f"ALTER TABLE {schema}.{from_table} RENAME TO {to_table}"
 
 
 # noinspection SqlDialectInspection
 @compiles(RenameTable, "mssql")
 def visit_rename_table(rename_table: RenameTable, compiler, **kw):
     _ = kw
-    database, schema = _get_mssql_database_schema(rename_table.schema, compiler)
 
-    from_table = compiler.preparer.quote_identifier(rename_table.from_name)
+    schema = compiler.preparer.format_schema(rename_table.schema.get())
+    from_table = compiler.preparer.quote(rename_table.from_name)
     to_table = rename_table.to_name  # no quoting is intentional
-    statements = [
-        f"USE [{database}]",
-        f"EXEC sp_rename '{schema}.{from_table}', '{to_table}'",
-    ]
-    return join_ddl_statements(statements, compiler, **kw)
+
+    return f"EXEC sp_rename '{schema}.{from_table}', '{to_table}'"
 
 
 # noinspection SqlDialectInspection
 @compiles(RenameTable, "ibm_db_sa")
 def visit_rename_table(rename_table: RenameTable, compiler, **kw):
     _ = kw
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    rename_table = copy.deepcopy(rename_table)
-    rename_table.from_name = ibm_db_sa_fix_name(rename_table.from_name)
-    rename_table.to_name = ibm_db_sa_fix_name(rename_table.to_name)
-
-    from_table = compiler.preparer.quote_identifier(rename_table.from_name)
-    to_table = compiler.preparer.quote_identifier(rename_table.to_name)
+    from_table = compiler.preparer.quote(rename_table.from_name)
+    to_table = compiler.preparer.quote(rename_table.to_name)
     schema = compiler.preparer.format_schema(rename_table.schema.get())
     return f"RENAME TABLE {schema}.{from_table} TO {to_table}"
 
 
 @compiles(DropTable)
 def visit_drop_table(drop: DropTable, compiler, **kw):
     return _visit_drop_anything(drop, "TABLE", compiler, **kw)
 
 
-@compiles(DropTable, "mssql")
-def visit_drop_table_mssql(drop: DropTable, compiler, **kw):
-    return _visit_drop_anything_mssql(drop, "TABLE", compiler, **kw)
-
-
-@compiles(DropTable, "ibm_db_sa")
-def visit_drop_table_ibm_db_sa(drop: DropTable, compiler, **kw):
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    drop = copy.deepcopy(drop)
-    drop.name = ibm_db_sa_fix_name(drop.name)
-    return _visit_drop_anything(drop, "TABLE", compiler, **kw)
-
-
 @compiles(DropView)
 def visit_drop_view(drop: DropView, compiler, **kw):
     return _visit_drop_anything(drop, "VIEW", compiler, **kw)
 
 
-@compiles(DropView, "mssql")
-def visit_drop_view_mssql(drop: DropView, compiler, **kw):
-    return _visit_drop_anything_mssql(drop, "VIEW", compiler, **kw)
-
-
-@compiles(DropView, "ibm_db_sa")
-def visit_drop_view_ibm_db_sa(drop: DropView, compiler, **kw):
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    drop = copy.deepcopy(drop)
-    drop.name = ibm_db_sa_fix_name(drop.name)
-    return _visit_drop_anything(drop, "VIEW", compiler, **kw)
-
-
 @compiles(DropAlias)
 def visit_drop_alias(drop: DropAlias, compiler, **kw):
     # Not all dialects support a table ALIAS as a first class object.
     # For those that don't we just use views.
     return _visit_drop_anything(drop, "VIEW", compiler, **kw)
 
 
 @compiles(DropAlias, "mssql")
 def visit_drop_alias_mssql(drop: DropAlias, compiler, **kw):
     # What is called ALIAS for dialect ibm_db_sa is called SYNONYM for mssql
-    return _visit_drop_anything_mssql(drop, "SYNONYM", compiler, **kw)
+    return _visit_drop_anything(drop, "SYNONYM", compiler, **kw)
 
 
 @compiles(DropAlias, "ibm_db_sa")
-def visit_drop_alias_ibm_db_sa(drop: DropAlias, compiler, **kw):
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    drop = copy.deepcopy(drop)
-    drop.name = ibm_db_sa_fix_name(drop.name)
+def visit_drop_alias_mssql(drop: DropAlias, compiler, **kw):
     return _visit_drop_anything(drop, "ALIAS", compiler, **kw)
 
 
 @compiles(DropProcedure)
 def visit_drop_table(drop: DropProcedure, compiler, **kw):
     return _visit_drop_anything(drop, "PROCEDURE", compiler, **kw)
 
 
-@compiles(DropProcedure, "mssql")
-def visit_drop_table_mssql(drop: DropProcedure, compiler, **kw):
-    return _visit_drop_anything_mssql(drop, "PROCEDURE", compiler, **kw)
-
-
 @compiles(DropFunction)
 def visit_drop_table(drop: DropFunction, compiler, **kw):
     return _visit_drop_anything(drop, "FUNCTION", compiler, **kw)
 
 
-@compiles(DropFunction, "mssql")
-def visit_drop_table_mssql(drop: DropProcedure, compiler, **kw):
-    return _visit_drop_anything_mssql(drop, "FUNCTION", compiler, **kw)
-
-
 def _visit_drop_anything(
     drop: DropTable | DropView | DropProcedure | DropFunction | DropAlias,
     _type,
     compiler,
-    dont_quote_table=False,
     **kw,
 ):
     _ = kw
-    if dont_quote_table:
-        table = drop.name
-    else:
-        table = compiler.preparer.quote_identifier(drop.name)
+    table = compiler.preparer.quote(drop.name)
     schema = compiler.preparer.format_schema(drop.schema.get())
     text = [f"DROP {_type}"]
     if drop.if_exists:
         text.append("IF EXISTS")
     text.append(f"{schema}.{table}")
     return " ".join(text)
 
 
-def _visit_drop_anything_mssql(
-    drop: DropTable | DropAlias | DropView | DropProcedure | DropFunction,
-    _type,
-    compiler,
-    **kw,
-):
-    _ = kw
-    table = compiler.preparer.quote_identifier(drop.name)
-    database, schema = _get_mssql_database_schema(drop.schema, compiler)
-    statements = []
-    text = [f"DROP {_type}"]
-    if drop.if_exists:
-        text.append("IF EXISTS")
-    if isinstance(drop, (DropAlias, DropView, DropProcedure, DropFunction)):
-        # attention: this statement must be prefixed with a 'USE <database>' statement
-        text.append(f"{schema}.{table}")
-        statements.append(f"USE {database}")
-    else:
-        text.append(f"{database}.{schema}.{table}")
-    statements.append(" ".join(text))
-    return join_ddl_statements(statements, compiler, **kw)
-
-
 # noinspection SqlDialectInspection
 @compiles(AddPrimaryKey)
 def visit_add_primary_key(add_primary_key: AddPrimaryKey, compiler, **kw):
     _ = kw
-    table = compiler.preparer.quote_identifier(add_primary_key.table_name)
+    table = compiler.preparer.quote(add_primary_key.table_name)
     schema = compiler.preparer.format_schema(add_primary_key.schema.get())
-    pk_name = compiler.preparer.quote_identifier(
+    pk_name = compiler.preparer.quote(
         add_primary_key.name
         if add_primary_key.name is not None
         else "pk_"
         + "_".join([c.lower() for c in add_primary_key.key])
         + "_"
         + add_primary_key.table_name.lower()
     )
-    cols = ",".join(
-        [compiler.preparer.quote_identifier(col) for col in add_primary_key.key]
-    )
+    cols = ",".join([compiler.preparer.quote(col) for col in add_primary_key.key])
     return f"ALTER TABLE {schema}.{table} ADD CONSTRAINT {pk_name} PRIMARY KEY ({cols})"
 
 
 # noinspection SqlDialectInspection
 @compiles(AddPrimaryKey, "duckdb")
 def visit_add_primary_key(add_primary_key: AddPrimaryKey, compiler, **kw):
     _ = kw
-    table = compiler.preparer.quote_identifier(add_primary_key.table_name)
+    table = compiler.preparer.quote(add_primary_key.table_name)
     schema = compiler.preparer.format_schema(add_primary_key.schema.get())
-    pk_name = compiler.preparer.quote_identifier(
+    pk_name = compiler.preparer.quote(
         add_primary_key.name
         if add_primary_key.name is not None
         else "pk_"
         + "_".join([c.lower() for c in add_primary_key.key])
         + "_"
         + add_primary_key.table_name.lower()
     )
-    cols = ",".join(
-        [compiler.preparer.quote_identifier(col) for col in add_primary_key.key]
-    )
+    cols = ",".join([compiler.preparer.quote(col) for col in add_primary_key.key])
     return f"CREATE UNIQUE INDEX {pk_name} ON {schema}.{table} ({cols})"
 
 
 # noinspection SqlDialectInspection
-@compiles(AddPrimaryKey, "mssql")
-def visit_add_primary_key(add_primary_key: AddPrimaryKey, compiler, **kw):
-    _ = kw
-    database, schema = _get_mssql_database_schema(add_primary_key.schema, compiler)
-
-    table = compiler.preparer.quote_identifier(add_primary_key.table_name)
-    pk_name = compiler.preparer.quote_identifier(
-        add_primary_key.name
-        if add_primary_key.name is not None
-        else "pk_"
-        + "_".join([c.lower() for c in add_primary_key.key])
-        + "_"
-        + add_primary_key.table_name.lower()
-    )
-    cols = ",".join(
-        [compiler.preparer.quote_identifier(col) for col in add_primary_key.key]
-    )
-    return (
-        f"ALTER TABLE {database}.{schema}.{table} ADD CONSTRAINT {pk_name} PRIMARY KEY"
-        f" ({cols})"
-    )
-
-
-# noinspection SqlDialectInspection
-@compiles(AddPrimaryKey, "ibm_db_sa")
-def visit_add_primary_key(add_primary_key: AddPrimaryKey, compiler, **kw):
-    _ = kw
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    add_primary_key = copy.deepcopy(add_primary_key)
-    add_primary_key.table_name = ibm_db_sa_fix_name(add_primary_key.table_name)
-
-    table = compiler.preparer.quote_identifier(add_primary_key.table_name)
-    schema = compiler.preparer.format_schema(add_primary_key.schema.get())
-    pk_name = compiler.preparer.quote_identifier(
-        add_primary_key.name
-        if add_primary_key.name is not None
-        else "pk_"
-        + "_".join([c.lower() for c in add_primary_key.key])
-        + "_"
-        + add_primary_key.table_name.lower()
-    )
-    cols = ",".join(
-        [
-            compiler.preparer.quote_identifier(ibm_db_sa_fix_name(col))
-            for col in add_primary_key.key
-        ]
-    )
-    return f"ALTER TABLE {schema}.{table} ADD CONSTRAINT {pk_name} PRIMARY KEY ({cols})"
-
-
-# noinspection SqlDialectInspection
 @compiles(AddIndex)
 def visit_add_index(add_index: AddIndex, compiler, **kw):
     _ = kw
-    table = compiler.preparer.quote_identifier(add_index.table_name)
+    table = compiler.preparer.quote(add_index.table_name)
     schema = compiler.preparer.format_schema(add_index.schema.get())
-    index_name = compiler.preparer.quote_identifier(
+    index_name = compiler.preparer.quote(
         add_index.name
         if add_index.name is not None
         else "idx_"
         + "_".join([c.lower() for c in add_index.index])
         + "_"
         + add_index.table_name.lower()
     )
-    cols = ",".join(
-        [compiler.preparer.quote_identifier(col) for col in add_index.index]
-    )
+    cols = ",".join([compiler.preparer.quote(col) for col in add_index.index])
     return f"CREATE INDEX {index_name} ON {schema}.{table} ({cols})"
 
 
 # noinspection SqlDialectInspection
-@compiles(AddIndex, "mssql")
-def visit_add_index(add_index: AddIndex, compiler, **kw):
-    _ = kw
-    database, schema = _get_mssql_database_schema(add_index.schema, compiler)
-
-    table = compiler.preparer.quote_identifier(add_index.table_name)
-    index_name = compiler.preparer.quote_identifier(
-        add_index.name
-        if add_index.name is not None
-        else "idx_"
-        + "_".join([c.lower() for c in add_index.index])
-        + "_"
-        + add_index.table_name.lower()
-    )
-    cols = ",".join(
-        [compiler.preparer.quote_identifier(col) for col in add_index.index]
-    )
-    return f"CREATE INDEX {index_name} ON {database}.{schema}.{table} ({cols})"
-
-
-# noinspection SqlDialectInspection
-@compiles(AddIndex, "ibm_db_sa")
-def visit_add_index(add_index: AddIndex, compiler, **kw):
-    _ = kw
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    add_index = copy.deepcopy(add_index)
-    add_index.table_name = ibm_db_sa_fix_name(add_index.table_name)
-
-    table = compiler.preparer.quote_identifier(add_index.table_name)
-    schema = compiler.preparer.format_schema(add_index.schema.get())
-    index_name = compiler.preparer.quote_identifier(
-        add_index.name
-        if add_index.name is not None
-        else "idx_"
-        + "_".join([c.lower() for c in add_index.index])
-        + "_"
-        + add_index.table_name.lower()
-    )
-    cols = ",".join(
-        [
-            compiler.preparer.quote_identifier(ibm_db_sa_fix_name(col))
-            for col in add_index.index
-        ]
-    )
-    return f"CREATE INDEX {schema}.{index_name} ON {schema}.{table} ({cols})"
-
-
-# noinspection SqlDialectInspection
 @compiles(ChangeColumnTypes)
 def visit_change_column_types(change: ChangeColumnTypes, compiler, **kw):
     _ = kw
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     alter_columns = ",".join(
         [
-            f"ALTER COLUMN {compiler.preparer.quote_identifier(col)} SET DATA TYPE"
+            f"ALTER COLUMN {compiler.preparer.quote(col)} SET DATA TYPE"
             f" {compiler.type_compiler.process(_type)}"
             for col, _type, nullable in zip(
                 change.column_names, change.column_types, change.nullable
             )
         ]
         + [
             "ALTER COLUMN"
-            f" {compiler.preparer.quote_identifier(col)}"
+            f" {compiler.preparer.quote(col)}"
             f" {'SET' if not nullable else 'DROP'} NOT NULL"
             for col, nullable in zip(change.column_names, change.nullable)
             if nullable is not None
         ]
     )
     return f"ALTER TABLE {schema}.{table} {alter_columns}"
 
 
 # noinspection SqlDialectInspection
 @compiles(ChangeColumnTypes, "duckdb")
 def visit_change_column_types_duckdb(change: ChangeColumnTypes, compiler, **kw):
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     alter_columns = [
-        f"ALTER COLUMN {compiler.preparer.quote_identifier(col)} SET DATA TYPE"
+        f"ALTER COLUMN {compiler.preparer.quote(col)} SET DATA TYPE"
         f" {compiler.type_compiler.process(_type)}"
         for col, _type, nullable in zip(
             change.column_names, change.column_types, change.nullable
         )
     ] + [
         "ALTER COLUMN"
-        f" {compiler.preparer.quote_identifier(col)}"
+        f" {compiler.preparer.quote(col)}"
         f" {'SET' if not nullable else 'DROP'} NOT NULL"
         for col, nullable in zip(change.column_names, change.nullable)
         if nullable is not None
     ]
     statements = [
         f"ALTER TABLE {schema}.{table} {statement}" for statement in alter_columns
     ]
     return join_ddl_statements(statements, compiler, **kw)
 
 
 # noinspection SqlDialectInspection
 @compiles(ChangeColumnTypes, "mssql")
 def visit_change_column_types(change: ChangeColumnTypes, compiler, **kw):
     _ = kw
-    database, schema = _get_mssql_database_schema(change.schema, compiler)
 
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
+    schema = compiler.preparer.format_schema(change.schema.get())
 
     def modify_type(_type):
         if change.cap_varchar_max is not None:
             _type = copy.copy(_type)
             if isinstance(_type, sa.String) and (
                 _type.length is None or _type.length > change.cap_varchar_max
             ):
                 # impose some limit to allow use in primary key / index
                 _type.length = change.cap_varchar_max
         return _type
 
     statements = [
-        f"ALTER TABLE {database}.{schema}.{table} ALTER COLUMN"
-        f" {compiler.preparer.quote_identifier(col)} "
+        f"ALTER TABLE {schema}.{table} ALTER COLUMN"
+        f" {compiler.preparer.quote(col)} "
         f"{compiler.type_compiler.process(modify_type(_type))}"
         f"{'' if nullable is None else ' NULL' if nullable else ' NOT NULL'}"
         for col, _type, nullable in zip(
             change.column_names, change.column_types, change.nullable
         )
     ]
     return join_ddl_statements(statements, compiler, **kw)
 
 
 # noinspection SqlDialectInspection
 @compiles(ChangeColumnTypes, "ibm_db_sa")
 def visit_change_column_types(change: ChangeColumnTypes, compiler, **kw):
     _ = kw
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    change = copy.deepcopy(change)
-    change.table_name = ibm_db_sa_fix_name(change.table_name)
 
     def modify_type(_type):
         if change.cap_varchar_max is not None:
             _type = copy.copy(_type)
             if isinstance(_type, sa.String) and (
                 _type.length is None or _type.length > change.cap_varchar_max
             ):
                 # impose some limit to allow use in primary key / index
                 _type.length = change.cap_varchar_max
         return _type
 
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     statements = [
         f"ALTER TABLE {schema}.{table} ALTER COLUMN"
-        f" {compiler.preparer.quote_identifier(ibm_db_sa_fix_name(col))} SET DATA TYPE"
+        f" {compiler.preparer.quote(col)} SET DATA TYPE"
         f" {compiler.type_compiler.process(modify_type(_type))}"
         for col, _type, nullable in zip(
             change.column_names, change.column_types, change.nullable
         )
     ] + [
         f"ALTER TABLE {schema}.{table} ALTER COLUMN"
-        f" {compiler.preparer.quote_identifier(ibm_db_sa_fix_name(col))}"
+        f" {compiler.preparer.quote(col)}"
         f" {'SET' if not nullable else 'DROP'} NOT NULL"
         for col, nullable in zip(change.column_names, change.nullable)
         if nullable is not None
     ]
     statements.append(f"call sysproc.admin_cmd('REORG TABLE {schema}.{table}')")
     return join_ddl_statements(statements, compiler, **kw)
 
 
 # noinspection SqlDialectInspection
 @compiles(ChangeColumnNullable)
 def visit_change_column_nullable(change: ChangeColumnNullable, compiler, **kw):
     _ = kw
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     alter_columns = ",".join(
         [
             "ALTER COLUMN"
-            f" {compiler.preparer.quote_identifier(col)}"
+            f" {compiler.preparer.quote(col)}"
             f" {'SET' if not nullable else 'DROP'} NOT NULL"
             for col, nullable in zip(change.column_names, change.nullable)
         ]
     )
     return f"ALTER TABLE {schema}.{table} {alter_columns}"
 
 
 # noinspection SqlDialectInspection
 @compiles(ChangeColumnNullable, "ibm_db_sa")
 def visit_change_column_nullable(change: ChangeColumnNullable, compiler, **kw):
     _ = kw
-    # DB2 stores capitalized table names but sqlalchemy reflects them lowercase
-    change = copy.deepcopy(change)
-    change.table_name = ibm_db_sa_fix_name(change.table_name)
-
     statements = _get_nullable_change_statements(change, compiler)
     return join_ddl_statements(statements, compiler, **kw)
 
 
 @compiles(ChangeTableLogged, "postgresql")
 def visit_change_table_logged(change: ChangeTableLogged, compiler, **kw):
     _ = kw
-    table_name = compiler.preparer.quote_identifier(change.table_name)
+    table_name = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     logged = "LOGGED" if change.logged else "UNLOGGED"
     return f"ALTER TABLE {schema}.{table_name} SET {logged}"
 
 
 def _get_nullable_change_statements(change, compiler):
-    table = compiler.preparer.quote_identifier(change.table_name)
+    table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     statements = [
         f"ALTER TABLE {schema}.{table} ALTER COLUMN"
-        f" {compiler.preparer.quote_identifier(ibm_db_sa_fix_name(col))}"
+        f" {compiler.preparer.quote(col)}"
         f" {'SET' if not nullable else 'DROP'} NOT NULL"
         for col, nullable in zip(change.column_names, change.nullable)
     ]
     statements.append(f"call sysproc.admin_cmd('REORG TABLE {schema}.{table}')")
     return statements
 
 
-def ibm_db_sa_fix_name(name):
-    # DB2 seems to create tables uppercase if all lowercase given
-    # TODO: consider moving this replacement to call in sql.py
-    return name.upper() if name.islower() else name
+def _mssql_update_definition(
+    conn: sa.Connection,
+    name: str,
+    old_schema: Schema,
+    new_schema: Schema,
+) -> str:
+    """
+    Loads the definition of object `name` in `old_schema`, and replaces all references
+    to `old_schema` inside the definition with `new_schema`.
+
+    :return: updated definition referencing `new_schema` instead of `old_schema`.
+    """
+
+    # Get definition from database (using unquoted name)
+    query = f"SELECT OBJECT_DEFINITION(OBJECT_ID(N'{old_schema.get()}.{name}'))"
+    definition = conn.exec_driver_sql(query).scalar_one()
+
+    # Replace unquoted names with quoted ones
+    identifier_preparer = conn.dialect.identifier_preparer
+    old_schema = identifier_preparer.format_schema(old_schema.get())
+    new_schema = identifier_preparer.format_schema(new_schema.get())
+
+    # Replace schema in definition with new destination schema
+    string_literal = pp.QuotedString(quote_char="'", esc_quote="''")
+    quoted_identifier = pp.QuotedString(
+        quote_char="[", esc_quote="]]", end_quote_char="]"
+    )
+
+    schema_expr = pp.CaselessKeyword(old_schema).ignore(string_literal)
+    if old_schema.startswith("["):
+        schema_expr = schema_expr.ignore(quoted_identifier)
+    else:
+        schema_expr = schema_expr.ignore(quoted_identifier) | (
+            pp.Literal("[") + schema_expr + pp.Literal("]")
+        )
+
+    schema_expr = schema_expr.set_parse_action(pp.replace_with(new_schema))
+    expr = schema_expr + pp.FollowedBy(".")
+
+    return expr.transform_string(definition)
 
 
 STATEMENT_SEPERATOR = "; -- PYDIVERSE-PIPEDAG-SPLIT\n"
 
 
 def join_ddl_statements(statements, compiler, **kw):
     """Mechanism to combine multiple DDL statements into one."""
@@ -1260,17 +1122,12 @@
         else:
             statement_strings.append(compiler.process(statement, **kw))
     return STATEMENT_SEPERATOR.join(statement_strings)
 
 
 def split_ddl_statement(statement: str):
     """Split previously combined DDL statements apart"""
-    return statement.split(STATEMENT_SEPERATOR)
-
-
-def _get_mssql_database_schema(schema: Schema, compiler):
-    full_name = schema.get()
-    # it was already checked that there is exactly one dot in schema prefix + suffix
-    database_name, schema_name = full_name.split(".")
-    database = compiler.preparer.format_schema(database_name)
-    schema = compiler.preparer.format_schema(schema_name)
-    return database, schema
+    return [
+        statement
+        for statement in statement.split(STATEMENT_SEPERATOR)
+        if statement.strip() != ""
+    ]
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from contextvars import ContextVar, Token
 from enum import Enum
 from functools import cached_property
 from threading import Lock
 from typing import TYPE_CHECKING, ClassVar
 
 import structlog
-from attrs import define, evolve, frozen
+from attrs import define, evolve, field, frozen
 from box import Box
 
 from pydiverse.pipedag.util.import_ import import_object, load_object
+from pydiverse.pipedag.util.naming import NameDisambiguator
 
 if TYPE_CHECKING:
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
     from pydiverse.pipedag.core import Flow, Stage, Task
     from pydiverse.pipedag.engine.base import OrchestrationEngine
@@ -82,14 +83,15 @@
 
     It is used to retrieve a reference to the task object from within a running task.
     It also serves as a place to store temporary state while processing a task.
     """
 
     task: Task
     is_cache_valid: bool | None = None
+    name_disambiguator: NameDisambiguator = field(factory=NameDisambiguator)
 
     _context_var = ContextVar("task_context")
 
 
 class StageCommitTechnique(Enum):
     SCHEMA_SWAP = 0
     READ_VIEWS = 1
@@ -124,15 +126,17 @@
     strict_result_get_locking: bool
     ignore_task_version: bool
     instance_id: str  # may be used as database name or locking ID
     stage_commit_technique: StageCommitTechnique
     network_interface: str
     attrs: Box
 
-    # other configuration options
+    table_hook_args: Box
+
+    # run specific options
     ignore_fresh_input: bool = False
 
     # INTERNAL FLAGS - ONLY FOR PIPEDAG USE
     # When set to True, exceptions raised in a flow don't get logged
     _swallow_exceptions: bool = False
 
     @cached_property
@@ -141,80 +145,75 @@
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
         return tuple(map(import_object, self._config_dict.get("auto_blob", ())))
 
     @cached_property
     def store(self):
-        from pydiverse.pipedag.backend.table_cache import LocalTableCache
         from pydiverse.pipedag.materialize.store import PipeDAGStore
 
         # Load objects referenced in config
         try:
             table_store_config = self._config_dict["table_store"]
             table_store = load_object(table_store_config)
-            if "local_table_cache" in table_store_config:
-                local_cache_config = table_store_config["local_table_cache"]
-                local_table_cache = LocalTableCache(
-                    load_object(local_cache_config),
-                    local_cache_config.get("store_input", True),
-                    local_cache_config.get("store_output", False),
-                    local_cache_config.get("use_stored_input_as_cache", True),
-                )
-                unknown_attributes = set(local_cache_config.keys()) - {
-                    "class",
-                    "args",
-                    "store_input",
-                    "store_output",
-                    "use_stored_input_as_cache",
-                }
-                if len(unknown_attributes) > 0:
-                    raise AttributeError(
-                        (
-                            "Unknown attributes in local_table_cache config:"
-                            f" {unknown_attributes}"
-                        ),
-                    )
-            else:
-                local_table_cache = LocalTableCache(
-                    None,
-                    store_input=False,
-                    store_output=False,
-                    use_stored_input_as_cache=False,
-                )
         except Exception as e:
             raise RuntimeError("Failed loading table_store") from e
 
         try:
             blob_store = load_object(self._config_dict["blob_store"])
         except Exception as e:
             raise RuntimeError("Failed loading blob_store") from e
 
+        try:
+            local_table_cache = None
+            local_table_cache_config = table_store_config.get("local_table_cache", None)
+            if local_table_cache_config is not None:
+                local_table_cache = load_object(
+                    local_table_cache_config,
+                    move_keys_into_args=(
+                        "store_input",
+                        "store_output",
+                        "use_stored_input_as_cache",
+                    ),
+                )
+        except Exception as e:
+            raise RuntimeError("Failed loading local_table_cache") from e
+
         return PipeDAGStore(
             table=table_store,
             blob=blob_store,
             local_table_cache=local_table_cache,
         )
 
     def evolve(self, **changes) -> ConfigContext:
         """Create a new instance with the changes applied; Wrapper for attrs.evolve"""
-        return evolve(self, **changes)
+        evolved = evolve(self, **changes)
+
+        # Transfer cached properties
+        cached_properties = ["auto_table", "auto_blob", "store"]
+        for name in cached_properties:
+            if name in self.__dict__:
+                evolved.__dict__[name] = self.__dict__[name]
+                evolved.__dict__[f"__{name}_inherited"] = True
+
+        return evolved
 
     def create_lock_manager(self) -> BaseLockManager:
         return load_object(self._config_dict["lock_manager"])
 
     def create_orchestration_engine(self) -> OrchestrationEngine:
         return load_object(self._config_dict["orchestration"])
 
     def close(self):
         # If the store has been initialized (and thus cached in the __dict__),
         # dispose of it, and remove it from the cache.
         if store := self.__dict__.get("store", None):
-            store.dispose()
-            self.__dict__.pop("store")
+            if not self.__dict__.get("__store_inherited", False):
+                store.dispose()
+                self.__dict__.pop("store")
 
     def __getstate__(self):
         state = super().__getstate__()
         # store is not serializable, but @cached_property will reload
         # it from config_dict
         state.pop("store", None)
         state.pop("auto_table", None)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/run_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,20 +215,23 @@
             stage_id,
             success,
             StageState.INITIALIZING,
             StageState.READY,
         )
 
     def enter_commit_stage(self, stage_id: int):
+        self._await_deferred_ts_ops(stage_id)
         if self.has_stage_changed(stage_id):
             self._trigger_deferred_ts_ops(
                 stage_id, DeferredTableStoreOp.Condition.ON_STAGE_COMMIT
             )
         else:
-            self.abort_stage(stage_id)
+            self._trigger_deferred_ts_ops(
+                stage_id, DeferredTableStoreOp.Condition.ON_STAGE_ABORT
+            )
         self._await_deferred_ts_ops(stage_id)
 
         return self._enter_stage_state_transition(
             stage_id,
             StageState.READY,
             StageState.COMMITTING,
             StageState.COMMITTED,
@@ -370,22 +373,14 @@
         if stage_id not in self.deferred_ts_ops_futures:
             return
 
         futures = self.deferred_ts_ops_futures[stage_id]
         for future in futures:
             future.result()
 
-    @synchronized("deferred_ops_lock")
-    def abort_stage(self, stage_id: int):
-        self._await_deferred_ts_ops(stage_id)
-        self._trigger_deferred_ts_ops(
-            stage_id, DeferredTableStoreOp.Condition.ON_STAGE_ABORT
-        )
-        self._await_deferred_ts_ops(stage_id)
-
     # TASK
 
     def did_finish_task(self, task_id: int, final_state_value: int):
         final_state = FinalTaskState(final_state_value)
         task = self.tasks[task_id]
 
         self.task_state[task_id] = final_state
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,17 @@
             ignore_task_version=config["ignore_task_version"],
             instance_name=instance,
             instance_id=config["instance_id"],
             stage_commit_technique=stage_commit_technique,
             fail_fast=config["fail_fast"],
             network_interface=config["network_interface"],
             attrs=Box(config["attrs"], frozen_box=True),
+            table_hook_args=Box(
+                config["table_store"].get("hook_args", {}), frozen_box=True
+            ),
         )
 
         if "PYDIVERSE_PIPEDAG_PYTEST" not in os.environ:
             # If we're running test cases, this can be skipped to improve performance
             try:
                 # Make sure @cached_property store is set up and loaded
                 # and throw config errors early.
@@ -196,19 +199,18 @@
 
         return config_context
 
     def __get_merged_config_dict(self, instance, flow, default=None):
         search_paths = [
             ("instances", "__any__"),
             ("instances", instance),
-            ("flows", "__any__", "instances", "__any__"),
+            ("flows", "__any__"),
             ("flows", "__any__", "instances", instance),
-            ("flows", flow, "instances", "__any__"),
-            ("flows", flow, "instances", instance),
             ("flows", flow),
+            ("flows", flow, "instances", instance),
         ]
 
         search_paths = [path for path in search_paths if None not in path]
         dicts = [_get(self.config_dict, path, default=None) for path in search_paths]
 
         # Check for strict instance lookup
         # If instance is specified, make sure that a corresponding section can be found
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,14 +133,18 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.commit_task = CommitStageTask(self, self._ctx.flow)
         self._ctx.flow.add_task(self.commit_task)
         self._ctx.__exit__()
         del self._ctx
 
+        if len(self.tasks) == 0:
+            # Empty stage doesn't need to be committed
+            self.commit_task._skip_commit = True
+
     def all_tasks(self):
         yield from self.tasks
         yield self.commit_task
 
     def is_inner(self, other: Stage):
         outer = self.outer_stage
         while outer is not None:
@@ -164,16 +168,20 @@
             name=f"Commit '{stage.name}'",
         )
 
         self.stage = stage
         self.flow = flow
         self.upstream_stages = {stage}
         self.input_tasks = {}
+        self._skip_commit = False
 
         self.logger = self.logger.bind(logger_name="Commit Stage", stage=stage)
 
         self._bound_args = self._signature.bind()
         self._visualize_hidden = True
 
     def fn(self):
+        if self._skip_commit:
+            return
+
         self.logger.info("Committing stage")
         ConfigContext.get().store.commit_stage(self.stage)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import click
 
 from pydiverse.pipedag import PipedagConfig
 from pydiverse.pipedag.backend.table import SQLTableStore
-from pydiverse.pipedag.backend.table.util.sql_ddl import DropSchema
+from pydiverse.pipedag.backend.table.sql.ddl import DropSchema
 from pydiverse.pipedag.management.cli import cli
 
 
 @cli.command(
     help="delete all metadata",
 )
 @click.option(
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,22 +73,24 @@
     _query_hash: str
     _is_cache_valid: bool
 
     # The public interface is exposed as functions
     def is_cache_valid(self):
         return self._is_cache_valid
 
-    def store_raw_sql_metadata(self, store: BaseTableStore, prev_tables, post_tables):
+    def store_raw_sql_metadata(
+        self, store: BaseTableStore, prev_objects: list[str], new_objects: list[str]
+    ):
         # Store metadata
         # Attention: Raw SQL statements may only be executed sequentially within
-        #            stage for store.list_tables to work
+        #            stage for store.get_objects_in_stage to work
         store.store_raw_sql_metadata(
             RawSqlMetadata(
-                prev_tables=prev_tables,
-                tables=post_tables,
+                prev_objects=prev_objects,
+                new_objects=new_objects,
                 stage=self._stage.name,
                 query_hash=self._query_hash,
                 task_hash=self._task_hash,
             )
         )
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,16 @@
                         raise indexes_type_error
 
         # cache_key will be overridden shortly before handing over to downstream tasks
         # that use it to compute their input_hash for cache_invalidation due to input
         # change
         self.cache_key = None
 
-    def __str__(self):
-        return f"<Table: {self.name} ({self.stage.name})>"
+    def __repr__(self):
+        return f"<Table '{self.name}' ({self.stage.name})>"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
@@ -116,15 +116,15 @@
         # cache_key will be overridden shortly before handing over to downstream tasks
         # that use it to compute their input_hash for cache_invalidation due to input
         # change
         self.cache_key = None
 
     def __str__(self):
         sql_short = self.sql.strip()[0:40].replace("\n", "").strip()
-        return f"<Raw SQL: {self.name}/{self.stage}:{sql_short}>"
+        return f"<Raw SQL '{self.name}' ({self.stage}) - {sql_short}>"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
@@ -160,16 +160,16 @@
         self.stage = stage
 
         # cache_key will be overridden shortly before handing over to downstream tasks
         # that use it to compute their input_hash for cache_invalidation due to input
         # change
         self.cache_key = None
 
-    def __str__(self):
-        return f"<Blob: {self.name} ({self.stage.name})>"
+    def __repr__(self):
+        return f"<Blob '{self.name}' ({self.stage.name})>"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,20 +52,20 @@
 @dataclass
 class RawSqlMetadata:
     """Metadata associated with raw sql statements
 
     The `query_hash` is a hash of the raw sql string.
     The `task_hash` is the combined hash of the task that produced statement.
 
-    The `tables` and `stage` values are used to retrieve the appropriate
+    The `prev_objects` and `stage` values are used to retrieve the appropriate
     tables from the cache.
 
     Attention: `task_hash` is sometimes taken from cache and thus is not guaranteed
     to refer to the `task_hash` that corresponds to the currently executed task.
     Instead, it refers to the task that originally produced this object.
     """
 
-    prev_tables: list[str]
-    tables: list[str]
+    prev_objects: list[str]
+    new_objects: list[str]
     stage: str
     query_hash: str
     task_hash: str
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pydiverse.pipedag.context.run_context import StageState
 from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.errors import DuplicateNameError, StageError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.materialize.metadata import TaskMetadata
 from pydiverse.pipedag.util import Disposable, deep_map
-from pydiverse.pipedag.util.naming import NameDisambiguator
 
 
 class PipeDAGStore(Disposable):
     """Main storage interface for materializing tasks
 
     Depending on the use case, the store can be configured using different
     backends for storing tables, blobs and managing locks.
@@ -29,19 +28,20 @@
     between the different backends, the stages and the materializing tasks.
     """
 
     def __init__(
         self,
         table: backend.table.BaseTableStore,
         blob: backend.blob.BaseBlobStore,
-        local_table_cache: backend.table_cache.LocalTableCache,
+        local_table_cache: backend.table.cache.BaseTableCache | None,
     ):
         self.table_store = table
         self.blob_store = blob
         self.local_table_cache = local_table_cache
+        self.table_store.local_table_cache = local_table_cache
 
         self.logger = structlog.get_logger()
 
         from pydiverse.pipedag.util.json import PipedagJSONDecoder, PipedagJSONEncoder
 
         self.json_encoder = PipedagJSONEncoder()
         self.json_decoder = PipedagJSONDecoder()
@@ -50,15 +50,15 @@
         """
         Clean up and close all open resources.
 
         Don't use the store object any more after disposal!
         """
         self.table_store.dispose()
         self.blob_store.dispose()
-        if self.local_table_cache is not None:
+        if self.local_table_cache:
             self.local_table_cache.dispose()
         super().dispose()
 
     # ### Stage ### #
 
     def init_stage(self, stage: Stage):
         """Initializes the stage in all backends
@@ -71,14 +71,16 @@
         Don't use this function directly. Instead, use `ensure_stage_is_ready`
         to prevent unnecessary locking.
         """
 
         RunContext.get().validate_stage_lock(stage)
         self.table_store.init_stage(stage)
         self.blob_store.init_stage(stage)
+        if self.local_table_cache:
+            self.local_table_cache.init_stage(stage)
 
         # Once stage reference counter hits 0 (this means all tasks that
         # have any task contained in the stage as an upstream dependency),
         # the lock gets automatically released by the RunContextServer
 
     def ensure_stage_is_ready(self, stage: Stage):
         """Initializes a stage if it hasn't been created yet
@@ -104,33 +106,22 @@
     # ### Materialization ### #
 
     def dematerialize_item(
         self,
         item: Table | Blob | Any,
         as_type: type[T],
         ctx: RunContext | None = None,
-        namer: NameDisambiguator | None = None,
     ):
         if ctx is None:
             ctx = RunContext.get()
 
         if isinstance(item, Table):
             ctx.validate_stage_lock(item.stage)
-            if self.local_table_cache.has_cache_table(item, as_type):
-                return self.local_table_cache.retrieve_table_obj(item, as_type, namer)
-            else:
-                obj = self.table_store.retrieve_table_obj(
-                    item, as_type=as_type, namer=namer
-                )
-                table = item.copy_without_obj()
-                table.obj = obj
-                self.local_table_cache.store_table(
-                    table, task=None, task_info=None, is_input=True
-                )
-                return obj
+            obj = self.table_store.retrieve_table_obj(item, as_type=as_type)
+            return obj
         elif isinstance(item, Blob):
             ctx.validate_stage_lock(item.stage)
             return self.blob_store.retrieve_blob(item)
         return item
 
     def dematerialize_task_inputs(
         self,
@@ -148,22 +139,19 @@
         :param kwargs: The keyword arguments
         :return: A tuple with the dematerialized args and kwargs
         """
 
         ctx = RunContext.get()
 
         input_tables = []
-        namer = NameDisambiguator(prefix="t")
 
         def dematerialize_mapper(x):
             if isinstance(x, Table):
                 input_tables.append(x)
-            return self.dematerialize_item(
-                x, as_type=task.input_type, ctx=ctx, namer=namer
-            )
+            return self.dematerialize_item(x, as_type=task.input_type, ctx=ctx)
 
         d_args = deep_map(args, dematerialize_mapper)
         d_kwargs = deep_map(kwargs, dematerialize_mapper)
 
         return d_args, d_kwargs, input_tables
 
     def materialize_task(
@@ -280,17 +268,14 @@
                 output_json, self.table_store, stage
             )
 
         def store_table(table: Table):
             if task.lazy:
                 self.table_store.store_table_lazy(table, task, task_info)
             else:
-                self.local_table_cache.store_table(
-                    table, task, task_info, is_input=False
-                )
                 self.table_store.store_table(table, task, task_info)
 
         # Materialize
         self._check_names(task, tables, blobs)
         self._store_task_transaction(
             task,
             tables,
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/disposable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from __future__ import annotations
+
 from pydiverse.pipedag.errors import DisposedError
 
 
 class Disposable:
     def __getattribute__(self, name):
         try:
             object.__getattribute__(self, "_Disposable__disposed")
             obj_type = object.__getattribute__(self, "__class__")
             raise DisposedError(f"Object of type {obj_type} has already been disposed.")
         except AttributeError:
-            return object.__getattribute__(self, name)
+            pass
+
+        return object.__getattribute__(self, name)
 
     def __setattr__(self, key, value):
         try:
             object.__getattribute__(self, "_Disposable__disposed")
             obj_type = object.__getattribute__(self, "__class__")
             raise DisposedError(f"Object of type {obj_type} has already been disposed.")
         except AttributeError:
-            return object.__setattr__(self, key, value)
+            pass
+
+        return object.__setattr__(self, key, value)
 
     def dispose(self):
         object.__setattr__(self, "_Disposable__disposed", True)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/hashing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import base64
 import hashlib
 
 
 def stable_hash(*args: str) -> str:
     """Compute a hash over a set of strings
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/import_.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import builtins
 import importlib
+from collections.abc import Collection
 from typing import Any
 
 
 def requires(requirements: Any | list, exception: BaseException | type[BaseException]):
     """Class decorator for handling optional imports.
 
     If any of the requirements are falsy, this decorator prevents the class
@@ -63,30 +64,34 @@
     obj = module or builtins
     for part in parts[n:]:
         obj = getattr(obj, part)
 
     return obj
 
 
-def load_object(config_dict: dict):
+def load_object(config_dict: dict, move_keys_into_args: Collection[str] | None = None):
     """Instantiates an instance of an object given
 
     The import path (module.Class) should be specified as the "class" value
     of the dict. The args section of the dict get used as the instance config.
 
     If the class defines a `_init_conf_` function, it gets called using the
     config values, otherwise they just get passed to the class initializer.
 
-    >>> # module.Class(argument="value")
-    >>> load_object({
-    >>>     "class": "module.Class",
-    >>>     "args": {
-    >>>         "argument": "value",
-    >>>     },
-    >>> })
+    Additionally, any values of `config_dict` whose associated keys are in
+    `move_keys_into_args`, get also passed as an argument to the initializer.
+    ::
+
+        # module.Class(argument="value")
+        load_object({
+            "class": "module.Class",
+            "args": {
+                "argument": "value",
+            },
+        })
     """
 
     if "class" not in config_dict:
         raise RuntimeError(
             "Attribute 'class' is missing in configuration "
             "section that supports multiple backends\n"
             f"config section: {config_dict}"
@@ -95,12 +100,16 @@
 
     args = config_dict.get("args", {})
     if not isinstance(args, dict):
         raise TypeError(
             f"Invalid type for args section: {type(args)}\n"
             f"config section: {config_dict}"
         )
+
+    if move_keys_into_args:
+        args = args | {k: v for k, v in config_dict.items() if k in move_keys_into_args}
+
     try:
         init_conf = cls._init_conf_
         return init_conf(args)
     except AttributeError:
         return cls(**args)
```

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.5.0/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/structlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import sys
 import textwrap
 from io import StringIO
 
 import structlog
 from structlog.typing import EventDict, WrappedLogger
```

### Comparing `pydiverse_pipedag-0.5.0/PKG-INFO` & `pydiverse_pipedag-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.5.0
+Version: 0.6.0
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -29,14 +29,15 @@
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pandas (>=1.4.3)
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pydot (>=1.4.2)
 Requires-Dist: pynng (>=0.7.1)
+Requires-Dist: pyparsing (>=3.0)
 Requires-Dist: python-box (>=6.1.0)
 Requires-Dist: structlog (>=22.1.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pydiverse.pipedag
 
@@ -181,15 +182,15 @@
         # print final sql statements
         print_sql: true
 
       local_table_cache:
         store_input: true
         store_output: true
         use_stored_input_as_cache: true
-        class: "pydiverse.pipedag.backend.table_cache.ParquetTableCache"
+        class: "pydiverse.pipedag.backend.table.cache.ParquetTableCache"
         args:
           base_path: "/tmp/pipedag/table_cache"
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
       args:
         base_path: "/tmp/pipedag/blobs"
```

