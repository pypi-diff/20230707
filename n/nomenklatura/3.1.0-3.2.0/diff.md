# Comparing `tmp/nomenklatura-3.1.0.tar.gz` & `tmp/nomenklatura-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.1.0.tar", last modified: Mon Jul  3 09:52:57 2023, max compression
+gzip compressed data, was "nomenklatura-3.2.0.tar", last modified: Fri Jul  7 11:04:46 2023, max compression
```

## Comparing `nomenklatura-3.1.0.tar` & `nomenklatura-3.2.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:52:57.109529 nomenklatura-3.1.0/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:52:30.000000 nomenklatura-3.1.0/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 09:52:57.000000 nomenklatura-3.1.0/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:52:57.113529 nomenklatura-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-03 09:50:51.000000 nomenklatura-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.231559 nomenklatura-3.2.0/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.239559 nomenklatura-3.2.0/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.239559 nomenklatura-3.2.0/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.239559 nomenklatura-3.2.0/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:04:46.235559 nomenklatura-3.2.0/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:04:19.000000 nomenklatura-3.2.0/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 11:04:46.000000 nomenklatura-3.2.0/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:04:46.243559 nomenklatura-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-07 11:02:41.000000 nomenklatura-3.2.0/setup.py
```

### Comparing `nomenklatura-3.1.0/LICENSE` & `nomenklatura-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/PKG-INFO` & `nomenklatura-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.1.0
+Version: 3.2.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.1.0/README.md` & `nomenklatura-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/cache.py` & `nomenklatura-3.2.0/nomenklatura/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         except OperationalError as exc:
             log.info("Error while saving to cache: %s" % exc)
 
     def set_json(self, key: str, value: Any) -> None:
         return self.set(key, json.dumps(value))
 
     def get(self, key: str, max_age: Optional[int] = None) -> Optional[Value]:
-        if max_age == 0:
+        if max_age is not None and max_age < 1:
             return None
 
         cache_cutoff = None
         if max_age is not None:
             cache_cutoff = datetime.utcnow() - randomize_cache(max_age)
 
         cache = self._preload.get(key)
```

### Comparing `nomenklatura-3.1.0/nomenklatura/cli.py` & `nomenklatura-3.2.0/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.2.0/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.2.0/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/catalog.py` & `nomenklatura-3.2.0/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/coverage.py` & `nomenklatura-3.2.0/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/dataset.py` & `nomenklatura-3.2.0/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/publisher.py` & `nomenklatura-3.2.0/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/resource.py` & `nomenklatura-3.2.0/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/dataset/util.py` & `nomenklatura-3.2.0/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/db.py` & `nomenklatura-3.2.0/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/__init__.py` & `nomenklatura-3.2.0/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/aleph.py` & `nomenklatura-3.2.0/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/common.py` & `nomenklatura-3.2.0/nomenklatura/enrich/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 import logging
 from banal import as_bool
 from typing import Union, Any, Dict, Optional, Generator
 from abc import ABC, abstractmethod
 from requests import Session
-from requests.exceptions import RequestException, HTTPError
+from requests.exceptions import RequestException
 from followthemoney import model
 
 from nomenklatura import __version__
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.util import ParamsType, normalize_url
@@ -60,28 +60,30 @@
         self,
         url: str,
         params: ParamsType = None,
         hidden: ParamsType = None,
         cache_days: Optional[int] = None,
     ) -> str:
         url = normalize_url(url, params=params)
-        cache_days_ = cache_days or self.cache_days
+        cache_days_ = self.cache_days if cache_days is None else cache_days
         response = self.cache.get(url, max_age=cache_days_)
         if response is None:
+            log.debug("HTTP GET: %s", url)
             hidden_url = normalize_url(url, params=hidden)
             try:
                 resp = self.session.get(hidden_url)
                 resp.raise_for_status()
             except RequestException as rex:
                 if rex.response is not None and rex.response.status_code in (401, 403):
                     raise EnrichmentAbort("Authorization failure: %s" % url) from rex
                 msg = "HTTP fetch failed [%s]: %s" % (url, rex)
                 raise EnrichmentException(msg) from rex
             response = resp.text
-            self.cache.set(url, response)
+            if cache_days is not None and cache_days > 0:
+                self.cache.set(url, response)
         return response
 
     def http_remove_cache(self, url: str, params: ParamsType = None) -> None:
         url = normalize_url(url, params=params)
         self.cache.delete(url)
 
     def http_get_json_cached(
@@ -97,36 +99,37 @@
     def http_post_json_cached(
         self,
         url: str,
         cache_key: str,
         json: Any,
         cache_days: Optional[int] = None,
     ) -> Any:
-        cache_days_ = cache_days or self.cache_days
+        cache_days_ = self.cache_days if cache_days is None else cache_days
         resp_data = self.cache.get_json(cache_key, max_age=cache_days_)
         if resp_data is None:
             try:
                 resp = self.session.post(url, json=json)
                 resp.raise_for_status()
             except RequestException as rex:
                 if rex.response is not None and rex.response.status_code in (401, 403):
                     raise EnrichmentAbort("Authorization failure: %s" % url) from rex
                 msg = "HTTP POST failed [%s]: %s" % (url, rex)
                 raise EnrichmentException(msg) from rex
             resp_data = resp.json()
-            self.cache.set_json(cache_key, resp_data)
+            if cache_days is not None and cache_days > 0:
+                self.cache.set_json(cache_key, resp_data)
         return resp_data
 
     def _make_data_entity(
         self, entity: CE, data: Dict[str, Any], cleaned: bool = True
     ) -> CE:
         return type(entity).from_dict(
             model,
             data,
-            default_dataset=self.dataset.name,
+            default_dataset=self.dataset,
             cleaned=cleaned,
         )
 
     def load_entity(self, entity: CE, data: Dict[str, Any]) -> CE:
         proxy = self._make_data_entity(entity, data, cleaned=False)
         for prop in proxy.iterprops():
             if prop.stub:
```

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.2.0/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.2.0/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,15 @@
             params = {
                 "format": "json",
                 "search": name,
                 "action": "wbsearchentities",
                 "language": "en",
                 "strictlanguage": "false",
             }
-            data = self.http_get_json_cached(
-                WD_API, params=params, cache_days=self.cache_days
-            )
+            data = self.http_get_json_cached(WD_API, params=params)
             if "search" not in data:
                 self.http_remove_cache(WD_API, params=params)
                 log.warning("Search response [%s] does not include results" % name)
                 continue
             for result in data["search"]:
                 item = self.fetch_item(result["id"])
                 if item is not None:
@@ -102,29 +100,30 @@
         # https://www.mediawiki.org/wiki/Wikibase/API
         # https://www.wikidata.org/w/api.php?action=help&modules=wbgetentities
         params = {**kwargs, "format": "json", "ids": id, "action": "wbgetentities"}
         data = self.http_get_json_cached(WD_API, params=params, cache_days=cache_days)
         return cast(Dict[str, Any], data)
 
     def fetch_item(self, qid: str) -> Optional[Item]:
-        data = self.wikibase_getentities(qid, cache_days=self.cache_days)
+        data = self.wikibase_getentities(qid)
         entity = data.get("entities", {}).get(qid)
         if entity is None:
             return None
         return Item(entity)
 
     @cache
     def get_label(self, qid: str) -> LangText:
         cache_key = f"{LABEL_PREFIX}{qid}"
         cached = self.cache.get_json(cache_key, max_age=self.label_cache_days)
         if cached is not None:
             return LangText.parse(cached)
+
         data = self.wikibase_getentities(
             qid,
-            cache_days=self.cache_days,
+            cache_days=0,
             props="labels",
         )
         entity = data.get("entities", {}).get(qid)
         label = pick_obj_lang(entity.get("labels", {}))
         if label.text is None:
             label.text = qid
         label.original = qid
```

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.2.0/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/enrich/yente.py` & `nomenklatura-3.2.0/nomenklatura/enrich/yente.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,20 +62,15 @@
                     "schema": entity.schema.name,
                     "properties": props,
                 }
             }
         }
         for retry in range(4):
             try:
-                response = self.http_post_json_cached(
-                    url,
-                    cache_key,
-                    query,
-                    cache_days=self.cache_days,
-                )
+                response = self.http_post_json_cached(url, cache_key, query)
             except EnrichmentException as exc:
                 log.info("Error matching %r: %s", entity, exc)
                 if retry == 3:
                     raise
                 time.sleep((retry + 1) ** 2)
 
         inner_resp = response.get("responses", {}).get("entity", {})
@@ -106,9 +101,9 @@
 
     def expand(self, entity: CE, match: CE) -> Generator[CE, None, None]:
         url = self.make_url(match)
         for source_url in match.get("sourceUrl", quiet=True):
             if source_url.startswith(self._api):
                 url = source_url
         url = normalize_url(url, {"nested": self._nested})
-        response = self.http_get_json_cached(url, cache_days=self.cache_days)
+        response = self.http_get_json_cached(url)
         yield from self._traverse_nested(match, response)
```

### Comparing `nomenklatura-3.1.0/nomenklatura/entity.py` & `nomenklatura-3.2.0/nomenklatura/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 from followthemoney.types.common import PropertyType
 from followthemoney.property import Property
 from followthemoney.util import gettext, value_list
 from followthemoney.proxy import P
 from followthemoney.types import registry
 from followthemoney.proxy import EntityProxy
 
-from nomenklatura.dataset import DS
+from nomenklatura.dataset import DS, Dataset, DefaultDataset
 from nomenklatura.publish.names import pick_name
 from nomenklatura.statement.statement import Statement
 from nomenklatura.util import BASE_ID
 
 if TYPE_CHECKING:
     from nomenklatura.store import View
 
 CE = TypeVar("CE", bound="CompositeEntity")
-DEFAULT_DATASET = "default"
 
 
 class CompositeEntity(EntityProxy):
     """An entity object that can link to a set of datasets that it is sourced from."""
 
     __slots__ = (
         "schema",
@@ -38,15 +37,15 @@
     )
 
     def __init__(
         self,
         model: "Model",
         data: Dict[str, Any],
         cleaned: bool = True,
-        default_dataset: str = DEFAULT_DATASET,
+        default_dataset: Dataset = DefaultDataset,
     ):
         data = dict(data or {})
         schema = model.get(data.pop("schema", None))
         if schema is None:
             raise InvalidData(gettext("No schema for entity."))
         self.schema = schema
 
@@ -92,15 +91,15 @@
         if self.id is not None:
             yield Statement(
                 canonical_id=self.id,
                 entity_id=self.id,
                 prop=BASE_ID,
                 schema=self.schema.name,
                 value=self.checksum(),
-                dataset=self.default_dataset,
+                dataset=self.default_dataset.name,
             )
         yield from self._iter_stmt()
 
     @property
     def first_seen(self) -> Optional[str]:
         seen = (s.first_seen for s in self._iter_stmt() if s.first_seen is not None)
         return min(seen, default=None)
@@ -131,19 +130,19 @@
         for stmt in self._iter_stmt():
             if stmt.entity_id is not None and stmt.entity_id != self.id:
                 referents.add(stmt.entity_id)
         return referents
 
     @property
     def key_prefix(self) -> Optional[str]:
-        return self.default_dataset
+        return self.default_dataset.name
 
     @key_prefix.setter
     def key_prefix(self, dataset: str) -> None:
-        self.default_dataset = dataset
+        raise NotImplementedError()
 
     def _pick_caption(self) -> str:
         is_thing = self.schema.is_a("Thing")
         for prop in self.schema.caption:
             values = self.get(prop)
             if is_thing and len(values) > 1:
                 name = pick_name(values)
@@ -230,15 +229,15 @@
                 original_value = value
 
             stmt = Statement(
                 entity_id=self.id,
                 prop=prop.name,
                 schema=schema or self.schema.name,
                 value=clean,
-                dataset=dataset or self.default_dataset,
+                dataset=dataset or self.default_dataset.name,
                 lang=lang,
                 original_value=original_value,
                 first_seen=seen,
             )
             self.add_statement(stmt)
 
     def claim_many(
@@ -458,22 +457,26 @@
 
     @classmethod
     def from_dict(
         cls: Type[CE],
         model: Model,
         data: Dict[str, Any],
         cleaned: bool = True,
-        default_dataset: str = DEFAULT_DATASET,
+        default_dataset: Dataset = DefaultDataset,
     ) -> CE:
         return cls(model, data, cleaned=cleaned, default_dataset=default_dataset)
 
     @classmethod
-    def from_statements(cls: Type[CE], statements: Iterable[Statement]) -> CE:
+    def from_statements(
+        cls: Type[CE],
+        statements: Iterable[Statement],
+        default_dataset: Dataset = DefaultDataset,
+    ) -> CE:
         obj: Optional[CE] = None
         for stmt in statements:
             if obj is None:
                 data = {"schema": stmt.schema, "id": stmt.canonical_id}
-                obj = cls(model, data, default_dataset=stmt.dataset)
+                obj = cls(model, data, default_dataset=default_dataset)
             obj.add_statement(stmt)
         if obj is None:
             raise ValueError("No statements given!")
         return obj
```

### Comparing `nomenklatura-3.1.0/nomenklatura/index/entry.py` & `nomenklatura-3.2.0/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/index/index.py` & `nomenklatura-3.2.0/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/index/tokenizer.py` & `nomenklatura-3.2.0/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/judgement.py` & `nomenklatura-3.2.0/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/__init__.py` & `nomenklatura-3.2.0/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.2.0/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.2.0/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/pairs.py` & `nomenklatura-3.2.0/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/types.py` & `nomenklatura-3.2.0/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/util.py` & `nomenklatura-3.2.0/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/model.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/names.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/train.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v1/util.py` & `nomenklatura-3.2.0/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/model.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/names.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/train.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/matching/v2/util.py` & `nomenklatura-3.2.0/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/publish/dates.py` & `nomenklatura-3.2.0/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/publish/edges.py` & `nomenklatura-3.2.0/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/publish/names.py` & `nomenklatura-3.2.0/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/resolver/edge.py` & `nomenklatura-3.2.0/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/resolver/identifier.py` & `nomenklatura-3.2.0/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/resolver/resolver.py` & `nomenklatura-3.2.0/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/senzing.py` & `nomenklatura-3.2.0/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/statement/serialize.py` & `nomenklatura-3.2.0/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/statement/statement.py` & `nomenklatura-3.2.0/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/store/__init__.py` & `nomenklatura-3.2.0/nomenklatura/store/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,11 +34,14 @@
         dataset = Dataset.make({"name": path.stem, "title": path.stem})
     store = MemoryStore(dataset, resolver)
     with store.writer() as writer:
         with open(path, "rb") as fh:
             while line := fh.readline():
                 data = orjson.loads(line)
                 proxy = CompositeEntity.from_dict(
-                    model, data, cleaned=cleaned, default_dataset=dataset.name
+                    model,
+                    data,
+                    cleaned=cleaned,
+                    default_dataset=dataset,
                 )
                 writer.add_entity(proxy)
     return store
```

### Comparing `nomenklatura-3.1.0/nomenklatura/store/base.py` & `nomenklatura-3.2.0/nomenklatura/store/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,33 @@
 
     def assemble(self, statements: List[Statement]) -> Optional[CE]:
         if not len(statements):
             return None
         for stmt in statements:
             if stmt.prop_type == registry.entity.name:
                 stmt.value = self.resolver.get_canonical(stmt.value)
-        entity = self.entity_class.from_statements(statements)
+        entity = self.entity_class.from_statements(
+            statements,
+            default_dataset=self.dataset,
+        )
         if entity.id is not None:
             entity.extra_referents.update(self.resolver.get_referents(entity.id))
         return entity
 
     def update(self, id: StrIdent) -> None:
         canonical_id = self.resolver.get_canonical(id)
         with self.writer() as writer:
             for referent in self.resolver.get_referents(canonical_id):
                 for stmt in writer.pop(referent):
                     stmt.canonical_id = canonical_id
                     writer.add_statement(stmt)
 
+    def __repr__(self) -> str:
+        return f"<{type(self).__name__}({self.dataset.name!r})>"
+
 
 class Writer(Generic[DS, CE]):
     """Bulk writing operations."""
 
     def __init__(self, store: Store[DS, CE]):
         self.store = store
 
@@ -73,14 +79,17 @@
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         self.flush()
 
+    def __repr__(self) -> str:
+        return f"<{type(self).__name__}({self.store!r})>"
+
 
 class View(Generic[DS, CE]):
     def __init__(self, store: Store[DS, CE], scope: DS, external: bool = False):
         self.store = store
         self.scope = scope
         self.scope_names = scope.scope_names
         self.external = external
@@ -104,8 +113,8 @@
             for prop, adjacent in self.get_inverted(entity.id):
                 yield prop, adjacent
 
     def entities(self) -> Generator[CE, None, None]:
         raise NotImplementedError()
 
     def __repr__(self) -> str:
-        return f"<View({self.scope!r})>"
+        return f"<{type(self).__name__}({self.scope.name!r})>"
```

### Comparing `nomenklatura-3.1.0/nomenklatura/store/level.py` & `nomenklatura-3.2.0/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/store/memory.py` & `nomenklatura-3.2.0/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/store/util.py` & `nomenklatura-3.2.0/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/tui/app.py` & `nomenklatura-3.2.0/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/tui/comparison.py` & `nomenklatura-3.2.0/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/tui/util.py` & `nomenklatura-3.2.0/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/util.py` & `nomenklatura-3.2.0/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura/xref.py` & `nomenklatura-3.2.0/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.2.0/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.1.0
+Version: 3.2.0
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.1.0/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.2.0/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.1.0/setup.py` & `nomenklatura-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.1.0",
+    version="3.2.0",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
@@ -21,17 +21,17 @@
     package_data={"": ["nomenklatura/data/*", "nomenklatura/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.3.0, < 4.0.0",
         "shortuuid >= 1.0.11, < 2.0.0",
         "jellyfish >= 1.0.0, < 2.0.0",
         "rich >= 10.9.0, < 14.0.0",
-        "textual >= 0.19.0, < 0.29.0",
+        "textual >= 0.19.0, < 1.0.0",
         "scikit-learn == 1.2.2",
-        "click >= 8.0.0, < 9.0.0",
+        "click >= 8.0.0, < 8.1.4",
     ],
     tests_require=[],
     entry_points={
         "console_scripts": [
             "nk = nomenklatura.cli:cli",
             "nomenklatura = nomenklatura.cli:cli",
         ],
```

