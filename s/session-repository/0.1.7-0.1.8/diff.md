# Comparing `tmp/session-repository-0.1.7.tar.gz` & `tmp/session-repository-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.7.tar", last modified: Thu Jul  6 07:25:01 2023, max compression
+gzip compressed data, was "session-repository-0.1.8.tar", last modified: Fri Jul  7 07:53:43 2023, max compression
```

## Comparing `session-repository-0.1.7.tar` & `session-repository-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.333123 session-repository-0.1.7/
--rw-rw-rw-   0        0        0      599 2023-07-06 07:25:01.331092 session-repository-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.305547 session-repository-0.1.7/session_repository/
--rw-rw-rw-   0        0        0     8431 2023-07-06 07:21:41.000000 session-repository-0.1.7/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.7/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.7/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:25:01.326988 session-repository-0.1.7/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-06 07:25:01.000000 session-repository-0.1.7/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 07:25:01.334193 session-repository-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-06 07:21:55.000000 session-repository-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.742425 session-repository-0.1.8/
+-rw-rw-rw-   0        0        0      599 2023-07-07 07:53:43.740239 session-repository-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.708397 session-repository-0.1.8/session_repository/
+-rw-rw-rw-   0        0        0     8653 2023-07-07 07:52:17.000000 session-repository-0.1.8/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.8/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7777 2023-07-07 07:51:19.000000 session-repository-0.1.8/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.733922 session-repository-0.1.8/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:53:43.742925 session-repository-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-07 07:52:40.000000 session-repository-0.1.8/setup.py
```

### Comparing `session-repository-0.1.7/PKG-INFO` & `session-repository-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.7
+Version: 0.1.8
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.7.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.7/session_repository/core.py` & `session-repository-0.1.8/session_repository/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
         return results
 
     def _select_all(
         self,
         model,
         filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
     ) -> List:
         def _select_from_session(session: Session):
@@ -87,14 +88,19 @@
                 query=query,
                 relationship_dict=disabled_relationships,
             )
             query = apply_filters(
                 query=query,
                 filter_dict=filters,
             )
+            query = apply_filters(
+                query=query,
+                filter_dict=optional_filters,
+                with_optional=True,
+            )
             query = apply_order_by(
                 query=query,
                 model=model,
                 order_by=order_by,
                 direction=direction,
             )
             query = apply_limit(
```

### Comparing `session-repository-0.1.7/session_repository/utils.py` & `session-repository-0.1.8/session_repository/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,33 @@
                 relationship_dict=sub_relationships,
                 parents=sub_items,
             )
 
     return query
 
 
-def apply_filters(query: Query, filter_dict: _FilterType):
-    filters = get_filters(filters=filter_dict)
+def apply_filters(
+    query: Query,
+    filter_dict: _FilterType,
+    with_optional: bool = False,
+):
+    filters = get_filters(
+        filters=filter_dict,
+        with_optional=with_optional,
+    )
 
     return query if len(filters) == 0 else query.filter(and_(*filters))
 
 
-def apply_order_by(query: Query, model, order_by: list[str] | str, direction: str):
+def apply_order_by(
+    query: Query,
+    model,
+    order_by: list[str] | str,
+    direction: str,
+):
     if order_by is None:
         return query
 
     if isinstance(order_by, str):
         order_by = [order_by]
 
     if direction == "desc":
@@ -67,15 +79,18 @@
 
     if direction == "asc":
         return query.order_by(*[asc(getattr(model, column)) for column in order_by])
 
     return query
 
 
-def build_order_by(model, order_by: dict):
+def build_order_by(
+    model,
+    order_by: dict,
+):
     if isinstance(order_by, dict):
         order_by_list = []
         for key, value in order_by.items():
             if isinstance(value, dict):
                 relationship = getattr(model, key)
                 order_by_relationship = build_order_by(value, relationship)
                 order_by_list.extend(order_by_relationship)
@@ -86,15 +101,19 @@
                 elif value == "DESC":
                     order_by_list.append(desc(column))
         return order_by_list
     else:
         raise ValueError("Invalid nomenclature format.")
 
 
-def apply_pagination(query: Query, page: int, per_page: int):
+def apply_pagination(
+    query: Query,
+    page: int,
+    per_page: int,
+):
     pagination = None
     if page is not None and per_page is not None:
         total_results = query.count()
         total_pages = (total_results + per_page - 1) // per_page
 
         pagination = {
             "total": total_results,
@@ -106,26 +125,32 @@
         pagination = json.dumps(pagination)
 
         query = query.offset((page - 1) * per_page).limit(per_page)
 
     return query, pagination
 
 
-def apply_limit(query: Query, limit: int):
+def apply_limit(
+    query: Query,
+    limit: int,
+):
     return query.limit(limit) if limit is not None else query
 
 
-def get_conditions_from_dict(values: _FilterType):
+def get_conditions_from_dict(
+    values: _FilterType,
+    with_optional: bool = False,
+):
     conditions = []
     for key, value in values.items():
         if type(value) == set:
             value = list(value)
         elif type(value) == dict:
             for k, v in value.items():
-                if v is None:
+                if with_optional and v is None:
                     continue
 
                 match k:
                     case Operators.EQUAL:
                         conditions.append(key == v)
                     case Operators.DIFFERENT:
                         conditions.append(key != v)
@@ -175,36 +200,45 @@
                         v = v if isinstance(v, Iterable) else [v]
                         if isinstance(key, tuple):
                             conditions.append(tuple_(*key).in_(v))
                         else:
                             conditions.append(key.in_(v))
                     case Operators.NOT_IN:
                         v = v if isinstance(v, Iterable) else [v]
-                        conditions.append(key.notin_(v))
+                        if isinstance(key, tuple):
+                            conditions.append(tuple_(*key).notin_(v))
+                        else:
+                            conditions.append(key.notin_(v))
                     case Operators.HAS:
                         v = get_filters(v)
                         for condition in v:
                             conditions.append(key.has(condition))
                     case Operators.ANY:
                         v = get_filters(v)
                         conditions.append(key.any(and_(*v)))
 
     return conditions
 
 
-def get_filters(filters: _FilterType):
+def get_filters(
+    filters: _FilterType,
+    with_optional: bool = False,
+):
     if filters is None:
         return []
     if not isinstance(filters, dict):
         raise TypeError("<filters> must be type of <dict>")
 
     filters = [{x: y} for x, y in filters.items()]
 
     conditions = []
     for filter_c in filters:
         if not type(filter_c) == dict:
             continue
 
-        conditions_from_dict = get_conditions_from_dict(filter_c)
+        conditions_from_dict = get_conditions_from_dict(
+            filter_c,
+            with_optional=with_optional,
+        )
         conditions.extend(conditions_from_dict)
 
     return conditions
```

### Comparing `session-repository-0.1.7/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.8/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.7
+Version: 0.1.8
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.7.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.7/setup.py` & `session-repository-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.7"
+version = "0.1.8"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

