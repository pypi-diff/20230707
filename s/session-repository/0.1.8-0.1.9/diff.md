# Comparing `tmp/session-repository-0.1.8.tar.gz` & `tmp/session-repository-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.8.tar", last modified: Fri Jul  7 07:53:43 2023, max compression
+gzip compressed data, was "session-repository-0.1.9.tar", last modified: Fri Jul  7 08:00:41 2023, max compression
```

## Comparing `session-repository-0.1.8.tar` & `session-repository-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.742425 session-repository-0.1.8/
--rw-rw-rw-   0        0        0      599 2023-07-07 07:53:43.740239 session-repository-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.708397 session-repository-0.1.8/session_repository/
--rw-rw-rw-   0        0        0     8653 2023-07-07 07:52:17.000000 session-repository-0.1.8/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.8/session_repository/enum.py
--rw-rw-rw-   0        0        0     7777 2023-07-07 07:51:19.000000 session-repository-0.1.8/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:53:43.733922 session-repository-0.1.8/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 07:53:43.000000 session-repository-0.1.8/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 07:53:43.742925 session-repository-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-07 07:52:40.000000 session-repository-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:00:41.371751 session-repository-0.1.9/
+-rw-rw-rw-   0        0        0      599 2023-07-07 08:00:41.369668 session-repository-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 08:00:41.345565 session-repository-0.1.9/session_repository/
+-rw-rw-rw-   0        0        0     9344 2023-07-07 07:59:50.000000 session-repository-0.1.9/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.9/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7777 2023-07-07 07:51:19.000000 session-repository-0.1.9/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:00:41.365686 session-repository-0.1.9/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-07 08:00:41.000000 session-repository-0.1.9/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-07 08:00:41.000000 session-repository-0.1.9/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:00:41.000000 session-repository-0.1.9/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 08:00:41.000000 session-repository-0.1.9/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 08:00:41.000000 session-repository-0.1.9/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:00:41.372767 session-repository-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-07 08:00:24.000000 session-repository-0.1.9/setup.py
```

### Comparing `session-repository-0.1.8/PKG-INFO` & `session-repository-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.8
+Version: 0.1.9
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.8/session_repository/core.py` & `session-repository-0.1.9/session_repository/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,26 +42,40 @@
     def session_manager(self):
         return self._session_factory()
 
     def _select(
         self,
         model,
         filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         current_session: Optional[Session] = None,
     ) -> Optional[Any]:
         def _select_from_session(session: Session):
             query = session.query(model)
-            query = apply_no_load(query=query, relationship_dict=disabled_relationships)
-            query = apply_filters(query=query, filter_dict=filters)
+            query = apply_no_load(
+                query=query,
+                relationship_dict=disabled_relationships,
+            )
+            query = apply_filters(
+                query=query,
+                filter_dict=filters,
+            )
+            query = apply_filters(
+                query=query,
+                filter_dict=optional_filters,
+                with_optional=True,
+            )
             result = query.first()
 
             if self._logger is not None:
                 query_compiled = query.statement.compile(
-                    compile_kwargs={"literal_binds": self._literal_binds}
+                    compile_kwargs={
+                        "literal_binds": self._literal_binds,
+                    }
                 )
                 self._logger.info(query_compiled.string)
 
             return result
 
         if current_session is not None:
             results = _select_from_session(session=current_session)
@@ -108,15 +122,17 @@
                 limit=limit,
             )
 
             results = query.all()
 
             if self._logger is not None:
                 query_compiled = query.statement.compile(
-                    compile_kwargs={"literal_binds": self._literal_binds}
+                    compile_kwargs={
+                        "literal_binds": self._literal_binds,
+                    }
                 )
                 self._logger.info(query_compiled.string)
 
             return results
 
         if current_session is not None:
             results = _select_from_session(session=current_session)
@@ -128,14 +144,15 @@
 
     def _select_paginate(
         self,
         model,
         page: int,
         per_page: int,
         filters: Optional[_FilterType] = None,
+        optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
     ) -> Tuple[List, str]:
         def _select_from_session(session: Session):
@@ -144,14 +161,19 @@
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
@@ -164,15 +186,17 @@
                 per_page=per_page,
             )
 
             results = query.all()
 
             if self._logger is not None:
                 query_compiled = query.statement.compile(
-                    compile_kwargs={"literal_binds": self._literal_binds}
+                    compile_kwargs={
+                        "literal_binds": self._literal_binds,
+                    }
                 )
                 self._logger.info(query_compiled.string)
 
             return results, pagination
 
         if current_session is not None:
             results = _select_from_session(session=current_session)
```

### Comparing `session-repository-0.1.8/session_repository/utils.py` & `session-repository-0.1.9/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.1.8/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.9/session_repository.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.8
+Version: 0.1.9
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.8/setup.py` & `session-repository-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.8"
+version = "0.1.9"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

