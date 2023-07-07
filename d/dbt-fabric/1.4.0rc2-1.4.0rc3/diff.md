# Comparing `tmp/dbt-fabric-1.4.0rc2.tar.gz` & `tmp/dbt-fabric-1.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.4.0rc2.tar", last modified: Wed Jun 14 00:00:21 2023, max compression
+gzip compressed data, was "dbt-fabric-1.4.0rc3.tar", last modified: Fri Jul  7 06:49:12 2023, max compression
```

## Comparing `dbt-fabric-1.4.0rc2.tar` & `dbt-fabric-1.4.0rc3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.623928 dbt-fabric-1.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:00:21.623928 dbt-fabric-1.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.211070 dbt-fabric-1.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 06:49:12.211070 dbt-fabric-1.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.203070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.207070 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:49:12.211070 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 06:49:12.000000 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-07 06:49:12.000000 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:49:12.000000 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 06:49:12.000000 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 06:49:12.000000 dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:49:12.211070 dbt-fabric-1.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 06:48:27.000000 dbt-fabric-1.4.0rc3/setup.py
```

### Comparing `dbt-fabric-1.4.0rc2/LICENSE` & `dbt-fabric-1.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/PKG-INFO` & `dbt-fabric-1.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.4.0rc2/README.md` & `dbt-fabric-1.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.4.0rc3/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         con_str.append(bool_to_connection_string_arg("encrypt", credentials.encrypt))
         con_str.append(
             bool_to_connection_string_arg("TrustServerCertificate", credentials.trust_cert)
         )
 
         plugin_version = __version__.version
         application_name = f"dbt-{credentials.type}/{plugin_version}"
-        con_str.append(f"Application Name={application_name}")
+        con_str.append(f"APP={application_name}")
 
         con_str_concat = ";".join(con_str)
 
         index = []
         for i, elem in enumerate(con_str):
             if "pwd=" in elem.lower():
                 index.append(i)
```

### Comparing `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.4.0rc3/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/test.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/split_part.sql` & `dbt-fabric-1.4.0rc3/dbt/include/fabric/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.4.0rc3/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc2/setup.py` & `dbt-fabric-1.4.0rc3/setup.py`

 * *Files identical despite different names*

