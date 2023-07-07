# Comparing `tmp/clickhouse-connect-0.6.4.tar.gz` & `tmp/clickhouse-connect-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.4.tar", last modified: Thu Jun 22 22:54:18 2023, max compression
+gzip compressed data, was "clickhouse-connect-0.6.5.tar", last modified: Thu Jul  6 12:26:25 2023, max compression
```

## Comparing `clickhouse-connect-0.6.4.tar` & `clickhouse-connect-0.6.5.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.953019 clickhouse-connect-0.6.4/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.953019 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.953019 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.957019 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.957019 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.957019 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.957019 clickhouse-connect-0.6.4/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38860 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/json_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:54:18.953019 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:54:18.961019 clickhouse-connect-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 22:54:18.000000 clickhouse-connect-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39597 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/json_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/setup.py
```

### Comparing `clickhouse-connect-0.6.4/LICENSE` & `clickhouse-connect-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/PKG-INFO` & `clickhouse-connect-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.4
+Version: 0.6.5
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.4/README.md` & `clickhouse-connect-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/common.py` & `clickhouse-connect-0.6.5/clickhouse_connect/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import sys
 from dataclasses import dataclass
 from typing import Any, Sequence, Optional, Dict
 
-import pkg_resources
+from importlib_metadata import PackageNotFoundError, distribution
 
 from clickhouse_connect.driver.exceptions import ProgrammingError
 
 
 def version():
     try:
-        return pkg_resources.get_distribution('clickhouse-connect').version
-    except pkg_resources.ResolutionError:
+        return distribution('clickhouse-connect').version
+    except PackageNotFoundError:
         return 'development'
 
 
+def format_error(msg: str) -> str:
+    max_size = _common_settings['max_error_size'].value
+    if max_size:
+        return msg[:max_size]
+    return msg
+
+
 @dataclass
 class CommonSetting:
     name: str
     options: Sequence[Any]
     default: Any
     value: Optional[Any] = None
 
@@ -62,7 +69,9 @@
 _init_common('max_connection_age', (), 10 * 60)  # Max time in seconds to keep reusing a database TCP connection
 _init_common('product_name', (), '')  # Product name used as part of client identification for ClickHouse query_log
 _init_common('readonly', (0, 1), 0)  # Implied "read_only" ClickHouse settings for versions prior to 19.17
 
 # Use the client protocol version  This is needed for DateTime timezone columns but breaks with current version of
 # chproxy
 _init_common('use_protocol_version', (True, False), True)
+
+_init_common('max_error_size', (), 1024)
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     @property
     def name(self):
         name = f'{self.base_type}{self._name_suffix}'
         for wrapper in reversed(self.wrappers):
             name = f'{wrapper}({name})'
         return name
 
-    def data_size(self, sample: Collection) -> int:
+    def data_size(self, sample: Sequence) -> int:
         if self.low_card:
             values = set(sample)
             d_size = self._data_size(values) + 2
         else:
             d_size = self._data_size(sample)
         if self.nullable:
             d_size += 1
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from clickhouse_connect.driver.query import QueryContext
 from clickhouse_connect.driver.types import ByteSource
 from clickhouse_connect.json_impl import any_to_json
 from clickhouse_connect.datatypes.base import ClickHouseType, TypeDef
 from clickhouse_connect.driver.common import must_swap
 from clickhouse_connect.datatypes.registry import get_from_name
 
-
 logger = logging.getLogger(__name__)
 
 
 class Array(ClickHouseType):
     __slots__ = ('element_type',)
     python_type = list
 
@@ -84,32 +83,35 @@
             column = data
         final_type.write_column_data(column, dest, ctx)
 
 
 class Tuple(ClickHouseType):
     _slots = 'element_names', 'element_types'
     python_type = tuple
-    valid_formats = 'tuple', 'json', 'native'  # native is 'tuple' for unnamed tuples, and dict for named tuples
+    valid_formats = 'tuple', 'dict', 'json', 'native'  # native is 'tuple' for unnamed tuples, and dict for named tuples
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
         self.element_names = type_def.keys
         self.element_types = [get_from_name(name) for name in type_def.values]
         if self.element_names:
             self._name_suffix = f"({', '.join(k + ' ' + str(v) for k, v in zip(type_def.keys, type_def.values))})"
         else:
             self._name_suffix = type_def.arg_str
 
     def _data_size(self, sample: Collection) -> int:
         if len(sample) == 0:
             return 0
         elem_size = 0
+        is_dict = self.element_names and isinstance(self._first_value(list(sample)), dict)
         for ix, e_type in enumerate(self.element_types):
             if e_type.byte_size > 0:
                 elem_size += e_type.byte_size
+            elif is_dict:
+                elem_size += e_type.data_size([x.get(self.element_names[ix], None) for x in sample])
             else:
                 elem_size += e_type.data_size([x[ix] for x in sample])
         return elem_size
 
     def read_column_prefix(self, source: ByteSource):
         for e_type in self.element_types:
             e_type.read_column_prefix(source)
@@ -132,18 +134,29 @@
         return tuple(zip(*columns))
 
     def write_column_prefix(self, dest: bytearray):
         for e_type in self.element_types:
             e_type.write_column_prefix(dest)
 
     def write_column_data(self, column: Sequence, dest: bytearray, ctx: InsertContext):
-        columns = list(zip(*column))
+        if self.element_names and isinstance(self._first_value(column), dict):
+            columns = self.convert_dict_insert(column)
+        else:
+            columns = list(zip(*column))
         for e_type, elem_column in zip(self.element_types, columns):
             e_type.write_column_data(elem_column, dest, ctx)
 
+    def convert_dict_insert(self, column: Sequence) -> Sequence:
+        names = self.element_names
+        col = [[] for _ in names]
+        for x in column:
+            for ix, name in enumerate(names):
+                col[ix].append(x.get(name))
+        return col
+
 
 class Map(ClickHouseType):
     _slots = 'key_type', 'value_type'
     python_type = dict
 
     def __init__(self, type_def: TypeDef):
         super().__init__(type_def)
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,14 @@
         else:
             self.tzinfo = None
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         if self.read_format(ctx) == 'int':
             return source.read_array(self._array_type, num_rows)
         active_tz = ctx.active_tz(self.tzinfo)
-        if active_tz == pytz.UTC:
-            active_tz = None
         if ctx.use_numpy:
             np_array = numpy_conv.read_numpy_array(source, '<u4', num_rows).astype(self.np_type)
             if ctx.as_pandas and active_tz:
                 return pd.DatetimeIndex(np_array, tz='UTC').tz_convert(active_tz)
             return np_array
         return data_conv.read_datetime_col(source, num_rows, active_tz)
 
@@ -167,16 +165,14 @@
     def nano_divisor(self):
         return 1000000000 // self.prec
 
     def _read_column_binary(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         if self.read_format(ctx) == 'int':
             return source.read_array('q', num_rows)
         active_tz = ctx.active_tz(self.tzinfo)
-        if active_tz == pytz.UTC:
-            active_tz = None
         if ctx.use_numpy:
             np_array = numpy_conv.read_numpy_array(source, self.np_type, num_rows)
             if ctx.as_pandas and active_tz and active_tz != pytz.UTC:
                 return pd.DatetimeIndex(np_array, tz='UTC').tz_convert(active_tz)
             return np_array
         column = source.read_array('q', num_rows)
         if active_tz and active_tz != pytz.UTC:
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from clickhouse_connect.datatypes.registry import get_from_name
 from clickhouse_connect.datatypes.base import ClickHouseType
 from clickhouse_connect.driver.common import dict_copy, StreamContext, coerce_int, coerce_bool
 from clickhouse_connect.driver.constants import CH_VERSION_WITH_PROTOCOL, PROTOCOL_VERSION_WITH_LOW_CARD
 from clickhouse_connect.driver.exceptions import ProgrammingError, OperationalError
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.insert import InsertContext
+from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.models import ColumnDef, SettingDef, SettingStatus
 from clickhouse_connect.driver.query import QueryResult, to_arrow, QueryContext, arrow_buffer
 
 io.DEFAULT_BUFFER_SIZE = 1024 * 256
 logger = logging.getLogger(__name__)
 arrow_str_setting = 'output_format_arrow_string_as_string'
 
@@ -32,14 +33,15 @@
     """
     compression: str = None
     write_compression: str = None
     protocol_version = 0
     valid_transport_settings = set()
     optional_transport_settings = set()
     database = None
+    max_error_message = 0
 
     def __init__(self,
                  database: str,
                  query_limit: int,
                  uri: str,
                  query_retries: int,
                  server_host_name: Optional[str],
@@ -58,15 +60,15 @@
             tuple(self.command('SELECT version(), timezone()', use_database=False))
         try:
             self.server_tz = pytz.timezone(server_tz)
         except UnknownTimeZoneError:
             logger.warning('Warning, server is using an unrecognized timezone %s, will use UTC default', server_tz)
         offsets_differ = datetime.now().astimezone().utcoffset() != datetime.now(tz=self.server_tz).utcoffset()
         self.apply_server_timezone = apply_server_timezone == 'always' or (
-                    coerce_bool(apply_server_timezone) and offsets_differ)
+                coerce_bool(apply_server_timezone) and offsets_differ)
         readonly = 'readonly'
         if not self.min_version('19.17'):
             readonly = common.get_setting('readonly')
         server_settings = self.query(f'SELECT name, value, {readonly} as readonly FROM system.settings LIMIT 10000')
         self.server_settings = {row['name']: SettingDef(**row) for row in server_settings.named_results()}
         if database and not database == '__default__':
             self.database = database
@@ -181,14 +183,16 @@
         del kwargs['self']
         query_context = self.create_query_context(**kwargs)
         if query_context.is_command:
             response = self.command(query,
                                     parameters=query_context.parameters,
                                     settings=query_context.settings,
                                     external_data=query_context.external_data)
+            if isinstance(response, QuerySummary):
+                return response.as_query_result()
             return QueryResult([response] if isinstance(response, list) else [[response]])
         return self._query_with_context(query_context)
 
     def query_column_block_stream(self,
                                   query: str = None,
                                   parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                                   settings: Optional[Dict[str, Any]] = None,
@@ -478,26 +482,27 @@
     @abstractmethod
     def command(self,
                 cmd: str,
                 parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                 data: Union[str, bytes] = None,
                 settings: Dict[str, Any] = None,
                 use_database: bool = True,
-                external_data: Optional[ExternalData] = None) -> Union[str, int, Sequence[str]]:
+                external_data: Optional[ExternalData] = None) -> Union[str, int, Sequence[str], QuerySummary]:
         """
         Client method that returns a single value instead of a result set
         :param cmd: ClickHouse query/command as a python format string
         :param parameters: Optional dictionary of key/values pairs to be formatted
         :param data: Optional 'data' for the command (for INSERT INTO in particular)
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param use_database: Send the database parameter to ClickHouse so the command will be executed in the client
          database context.  Otherwise, no database will be specified with the command.  This is useful for determining
          the default user database
         :param external_data ClickHouse "external data" to send with command/query
-        :return: Decoded response from ClickHouse as either a string, int, or sequence of strings
+        :return: Decoded response from ClickHouse as either a string, int, or sequence of strings, or QuerySummary
+        if no data returned
         """
 
     @abstractmethod
     def ping(self) -> bool:
         """
         Validate the connection, does not throw an Exception (see debug logs)
         :return: ClickHouse server is up and reachable
@@ -509,15 +514,15 @@
                data: Sequence[Sequence[Any]] = None,
                column_names: Union[str, Iterable[str]] = '*',
                database: Optional[str] = None,
                column_types: Sequence[ClickHouseType] = None,
                column_type_names: Sequence[str] = None,
                column_oriented: bool = False,
                settings: Optional[Dict[str, Any]] = None,
-               context: InsertContext = None) -> None:
+               context: InsertContext = None) -> QuerySummary:
         """
         Method to insert multiple rows/data matrix of native Python objects.  If context is specified arguments
         other than data are ignored
         :param table: Target table
         :param data: Sequence of sequences of Python data
         :param column_names: Ordered list of column names or '*' if column types should be retrieved from the
             ClickHouse table definition
@@ -526,15 +531,15 @@
             the server
         :param column_type_names: ClickHouse column type names.  If set then column data does not need to be
             retrieved from the server
         :param column_oriented: If true the data is already "pivoted" in column form
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param context: Optional reusable insert context to allow repeated inserts into the same table with
             different data batches
-        :return: No return, throws an exception if the insert fails
+        :return: QuerySummary with summary information, throws exception if insert fails
         """
         if (context is None or context.empty) and data is None:
             raise ProgrammingError('No data specified for insert') from None
         if context is None:
             context = self.create_insert_context(table,
                                                  column_names,
                                                  database,
@@ -542,60 +547,67 @@
                                                  column_type_names,
                                                  column_oriented,
                                                  settings)
         if data is not None:
             if not context.empty:
                 raise ProgrammingError('Attempting to insert new data with non-empty insert context') from None
             context.data = data
-        self.data_insert(context)
+        return self.data_insert(context)
 
     def insert_df(self, table: str = None,
                   df=None,
                   database: Optional[str] = None,
                   settings: Optional[Dict] = None,
                   column_names: Optional[Sequence[str]] = None,
                   column_types: Sequence[ClickHouseType] = None,
                   column_type_names: Sequence[str] = None,
-                  context: InsertContext = None) -> None:
+                  context: InsertContext = None) -> QuerySummary:
         """
         Insert a pandas DataFrame into ClickHouse.  If context is specified arguments other than df are ignored
         :param table: ClickHouse table
         :param df: two-dimensional pandas dataframe
         :param database: Optional ClickHouse database
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
         :param column_names: An optional list of ClickHouse column names.  If not set, the DataFrame column names
            will be used
         :param column_types: ClickHouse column types.  If set then column data does not need to be retrieved from
             the server
         :param column_type_names: ClickHouse column type names.  If set then column data does not need to be
             retrieved from the server
         :param context: Optional reusable insert context to allow repeated inserts into the same table with
             different data batches
-        :return: No return, throws an exception if the insert fails
+        :return: QuerySummary with summary information, throws exception if insert fails
         """
         if context is None:
             if column_names is None:
                 column_names = df.columns
             elif len(column_names) != len(df.columns):
                 raise ProgrammingError('DataFrame column count does not match insert_columns') from None
-        self.insert(table, df, column_names, database, column_types=column_types, column_type_names=column_type_names,
-                    settings=settings, context=context)
-
-    def insert_arrow(self, table: str, arrow_table, database: str = None, settings: Optional[Dict] = None):
+        return self.insert(table,
+                           df,
+                           column_names,
+                           database,
+                           column_types=column_types,
+                           column_type_names=column_type_names,
+                           settings=settings, context=context)
+
+    def insert_arrow(self, table: str,
+                     arrow_table, database: str = None,
+                     settings: Optional[Dict] = None) -> QuerySummary:
         """
         Insert a PyArrow table DataFrame into ClickHouse using raw Arrow format
         :param table: ClickHouse table
         :param arrow_table: PyArrow Table object
         :param database: Optional ClickHouse database
         :param settings: Optional dictionary of ClickHouse settings (key/string values)
-        :return: No return, throws an exception if the insert fails
+        :return: QuerySummary with summary information, throws exception if insert fails
         """
         full_table = table if '.' in table or not database else f'{database}.{table}'
         column_names, insert_block = arrow_buffer(arrow_table)
-        self.raw_insert(full_table, column_names, insert_block, settings, 'Arrow')
+        return self.raw_insert(full_table, column_names, insert_block, settings, 'Arrow')
 
     def create_insert_context(self,
                               table: str,
                               column_names: Optional[Union[str, Sequence[str]]] = None,
                               database: Optional[str] = None,
                               column_types: Sequence[ClickHouseType] = None,
                               column_type_names: Sequence[str] = None,
@@ -647,19 +659,21 @@
                              column_oriented=column_oriented,
                              settings=settings,
                              data=data)
 
     def min_version(self, version_str: str) -> bool:
         """
         Determine whether the connected server is at least the submitted version
+        For Altinity Stable versions like 22.8.15.25.altinitystable
+        the last condition in the first list comprehension expression is added
         :param version_str: A version string consisting of up to 4 integers delimited by dots
         :return: True if version_str is greater than the server_version, False if less than
         """
         try:
-            server_parts = [int(x) for x in self.server_version.split('.')]
+            server_parts = [int(x) for x in self.server_version.split('.') if x.isnumeric()]
             server_parts.extend([0] * (4 - len(server_parts)))
             version_parts = [int(x) for x in version_str.split('.')]
             version_parts.extend([0] * (4 - len(version_parts)))
         except ValueError:
             logger.warning('Server %s or requested version %s does not match format of numbers separated by dots',
                            self.server_version, version_str)
             return False
@@ -667,27 +681,27 @@
             if x > y:
                 return True
             if x < y:
                 return False
         return True
 
     @abstractmethod
-    def data_insert(self, context: InsertContext):
+    def data_insert(self, context: InsertContext) -> QuerySummary:
         """
         Subclass implementation of the data insert
         :context: InsertContext parameter object
         :return: No return, throws an exception if the insert fails
         """
 
     @abstractmethod
     def raw_insert(self, table: str,
                    column_names: Optional[Sequence[str]] = None,
                    insert_block: Union[str, bytes, Generator[bytes, None, None], BinaryIO] = None,
                    settings: Optional[Dict] = None,
-                   fmt: Optional[str] = None):
+                   fmt: Optional[str] = None) -> QuerySummary:
         """
         Insert data already formatted in a bytes object
         :param table: Table name (whether qualified with the database name or not)
         :param column_names: Sequence of column names
         :param insert_block: Binary or string data already in a recognized ClickHouse format
         :param settings:  Optional dictionary of ClickHouse settings (key/string values)
         :param fmt: Valid clickhouse format
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import logging
 import re
+from datetime import datetime
 from typing import Optional, Dict, Union, Any
 
+import pytz
+
 logger = logging.getLogger(__name__)
 
 _empty_map = {}
 
 
 # pylint: disable=too-many-instance-attributes
 class BaseQueryContext:
+    local_tz: pytz.timezone
+
     def __init__(self,
                  settings: Optional[Dict[str, Any]] = None,
                  query_formats: Optional[Dict[str, str]] = None,
                  column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
                  encoding: Optional[str] = None,
                  use_extended_dtypes: bool = False,
                  use_numpy: bool = False):
@@ -51,7 +56,17 @@
         for type_pattern, fmt in self._active_col_type_fmts.items():
             if type_pattern.match(ch_type):
                 return fmt
         for type_pattern, fmt in self.type_formats.items():
             if type_pattern.match(ch_type):
                 return fmt
         return None
+
+
+def _init_context_cls():
+    local_tz = datetime.now().astimezone().tzinfo
+    if local_tz.tzname(datetime.now()) in ('UTC', 'GMT', 'Universal', 'GMT-0', 'Zulu', 'Greenwich'):
+        local_tz = pytz.UTC
+    BaseQueryContext.local_tz = local_tz
+
+
+_init_context_cls()
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/httpclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from clickhouse_connect.driver.common import dict_copy, coerce_bool, coerce_int
 from clickhouse_connect.driver.compression import available_compression
 from clickhouse_connect.driver.exceptions import DatabaseError, OperationalError, ProgrammingError
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.httputil import ResponseSource, get_pool_manager, get_response_data, \
     default_pool_manager, get_proxy_manager, all_managers, check_env_proxy, check_conn_reset
 from clickhouse_connect.driver.insert import InsertContext
+from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.query import QueryResult, QueryContext, quote_identifier, bind_query
 from clickhouse_connect.driver.transform import NativeTransform
 
 logger = logging.getLogger(__name__)
 columns_only_re = re.compile(r'LIMIT 0\s*$', re.IGNORECASE)
 
 
@@ -211,83 +212,95 @@
                                      stream=True,
                                      retries=self.query_retries,
                                      fields=fields,
                                      server_wait=not context.streaming)
         byte_source = RespBuffCls(ResponseSource(response))  # pylint: disable=not-callable
         context.set_response_tz(self._check_tz_change(response.headers.get('X-ClickHouse-Timezone')))
         query_result = self._transform.parse_response(byte_source, context)
-        if 'X-ClickHouse-Summary' in response.headers:
-            try:
-                summary = json.loads(response.headers['X-ClickHouse-Summary'])
-                query_result.summary = summary
-            except json.JSONDecodeError:
-                pass
-        query_result.query_id = response.headers.get('X-ClickHouse-Query-Id')
+        query_result.summary = self._summary(response)
         return query_result
 
-    def data_insert(self, context: InsertContext):
+    def data_insert(self, context: InsertContext) -> QuerySummary:
         """
         See BaseClient doc_string for this method
         """
         if context.empty:
             logger.debug('No data included in insert, skipping')
-            return
+            return QuerySummary()
         if context.compression is None:
             context.compression = self.write_compression
         block_gen = self._transform.build_insert(context)
 
         def error_handler(response: HTTPResponse):
             # If we actually had a local exception when building the insert, throw that instead
             if context.insert_exception:
                 ex = context.insert_exception
                 context.insert_exception = None
                 raise ProgrammingError('Internal serialization error.  This usually indicates invalid data types ' +
                                        'in an inserted row or column') from ex  # type: ignore
             self._error_handler(response)
 
-        self.raw_insert(context.table,
-                        context.column_names,
-                        block_gen,
-                        context.settings,
-                        self._write_format,
-                        context.compression,
-                        error_handler)
+        resp = self.raw_insert(insert_block=block_gen,
+                               settings=context.settings,
+                               compression=context.compression,
+                               status_handler=error_handler)
         context.data = None
+        return resp
 
-    def raw_insert(self, table: str,
+    def raw_insert(self, table: str = None,
                    column_names: Optional[Sequence[str]] = None,
                    insert_block: Union[str, bytes, Generator[bytes, None, None], BinaryIO] = None,
                    settings: Optional[Dict] = None,
                    fmt: Optional[str] = None,
                    compression: Optional[str] = None,
-                   status_handler: Optional[Callable] = None):
+                   status_handler: Optional[Callable] = None) -> QuerySummary:
         """
         See BaseClient doc_string for this method
         """
         write_format = fmt if fmt else self._write_format
+        params = {}
         headers = {'Content-Type': 'application/octet-stream'}
         if compression:
             headers['Content-Encoding'] = compression
-        cols = f" ({', '.join([quote_identifier(x) for x in column_names])})" if column_names is not None else ''
-        params = {'query': f'INSERT INTO {table}{cols} FORMAT {write_format}'}
+        if table:
+            cols = f" ({', '.join([quote_identifier(x) for x in column_names])})" if column_names is not None else ''
+            query = f'INSERT INTO {table}{cols} FORMAT {write_format}'
+            if isinstance(insert_block, str):
+                insert_block = query + '\n' + insert_block
+            elif isinstance(insert_block, (bytes, bytearray, BinaryIO)):
+                insert_block = (query + '\n').encode() + insert_block
+            else:
+                params['query'] = query
         if self.database:
             params['database'] = self.database
         params.update(self._validate_settings(settings or {}))
         response = self._raw_request(insert_block, params, headers,
                                      error_handler=status_handler,
                                      server_wait=False)
         logger.debug('Insert response code: %d, content: %s', response.status, response.data)
+        return QuerySummary(self._summary(response))
+
+    @staticmethod
+    def _summary(response: HTTPResponse):
+        summary = {}
+        if 'X-ClickHouse-Summary' in response.headers:
+            try:
+                summary = json.loads(response.headers['X-ClickHouse-Summary'])
+            except json.JSONDecodeError:
+                pass
+        summary['query_id'] = response.headers.get('X-ClickHouse-Query-Id', '')
+        return summary
 
     def command(self,
                 cmd,
                 parameters: Optional[Union[Sequence, Dict[str, Any]]] = None,
                 data: Union[str, bytes] = None,
                 settings: Optional[Dict] = None,
                 use_database: int = True,
-                external_data: Optional[ExternalData] = None) -> Union[str, int, Sequence[str]]:
+                external_data: Optional[ExternalData] = None) -> Union[str, int, Sequence[str], QuerySummary]:
         """
         See BaseClient doc_string for this method
         """
         cmd, params = bind_query(cmd, parameters, self.server_tz)
         headers = {}
         payload = None
         fields = None
@@ -310,29 +323,34 @@
             payload = cmd
         if use_database and self.database:
             params['database'] = self.database
         params.update(self._validate_settings(settings or {}))
 
         method = 'POST' if payload or fields else 'GET'
         response = self._raw_request(payload, params, headers, method, fields=fields)
-        result = response.data.decode()[:-1].split('\t')
-        if len(result) == 1:
+        if response.data:
             try:
-                return int(result[0])
-            except ValueError:
-                return result[0]
-        return result
+                result = response.data.decode()[:-1].split('\t')
+                if len(result) == 1:
+                    try:
+                        return int(result[0])
+                    except ValueError:
+                        return result[0]
+                return result
+            except UnicodeDecodeError:
+                return str(response.data)
+        return QuerySummary(self._summary(response))
 
     def _error_handler(self, response: HTTPResponse, retried: bool = False) -> None:
         err_str = f'HTTPDriver for {self.url} returned response code {response.status})'
         err_content = get_response_data(response)
+
         if err_content:
-            err_msg = err_content.decode(errors='backslashreplace')
-            logger.error(err_msg)
-            err_str = f':{err_str}\n {err_msg[0:240]}'
+            err_msg = common.format_error(err_content.decode(errors='backslashreplace'))
+            err_str = f':{err_str}\n {err_msg}'
         raise OperationalError(err_str) if retried else DatabaseError(err_str) from None
 
     def _raw_request(self,
                      data,
                      params: Dict[str, str],
                      headers: Optional[Dict[str, Any]] = None,
                      method: str = 'POST',
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import logging
 from math import log
 from typing import Iterable, Sequence, Optional, Any, Dict, NamedTuple, Generator, Union, TYPE_CHECKING
 
+from clickhouse_connect.driver.query import quote_identifier
+
 from clickhouse_connect.driver.ctypes import data_conv
 from clickhouse_connect.driver.context import BaseQueryContext
 from clickhouse_connect.driver.options import np, pd
 from clickhouse_connect.driver.exceptions import ProgrammingError
 
 if TYPE_CHECKING:
     from clickhouse_connect.datatypes.base import ClickHouseType
 
 logger = logging.getLogger(__name__)
 DEFAULT_BLOCK_BYTES = 1 << 24   # Try to generate blocks between 16 and 32MB in raw size
 
 
 class InsertBlock(NamedTuple):
+    prefix: bytes
     column_count: int
     row_count: int
     column_names: Iterable[str]
     column_types: Iterable['ClickHouseType']
     column_data: Iterable[Sequence[Any]]
 
 
@@ -118,17 +121,22 @@
 
     def next_block(self) -> Generator[InsertBlock, None, None]:
         while True:
             block_end = min(self.current_row + self.block_size, self.row_count)
             row_count = block_end - self.current_row
             if row_count <= 0:
                 return
+            if self.current_block == 0:
+                cols = f" ({', '.join([quote_identifier(x) for x in self.column_names])})"
+                prefix = f'INSERT INTO {self.table}{cols} FORMAT Native\n'.encode()
+            else:
+                prefix = bytes()
             self.current_block += 1
             data = self._next_block_data(self.current_row, block_end)
-            yield InsertBlock(self.column_count, row_count, self.column_names, self.column_types, data)
+            yield InsertBlock(prefix, self.column_count, row_count, self.column_names, self.column_types, data)
             self.current_row = block_end
 
     def _column_block_data(self, block_start, block_end):
         if block_start == 0 and self.row_count <= block_end:
             return self._block_columns  # Optimization if we don't need to break up the block
         return [col[block_start: block_end] for col in self._block_columns]
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,24 +155,30 @@
         if self.column_tzs and name in self.column_tzs:
             self.column_tz = self.column_tzs[name]
         else:
             self.column_tz = None
 
     def active_tz(self, datatype_tz: Optional[tzinfo]):
         if self.column_tz:
-            return self.column_tz
-        if datatype_tz:
-            return datatype_tz
-        if self.query_tz:
-            return self.query_tz
-        if self.response_tz:
-            return self.response_tz
-        if self.apply_server_tz:
-            return self.server_tz
-        return None
+            active_tz = self.column_tz
+        elif datatype_tz:
+            active_tz = datatype_tz
+        elif self.query_tz:
+            active_tz = self.query_tz
+        elif self.response_tz:
+            active_tz = self.response_tz
+        elif self.apply_server_tz:
+            active_tz = self.server_tz
+        else:
+            active_tz = self.local_tz
+        #  Special case where if everything is UTC, including the local timezone, we use naive timezones
+        #  for performance reasons
+        if active_tz == pytz.UTC and active_tz.utcoffset(datetime.now()) == self.local_tz.utcoffset(datetime.now()):
+            return None
+        return active_tz
 
     def updated_copy(self,
                      query: Optional[str] = None,
                      parameters: Optional[Dict[str, Any]] = None,
                      settings: Optional[Dict[str, Any]] = None,
                      query_formats: Optional[Dict[str, str]] = None,
                      column_formats: Optional[Dict[str, Union[str, Dict[str, str]]]] = None,
@@ -230,19 +236,19 @@
                  source: Closable = None,
                  query_id: str = None,
                  summary: Dict[str, Any] = None):
         self._result_rows = result_set
         self._result_columns = None
         self._block_gen = block_gen or empty_gen()
         self._in_context = False
+        self._query_id = query_id
         self.column_names = column_names
         self.column_types = column_types
         self.column_oriented = column_oriented
         self.source = source
-        self.query_id = query_id
         self.summary = {} if summary is None else summary
 
     @property
     def result_set(self) -> Matrix:
         if self.column_oriented:
             return self.result_columns
         return self.result_rows
@@ -264,25 +270,31 @@
             result = []
             with self.row_block_stream as stream:
                 for block in stream:
                     result.extend(block)
             self._result_rows = result
         return self._result_rows
 
+    @property
+    def query_id(self) -> str:
+        query_id = self.summary.get('query_id')
+        if query_id:
+            return query_id
+        return self._query_id
+
     def _column_block_stream(self):
         if self._block_gen is None:
             raise StreamClosedError
         block_stream = self._block_gen
         self._block_gen = None
         return block_stream
 
     def _row_block_stream(self):
         for block in self._column_block_stream():
             yield list(zip(*block))
-            # yield data_conv.pivot(block, 0, len(block))
 
     @property
     def column_block_stream(self) -> StreamContext:
         return StreamContext(self, self._column_block_stream())
 
     @property
     def row_block_stream(self):
@@ -324,15 +336,14 @@
             self.source.close()
             self.source = None
         if self._block_gen is not None:
             self._block_gen.close()
             self._block_gen = None
 
 
-local_tz = datetime.now().astimezone().tzinfo
 BS = '\\'
 must_escape = (BS, '\'')
 
 
 def quote_identifier(identifier: str):
     first_char = identifier[0]
     if first_char in ('`', '"') and identifier[-1] == first_char:
@@ -376,15 +387,15 @@
     :return: Literal string for python value
     """
     if value is None:
         return 'NULL'
     if isinstance(value, str):
         return format_str(value)
     if isinstance(value, datetime):
-        if value.tzinfo is None and server_tz != local_tz:
+        if value.tzinfo is None:
             value = value.replace(tzinfo=server_tz)
         return f"'{value.strftime('%Y-%m-%d %H:%M:%S')}'"
     if isinstance(value, date):
         return f"'{value.isoformat()}'"
     if isinstance(value, list):
         return f"[{', '.join(format_query_value(x, server_tz) for x in value)}]"
     if isinstance(value, tuple):
@@ -419,15 +430,15 @@
         return '\\N'
     if isinstance(value, str):
         if top_level:
             # At the top levels, strings must not be surrounded by quotes
             return escape_str(value)
         return format_str(value)
     if isinstance(value, datetime):
-        if value.tzinfo is None and server_tz != local_tz:
+        if value.tzinfo is None:
             value = value.replace(tzinfo=server_tz)
         val = value.strftime('%Y-%m-%d %H:%M:%S')
         if top_level:
             return val
         return f"'{val}'"
     if isinstance(value, date):
         if top_level:
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional, Sequence, Dict, Any
 
 from clickhouse_connect.driver import Client
+from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.query import quote_identifier
 
 
 def insert_file(client: Client,
                 table: str,
                 file_path: str,
                 fmt: Optional[str] = None,
                 column_names: Optional[Sequence[str]] = None,
                 database: Optional[str] = None,
-                settings: Optional[Dict[str, Any]] = None):
+                settings: Optional[Dict[str, Any]] = None) -> QuerySummary:
     full_table = f'{quote_identifier(database)}.{quote_identifier(table)}' if database else quote_identifier(table)
     if not fmt:
         fmt = 'CSV' if column_names else 'CSVWithNames'
     with open(file_path, 'rb') as file:
-        client.raw_insert(full_table, column_names=column_names, insert_block=file, fmt=fmt, settings=settings)
+        return client.raw_insert(full_table, column_names=column_names, insert_block=file, fmt=fmt, settings=settings)
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     @staticmethod
     def build_insert(context: InsertContext):
         compressor = get_compressor(context.compression)
 
         def chunk_gen():
             for x in context.next_block():
                 output = bytearray()
+                output += x.prefix
                 write_leb128(x.column_count, output)
                 write_leb128(x.row_count, output)
                 for col_name, col_type, data in zip(x.column_names, x.column_types, x.column_data):
                     write_leb128(len(col_name), output)
                     output += col_name.encode()
                     write_leb128(len(col_type.name), output)
                     output += col_type.name.encode()
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.6.5/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.6.5/clickhouse_connect/entry_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 
 import sys
-import pkg_resources
+from importlib_metadata import PackageNotFoundError, distribution
 
 EXPECTED_EPS = {'sqlalchemy.dialects:clickhousedb',
                 'sqlalchemy.dialects:clickhousedb.connect'}
 
 
 def validate_entrypoints():
     expected_eps = EXPECTED_EPS.copy()
     try:
-        dist = pkg_resources.get_distribution('clickhouse-connect')
-    except pkg_resources.DistributionNotFound:
+        dist = distribution('clickhouse-connect')
+    except PackageNotFoundError:
         print ('\nClickHouse Connect package not found in this Python installation')
         return -1
     entry_map = dist.get_entry_map()
     print()
     for ep_group, entry_points in entry_map.items():
         print (ep_group)
         for entry_point in entry_points.values():
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.6.5/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.6.5/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.6.5/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.6.5/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.4
+Version: 0.6.5
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.4/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.6.5/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 clickhouse_connect/driver/insert.py
 clickhouse_connect/driver/models.py
 clickhouse_connect/driver/npconv.py
 clickhouse_connect/driver/npquery.py
 clickhouse_connect/driver/options.py
 clickhouse_connect/driver/parser.py
 clickhouse_connect/driver/query.py
+clickhouse_connect/driver/summary.py
 clickhouse_connect/driver/tools.py
 clickhouse_connect/driver/transform.py
 clickhouse_connect/driver/types.py
 clickhouse_connect/driverc/__init__.py
 clickhouse_connect/tools/__init__.py
 clickhouse_connect/tools/datagen.py
 clickhouse_connect/tools/testing.py
```

### Comparing `clickhouse-connect-0.6.4/setup.py` & `clickhouse-connect-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         package_data={'clickhouse_connect': ['VERSION']},
         url='https://github.com/ClickHouse/clickhouse-connect',
         packages=find_packages(exclude=['tests*']),
         python_requires='~=3.7',
         license='Apache License 2.0',
         install_requires=[
             'certifi',
+            'importlib_metadata',
             'urllib3>=1.26',
             'pytz',
             'zstandard',
             'lz4'
         ],
         extras_require={
             'sqlalchemy': ['sqlalchemy>1.3.21,<2.0'],
```

