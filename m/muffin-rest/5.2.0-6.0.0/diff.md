# Comparing `tmp/muffin_rest-5.2.0.tar.gz` & `tmp/muffin_rest-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.2.0.tar", max compression
+gzip compressed data, was "muffin_rest-6.0.0.tar", max compression
```

## Comparing `muffin_rest-5.2.0.tar` & `muffin_rest-6.0.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1082 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/LICENSE
--rw-r--r--   0        0        0     2616 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/README.rst
--rw-r--r--   0        0        0     1242 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/errors.py
--rw-r--r--   0        0        0     5607 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/filters.py
--rw-r--r--   0        0        0    10772 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2382 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5378 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1215 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1983 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0      702 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/utils.py
--rw-r--r--   0        0        0        0 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2466 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/utils.py
--rw-r--r--   0        0        0     2743 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/LICENSE
+-rw-r--r--   0        0        0     2616 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/README.rst
+-rw-r--r--   0        0        0     1242 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5607 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10318 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/handler.py
+-rw-r--r--   0        0        0      715 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/marshmallow.py
+-rw-r--r--   0        0        0     4805 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2382 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5378 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1215 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1983 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0      702 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/peewee/utils.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-07-07 06:58:09.692150 muffin_rest-6.0.0/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-07-07 06:58:09.696150 muffin_rest-6.0.0/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-07-07 06:58:09.696150 muffin_rest-6.0.0/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-07-07 06:58:09.696150 muffin_rest-6.0.0/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-07-07 06:58:09.696150 muffin_rest-6.0.0/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2743 2023-07-07 06:58:09.696150 muffin_rest-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-6.0.0/PKG-INFO
```

### Comparing `muffin_rest-5.2.0/LICENSE` & `muffin_rest-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/README.rst` & `muffin_rest-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/__init__.py` & `muffin_rest-6.0.0/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/api.py` & `muffin_rest-6.0.0/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/errors.py` & `muffin_rest-6.0.0/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/filters.py` & `muffin_rest-6.0.0/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/handler.py` & `muffin_rest-6.0.0/muffin_rest/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from muffin import Request
 from muffin.handler import Handler, HandlerMeta
 
 from muffin_rest import LIMIT_PARAM, OFFSET_PARAM, openapi
 from muffin_rest.api import API
 from muffin_rest.errors import APIError
 from muffin_rest.filters import Filter
+from muffin_rest.marshmallow import load_data
 from muffin_rest.sorting import Sort
 from muffin_rest.types import TSchemaRes
 
 from .errors import HandlerNotBindedError
 from .options import RESTOptions
 from .types import TVData, TVResource
 
@@ -217,37 +218,21 @@
         assert self.meta.Schema, "RESTHandler.meta.Schema is required."
         query = request.url.query
         return self.meta.Schema(
             only=query.get("schema_only"),
             exclude=query.get("schema_exclude", ()),
         )
 
-    async def parse(self, request: Request):
-        """Parse data from the given request."""
-        try:
-            return await request.data(raise_errors=True)
-        except (ValueError, TypeError) as exc:
-            raise APIError.BAD_REQUEST(str(exc)) from exc
-
     async def load(
         self, request: Request, resource: Optional[TVResource] = None
     ) -> TVData[TVResource]:
         """Load data from request and create/update a resource."""
-        data = await self.parse(request)
         schema = await self.get_schema(request, resource=resource)
-        if not schema:
-            return cast(TVData[TVResource], data)
-
         return cast(
-            TVData[TVResource],
-            schema.load(
-                cast(Union[dict, list], data),
-                partial=resource is not None,
-                many=isinstance(data, list),
-            ),
+            TVData[TVResource], await load_data(request, schema, partial=resource is not None)
         )
 
     @overload
     async def dump(  # type: ignore[misc]
         self, request, data: TVData, *, many: Literal[True], **opts
     ) -> List[TSchemaRes]:
         ...
```

### Comparing `muffin_rest-5.2.0/muffin_rest/mongo/__init__.py` & `muffin_rest-6.0.0/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/mongo/filters.py` & `muffin_rest-6.0.0/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/mongo/schema.py` & `muffin_rest-6.0.0/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/mongo/sorting.py` & `muffin_rest-6.0.0/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/mongo/utils.py` & `muffin_rest-6.0.0/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/openapi.py` & `muffin_rest-6.0.0/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/options.py` & `muffin_rest-6.0.0/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/filters.py` & `muffin_rest-6.0.0/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/handler.py` & `muffin_rest-6.0.0/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/openapi.py` & `muffin_rest-6.0.0/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/options.py` & `muffin_rest-6.0.0/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/schemas.py` & `muffin_rest-6.0.0/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/sorting.py` & `muffin_rest-6.0.0/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/peewee/utils.py` & `muffin_rest-6.0.0/muffin_rest/peewee/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/redoc.html` & `muffin_rest-6.0.0/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/sorting.py` & `muffin_rest-6.0.0/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-6.0.0/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-6.0.0/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-6.0.0/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/swagger.html` & `muffin_rest-6.0.0/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/types.py` & `muffin_rest-6.0.0/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/muffin_rest/utils.py` & `muffin_rest-6.0.0/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.2.0/pyproject.toml` & `muffin_rest-6.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.2.0"
+version = "6.0.0"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.2.0/PKG-INFO` & `muffin_rest-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.2.0
+Version: 6.0.0
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

