# Comparing `tmp/nasbio-0.1.8.tar.gz` & `tmp/nasbio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasbio-0.1.8.tar", max compression
+gzip compressed data, was "nasbio-0.1.9.tar", max compression
```

## Comparing `nasbio-0.1.8.tar` & `nasbio-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       48 2022-11-07 12:13:08.769736 nasbio-0.1.8/README.md
--rw-r--r--   0        0        0       57 2022-11-07 12:20:52.145014 nasbio-0.1.8/nasbio/__init__.py
--rw-r--r--   0        0        0      725 2022-11-07 15:18:15.267182 nasbio-0.1.8/nasbio/app/__init__.py
--rw-r--r--   0        0        0      180 2022-11-07 16:04:23.072127 nasbio-0.1.8/nasbio/celery.py
--rw-r--r--   0        0        0     2419 2022-11-07 12:20:04.842986 nasbio-0.1.8/nasbio/config.py
--rw-r--r--   0        0        0      153 2022-11-07 13:07:33.042237 nasbio-0.1.8/nasbio/db/__init__.py
--rw-r--r--   0        0        0      426 2022-11-07 13:05:36.117703 nasbio-0.1.8/nasbio/db/async_session.py
--rw-r--r--   0        0        0      866 2022-11-07 13:02:31.511539 nasbio-0.1.8/nasbio/db/base_class.py
--rw-r--r--   0        0        0      483 2022-11-07 13:05:15.707703 nasbio-0.1.8/nasbio/db/session.py
--rw-r--r--   0        0        0     6399 2022-11-10 10:54:00.058589 nasbio-0.1.8/nasbio/sqlalchemy.py
--rw-r--r--   0        0        0     5436 2022-11-16 17:30:05.678040 nasbio-0.1.8/nasbio/strawberry.py
--rw-r--r--   0        0        0      102 2022-11-16 17:25:12.726958 nasbio-0.1.8/nasbio/utils.py
--rw-r--r--   0        0        0      493 2022-11-16 17:30:05.668040 nasbio-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 nasbio-0.1.8/setup.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 nasbio-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       48 2022-11-07 12:13:08.769736 nasbio-0.1.9/README.md
+-rw-r--r--   0        0        0       57 2022-11-07 12:20:52.145014 nasbio-0.1.9/nasbio/__init__.py
+-rw-r--r--   0        0        0      725 2022-11-07 15:18:15.267182 nasbio-0.1.9/nasbio/app/__init__.py
+-rw-r--r--   0        0        0      180 2022-11-07 16:04:23.072127 nasbio-0.1.9/nasbio/celery.py
+-rw-r--r--   0        0        0     2419 2022-11-07 12:20:04.842986 nasbio-0.1.9/nasbio/config.py
+-rw-r--r--   0        0        0      153 2022-11-07 13:07:33.042237 nasbio-0.1.9/nasbio/db/__init__.py
+-rw-r--r--   0        0        0      426 2022-11-07 13:05:36.117703 nasbio-0.1.9/nasbio/db/async_session.py
+-rw-r--r--   0        0        0      866 2022-11-07 13:02:31.511539 nasbio-0.1.9/nasbio/db/base_class.py
+-rw-r--r--   0        0        0      483 2022-11-07 13:05:15.707703 nasbio-0.1.9/nasbio/db/session.py
+-rw-r--r--   0        0        0     6301 2022-11-16 18:44:08.686544 nasbio-0.1.9/nasbio/sqlalchemy.py
+-rw-r--r--   0        0        0     5436 2022-11-16 17:30:05.678040 nasbio-0.1.9/nasbio/strawberry.py
+-rw-r--r--   0        0        0      433 2022-11-16 18:33:05.104541 nasbio-0.1.9/nasbio/utils.py
+-rw-r--r--   0        0        0      493 2022-11-16 18:44:49.408051 nasbio-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 nasbio-0.1.9/setup.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 nasbio-0.1.9/PKG-INFO
```

### Comparing `nasbio-0.1.8/nasbio/app/__init__.py` & `nasbio-0.1.9/nasbio/app/__init__.py`

 * *Files identical despite different names*

### Comparing `nasbio-0.1.8/nasbio/config.py` & `nasbio-0.1.9/nasbio/config.py`

 * *Files identical despite different names*

### Comparing `nasbio-0.1.8/nasbio/db/base_class.py` & `nasbio-0.1.9/nasbio/db/base_class.py`

 * *Files identical despite different names*

### Comparing `nasbio-0.1.8/nasbio/sqlalchemy.py` & `nasbio-0.1.9/nasbio/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,30 +58,27 @@
     @classmethod
     def find_by_refseq_id(cls, refseq_id: str):
         """Find a model by its RefSeq accession ID."""
         with create_session() as db:
             return db.query(cls).filter((cls.id == refseq_id) | (cls.acc == refseq_id.split('.')[0])).first()
 
 
-# class ExternalResourceMixin:
-#     __table__: Table
-#     query: BaseQuery
-#
-#     # Keep track when records are created and updated.
-#     created_at = db.Column(db.DateTime(), index=True, default=datetime.utcnow)
-#     updated_at = db.Column(db.DateTime(), index=True, default=datetime.utcnow, onupdate=datetime.utcnow)
-#     created_by = db.Column(db.Integer, default=1)
-#     updated_by = db.Column(db.Integer)
-#
-#     @classmethod
-#     def get_by_id(cls, id: Union[int, str, List[str]]):
-#         try:
-#             return cls.query.get(id)
-#         except ValueError:
-#             return None
+class ExternalResourceMixin:
+    # Keep track when records are created and updated.
+    created_at = Column(DateTime(), index=True, default=datetime.utcnow)
+    updated_at = Column(DateTime(), index=True, default=datetime.utcnow, onupdate=datetime.utcnow)
+    created_by = Column(String)
+    updated_by = Column(String)
+
+    # @classmethod
+    # def get_by_id(cls, id: Union[int, str, List[str]]):
+    #     try:
+    #         return cls.query.get(id)
+    #     except ValueError:
+    #         return None
 
 
 # def sort_query(model: Any, query: Query, sort_keys: Dict[str, InstrumentedAttribute],
 #                order_by: Iterator[str]) -> Query:
 #     """Sort list with order_by fields, append id_ASC/id_DESC if not present."""
 #     sort_list = [order.split('_') for order in order_by]
 #     query = query.order_by(*[sort_keys[sort_key].desc() if sort_order == 'DESC' else sort_keys[sort_key]
```

### Comparing `nasbio-0.1.8/nasbio/strawberry.py` & `nasbio-0.1.9/nasbio/strawberry.py`

 * *Files identical despite different names*

### Comparing `nasbio-0.1.8/setup.py` & `nasbio-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'psycopg2-binary>=2.9.5,<3.0.0',
  'sqlalchemy>=1.4.43,<2.0.0',
  'strawberry-graphql[fastapi]>=0.140.0,<0.141.0',
  'uvicorn[standard]>=0.19.0,<0.20.0']
 
 setup_kwargs = {
     'name': 'nasbio',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# NASBio Web Services\n## Common Python Packages\n',
     'author': 'Kah Wai LIM',
     'author_email': 'kahwai222@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nasbio-0.1.8/PKG-INFO` & `nasbio-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasbio
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Kah Wai LIM
 Author-email: kahwai222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

