# Comparing `tmp/dbt-oracle-1.5.1rc1.tar.gz` & `tmp/dbt-oracle-1.5.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-oracle-1.5.1rc1.tar", last modified: Thu Jun 15 17:12:17 2023, max compression
+gzip compressed data, was "dbt-oracle-1.5.1rc2.tar", last modified: Thu Jul  6 23:24:55 2023, max compression
```

## Comparing `dbt-oracle-1.5.1rc1.tar` & `dbt-oracle-1.5.1rc2.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.731519 dbt-oracle-1.5.1rc1/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.1rc1/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.1rc1/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.1rc1/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.1rc1/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-06-15 17:12:17.731717 dbt-oracle-1.5.1rc1/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.274199 dbt-oracle-1.5.1rc1/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.1rc1/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.278561 dbt-oracle-1.5.1rc1/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.1rc1/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.281213 dbt-oracle-1.5.1rc1/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.1rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.300392 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    11633 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    16010 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.303137 dbt-oracle-1.5.1rc1/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.1rc1/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.328338 dbt-oracle-1.5.1rc1/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.346517 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    14870 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/columns.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.237899 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.371106 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4373 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.374613 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/python_model/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3412 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/python_model/python.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.378757 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.400526 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.425796 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5486 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.430916 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.437725 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/view.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/schema_tests.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.539295 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.597033 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     4177 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.1rc1/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1446 2023-06-15 17:12:17.733257 dbt-oracle-1.5.1rc1/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-06-15 17:11:44.000000 dbt-oracle-1.5.1rc1/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.636261 dbt-oracle-1.5.1rc1/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.1rc1/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.1rc1/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.240158 dbt-oracle-1.5.1rc1/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.679712 dbt-oracle-1.5.1rc1/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.684892 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/fixtures.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.692247 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.698927 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.701920 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.722119 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.724696 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/test_simple_seed.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.726755 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_caching.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.730716 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_dateutils.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.924222 dbt-oracle-1.5.1rc2/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.1rc2/HISTORY.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.1rc2/LICENSE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.1rc2/MANIFEST.in
+-rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.1rc2/NOTICE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-06 23:24:55.924393 dbt-oracle-1.5.1rc2/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/README.md
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.679486 dbt-oracle-1.5.1rc2/bin/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.1rc2/bin/create-pem-from-p12
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.681639 dbt-oracle-1.5.1rc2/dbt/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.1rc2/dbt/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.684117 dbt-oracle-1.5.1rc2/dbt/adapters/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.1rc2/dbt/adapters/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.700775 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-07-03 19:36:07.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__version__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/column.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connection_helper.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11633 2023-07-05 22:26:22.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connections.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14634 2023-07-06 17:14:57.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/impl.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/keyword_catalog.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    10054 2023-07-06 22:57:39.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/python_submissions.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/relation.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.702580 dbt-oracle-1.5.1rc2/dbt/include/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.1rc2/dbt/include/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.712661 dbt-oracle-1.5.1rc2/dbt/include/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/dbt_project.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.728603 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14870 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/adapters.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/apply_grants.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/catalog.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/columns.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.665531 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.740613 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4373 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.752296 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3412 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/python.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.756227 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.768434 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.774998 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5486 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/table.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.782236 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.788842 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/view.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/schema_tests.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.861091 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/data_types.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/dateadd.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datediff.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datetrunc.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/except.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/hash.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/last_day.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/position.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/right.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/timestamps.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/profile_template.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.867016 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4219 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/requires.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/top_level.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.1rc2/pyproject.toml
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1449 2023-07-06 23:24:55.926019 dbt-oracle-1.5.1rc2/setup.cfg
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-07-06 23:24:15.000000 dbt-oracle-1.5.1rc2/setup.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.873521 dbt-oracle-1.5.1rc2/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/README.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.1rc2/tests/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.1rc2/tests/conftest.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.666638 dbt-oracle-1.5.1rc2/tests/functional/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.892958 dbt-oracle-1.5.1rc2/tests/functional/adapter/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.897876 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/fixtures.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.903565 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.909258 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.912328 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_unique_id.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.914778 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/test_alter_column_type.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.919222 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/test_simple_seed.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.921130 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/test_invalidate_deletes.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_basic.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_caching.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_config.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_data_types.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_genreferences.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_generictests_where.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_grants.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_quoted_relations.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.923588 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_common_utils.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt-oracle-1.5.1rc1/LICENSE.txt` & `dbt-oracle-1.5.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/PKG-INFO` & `dbt-oracle-1.5.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.1rc1
+Version: 1.5.1rc2
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.1rc1/README.md` & `dbt-oracle-1.5.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/bin/create-pem-from-p12` & `dbt-oracle-1.5.1rc2/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/__init__.py` & `dbt-oracle-1.5.1rc2/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/__init__.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__init__.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__version__.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 """
-version = "1.5.1"
+version = "1.5.2"
```

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/column.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connection_helper.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connections.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
     cclass: Optional[str] = None
     purity: Optional[str] = None
 
     # Connection retry params
     retry_count: Optional[int] = 1
     retry_delay: Optional[int] = 3
 
-    # Fetch an auth token to run Python UDF
-    oml_auth_token_uri: Optional[str] = None
+    # Base URL for ADB-S OML REST API
+    oml_cloud_service_url: Optional[str] = None
 
 
     _ALIASES = {
         'dbname': 'database',
         'pass': 'password',
     }
 
@@ -132,15 +132,15 @@
         """
         return (
             'user', 'database', 'schema',
             'protocol', 'host', 'port', 'tns_name',
             'service', 'connection_string',
             'shardingkey', 'supershardingkey',
             'cclass', 'purity', 'retry_count',
-            'retry_delay', 'oml_auth_token_uri'
+            'retry_delay', 'oml_cloud_service_url'
         )
 
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
         # If database is not defined as adapter credentials
         data = super().__pre_deserialize__(data)
         if "database" not in data:
```

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/impl.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import ConstraintType
 from dbt.events import AdapterLogger
 
 from dbt.utils import filter_null_values
 
 from dbt.adapters.oracle.keyword_catalog import KEYWORDS
+from dbt.adapters.oracle.python_submissions import OracleADBSPythonJob
+from dbt.adapters.oracle.connections import AdapterResponse
 
 logger = AdapterLogger("oracle")
 
 # Added 6 random hex letters (56c36b) to table_a and table_b to avoid ORA-32031.
 # Some dbt test cases use relation names table_a and table_b
 # Oracle error: ORA-32031: illegal reference of a query name in WITH clause
 COLUMNS_EQUAL_SQL = '''
@@ -363,53 +365,31 @@
         except requests.exceptions.RequestException:
             raise dbt.exceptions.DbtRuntimeError("Error getting OML OAuth2.0 token")
         else:
             return r.json()["accessToken"]
 
     def submit_python_job(self, parsed_model: dict, compiled_code: str):
         """Submit user defined Python function
-
-        The function pyqEval when used in Oracle Autonomous Database,
-        calls a user-defined Python function.
-
-        pyqEval(PAR_LST, OUT_FMT, SRC_NAME, SRC_OWNER, ENV_NAME)
-
-        - PAR_LST -> Parameter List
-        - OUT_FMT -> JSON clob of the columns
-        - ENV_NAME -> Name of conda environment
+        https://docs.oracle.com/en/database/oracle/machine-learning/oml4py/1/mlepe/op-py-scripts-v1-do-eval-scriptname-post.html
 
 
         """
         identifier = parsed_model["alias"]
-        oml_oauth_access_token = self.get_oml_auth_token()
         py_q_script_name = f"{identifier}_dbt_py_script"
-        py_q_eval_output_fmt = '{"result":"number"}'
-        py_q_eval_result_table = f"o$pt_dbt_pyqeval_{identifier}_tmp_{datetime.datetime.utcnow().strftime('%H%M%S')}"
-
-        conda_env_name = parsed_model["config"].get("conda_env_name")
-        if conda_env_name:
-            logger.info("Custom python environment is %s", conda_env_name)
-            py_q_eval_sql = f"""CREATE GLOBAL TEMPORARY TABLE {py_q_eval_result_table} 
-                                AS SELECT * FROM TABLE(pyqEval(par_lst => NULL, 
-                                                               out_fmt => ''{py_q_eval_output_fmt}'',
-                                                               scr_name => ''{py_q_script_name}'', 
-                                                               scr_owner => NULL, 
-                                                               env_name => ''{conda_env_name}''))"""
-        else:
-            py_q_eval_sql = f"""CREATE GLOBAL TEMPORARY TABLE {py_q_eval_result_table} 
-                                AS SELECT * FROM TABLE(pyqEval(par_lst => NULL, 
-                                                               out_fmt => ''{py_q_eval_output_fmt}'',
-                                                               scr_name => ''{py_q_script_name}'', 
-                                                               scr_owner => NULL))"""
-
-        py_exec_main_sql = f""" 
-                BEGIN
-                   sys.pyqSetAuthToken('{oml_oauth_access_token}');
-                   sys.pyqScriptCreate('{py_q_script_name}', '{compiled_code.strip()}', FALSE, TRUE);
-                   EXECUTE IMMEDIATE '{py_q_eval_sql}';
-                   EXECUTE IMMEDIATE 'DROP TABLE {py_q_eval_result_table}';
-                   sys.pyqScriptDrop('{py_q_script_name}');
-                END;
+        py_q_create_script = f"""
+            BEGIN
+              sys.pyqScriptCreate('{py_q_script_name}', '{compiled_code.strip()}', FALSE, TRUE);
+            END;
         """
-        response, _ = self.execute(sql=py_exec_main_sql)
+        response, _ = self.execute(sql=py_q_create_script)
+        python_job = OracleADBSPythonJob(parsed_model=parsed_model,
+                                         credential=self.config.credentials)
+        python_job()
+        py_q_drop_script = f"""
+                 BEGIN
+                   sys.pyqScriptDrop('{py_q_script_name}');
+                 END;
+             """
+
+        response, _ = self.execute(sql=py_q_drop_script)
         logger.info(response)
         return response
```

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/keyword_catalog.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/relation.py` & `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/__init__.py` & `dbt-oracle-1.5.1rc2/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/__init__.py` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/adapters.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/apply_grants.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/catalog.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/columns.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/python_model/python.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/view.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/schema_tests.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/data_types.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datediff.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/except.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/hash.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/last_day.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/position.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/right.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt/include/oracle/profile_template.yml` & `dbt-oracle-1.5.1rc2/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/PKG-INFO` & `dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.1rc1
+Version: 1.5.1rc2
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/SOURCES.txt` & `dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 dbt/adapters/oracle/__init__.py
 dbt/adapters/oracle/__version__.py
 dbt/adapters/oracle/column.py
 dbt/adapters/oracle/connection_helper.py
 dbt/adapters/oracle/connections.py
 dbt/adapters/oracle/impl.py
 dbt/adapters/oracle/keyword_catalog.py
+dbt/adapters/oracle/python_submissions.py
 dbt/adapters/oracle/relation.py
 dbt/include/__init__.py
 dbt/include/oracle/__init__.py
 dbt/include/oracle/dbt_project.yml
 dbt/include/oracle/profile_template.yml
 dbt/include/oracle/macros/adapters.sql
 dbt/include/oracle/macros/apply_grants.sql
```

### Comparing `dbt-oracle-1.5.1rc1/setup.cfg` & `dbt-oracle-1.5.1rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dbt-oracle
-version = 1.5.1
+version = 1.5.1rc2
 description = dbt (data build tool) adapter for the Oracle database
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Oracle dbt
 author = Oracle
 license = Apache Software License 2.0
 classifiers = 
@@ -26,20 +26,20 @@
 
 [options]
 python_requires = >=3.7.2
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
-	dbt-core==1.5.1
+	dbt-core==1.5.2
 	cx_Oracle==8.3.0
-	oracledb==1.3.1
+	oracledb==1.3.2
 test_suite = tests
 test_requires = 
-	dbt-tests-adapter==1.5.1
+	dbt-tests-adapter==1.5.2
 	pytest
 scripts = 
 	bin/create-pem-from-p12
 
 [options.package_data]
 dbt = include/oracle/dbt_project.yml, include/oracle/macros/*.sql, include/oracle/macros/**/**/*.sql, include/oracle/profile_template.yml
```

### Comparing `dbt-oracle-1.5.1rc1/setup.py` & `dbt-oracle-1.5.1rc2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 requirements = [
-        "dbt-core==1.5.1",
+        "dbt-core==1.5.2",
         "cx_Oracle==8.3.0",
-        "oracledb==1.3.1"
+        "oracledb==1.3.2"
 ]
 
 test_requirements = [
-    "dbt-tests-adapter==1.5.1",
+    "dbt-tests-adapter==1.5.2",
     "pytest"
 ]
 
 project_urls = {
     'Documentation': 'https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile',
     'Source': 'https://github.com/oracle/dbt-oracle',
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.5.1rc1'
+VERSION = '1.5.1rc2'
 setup(
     author="Oracle",
     python_requires='>=3.7.2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt-oracle-1.5.1rc1/tests/README.md` & `dbt-oracle-1.5.1rc2/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/__init__.py` & `dbt-oracle-1.5.1rc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/conftest.py` & `dbt-oracle-1.5.1rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/__init__.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/fixtures.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/test_constraints.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/__init__.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/test_simple_seed.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/test_simple_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_basic.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_caching.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_concurrency.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_config.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_data_types.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_generate.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_genreferences.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_ephemeral.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_generictests_where.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_grants.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_quoted_relations.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_common_utils.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_dateutils.py` & `dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*

