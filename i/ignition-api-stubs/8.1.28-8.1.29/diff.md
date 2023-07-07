# Comparing `tmp/ignition-api-stubs-8.1.28.tar.gz` & `tmp/ignition-api-stubs-8.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignition-api-stubs-8.1.28.tar", last modified: Fri Jun  2 20:24:41 2023, max compression
+gzip compressed data, was "ignition-api-stubs-8.1.29.tar", last modified: Fri Jul  7 20:18:35 2023, max compression
```

## Comparing `ignition-api-stubs-8.1.28.tar` & `ignition-api-stubs-8.1.29.tar`

### file list

```diff
@@ -1,407 +1,407 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.895257 ignition-api-stubs-8.1.28/
--rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-06-02 20:24:41.895257 ignition-api-stubs-8.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 20:24:41.899257 ignition-api-stubs-8.1.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.839257 ignition-api-stubs-8.1.28/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.839257 ignition-api-stubs-8.1.28/stubs/ch/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/ch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.839257 ignition-api-stubs-8.1.28/stubs/ch/qos/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/ch/qos/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.839257 ignition-api-stubs-8.1.28/stubs/ch/qos/logback/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/ch/qos/logback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.839257 ignition-api-stubs-8.1.28/stubs/ch/qos/logback/classic/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/ch/qos/logback/classic/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/codahale/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/codahale/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/codahale/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/codahale/metrics/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/google/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/google/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/google/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/google/common/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/google/common/collect/
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/google/common/collect/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/google/common/eventbus/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/google/common/eventbus/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/binding/
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/components/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/components/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/model/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/script/
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/script/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/script/builtin/
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/sqltags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/sqltags/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.843257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/common/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/common/rosters/
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/launch/
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/model/
--rw-r--r--   0 runner    (1001) docker     (122)     4075 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/progress/
--rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/
--rw-r--r--   0 runner    (1001) docker     (122)     1402 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/
--rw-r--r--   0 runner    (1001) docker     (122)    10151 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/query/
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/binding/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/binding/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/browsing/
--rw-r--r--   0 runner    (1001) docker     (122)     3590 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/config/
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/db/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/db/namedquery/
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.847257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/document/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/document/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/execution/
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/functions/
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/functional/
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/functional/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/
--rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/reflect/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/reflect/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/stream/
--rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gui/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gui/progress/
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/translation/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/translation/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/licensing/
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.851257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/messages/
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/values/
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/modules/
--rw-r--r--   0 runner    (1001) docker     (122)     4709 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/opc/
--rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/
--rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/resource/
--rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/abc/
--rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/
--rw-r--r--   0 runner    (1001) docker     (122)     8422 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/http/
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/hints/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/hints/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/message/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/history/
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/history/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.855257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/config/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/config/types/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/config/types/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/model/
--rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/
--rw-r--r--   0 runner    (1001) docker     (122)     4590 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/schedule/
--rw-r--r--   0 runner    (1001) docker     (122)     4957 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/util/
--rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.859257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/gateway/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/gateway/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/gateway/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/serial/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/serial/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/serial/scripting/
--rw-r--r--   0 runner    (1001) docker     (122)     2338 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/opccom/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/opccom/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/opccom/hda/
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/opccom/hda/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/perspective/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/perspective/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/perspective/common/
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/perspective/common/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.863257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/sfc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/sfc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/sfc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/sfc/api/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/components/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/components/model/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/vision/api/client/components/model/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/palantir/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/palantir/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/cinch/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/cinch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/cinch/core/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/palantir/ptoss/cinch/core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/com/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/dev/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.867257 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/helper/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/helper/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/dev/thecesrom/utils/decorators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-06-02 20:24:41.000000 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10815 2023-06-02 20:24:41.000000 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 20:24:41.000000 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-02 20:24:41.000000 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-02 20:24:41.000000 ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/awt/
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/awt/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/awt/event/
--rw-r--r--   0 runner    (1001) docker     (122)     2583 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/awt/event/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/awt/geom/
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/awt/geom/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/awt/image/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/awt/image/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/awt/print/
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/awt/print/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.871257 ignition-api-stubs-8.1.28/stubs/java/beans/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/beans/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/io/
--rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/lang/
--rw-r--r--   0 runner    (1001) docker     (122)     9737 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/lang/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/lang/reflect/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/lang/reflect/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/math/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/net/
--rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/net/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/net/http/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/net/http/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/nio/
--rw-r--r--   0 runner    (1001) docker     (122)     7653 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/nio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/nio/channels/
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/nio/channels/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/nio/charset/
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/nio/charset/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/nio/file/
--rw-r--r--   0 runner    (1001) docker     (122)     7943 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/nio/file/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/nio/file/attribute/
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/nio/file/attribute/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/org/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/org/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.875257 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/animation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/animation/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/animation/timing/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/org/jdesktop/core/animation/timing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/security/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/security/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/text/
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/text/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/time/
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/time/format/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/time/format/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/time/temporal/
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/time/temporal/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/util/
--rw-r--r--   0 runner    (1001) docker     (122)    16259 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/util/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/util/concurrent/
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/util/concurrent/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/util/function/
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/util/function/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/util/regex/
--rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/util/regex/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.879257 ignition-api-stubs-8.1.28/stubs/java/util/stream/
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/java/util/stream/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/security/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/security/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/security/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/security/auth/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/swing/
--rw-r--r--   0 runner    (1001) docker     (122)     6507 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/swing/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/swing/event/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/swing/event/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/swing/plaf/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/swing/plaf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/javax/swing/text/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/javax/swing/text/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/apache/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/lang3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/lang3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/lang3/builder/
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/lang3/builder/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.883257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/
--rw-r--r--   0 runner    (1001) docker     (122)      587 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/util/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/util/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/apache/log4j/
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/log4j/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/apache/log4j/spi/
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/apache/log4j/spi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/json/
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/python/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/python/core/
--rw-r--r--   0 runner    (1001) docker     (122)    23038 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/python/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/python/expose/
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/python/expose/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/slf4j/
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/slf4j/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.887257 ignition-api-stubs-8.1.28/stubs/org/slf4j/event/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/org/slf4j/event/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.895257 ignition-api-stubs-8.1.28/stubs/system/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/alarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.895257 ignition-api-stubs-8.1.28/stubs/system/bacnet/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/bacnet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    12890 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/bacnet/enumerated.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/bacnet/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/dataset.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/date.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/db.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/device.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1279 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/dnp3.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/eam.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/file.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/groups.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/gui.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/iec61850.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/math.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/nav.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/net.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/opc.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/opchda.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/opcua.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:41.895257 ignition-api-stubs-8.1.28/stubs/system/perspective/
--rw-r--r--   0 runner    (1001) docker     (122)     3888 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/perspective/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/perspective/workstation.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/print.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/project.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/report.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/roster.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/secsgem.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/security.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/serial.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/sfc.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/tag.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/twilio.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/user.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/util.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-06-02 20:24:23.000000 ignition-api-stubs-8.1.28/stubs/system/vision.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.954964 ignition-api-stubs-8.1.29/
+-rw-r--r--   0 runner    (1001) docker     (122)     7352 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-07-07 20:18:35.954964 ignition-api-stubs-8.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 20:18:35.954964 ignition-api-stubs-8.1.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.914960 ignition-api-stubs-8.1.29/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.914960 ignition-api-stubs-8.1.29/stubs/ch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/ch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.914960 ignition-api-stubs-8.1.29/stubs/ch/qos/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/ch/qos/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.914960 ignition-api-stubs-8.1.29/stubs/ch/qos/logback/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/ch/qos/logback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.914960 ignition-api-stubs-8.1.29/stubs/ch/qos/logback/classic/
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/ch/qos/logback/classic/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/codahale/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/codahale/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/codahale/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/codahale/metrics/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/google/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/google/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/google/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/google/common/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/google/common/collect/
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/google/common/collect/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/google/common/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/google/common/eventbus/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/binding/
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/components/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/script/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/script/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/script/builtin/
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/sqltags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/sqltags/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/sqltags/project/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/common/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/common/rosters/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/alarming/common/rosters/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/launch/
+-rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.918961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     4075 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/progress/
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (122)     1402 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/
+-rw-r--r--   0 runner    (1001) docker     (122)    10151 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/binding/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/binding/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/browsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     3590 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/db/namedquery/
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/document/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/document/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/execution/
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/functional/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/
+-rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/reflect/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/reflect/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/stream/
+-rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gui/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gui/progress/
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.922961 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/translation/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/translation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/licensing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/messages/
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/values/
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     4709 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/opc/
+-rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/resource/
+-rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/abc/
+-rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/
+-rw-r--r--   0 runner    (1001) docker     (122)     8422 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/http/
+-rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/hints/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/hints/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/message/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/history/
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/history/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.926962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/config/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/config/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/config/types/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/tagpaths/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/
+-rw-r--r--   0 runner    (1001) docker     (122)     4590 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/schedule/
+-rw-r--r--   0 runner    (1001) docker     (122)     4957 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/encoding/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/gateway/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/gateway/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/gateway/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/serial/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/serial/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/serial/scripting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2338 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/opccom/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/opccom/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/opccom/hda/
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/opccom/hda/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/perspective/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/perspective/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.930962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/perspective/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/perspective/common/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/sfc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/sfc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/sfc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/sfc/api/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/components/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/components/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/vision/api/client/components/model/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/palantir/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/palantir/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/cinch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/cinch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/cinch/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/palantir/ptoss/cinch/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/com/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/dev/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/helper/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/helper/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/dev/thecesrom/utils/decorators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-07-07 20:18:35.000000 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10815 2023-07-07 20:18:35.000000 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 20:18:35.000000 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-07 20:18:35.000000 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-07 20:18:35.000000 ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/java/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.934962 ignition-api-stubs-8.1.29/stubs/java/awt/
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/awt/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/awt/event/
+-rw-r--r--   0 runner    (1001) docker     (122)     2583 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/awt/event/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/awt/geom/
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/awt/geom/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/awt/image/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/awt/image/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/awt/print/
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/awt/print/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/beans/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/beans/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/lang/
+-rw-r--r--   0 runner    (1001) docker     (122)     9737 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/lang/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/lang/reflect/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/lang/reflect/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/math/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/net/
+-rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/net/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/net/http/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/net/http/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/nio/
+-rw-r--r--   0 runner    (1001) docker     (122)     7653 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/nio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/nio/channels/
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/nio/channels/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/nio/charset/
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/nio/charset/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/nio/file/
+-rw-r--r--   0 runner    (1001) docker     (122)     7943 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/nio/file/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/nio/file/attribute/
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/nio/file/attribute/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/org/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/org/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/animation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/animation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/animation/timing/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/org/jdesktop/core/animation/timing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/security/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/security/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/text/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/time/
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.938963 ignition-api-stubs-8.1.29/stubs/java/time/format/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/time/format/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/time/temporal/
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/time/temporal/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/util/
+-rw-r--r--   0 runner    (1001) docker     (122)    16259 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/util/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/util/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (122)     1919 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/util/concurrent/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/util/function/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/util/function/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/util/regex/
+-rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/util/regex/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/java/util/stream/
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/java/util/stream/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/security/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/security/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/security/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/security/auth/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/swing/
+-rw-r--r--   0 runner    (1001) docker     (122)     6507 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/swing/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/swing/event/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/swing/event/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/swing/plaf/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/swing/plaf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/javax/swing/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/javax/swing/text/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/apache/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/lang3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/lang3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/lang3/builder/
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/lang3/builder/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.942963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/util/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/apache/log4j/
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/log4j/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/apache/log4j/spi/
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/apache/log4j/spi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/json/
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/python/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/python/core/
+-rw-r--r--   0 runner    (1001) docker     (122)    23038 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/python/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/python/expose/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/python/expose/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/slf4j/
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/slf4j/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.946963 ignition-api-stubs-8.1.29/stubs/org/slf4j/event/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/org/slf4j/event/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.950964 ignition-api-stubs-8.1.29/stubs/system/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/alarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.954964 ignition-api-stubs-8.1.29/stubs/system/bacnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/bacnet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    12890 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/bacnet/enumerated.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/bacnet/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/dataset.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/date.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3550 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/device.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1279 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/dnp3.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/eam.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/groups.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/iec61850.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/nav.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/net.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/opc.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/opchda.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/opcua.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:35.954964 ignition-api-stubs-8.1.29/stubs/system/perspective/
+-rw-r--r--   0 runner    (1001) docker     (122)     3888 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/perspective/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/perspective/workstation.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/print.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/project.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/report.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/roster.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/secsgem.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/serial.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/sfc.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/twilio.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2350 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-07-07 20:18:20.000000 ignition-api-stubs-8.1.29/stubs/system/vision.pyi
```

### Comparing `ignition-api-stubs-8.1.28/CHANGELOG.md` & `ignition-api-stubs-8.1.29/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v8.1.29 (2023-07-07)
+
 ## v8.1.28 (2023-06-02)
 
 ### Feat
 
 - **system**: add system.vision.getKeyboardLayouts (#122)
 - **system**: add system.project.requestScan (#121)
```

### Comparing `ignition-api-stubs-8.1.28/LICENSE` & `ignition-api-stubs-8.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/PKG-INFO` & `ignition-api-stubs-8.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignition-api-stubs
-Version: 8.1.28
+Version: 8.1.29
 Summary: Ignition Scripting API Stubs
 Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ignition-api-stubs-8.1.28/README.md` & `ignition-api-stubs-8.1.29/README.md`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/pyproject.toml` & `ignition-api-stubs-8.1.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "ignition-api-stubs"
-version = "8.1.28"
+version = "8.1.29"
 description = "Ignition Scripting API Stubs"
 readme = "README.md"
 keywords = [
   "hmi",
   "ignition",
   "inductive automation",
   "scada",
```

### Comparing `ignition-api-stubs-8.1.28/stubs/ch/qos/logback/classic/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/ch/qos/logback/classic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/codahale/metrics/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/codahale/metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/google/common/collect/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/google/common/collect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/binding/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/factorypmi/application/script/builtin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/launch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/progress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/alarming/query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/browsing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/db/namedquery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/execution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/expressions/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gson/stream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/gui/progress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/jsonschema/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/licensing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/model/values/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/modules/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/opc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/project/resource/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/abc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/adapters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/script/message/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/user/schedule/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/gateway/project/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/ignition/modules/serial/scripting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/opccom/hda/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/opccom/hda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/com/inductiveautomation/perspective/common/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/com/inductiveautomation/perspective/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/PKG-INFO` & `ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignition-api-stubs
-Version: 8.1.28
+Version: 8.1.29
 Summary: Ignition Scripting API Stubs
 Author-email: César Román <cesar@coatl.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ignition-api-stubs-8.1.28/stubs/ignition_api_stubs.egg-info/SOURCES.txt` & `ignition-api-stubs-8.1.29/stubs/ignition_api_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/awt/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/awt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/awt/event/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/awt/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/awt/geom/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/awt/geom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/awt/print/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/awt/print/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/beans/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/beans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/io/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/lang/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/lang/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/net/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/net/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/nio/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/nio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/nio/channels/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/nio/channels/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/nio/charset/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/nio/charset/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/nio/file/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/nio/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/nio/file/attribute/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/nio/file/attribute/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/text/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/time/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/time/temporal/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/time/temporal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/util/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/util/concurrent/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/util/concurrent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/util/function/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/util/function/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/util/regex/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/util/regex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/java/util/stream/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/java/util/stream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/javax/swing/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/javax/swing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/javax/swing/event/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/javax/swing/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/apache/commons/lang3/builder/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/apache/commons/lang3/builder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/apache/commons/math3/exception/util/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/apache/commons/math3/exception/util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/apache/log4j/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/apache/log4j/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/apache/log4j/spi/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/apache/log4j/spi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/json/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/python/core/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/python/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/org/slf4j/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/org/slf4j/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/alarm.pyi` & `ignition-api-stubs-8.1.29/stubs/system/alarm.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/bacnet/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/system/bacnet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/bacnet/enumerated.pyi` & `ignition-api-stubs-8.1.29/stubs/system/bacnet/enumerated.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/bacnet/enums.pyi` & `ignition-api-stubs-8.1.29/stubs/system/bacnet/enums.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/dataset.pyi` & `ignition-api-stubs-8.1.29/stubs/system/dataset.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/date.pyi` & `ignition-api-stubs-8.1.29/stubs/system/date.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/db.pyi` & `ignition-api-stubs-8.1.29/stubs/system/db.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 def dateFormat(date: Date, formatPattern: AnyStr) -> AnyStr: ...
 def execSProcCall(callContext: SProcCall) -> None: ...
 def getConnectionInfo(name: Optional[AnyStr] = ...) -> BasicDataset: ...
 def getConnections() -> BasicDataset: ...
 def refresh(component: JComponent, propertyName: AnyStr) -> bool: ...
 def removeDatasource(name: AnyStr) -> None: ...
 def rollbackTransaction(tx: AnyStr) -> None: ...
-def runNamedQuery(*args: Any) -> Any: ...
+def runNamedQuery(*args: Any) -> DatasetUtilities.PyDataSet: ...
 def runPrepQuery(
     query: AnyStr, args: List[Any], database: AnyStr = ..., tx: Optional[AnyStr] = ...
 ) -> DatasetUtilities.PyDataSet: ...
 def runPrepUpdate(
     query: AnyStr,
     args: List[Any],
     database: AnyStr = ...,
```

### Comparing `ignition-api-stubs-8.1.28/stubs/system/device.pyi` & `ignition-api-stubs-8.1.29/stubs/system/device.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/dnp3.pyi` & `ignition-api-stubs-8.1.29/stubs/system/dnp3.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/eam.pyi` & `ignition-api-stubs-8.1.29/stubs/system/eam.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/file.pyi` & `ignition-api-stubs-8.1.29/stubs/system/file.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/gui.pyi` & `ignition-api-stubs-8.1.29/stubs/system/gui.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/iec61850.pyi` & `ignition-api-stubs-8.1.29/stubs/system/iec61850.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/math.pyi` & `ignition-api-stubs-8.1.29/stubs/system/math.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/nav.pyi` & `ignition-api-stubs-8.1.29/stubs/system/nav.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/net.pyi` & `ignition-api-stubs-8.1.29/stubs/system/net.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/opc.pyi` & `ignition-api-stubs-8.1.29/stubs/system/opc.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/opchda.pyi` & `ignition-api-stubs-8.1.29/stubs/system/opchda.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/perspective/__init__.pyi` & `ignition-api-stubs-8.1.29/stubs/system/perspective/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/print.pyi` & `ignition-api-stubs-8.1.29/stubs/system/print.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/report.pyi` & `ignition-api-stubs-8.1.29/stubs/system/report.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/roster.pyi` & `ignition-api-stubs-8.1.29/stubs/system/roster.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/secsgem.pyi` & `ignition-api-stubs-8.1.29/stubs/system/secsgem.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/security.pyi` & `ignition-api-stubs-8.1.29/stubs/system/security.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/serial.pyi` & `ignition-api-stubs-8.1.29/stubs/system/serial.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/sfc.pyi` & `ignition-api-stubs-8.1.29/stubs/system/sfc.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/tag.pyi` & `ignition-api-stubs-8.1.29/stubs/system/tag.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/user.pyi` & `ignition-api-stubs-8.1.29/stubs/system/user.pyi`

 * *Files identical despite different names*

### Comparing `ignition-api-stubs-8.1.28/stubs/system/util.pyi` & `ignition-api-stubs-8.1.29/stubs/system/util.pyi`

 * *Files identical despite different names*

