# Comparing `tmp/elefantolib_fastapi-0.5.0.tar.gz` & `tmp/elefantolib_fastapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.5.0.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.6.0.tar", max compression
```

## Comparing `elefantolib_fastapi-0.5.0.tar` & `elefantolib_fastapi-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      878 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0     1018 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/connection.py
--rw-r--r--   0        0        0      878 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/depends.py
--rw-r--r--   0        0        0      934 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/exceptions.py
--rw-r--r--   0        0        0      604 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/middleware.py
--rw-r--r--   0        0        0     2039 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/pagination.py
--rw-r--r--   0        0        0      209 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      721 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      307 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/schemas.py
--rw-r--r--   0        0        0      913 2023-06-29 14:55:41.595948 elefantolib_fastapi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.5.0/setup.py
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/connection.py
+-rw-r--r--   0        0        0      878 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/depends.py
+-rw-r--r--   0        0        0      934 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/exceptions.py
+-rw-r--r--   0        0        0     1337 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/pagination.py
+-rw-r--r--   0        0        0      209 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      721 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      307 2023-07-07 15:22:26.220281 elefantolib_fastapi-0.6.0/elefantolib_fastapi/schemas.py
+-rw-r--r--   0        0        0      913 2023-07-07 15:22:44.248410 elefantolib_fastapi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.6.0/setup.py
+-rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.6.0/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.5.0/README.md` & `elefantolib_fastapi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.5.0/elefantolib_fastapi/connection.py` & `elefantolib_fastapi-0.6.0/elefantolib_fastapi/connection.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.5.0/elefantolib_fastapi/depends.py` & `elefantolib_fastapi-0.6.0/elefantolib_fastapi/depends.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.5.0/elefantolib_fastapi/exceptions.py` & `elefantolib_fastapi-0.6.0/elefantolib_fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.5.0/elefantolib_fastapi/pagination.py` & `elefantolib_fastapi-0.6.0/elefantolib_fastapi/pagination.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,39 @@
-from elefantolib_fastapi import middleware
-
 from sqlalchemy import Select, func, select
 from sqlalchemy.ext.asyncio import AsyncSession
 
 
 class PageNumberPagination:
     def __init__(self, session: AsyncSession, query: Select, page: int, page_size: int):
         self.session = session
         self.query = query
         self.page = page
         self.page_size = page_size
-        self.request = middleware.request_object.get()
-        # computed later
-        self.number_of_pages = 0
-        self.next_page = ''
-        self.previous_page = ''
-
-    def _get_next_page(self) -> str | None:
-        if self.page >= self.number_of_pages:
-            return
-
-        return str(self.request.url.include_query_params(page=self.page + 1))
-
-    def _get_previous_page(self) -> str | None:
-        if self.page == 1 or self.page > self.number_of_pages + 1:
-            return
-
-        return str(self.request.url.include_query_params(page=self.page - 1))
 
     async def get_response(self) -> dict:
         limit = self.page_size
         offset = (self.page - 1) * self.page_size
 
         query = self.query.limit(limit).offset(offset)
+        count = await self._get_total_count()
+        pages = self._get_number_of_pages(count)
 
         return {
-            'count': await self._get_total_count(),
-            'next': self._get_next_page(),
-            'previous': self._get_previous_page(),
+            'count': count,
+            'pages': pages,
             'results': [i for i in await self.session.scalars(query)],
         }
 
     def _get_number_of_pages(self, count: int) -> int:
         rest = count % self.page_size
         quotient = count // self.page_size
 
         return quotient if not rest else quotient + 1
 
     async def _get_total_count(self) -> int:
-        count = await self.session.scalar(select(func.count()).select_from(self.query.subquery()))
-        self.number_of_pages = self._get_number_of_pages(count)
-
-        return count
+        return await self.session.scalar(select(func.count()).select_from(self.query.subquery()))
 
 
 async def paginate(db_session, query: Select, page: int, page_size: int) -> dict:
     async with db_session as session:
         paginator = PageNumberPagination(session, query, page, page_size)
         return await paginator.get_response()
```

### Comparing `elefantolib_fastapi-0.5.0/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.6.0/elefantolib_fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.5.0/pyproject.toml` & `elefantolib_fastapi-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = "^0.98.0"
+fastapi = "^0.99.1"
 redis = "^4.6.0"
 elefantolib = "^0.12.1"
-sqlalchemy = "^2.0.17"
+sqlalchemy = "^2.0.18"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-flake8 = "^1.1.1"
```

### Comparing `elefantolib_fastapi-0.5.0/setup.py` & `elefantolib_fastapi-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 ['elefantolib_fastapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['elefantolib>=0.12.1,<0.13.0',
- 'fastapi>=0.98.0,<0.99.0',
+ 'fastapi>=0.99.1,<0.100.0',
  'redis>=4.6.0,<5.0.0',
- 'sqlalchemy>=2.0.17,<3.0.0']
+ 'sqlalchemy>=2.0.18,<3.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
     'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `elefantolib_fastapi-0.5.0/PKG-INFO` & `elefantolib_fastapi-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: elefantolib (>=0.12.1,<0.13.0)
-Requires-Dist: fastapi (>=0.98.0,<0.99.0)
+Requires-Dist: fastapi (>=0.99.1,<0.100.0)
 Requires-Dist: redis (>=4.6.0,<5.0.0)
-Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.18,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Elefantolib for FastAPI
 
 > **_NOTE:_**  Only for this library developers. After clone this repository you should run command:
 >
```

