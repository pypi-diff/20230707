# Comparing `tmp/fullask_rest_framework-0.6.1.tar.gz` & `tmp/fullask_rest_framework-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask_rest_framework-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fullask_rest_framework-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fullask_rest_framework-0.6.1.tar` & `fullask_rest_framework-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
--rw-r--r--   0        0        0      292 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/.editorconfig
--rw-r--r--   0        0        0     1240 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/.gitignore
--rw-r--r--   0        0        0     1070 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/LICENSE
--rw-r--r--   0        0        0     3359 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/README.md
--rw-r--r--   0        0        0      150 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/__init__.py
--rw-r--r--   0        0        0      604 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/cli.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/index.html
--rw-r--r--   0        0        0      851 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/login_form.html
--rw-r--r--   0        0        0     1146 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-r--r--   0        0        0      202 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/views.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-r--r--   0        0        0      112 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-r--r--   0        0        0      322 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-r--r--   0        0        0      628 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-r--r--   0        0        0       65 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/tests.txt
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      292 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/base_model.py
--rw-r--r--   0        0        0     1004 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/__init__.py
--rw-r--r--   0        0        0     6242 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/app_factory.py
--rw-r--r--   0        0        0      104 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/exceptions.py
--rw-r--r--   0        0        0      683 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/extensions.py
--rw-r--r--   0        0        0      206 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/microapp.py
--rw-r--r--   0        0        0       46 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/warnings.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/__init__.py
--rw-r--r--   0        0        0      157 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/base.py
--rw-r--r--   0        0        0     2821 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/crud.py
--rw-r--r--   0        0        0     5952 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/fields.py
--rw-r--r--   0        0        0      261 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/filtering.py
--rw-r--r--   0        0        0     1014 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/pagination.py
--rw-r--r--   0        0        0      644 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/sorting.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/utils/__init__.py
--rw-r--r--   0        0        0      572 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/utils/jwt.py
--rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/__init__.py
--rw-r--r--   0        0        0      346 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/filtering.py
--rw-r--r--   0        0        0      364 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/pagination.py
--rw-r--r--   0        0        0      407 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/sorting.py
--rw-r--r--   0        0        0     2267 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      317 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/setup.cfg
--rw-r--r--   0        0        0      213 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/tox.ini
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 fullask_rest_framework-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/.editorconfig
+-rw-r--r--   0        0        0     1240 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3359 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/README.md
+-rw-r--r--   0        0        0      150 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/cli.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-r--r--   0        0        0      851 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/templates/login_form.html
+-rw-r--r--   0        0        0     1146 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-r--r--   0        0        0      202 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/views.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-r--r--   0        0        0      112 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-r--r--   0        0        0      322 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-r--r--   0        0        0      628 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-r--r--   0        0        0       65 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/tests.txt
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/db/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/db/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/db/sqlalchemy/base_model.py
+-rw-r--r--   0        0        0     1004 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/db/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0      469 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/db/transaction.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/__init__.py
+-rw-r--r--   0        0        0     6075 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/app_factory.py
+-rw-r--r--   0        0        0      104 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/exceptions.py
+-rw-r--r--   0        0        0      683 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/extensions.py
+-rw-r--r--   0        0        0      206 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/microapp.py
+-rw-r--r--   0        0        0       46 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/factory/warnings.py
+-rw-r--r--   0        0        0      351 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/httptypes/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/httptypes/filtering.py
+-rw-r--r--   0        0        0      364 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/httptypes/pagination.py
+-rw-r--r--   0        0        0      407 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/httptypes/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/base.py
+-rw-r--r--   0        0        0     2319 2023-07-07 15:22:37.934840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/crud.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/mongodb/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      584 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/sqlalchemy/decorators.py
+-rw-r--r--   0        0        0     4840 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/sqlalchemy/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/fields.py
+-rw-r--r--   0        0        0      268 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/filtering.py
+-rw-r--r--   0        0        0     1034 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/pagination.py
+-rw-r--r--   0        0        0      651 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/utils/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/fullask_rest_framework/utils/jwt.py
+-rw-r--r--   0        0        0     2267 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/setup.cfg
+-rw-r--r--   0        0        0      213 2023-07-07 15:22:37.938840 fullask_rest_framework-0.7.0/tox.ini
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 fullask_rest_framework-0.7.0/PKG-INFO
```

### Comparing `fullask_rest_framework-0.6.1/.gitignore` & `fullask_rest_framework-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/LICENSE` & `fullask_rest_framework-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/README.md` & `fullask_rest_framework-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/cli.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask_rest_framework-0.7.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask_rest_framework-0.7.0/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/mixins.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/db/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/factory/app_factory.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/factory/app_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import importlib
 import inspect
-import warnings
 from types import ModuleType
 from typing import Any, Dict, List, Optional
 
 from dependency_injector.containers import Container
 from dotenv import load_dotenv
 from flask import Flask
 from flask_smorest import Api
@@ -115,18 +114,15 @@
     def _register_micro_apps(cls, smorest_api: Api) -> None:
         """
         register micro apps, with cls.MICRO_APP_CONFIG settings.
         this also does the Dependency Injection,
         with dependency_injector's DynamicContainer.
         """
         if not cls.MICRO_APP_CONFIG:
-            return warnings.warn(
-                "No routing is currently set for the application, "
-                "please set it via MICRO_APP_CONFIG."
-            )
+            return
         for micro_app_information in cls.MICRO_APP_CONFIG:
             for app_package_string, url_prefix in micro_app_information.items():
                 micro_app = next(
                     (
                         cls
                         for name, cls in importlib.import_module(
                             app_package_string
```

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/factory/extensions.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/crud.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/repositories/crud.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Generic, List, Optional
 
+from fullask_rest_framework.httptypes import FilteringRequest, SortingRequest
 from fullask_rest_framework.repositories.base import BaseRepository, T
-from fullask_rest_framework.vo.filtering import FilteringRequest
-from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
-from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class CRUDRepositoryABC(BaseRepository, ABC, Generic[T]):
     """The Base CRUD Repository class."""
 
     @abstractmethod
     def save(self, entity: T) -> T:
@@ -57,27 +55,14 @@
         """
         Read all entities.
         if no entities are found, return empty list.
         """
         pass
 
     @abstractmethod
-    def read_all_with_pagination(
-        self,
-        pagination_request: PaginationRequest,
-        sorting_request: SortingRequest,
-        filtering_request: FilteringRequest,
-    ) -> PaginationResponse[T]:
-        """
-        Read all entities with pagination.
-        if no entities are found, return empty list.
-        """
-        pass
-
-    @abstractmethod
     def read_all_by_ids(self, ids: List[int]) -> List[Optional[T]]:
         """
         Read all entities with given ids.
 
         :return: list of all entities, with given ids.
         """
         pass
```

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/fields.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/pagination.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/pagination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from marshmallow import Schema, fields, post_load
 from marshmallow.validate import Range
 
-from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
+from fullask_rest_framework.httptypes.pagination import (
+    PaginationRequest,
+    PaginationResponse,
+)
 
 
 class PaginationRequestSchema(Schema):
     page = fields.Integer(
         validate=Range(min=1),
         metadata={"description": "The page number you want to look up."},
     )
```

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/sorting.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/schemas/sorting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from flask_marshmallow import Schema  # type: ignore[import]
 from marshmallow import post_load
 
+from fullask_rest_framework.httptypes.sorting import SortingRequest
 from fullask_rest_framework.schemas import fields
-from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class SortingRequestSchema(Schema):
     sort_by = fields.Sorting(
         metadata={
             "description": "The sort condition. It must conform to the format"
             "`fieldname:sortcondition (asc or desc)`."
```

### Comparing `fullask_rest_framework-0.6.1/fullask_rest_framework/utils/jwt.py` & `fullask_rest_framework-0.7.0/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.6.1/pyproject.toml` & `fullask_rest_framework-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "docs/",
     "tests/",
     ".github/"
 ]
 
 [tool.poetry]
 name = "fullask-rest-framework"
-version = "0.6.1"
+version = "0.7.0"
 description = ""
 authors = ["tgoddessana <twicegoddessana1229@gmail.com>"]
 
 [tool.poetry.dependencies]
 pip = "*"
 python = "^3.11"
 flask = "^2.2.3"
@@ -76,15 +76,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 wheel = "^0.40.0"
 twine = "^4.0.2"
 pre-commit = "^3.3.2"
-bumpversion = "^0.6.1"
+bumpversion = "^0.7.0"
 flit = "^3.9.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
 tox = "*"
```

### Comparing `fullask_rest_framework-0.6.1/PKG-INFO` & `fullask_rest_framework-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.6.1
+Version: 0.7.0
 Summary: A fully-supported flask extension to build REST API.
 Author-email: tgoddessana <twicegoddessana1229@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.6.1 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.7.0 Summary: A
 fully-supported flask extension to build REST API. Author-email: tgoddessana
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

