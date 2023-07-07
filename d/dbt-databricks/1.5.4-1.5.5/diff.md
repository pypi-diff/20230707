# Comparing `tmp/dbt-databricks-1.5.4.tar.gz` & `tmp/dbt-databricks-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.5.4.tar", last modified: Fri Jun  9 00:00:42 2023, max compression
+gzip compressed data, was "dbt-databricks-1.5.5.tar", last modified: Fri Jul  7 19:50:48 2023, max compression
```

## Comparing `dbt-databricks-1.5.4.tar` & `dbt-databricks-1.5.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.379444 dbt-databricks-1.5.4/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/MANIFEST.in
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-06-09 00:00:42.379214 dbt-databricks-1.5.4/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-05-17 18:30:31.000000 dbt-databricks-1.5.4/README.md
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.358986 dbt-databricks-1.5.4/dbt/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.358431 dbt-databricks-1.5.4/dbt/adapters/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.366624 dbt-databricks-1.5.4/dbt/adapters/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       23 2023-06-08 23:14:31.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2708 2023-05-02 22:11:51.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/auth.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/column.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    26708 2023-06-08 16:32:56.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/connections.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    19041 2023-05-17 18:30:31.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/impl.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    17731 2023-05-17 18:30:27.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/relation.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.359258 dbt-databricks-1.5.4/dbt/include/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.368146 dbt-databricks-1.5.4/dbt/include/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.370325 dbt-databricks-1.5.4/dbt/include/databricks/macros/
--rw-r--r--   0 andre.furlan   (502) staff       (20)    18180 2023-06-08 23:06:31.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.372383 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.374408 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4249 2023-06-08 23:06:31.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-05-02 16:19:19.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-05-02 16:19:19.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/seed.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.375631 dbt-databricks-1.5.4/dbt/include/databricks/macros/utils/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.5.4/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      535 2023-05-02 22:11:51.000000 dbt-databricks-1.5.4/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-06-09 00:00:42.378661 dbt-databricks-1.5.4/dbt_databricks.egg-info/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-06-09 00:00:42.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1421 2023-06-09 00:00:42.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-06-09 00:00:42.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-05-02 22:20:40.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 andre.furlan   (502) staff       (20)      105 2023-06-09 00:00:42.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-06-09 00:00:42.000000 dbt-databricks-1.5.4/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-06-09 00:00:42.379506 dbt-databricks-1.5.4/setup.cfg
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2607 2023-06-08 23:48:19.000000 dbt-databricks-1.5.4/setup.py
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.325054 dbt-databricks-1.5.5/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       46 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/MANIFEST.in
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5375 2023-07-07 19:50:48.324840 dbt-databricks-1.5.5/PKG-INFO
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     4572 2023-07-07 19:49:51.000000 dbt-databricks-1.5.5/README.md
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.302580 dbt-databricks-1.5.5/dbt/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.302355 dbt-databricks-1.5.5/dbt/adapters/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.313396 dbt-databricks-1.5.5/dbt/adapters/databricks/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      626 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       23 2023-07-07 19:49:21.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2708 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      586 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/column.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    28451 2023-07-03 13:50:59.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    19041 2023-07-07 19:49:51.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    17743 2023-07-03 13:45:37.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2863 2023-06-14 23:41:39.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2117 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.302727 dbt-databricks-1.5.5/dbt/include/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.314579 dbt-databricks-1.5.5/dbt/include/databricks/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       52 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/__init__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       77 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.317014 dbt-databricks-1.5.5/dbt/include/databricks/macros/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    18180 2023-06-29 15:29:40.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      592 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2409 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.319386 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.321674 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     4249 2023-06-14 23:41:39.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     3910 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2066 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2451 2023-06-14 23:41:39.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/seed.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5397 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1616 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      119 2023-06-14 23:41:39.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      648 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.322480 dbt-databricks-1.5.5/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      318 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      338 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      535 2023-06-14 20:34:56.000000 dbt-databricks-1.5.5/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-07-07 19:50:48.324477 dbt-databricks-1.5.5/dbt_databricks.egg-info/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5375 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1421 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        1 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        1 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      105 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        4 2023-07-07 19:50:48.000000 dbt-databricks-1.5.5/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       38 2023-07-07 19:50:48.325120 dbt-databricks-1.5.5/setup.cfg
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2607 2023-07-07 19:49:51.000000 dbt-databricks-1.5.5/setup.py
```

### Comparing `dbt-databricks-1.5.4/PKG-INFO` & `dbt-databricks-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.4
+Version: 1.5.5
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.4/README.md` & `dbt-databricks-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/column.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+import uuid
+import logging
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 import itertools
 import os
 import re
 import sys
@@ -15,14 +17,15 @@
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     cast,
+    Union,
 )
 
 from agate import Table
 
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.adapters.base.query_headers import MacroQueryStringSetter
@@ -47,21 +50,44 @@
 )
 from databricks.sql.exc import Error
 
 from dbt.adapters.databricks.__version__ import version as __version__
 from dbt.adapters.databricks.utils import redact_credentials
 
 from databricks.sdk.core import CredentialsProvider
-from databricks.sdk.oauth import OAuthClient, RefreshableCredentials
+from databricks.sdk.oauth import OAuthClient, SessionCredentials
 from dbt.adapters.databricks.auth import token_auth, m2m_auth
 
 import keyring
 
 logger = AdapterLogger("Databricks")
 
+
+class DbtCoreHandler(logging.Handler):
+    def __init__(self, level: Union[str, int], dbt_logger: AdapterLogger):
+        super().__init__(level=level)
+        self.logger = dbt_logger
+
+    def emit(self, record: logging.LogRecord) -> None:
+        # record.levelname will be debug, info, warning, error, or critical
+        # these map 1-to-1 with methods of the AdapterLogger
+        log_func = getattr(self.logger, record.levelname.lower())
+        log_func(record.msg)
+
+
+dbt_adapter_logger = AdapterLogger("databricks-sql-connector")
+
+pysql_logger = logging.getLogger("databricks.sql")
+pysql_logger_level = os.environ.get("DBT_DATABRICKS_CONNECTOR_LOG_LEVEL", "INFO").upper()
+pysql_logger.setLevel(pysql_logger_level)
+
+pysql_handler = DbtCoreHandler(dbt_logger=dbt_adapter_logger, level=pysql_logger_level)
+pysql_logger.addHandler(pysql_handler)
+
+
 CATALOG_KEY_IN_SESSION_PROPERTIES = "databricks.catalog"
 DBR_VERSION_REGEX = re.compile(r"([1-9][0-9]*)\.(x|0|[1-9][0-9]*)")
 DBT_DATABRICKS_INVOCATION_ENV = "DBT_DATABRICKS_INVOCATION_ENV"
 DBT_DATABRICKS_INVOCATION_ENV_REGEX = re.compile("^[A-z0-9\\-]+$")
 EXTRACT_CLUSTER_ID_FROM_HTTP_PATH_REGEX = re.compile(r"/?sql/protocolv1/o/\d+/(.*)")
 DBT_DATABRICKS_HTTP_SESSION_HEADERS = "DBT_DATABRICKS_HTTP_SESSION_HEADERS"
 
@@ -300,15 +326,15 @@
             )
             # optional branch. Try and keep going if it does not work
             try:
                 # try to get cached credentials
                 credsdict = keyring.get_password("dbt-databricks", host)
 
                 if credsdict:
-                    provider = RefreshableCredentials.from_dict(oauth_client, json.loads(credsdict))
+                    provider = SessionCredentials.from_dict(oauth_client, json.loads(credsdict))
                     # if refresh token is expired, this will throw
                     try:
                         if provider.token().valid:
                             return provider
                     except Exception as e:
                         logger.debug(e)
                         # whatever it is, get rid of the cache
@@ -353,15 +379,15 @@
             host=self.host,
             client_id=CLIENT_ID,
             client_secret=None,
             redirect_url=REDIRECT_URL,
             scopes=SCOPES,
         )
 
-        return RefreshableCredentials.from_dict(client=oauth_client, raw=self._credentials_provider)
+        return SessionCredentials.from_dict(client=oauth_client, raw=self._credentials_provider)
 
 
 class DatabricksSQLConnectionWrapper:
     """Wrap a Databricks SQL connector in a way that no-ops transactions"""
 
     _conn: DatabricksSQLConnection
     _is_cluster: bool
@@ -453,14 +479,25 @@
     def execute(self, sql: str, bindings: Optional[Sequence[Any]] = None) -> None:
         if sql.strip().endswith(";"):
             sql = sql.strip()[:-1]
         if bindings is not None:
             bindings = [self._fix_binding(binding) for binding in bindings]
         self._cursor.execute(sql, bindings)
 
+    @property
+    def hex_query_id(self) -> str:
+        """Return the hex GUID for this query
+
+        This UUID can be tied back to the Databricks query history API
+        """
+
+        _as_hex = uuid.UUID(bytes=self._cursor.active_result_set.command_id.operationId.guid)
+
+        return str(_as_hex)
+
     @classmethod
     def _fix_binding(cls, value: Any) -> Any:
         """Convert complex datatypes to primitives that can be loaded by
         the Spark driver"""
         if isinstance(value, DECIMALS):
             return float(value)
         else:
@@ -525,14 +562,19 @@
     def _get_comment_macro(self) -> Optional[str]:
         if self.config.query_comment.comment == DEFAULT_QUERY_COMMENT:
             return DATABRICKS_QUERY_COMMENT
         else:
             return self.config.query_comment.comment
 
 
+@dataclass
+class DatabricksAdapterResponse(AdapterResponse):
+    query_id: str = ""
+
+
 class DatabricksConnectionManager(SparkConnectionManager):
     TYPE: str = "databricks"
     credentials_provider: CredentialsProvider = None
 
     def compare_dbr_version(self, major: int, minor: int) -> int:
         version = (major, minor)
 
@@ -609,15 +651,15 @@
                 raise
             finally:
                 if close_cursor and cursor is not None:
                     cursor.close()
 
     def execute(
         self, sql: str, auto_begin: bool = False, fetch: bool = False
-    ) -> Tuple[AdapterResponse, Table]:
+    ) -> Tuple[DatabricksAdapterResponse, Table]:
         sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin)
         try:
             response = self.get_response(cursor)
             if fetch:
                 table = self.get_result_from_cursor(cursor)
             else:
@@ -724,13 +766,24 @@
             connect=connect,
             logger=logger,
             retryable_exceptions=retryable_exceptions,
             retry_limit=creds.connect_retries,
             retry_timeout=(timeout if timeout is not None else exponential_backoff),
         )
 
+    @classmethod
+    def get_response(cls, cursor: DatabricksSQLCursorWrapper) -> DatabricksAdapterResponse:
+        _query_id = getattr(cursor, "hex_query_id", None)
+        if cursor is None:
+            logger.debug("No cursor was provided. Query ID not available.")
+            query_id = "N/A"
+        else:
+            query_id = _query_id
+        message = "OK"
+        return DatabricksAdapterResponse(_message=message, query_id=query_id)  # type: ignore
+
 
 def _log_dbsql_errors(exc: Exception) -> None:
     if isinstance(exc, Error):
         logger.debug(f"{type(exc)}: {exc}")
         for key, value in sorted(exc.context.items()):
             logger.debug(f"{key}: {value}")
```

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/python_submissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,14 @@
         if response.status_code != 200:
             raise dbt.exceptions.DbtRuntimeError(
                 f"Error deleting an execution context.\n {response.content!r}"
             )
         return response.json()["id"]
 
     def get_cluster_status(self) -> Dict:
-
         # https://docs.databricks.com/dev-tools/api/latest/clusters.html#get
 
         response = requests.get(
             f"https://{self.host}/api/2.0/clusters/get",
             headers=self.auth_header,
             json={"cluster_id": self.cluster_id},
         )
@@ -284,15 +283,15 @@
         start_time = time.time()
 
         def get_elapsed() -> float:
             return time.time() - start_time
 
         while get_elapsed() < MAX_CLUSTER_START_TIME:
             status_response = self.get_cluster_status()
-            if status_response.get("state") == "Running":
+            if str(status_response.get("state")).lower() == "running":
                 return
             else:
                 time.sleep(5)
 
         raise dbt.exceptions.DbtRuntimeError(
             f"Cluster {self.cluster_id} restart timed out after {MAX_CLUSTER_START_TIME} seconds"
         )
```

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.5.5/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/seed.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.5.5/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.5.5/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.5.5/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.5.4
+Version: 1.5.5
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.5.4/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.5.5/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.5.4/setup.py` & `dbt-databricks-1.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-spark~=1.5.0",
-        "databricks-sql-connector~=2.6.1",
-        "databricks-sdk==0.1.6",
+        "databricks-sql-connector~=2.7.0",
+        "databricks-sdk==0.1.7",
         "keyring>=23.13.0",
         "protobuf>=4.21.0" # workaround for dbt-core issue
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
```

