# Comparing `tmp/abnosql-0.0.1.tar.gz` & `tmp/abnosql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.1.tar", last modified: Thu Jul  6 21:09:39 2023, max compression
+gzip compressed data, was "abnosql-0.0.2.tar", last modified: Fri Jul  7 02:13:49 2023, max compression
```

## Comparing `abnosql-0.0.1.tar` & `abnosql-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.941640 abnosql-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 21:09:21.000000 abnosql-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-06 21:09:39.941640 abnosql-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-06 21:09:21.000000 abnosql-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.937640 abnosql-0.0.1/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4078 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.941640 abnosql-0.0.1/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.941640 abnosql-0.0.1/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.941640 abnosql-0.0.1/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 21:09:21.000000 abnosql-0.0.1/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:39.937640 abnosql-0.0.1/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 21:09:39.000000 abnosql-0.0.1/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 21:09:39.941640 abnosql-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2313 2023-07-06 21:09:21.000000 abnosql-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 02:13:33.000000 abnosql-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-07 02:13:49.814130 abnosql-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-07 02:13:33.000000 abnosql-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4078 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 02:13:49.814130 abnosql-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-07-07 02:13:33.000000 abnosql-0.0.2/setup.py
```

### Comparing `abnosql-0.0.1/LICENSE` & `abnosql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/cli.py` & `abnosql-0.0.2/abnosql/cli.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.2/abnosql/mocks/mock_cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.2/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/plugin.py` & `abnosql-0.0.2/abnosql/plugin.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.2/abnosql/plugins/table/cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.2/abnosql/plugins/table/dynamodb.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/plugins/table/memory.py` & `abnosql-0.0.2/abnosql/plugins/table/memory.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/abnosql/table.py` & `abnosql-0.0.2/abnosql/table.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,74 +13,186 @@
 hookspec = pluggy.HookspecMarker('abnosql.table')
 
 
 class TableSpecs(plugin.PluginSpec):
 
     @hookspec(firstresult=True)
     def set_config(self, table: str) -> t.Dict:  # type: ignore[empty-body] # noqa E501
+        """Hook to set config
+
+        Args:
+
+            table: table name
+
+        Returns:
+
+            dictionary containing config
+
+        """
         pass
 
     @hookspec(firstresult=True)
     def get_item_post(self, table: str, item: t.Dict) -> t.Dict:  # type: ignore[empty-body] # noqa E501
+        """Hook invoked after get_item()
+
+        Args:
+
+            table: table name
+            item: dictionary item retrieved from get_item call
+
+        Returns:
+
+            dictionary containing updated item
+
+        """
         pass
 
     @hookspec
     def put_item_post(self, table: str, item: t.Dict) -> None:  # type: ignore[empty-body] # noqa E501
+        """Hook invoked after put_item()
+
+        Args:
+
+            table: table name
+            item: dictionary containing partition and range/sort key
+
+        """
         pass
 
     @hookspec
     def put_items_post(self, table: str, items: t.List[t.Dict]) -> None:  # type: ignore[empty-body] # noqa E501
+        """Hook invoked after put_items()
+
+        Args:
+
+            table: table name
+            item: list of dictionary items written to table
+
+        """
         pass
 
     @hookspec
     def delete_item_post(self, table: str, key: t.Dict) -> None:  # type: ignore[empty-body] # noqa E501
+        """Hook invoked after delete_item()
+
+        Args:
+
+            table: table name
+            key: dictionary of item written to table
+
+        """
         pass
 
 
 class TableBase(metaclass=ABCMeta):
     @abstractmethod
     def __init__(
         self, pm: plugin.PM, name: str, config: t.Optional[dict] = None
     ) -> None:
+        """Instantiate table object
+
+        Args:
+
+            pm: pluggy plugin manager
+            name: table name
+            config: optional config dict dict
+        """
         pass
 
     @abstractmethod
     def get_item(self, **kwargs) -> t.Dict:
+        """Get table/collection item
+
+        Args:
+
+            partition key and range/sort key (if used)
+
+        Returns:
+
+            item dictionary or None if not found
+
+        """
         pass
 
     @abstractmethod
     def put_item(self, item: t.Dict):
+        """Puts table/collection item
+
+        Args:
+
+            item: dictionary
+
+        """
         pass
 
     @abstractmethod
     def put_items(self, items: t.Iterable[t.Dict]):
+        """Puts multiple table/collection items
+
+        Args:
+
+            items: list of item dictionaries
+
+        """
         pass
 
     @abstractmethod
     def delete_item(self, **kwargs):
+        """Deletes table/collection item
+
+        Args:
+            partition key and range/sort key (if used)
+
+        """
         pass
 
     @abstractmethod
     def query(
         self,
         key: t.Dict[str, t.Any],
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
         next: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
+        """Perform key based query with optional exact match filters
+
+        Args:
+
+            key: dictionary containing partition key and range/sort key
+            filters: optional dictionary of key=value to query and filter on
+            limit: query limit
+            next: pagination token
+
+        Returns:
+            dictionary containing 'items' and 'next' pagination token
+
+        """
         pass
 
     @abstractmethod
     def query_sql(
         self,
         statement: str,
         parameters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
         next: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
+        """Perform key based query with optional exact match filters
+
+        Args:
+
+            statement: SQL statement to query table
+            parameters: optional dictionary containing @key = value placeholders
+            limit: query limit
+            next: pagination token
+
+        Returns:
+            dictionary containing 'items' and 'next' pagination token
+
+        """
         pass
 
 
 def get_sql_params(
     statement: str,
     parameters: t.Dict[str, t.Any],
     param_val: t.Callable,
```

### Comparing `abnosql-0.0.1/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.2/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.1/setup.py` & `abnosql-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     'moto[dynamodb]',
     'mypy',
     'pytest',
     'pytest-cov',
     'responses'
 ]
 dev_require = tests_require + [
+    'pdoc',
     'pre-commit'
 ]
 
 setup(
     name='abnosql',
     version=__version__,
     description='NoSQL Abstraction Library',
```

