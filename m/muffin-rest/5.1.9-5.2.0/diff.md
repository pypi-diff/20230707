# Comparing `tmp/muffin_rest-5.1.9.tar.gz` & `tmp/muffin_rest-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.1.9.tar", max compression
+gzip compressed data, was "muffin_rest-5.2.0.tar", max compression
```

## Comparing `muffin_rest-5.1.9.tar` & `muffin_rest-5.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1082 2023-06-13 06:36:23.688254 muffin_rest-5.1.9/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-13 06:36:23.688254 muffin_rest-5.1.9/README.rst
--rw-r--r--   0        0        0     1242 2023-06-13 06:36:23.688254 muffin_rest-5.1.9/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-13 06:36:23.688254 muffin_rest-5.1.9/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-13 06:36:23.688254 muffin_rest-5.1.9/muffin_rest/errors.py
--rw-r--r--   0        0        0     5164 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/filters.py
--rw-r--r--   0        0        0    10762 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2326 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5378 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1215 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1895 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0      702 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/peewee/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/muffin_rest/utils.py
--rw-r--r--   0        0        0     2826 2023-06-13 06:36:23.692254 muffin_rest-5.1.9/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/LICENSE
+-rw-r--r--   0        0        0     2616 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/README.rst
+-rw-r--r--   0        0        0     1242 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5607 2023-07-07 06:35:06.761596 muffin_rest-5.2.0/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10772 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2382 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5378 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1215 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1983 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0      702 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/peewee/utils.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2743 2023-07-07 06:35:06.765596 muffin_rest-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.2.0/PKG-INFO
```

### Comparing `muffin_rest-5.1.9/LICENSE` & `muffin_rest-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/README.rst` & `muffin_rest-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/__init__.py` & `muffin_rest-5.2.0/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/api.py` & `muffin_rest-5.2.0/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/errors.py` & `muffin_rest-5.2.0/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/filters.py` & `muffin_rest-5.2.0/muffin_rest/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Support API filters."""
 from __future__ import annotations
 
 import operator
-from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Optional, Tuple  # py38
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Mapping, Optional, Tuple  # py38
 
 import marshmallow as ma
 from asgi_tools._compat import json_loads  # type: ignore[]
 
 from .utils import Mutate, Mutator
 
 if TYPE_CHECKING:
@@ -24,26 +24,34 @@
     operators: Dict[str, Callable] = {
         "$lt": operator.lt,
         "$le": operator.le,
         "$gt": operator.gt,
         "$ge": operator.ge,
         "$eq": operator.eq,
         "$ne": operator.ne,
+        "$like": lambda v, c: c in v,
+        # List ops
         "$in": operator.contains,
         "$nin": lambda v, c: v not in c,
+        # Logic ops
+        "$or": lambda v, c: any(f(v, c) for f in v),
+        "$and": lambda v, c: all(f(v, c) for f in v),
+        "$not": lambda v, c: not v(c),
+        "$nor": lambda v, c: not any(f(v, c) for f in v),
     }
     operators["<"] = operators["$lt"]
     operators["<="] = operators["$le"]
     operators[">"] = operators["$gt"]
     operators[">="] = operators["$ge"]
     operators["=="] = operators["$eq"]
     operators["!="] = operators["$ne"]
     operators["<<"] = operators["$in"]
 
-    list_ops = ["$in", "<<"]
+    list_ops: Iterable[str] = ("$in", "<<", "$nin")
+    logic_ops: Iterable[str] = ("$or", "$and", "$not", "$nor")
 
     field: Any = None
     schema_field: ma.fields.Field = ma.fields.Raw()
     default_operator = "$eq"
 
     def __init__(
         self,
@@ -59,15 +67,15 @@
         :param name: The filter's name
         :param attr: Column/Property name.
         :param fields: Marshmallow Field instance
 
         """
         super(Filter, self).__init__(name, **meta)
         self.field = field if field is not None else self.field
-        self.schema_field: ma.fields.Field = schema_field or self.schema_field
+        self.schema_field = schema_field or self.schema_field
         self.default_operator = operator or self.default_operator
 
     async def apply(self, collection: Any, data: Optional[Mapping] = None):
         """Filter given collection."""
         if not data:
             return None, collection
 
@@ -83,39 +91,40 @@
 
     async def filter(self, collection, *ops: Tuple[Callable, Any], **_):
         """Apply the filter to collection."""
 
         def validator(obj):
             return all(op(get_value(obj, self.name), val) for op, val in ops)
 
-        return [o for o in collection if validator(o)]
+        return [item for item in collection if validator(item)]
 
-    def parse(self, data: Mapping) -> Tuple[Tuple[Callable, Any], ...]:
+    def parse(self, data: Mapping):
         """Parse operator and value from filter's data."""
-        val = data.get(self.name, ma.missing)
-        if not isinstance(val, dict):
-            return (
-                (
-                    self.operators[self.default_operator],
-                    self.schema_field.deserialize(val),
-                ),
-            )
-
-        return tuple(
-            (
-                self.operators[op],
-                (
-                    (self.schema_field.deserialize(val))
-                    if op not in self.list_ops
-                    else [self.schema_field.deserialize(v) for v in val]
-                ),
-            )
-            for (op, val) in val.items()
-            if op in self.operators
-        )
+        value = data.get(self.name, ma.missing)
+        return tuple(self._parse(value))
+
+    def _parse(self, value):
+        deserialize = self.schema_field.deserialize
+        if isinstance(value, dict):
+            for op, val in value.items():
+                operator = self.operators.get(op)
+                if operator is None:
+                    continue
+
+                if op in self.list_ops:
+                    yield operator, [deserialize(v) for v in val]
+
+                elif op in self.logic_ops:
+                    yield operator, [t for v in val for t in tuple(self._parse(v))]
+
+                else:
+                    yield operator, deserialize(val)
+
+        else:
+            yield (self.operators[self.default_operator], deserialize(value))
 
 
 class Filters(Mutator):
 
     """Build filters for handlers."""
 
     MUTATE_CLASS = Filter
```

### Comparing `muffin_rest-5.1.9/muffin_rest/handler.py` & `muffin_rest-5.2.0/muffin_rest/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,44 +101,42 @@
         return cls
 
     async def __call__(self, request: Request, *, method_name: Optional[str] = None, **_) -> Any:
         """Dispatch the given request by HTTP method."""
         method = getattr(self, method_name or request.method.lower())
         self.auth = await self.authorize(request)
         self.collection = await self.prepare_collection(request)
+        headers = None
         resource = await self.prepare_resource(request)
-        if resource or request.method != "GET":
-            try:
-                return await method(request, resource=resource)
-            except ValidationError as exc:
-                raise APIError.BAD_REQUEST("Invalid data", errors=exc.messages) from exc
-
-        meta = self.meta
-
-        # Filter collection
-        if meta.filters:
-            self.collection, self.filters = await meta.filters.apply(request, self.collection)
-
-        # Sort collection
-        if meta.sorting:
-            self.collection, self.sorting = await meta.sorting.apply(request, self.collection)
-
-        # Paginate the collection
-        headers = {}
-        if meta.limit:
-            limit, offset = self.paginate_prepare_params(request)
-            if limit and offset >= 0:
-                self.collection, total = await self.paginate(
-                    request,
-                    limit=limit,
-                    offset=offset,
-                )
-                headers = self.paginate_prepare_headers(limit, offset, total)
+        if request.method == "GET" and resource is None:
+            meta = self.meta
 
-        response = await method(request, resource=resource)
+            # Filter collection
+            if meta.filters:
+                self.collection, self.filters = await meta.filters.apply(request, self.collection)
+
+            # Sort collection
+            if meta.sorting:
+                self.collection, self.sorting = await meta.sorting.apply(request, self.collection)
+
+            # Paginate the collection
+            if meta.limit:
+                limit, offset = self.paginate_prepare_params(request)
+                if limit and offset >= 0:
+                    self.collection, total = await self.paginate(
+                        request,
+                        limit=limit,
+                        offset=offset,
+                    )
+                    headers = self.paginate_prepare_headers(limit, offset, total)
+
+        try:
+            response = await method(request, resource=resource)
+        except ValidationError as exc:
+            raise APIError.BAD_REQUEST("Bad request data", errors=exc.messages) from exc
 
         if headers:
             response = parse_response(response)
             response.headers.update(headers)
 
         return response
```

### Comparing `muffin_rest-5.1.9/muffin_rest/mongo/__init__.py` & `muffin_rest-5.2.0/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/mongo/filters.py` & `muffin_rest-5.2.0/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/mongo/schema.py` & `muffin_rest-5.2.0/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/mongo/sorting.py` & `muffin_rest-5.2.0/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/mongo/utils.py` & `muffin_rest-5.2.0/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/openapi.py` & `muffin_rest-5.2.0/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/options.py` & `muffin_rest-5.2.0/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/filters.py` & `muffin_rest-5.2.0/muffin_rest/peewee/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """Support filters for Peewee ORM."""
 from __future__ import annotations
 
 import operator
+from functools import reduce
 from typing import Any, Callable, Tuple, Type, Union, cast
 
 from peewee import ColumnBase, Field, ModelSelect
 
 from muffin_rest.filters import Filter, Filters
 
 from .utils import get_model_field_by_name
 
 
 class PWFilter(Filter):
     """Support Peewee."""
 
-    operators = Filter.operators
+    operators = dict(Filter.operators)
     operators["$in"] = operator.lshift
     operators["$none"] = operator.rshift
     operators["$like"] = operator.mod
     operators["$ilike"] = operator.pow
     operators["$contains"] = lambda f, v: f.contains(v)
     operators["$starts"] = lambda f, v: f.startswith(v)
     operators["$ends"] = lambda f, v: f.endswith(v)
     operators["$between"] = lambda f, v: f.between(*v)
     operators["$regexp"] = lambda f, v: f.regexp(v)
+    operators["$or"] = lambda col, value: reduce(operator.or_, [op(col, val) for op, val in value])
+    operators["$and"] = lambda col, value: reduce(
+        operator.and_, [op(col, val) for op, val in value]
+    )
 
-    list_ops = [*Filter.list_ops, "$between"]
+    list_ops = (*Filter.list_ops, "$between")
 
     async def filter(
         self, collection: ModelSelect, *ops: Tuple[Callable, Any], **kwargs
     ) -> ModelSelect:
         """Apply the filters to Peewee QuerySet.."""
-        if self.field and ops:
-            return self.query(collection, self.field, *ops, **kwargs)
-        return collection
-
-    def query(self, qs: ModelSelect, column: Field, *ops: Tuple, **_) -> ModelSelect:
-        """Filter a query."""
+        column = self.field
         if isinstance(column, ColumnBase):
-            return cast(ModelSelect, qs.where(*[op(column, val) for op, val in ops]))
-
-        return qs
+            collection = cast(ModelSelect, collection.where(*[op(column, val) for op, val in ops]))
+        return collection
 
 
 class PWFilters(Filters):
     """Bind Peewee filter class."""
 
     MUTATE_CLASS: Type[PWFilter] = PWFilter
```

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/handler.py` & `muffin_rest-5.2.0/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/openapi.py` & `muffin_rest-5.2.0/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/options.py` & `muffin_rest-5.2.0/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/schemas.py` & `muffin_rest-5.2.0/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/sorting.py` & `muffin_rest-5.2.0/muffin_rest/peewee/sorting.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 
 class PWSort(Sort):
     """Sorter for Peewee."""
 
     async def apply(self, collection: TVCollection, *, desc: bool = False) -> TVCollection:
         """Sort the collection."""
+        params = {"nulls": "LAST"} if isinstance(self.field, Field) and self.field.null else {}
         return collection.order_by_extend(
-            self.field.asc(nulls="LAST") if not desc else self.field.desc(nulls="LAST")
+            self.field.asc(**params) if not desc else self.field.desc(**params)
         )
 
 
 class PWSorting(Sorting):
     """Sort Peewee ORM Queries."""
 
     MUTATE_CLASS: Type[PWSort] = PWSort
```

### Comparing `muffin_rest-5.1.9/muffin_rest/peewee/utils.py` & `muffin_rest-5.2.0/muffin_rest/peewee/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/redoc.html` & `muffin_rest-5.2.0/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/sorting.py` & `muffin_rest-5.2.0/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.2.0/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.2.0/muffin_rest/sqlalchemy/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if TYPE_CHECKING:
     from .types import TVCollection
 
 
 class SAFilter(Filter):
     """Custom filter for sqlalchemy."""
 
-    operators = Filter.operators
+    operators = dict(Filter.operators)
     operators["$between"] = lambda c, v: c.between(*v)
     operators["$ends"] = lambda c, v: c.endswith(v)
     operators["$ilike"] = lambda c, v: c.ilike(v)
     operators["$in"] = lambda c, v: c.in_(v)
     operators["$like"] = lambda c, v: c.like(v)
     operators["$match"] = lambda c, v: c.match(v)
     operators["$nin"] = lambda c, v: ~c.in_(v)
```

### Comparing `muffin_rest-5.1.9/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.2.0/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/swagger.html` & `muffin_rest-5.2.0/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/types.py` & `muffin_rest-5.2.0/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/muffin_rest/utils.py` & `muffin_rest-5.2.0/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.9/pyproject.toml` & `muffin_rest-5.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.1.9"
+version = "5.2.0"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
@@ -47,50 +47,45 @@
 marshmallow-peewee = "^4.0.3"
 marshmallow-sqlalchemy = "^0.27.0"
 muffin-databases = "^0.5.0"
 muffin-mongo = "^0.5.1"
 muffin-peewee-aio = "*"
 pytest = "*"
 pytest-aio = { version = "*", extras = ["curio", "trio"] }
-pytest-mypy = "*"
 pyyaml = "*"
 types-PyYAML = "*"
 types-ujson = "*"
 ruff = "*"
+mypy = "*"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 
 [tool.poetry.group.example.dependencies]
 uvicorn = "*"
 muffin-peewee-aio = "*"
 marshmallow-peewee = "^4.0.3"
 
 
 [tool.pytest.ini_options]
-addopts = "-xsv --mypy"
+addopts = "-xsv"
 log_cli = true
 
 [tool.mypy]
 packages = ["muffin_rest"]
 ignore_missing_imports = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py38,py39,py310,py311,pypy39
 
 [testenv]
 deps = -e .[tests]
 commands =
-	pytest --mypy tests
-
-[testenv:pypy39]
-deps = -e .[tests]
-commands =
 	pytest tests
 """
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
```

### Comparing `muffin_rest-5.1.9/PKG-INFO` & `muffin_rest-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.1.9
+Version: 5.2.0
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

