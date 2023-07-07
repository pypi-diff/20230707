# Comparing `tmp/shipyard_fivetran-0.1.1.tar.gz` & `tmp/shipyard_fivetran-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.1.1a0.tar", max compression
```

## Comparing `shipyard_fivetran-0.1.1.tar` & `shipyard_fivetran-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0      632 2023-07-07 15:43:47.376627 shipyard_fivetran-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.1/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.1/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     2738 2023-07-07 15:42:18.108055 shipyard_fivetran-0.1.1/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2144 2023-07-07 15:42:18.108365 shipyard_fivetran-0.1.1/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.1/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      625 2023-06-21 13:51:00.826351 shipyard_fivetran-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-15 18:51:26.057456 shipyard_fivetran-0.1.1a0/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-20 19:00:52.344947 shipyard_fivetran-0.1.1a0/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     9921 2023-06-21 13:50:06.109327 shipyard_fivetran-0.1.1a0/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.1a0/PKG-INFO
```

### Comparing `shipyard_fivetran-0.1.1/pyproject.toml` & `shipyard_fivetran-0.1.1a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "shipyard-fivetran"
-version = "0.1.1"
+version = "0.1.1a0"
 description = "A local client for connecting and working with Fivetran"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>" ,"wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{include = "shipyard_fivetran"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = "2023.3"
-requests = "2.31.0"
-shipyard-templates = "0.1.6"
-shipyard-utils = "0.1.4"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
-shipyard-bp-utils = {path = "../shipyard-bp-utils",develop=true}
+shipyard-templates = {path = "../../shipyard-templates"}
+shipyard-bp-utils = {path = "../shipyard-bp-utils"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_fivetran-0.1.1/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.1.1a0/shipyard_fivetran/fivetran.py`

 * *Files identical despite different names*

