# Comparing `tmp/fastapi_amis_admin-0.6.0a1.tar.gz` & `tmp/fastapi_amis_admin-0.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.6.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_amis_admin-0.6.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin-0.6.0a1.tar` & `fastapi_amis_admin-0.6.0a2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11774 2023-07-06 09:16:23.130375 fastapi_amis_admin-0.6.0a1/README.md
--rw-r--r--   0        0        0      603 2023-07-06 09:27:30.735600 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    58904 2023-07-06 03:28:47.351308 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3822 2023-04-15 02:00:42.051799 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    13378 2023-07-06 08:54:37.120798 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     1765 2023-07-06 09:24:02.534616 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   151935 2023-06-13 06:14:32.628539 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     5096 2023-07-06 03:10:47.448565 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      309 2023-07-06 09:27:57.925619 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    23900 2023-07-06 09:25:23.717472 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/_sqlalchemy.py
--rw-r--r--   0        0        0      231 2023-07-06 09:24:27.054486 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     8077 2023-07-06 03:28:47.353316 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0    13932 2023-07-06 08:54:37.165775 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1950 2023-04-06 13:53:04.589440 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     3449 2023-07-06 07:52:37.418113 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/base.pot
--rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0     2772 2023-07-06 03:28:44.286972 fastapi_amis_admin-0.6.0a1/pyproject.toml
--rw-r--r--   0        0        0    13734 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11773 2023-07-06 09:39:50.967857 fastapi_amis_admin-0.6.0a2/README.md
+-rw-r--r--   0        0        0      603 2023-07-07 13:07:25.765268 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    58253 2023-07-07 12:00:05.711251 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3488 2023-07-07 10:00:42.574847 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    13378 2023-07-06 08:54:37.120798 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     1765 2023-07-06 09:24:02.534616 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   151935 2023-06-13 06:14:32.628539 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     5096 2023-07-06 03:10:47.448565 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      309 2023-07-06 09:27:57.925619 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    23526 2023-07-07 09:32:50.000249 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlalchemy.py
+-rw-r--r--   0        0        0      419 2023-07-07 10:02:58.918305 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     8077 2023-07-06 03:28:47.353316 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0    14025 2023-07-07 11:46:10.395305 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1950 2023-04-06 13:53:04.589440 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     3985 2023-07-07 10:02:58.926300 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/base.pot
+-rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0     2772 2023-07-07 08:06:42.191567 fastapi_amis_admin-0.6.0a2/pyproject.toml
+-rw-r--r--   0        0        0    13732 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.0a2/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.6.0a1/README.md` & `fastapi_amis_admin-0.6.0a2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 # mount AdminSite instance
 site.mount_app(app)
 
 
 # create initial database table
 @app.on_event("startup")
 async def startup():
-    await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
+    await site.db.async_run_sync(Base.metadata.create_all, is_session=False)
 
 
 if __name__ == '__main__':
     import uvicorn
 
     uvicorn.run(app)
 ```
@@ -318,15 +318,16 @@
 
 - [`Amis-Admin-Theme-Editor`](https://github.com/swelcker/amis-admin-theme-editor):Theme-Editor for the fastapi-amis-admin.
   Allows to add custom css styles and to apply theme --vars change on the fly.
 - [`FastAPI-User-Auth`](https://github.com/amisadmin/fastapi_user_auth): A simple and powerful `FastAPI` user `RBAC`
   authentication and authorization library.
 - [`FastAPI-Scheduler`](https://github.com/amisadmin/fastapi_scheduler): A simple scheduled task management `FastAPI` extension
   based on `APScheduler`.
-- [`FastAPI-Config`](https://github.com/amisadmin/fastapi-config): A visual dynamic configuration management extension package based on `FastAPI-Amis-Admin`.
+- [`FastAPI-Config`](https://github.com/amisadmin/fastapi-config): A visual dynamic configuration management extension package
+  based on `FastAPI-Amis-Admin`.
 - [`FastAPI-Amis-Admin-Demo`](https://github.com/amisadmin/fastapi_amis_admin_demo): An example `FastAPI-Amis-Admin` application.
 - [`FastAPI-User-Auth-Demo`](https://github.com/amisadmin/fastapi_user_auth_demo): An example `FastAPI-User-Auth` application.
 
 ## License
 
 - According to the `Apache2.0` protocol, `fastapi-amis-admin` is free and open source. It can be used for commercial for
   free, but please clearly display copyright information about `FastAPI-Amis-Admin` on the display interface.
```

#### html2text {}

```diff
@@ -86,15 +86,15 @@
 import Settings from fastapi_amis_admin.admin.site import AdminSite from
 fastapi_amis_admin.admin import admin # create FastAPI application app =
 FastAPI() # create AdminSite instance site = AdminSite(settings=Settings
 (database_url_async='sqlite+aiosqlite:///amisadmin.db')) # register ModelAdmin
 @site.register_admin class CategoryAdmin(admin.ModelAdmin): page_schema =
 'Category' # set model model = Category # mount AdminSite instance
 site.mount_app(app) # create initial database table @app.on_event("startup")
-async def startup(): await site.db.async_run_sync(SQLModel.metadata.create_all,
+async def startup(): await site.db.async_run_sync(Base.metadata.create_all,
 is_session=False) if __name__ == '__main__': import uvicorn uvicorn.run(app)
 ``` ## FormAdmin Example ```python from typing import Any from fastapi import
 FastAPI from pydantic import BaseModel from starlette.requests import Request
 from fastapi_amis_admin.amis.components import Form from
 fastapi_amis_admin.admin import admin from fastapi_amis_admin.admin.settings
 import Settings from fastapi_amis_admin.admin.site import AdminSite from
 fastapi_amis_admin.crud.schema import BaseApiOut from
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/__init__.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0a1"
+__version__ = "0.6.0a2"
 __url__ = "https://github.com/amisadmin/fastapi_amis_admin"
 
 import gettext
 import os
 
 from .utils.translation import i18n
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-from fastapi import Body, Depends, FastAPI, HTTPException, Query, Request
+from fastapi import Body, Depends, FastAPI, HTTPException, Request
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from pydantic.utils import deep_update
 from sqlalchemy import Column, Table, delete, insert
 from sqlalchemy.orm import InstrumentedAttribute, RelationshipProperty
 from sqlalchemy.sql.elements import Label
 from sqlalchemy.util import md5_hex
@@ -70,14 +70,15 @@
 from fastapi_amis_admin.crud.parser import (
     SqlaField,
     TableModelParser,
     get_python_type_parse,
 )
 from fastapi_amis_admin.crud.schema import BaseApiOut, CrudEnum, Paginator
 from fastapi_amis_admin.crud.utils import (
+    IdStrQuery,
     SqlalchemyDatabase,
     get_engine_db,
     parser_str_set_list,
     schema_create_by_schema,
 )
 from fastapi_amis_admin.utils.functools import cached_property
 from fastapi_amis_admin.utils.translation import i18n as _
@@ -135,22 +136,16 @@
             )
         return None
 
     @property
     def route_delete(self):
         async def route(
             request: Request,
+            link_id: IdStrQuery,
             item_id: List[str] = Depends(self.pk_admin.filtered_item_id),
-            link_id: str = Query(
-                ...,
-                min_length=1,
-                title="link_id",
-                example="1,2,3",
-                description="link model Primary key or list of link model primary keys",
-            ),
         ):
             if not await self.pk_admin.has_update_permission(request, item_id, None):
                 return self.pk_admin.error_no_router_permission(request)
             stmt = (
                 delete(self.link_model)
                 .where(self.link_col.in_(list(map(get_python_type_parse(self.link_col), parser_str_set_list(link_id)))))
                 .where(self.item_col.in_(list(map(get_python_type_parse(self.item_col), item_id))))
@@ -160,33 +155,24 @@
 
         return route
 
     @property
     def route_create(self):
         async def route(
             request: Request,
+            link_id: IdStrQuery,
             item_id: List[str] = Depends(self.pk_admin.filtered_item_id),
-            link_id: str = Query(
-                ...,
-                min_length=1,
-                title="link_id",
-                example="1,2,3",
-                description="link model Primary key or list of link model primary keys",
-            ),
         ):
             if not await self.pk_admin.has_update_permission(request, item_id, None):
                 return self.pk_admin.error_no_router_permission(request)
             values = []
             for item in map(get_python_type_parse(self.item_col), item_id):
                 values.extend(
                     {self.link_col.key: link, self.item_col.key: item}
-                    for link in map(
-                        get_python_type_parse(self.link_col),
-                        parser_str_set_list(link_id),
-                    )
+                    for link in map(get_python_type_parse(self.link_col), parser_str_set_list(link_id))
                 )
             stmt = insert(self.link_model).values(values)
             try:
                 result = await self.pk_admin.db.async_execute(stmt)
             except Exception as error:
                 return self.pk_admin.error_execute_sql(request=request, error=error)
             return BaseApiOut(data=result.rowcount)  # type: ignore
@@ -204,15 +190,16 @@
             required=False,
             modalMode="dialog",
             size="full",
             pickerSchema={"&": "${body}"},
             source={
                 "method": "post",
                 "data": "${body.api.data}",
-                "url": "${body.api.url}&link_model=" + self.pk_admin.model.__table__.name + "&link_item_id=${api.qsOptions.id}",
+                "url": "${body.api.url}&link_model=" + self.pk_admin.model.__table__.name + "&op=in_&link_item_id=${"
+                "api.qsOptions.id}",
             },
         )
         adaptor = None
         if await self.pk_admin.has_update_permission(request, None, None):
             button_create = ActionType.Ajax(
                 actionType="ajax",
                 label=_("Add Association"),
@@ -239,17 +226,17 @@
                         schemaApi=AmisAPI(
                             method="post",
                             url=url,
                             data={},
                             cache=300000,
                             responseData={
                                 "&": "${body}",
-                                "api.url": "${body.api.url}&link_model="
+                                "api.url": "${body.api.url}&op=not_in&link_model="
                                 + self.pk_admin.model.__table__.name
-                                + "&link_item_id=!${api.qsOptions.id}",
+                                + "&link_item_id=${api.qsOptions.id}",
                             },
                             qsOptions={"id": f"${self.pk_admin.pk_name}"},
                             adaptor=adaptor,
                         )
                     ),
                 ),
             )
@@ -1231,23 +1218,18 @@
     @property
     def route_submit(self):
         default = ... if self.schema else None
         schema = self.schema or Any
 
         async def route(
             request: Request,
+            item_id: List[str] = Depends(self.admin.filtered_item_id),
             data: schema = Body(default=default),  # type:ignore
-            item_id: str = Query(
-                None,
-                title="item_id",
-                example="1,2,3",
-                description="Primary key or list of primary keys",
-            ),
         ):
-            return await self.handle(request, parser_str_set_list(set_str=item_id), data)
+            return await self.handle(request, item_id, data)
 
         return route
 
 
 class AdminGroup(PageSchemaAdmin):
     def __init__(self, app: "AdminApp") -> None:
         super().__init__(app)
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 import logging
 import traceback
 from typing import Union
 
 from fastapi import FastAPI
 from fastapi.exceptions import RequestValidationError
+from fastapi.utils import is_body_allowed_for_status_code
 from pydantic import ValidationError
 from starlette.exceptions import HTTPException
 from starlette.requests import ClientDisconnect, Request
 from starlette.responses import Response
 from starlette.status import (
     HTTP_417_EXPECTATION_FAILED,
     HTTP_422_UNPROCESSABLE_ENTITY,
     HTTP_500_INTERNAL_SERVER_ERROR,
 )
 
 from fastapi_amis_admin.crud import BaseApiOut
 
 try:
-    from fastapi.utils import is_body_allowed_for_status_code
-except ImportError:  # fastapi < 0.83.0
-
-    def is_body_allowed_for_status_code(status_code: Union[int, str, None]) -> bool:
-        if status_code is None:
-            return True
-        current_status_code = int(status_code)
-        return not (current_status_code < 200 or current_status_code in {204, 304})
-
-
-try:
     import ujson
     from fastapi.responses import UJSONResponse as JSONResponse
 except ImportError:
     ujson = None
     from fastapi.responses import JSONResponse
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/parser.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/settings.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/components.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/constants.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/app.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/templates/page.html` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/templates/page.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/amis/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/README.md` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/_sqlalchemy.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/_sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,27 @@
     Pattern,
     Tuple,
     Type,
     Union,
 )
 from uuid import UUID
 
-from fastapi import APIRouter, Body, Depends, Query
+from fastapi import APIRouter, Body, Depends
 from fastapi.encoders import DictIntStrAny, SetIntStr
 from pydantic import EmailStr, Extra, IPvAnyAddress, Json
 from pydantic.fields import ModelField
 from pydantic.utils import ValueItems
 from sqlalchemy import Column, Table, func
 from sqlalchemy.engine import Result
 from sqlalchemy.future import select
 from sqlalchemy.orm import InstrumentedAttribute, Session, object_session
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import BinaryExpression, Label, UnaryExpression
 from starlette.requests import Request
+from typing_extensions import Literal
 
 try:
     from functools import cached_property
 except ImportError:
     from sqlalchemy.util.langhelpers import memoized_property as cached_property
 
 from .base import (
@@ -51,17 +52,18 @@
     TableModelT,
     get_modelfield_by_alias,
     get_python_type_parse,
     parse_obj_to_schema,
 )
 from .schema import BaseApiOut, ItemListSchema
 from .utils import (
+    IdStrQuery,
+    ItemIdListDepend,
     SqlalchemyDatabase,
     get_engine_db,
-    parser_item_id,
     parser_str_set_list,
     schema_create_by_modelfield,
 )
 
 sql_operator_pattern: Pattern = re.compile(r"^\[(=|<=|<|>|>=|!|!=|<>|\*|!\*|~|!~|-)]")
 sql_operator_map: Dict[str, str] = {
     "=": "__eq__",
@@ -168,43 +170,33 @@
             select_maker = self.get_select
         return select_maker
 
     async def get_link_clause(
         self,
         request: Request,
         link_model: str = None,
-        link_item_id: Union[int, str] = Query(
-            None,
-            title="pk",
-            example="1,2,3",
-            description="Link Model Primary key or list of primary keys",
-        ),
+        link_item_id: IdStrQuery = None,
+        op: Literal["in_", "not_in", None] = None,
     ) -> Optional[Any]:
         if link_model and link_item_id:
             result = self.link_models.get(link_model)
             if not result:
                 return None
             table, pk_col, link_col = result
             if table is not None:
-                op = "in_"
-                if isinstance(link_item_id, str) and link_item_id.startswith("!"):
-                    op = "not_in"
-                    link_item_id = link_item_id[1:]
-                    if not link_item_id:
-                        return None
                 link_item_id = list(
                     map(
                         get_python_type_parse(link_col),
                         parser_str_set_list(link_item_id),
                     )
                 )
-                if op == "in_":
-                    return self.pk.in_(select(pk_col).where(link_col.in_(link_item_id)))
-                elif op == "not_in":
+                if op == "not_in":
                     return self.pk.not_in(select(pk_col).where(link_col.in_(link_item_id)))
+                else:
+                    return self.pk.in_(select(pk_col).where(link_col.in_(link_item_id)))
         return None
 
     @staticmethod
     def _parser_query_value(
         value: Any, operator: str = "__eq__", python_type_parse: Callable = str
     ) -> Tuple[Optional[str], Union[tuple, None]]:
         if isinstance(value, str):
@@ -458,15 +450,15 @@
         return data
 
     @property
     def filtered_item_id(self) -> Callable:
         """Filter the id of the data that the user has permission to operate on."""
 
         async def depend(
-            item_id: List[str] = Depends(parser_item_id),
+            item_id: ItemIdListDepend,
             stmt: Select = Depends(self._select_maker),
         ):
             filtered_id = await self.db.async_scalars(stmt.where(self.pk.in_(item_id)).with_only_columns(self.pk))
             return filtered_id.all()
 
         return depend
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/parser.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,18 @@
         fields = self.filter_insfield(fields, save_class=save_class)
         modelfields = [self.get_modelfield(ins, clone=True) for ins in fields]
         # Filter out any None values or out excluded fields
         modelfields = [field for field in modelfields if field and field.name not in exclude]
         return modelfields
 
 
+SQLModelFieldParser = TableModelParser
+"""Deprecated, use TableModelParser instead."""
+
+
 @lru_cache()
 def get_python_type_parse(field: Union[InstrumentedAttribute, Column, Label]) -> Callable:
     try:
         python_type = field.expression.type.python_type
         if issubclass(python_type, datetime.date):
             if issubclass(python_type, datetime.datetime):
                 return parse_datetime
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/crud/utils.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/crud/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import warnings
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Set, Type, Union
 
-from fastapi.params import Path
+from fastapi import Depends, Path, Query
 from fastapi.utils import create_cloned_field
 from pydantic import BaseConfig, BaseModel, Extra
 from pydantic.fields import ModelField
 from pydantic.main import ModelMetaclass
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy_database import AsyncDatabase, Database
+from typing_extensions import Annotated
 
 from .schema import BaseApiSchema
 
 SqlalchemyDatabase = Union[Engine, AsyncEngine, Database, AsyncDatabase]
 
 
 def validator_skip_blank(cls, v, config: BaseConfig, field: ModelField, *args, **kwargs):
@@ -67,32 +69,51 @@
             else:
                 modelfield.pre_validators.insert(0, validator_skip_blank)
         namespaces["__fields__"][modelfield.name] = modelfield
         namespaces["__annotations__"][modelfield.name] = modelfield.type_
     return ModelMetaclass(schema_name, (BaseApiSchema,), namespaces)
 
 
-def parser_str_set_list(set_str: Union[int, str]) -> List[str]:
-    if isinstance(set_str, int):
-        return [str(set_str)]
-    elif not isinstance(set_str, str):
+IdStrQuery = Annotated[
+    str,
+    Query(
+        title="ids",
+        example="1,2,3",
+        description="Primary key or list of primary keys",
+    ),
+]
+
+
+def parser_str_set_list(item_id: Union[int, str]) -> List[str]:
+    if isinstance(item_id, int):
+        return [str(item_id)]
+    elif not isinstance(item_id, str):
         return []
-    return list(set(set_str.split(",")))
+    return list(set(item_id.split(",")))
+
+
+ItemIdListDepend = Annotated[List[str], Depends(parser_str_set_list)]
 
 
 def parser_item_id(
     item_id: str = Path(
         ...,
         min_length=1,
         title="pk",
         example="1,2,3",
         description="Primary key or list of primary keys",
     )
 ) -> List[str]:
-    return parser_str_set_list(set_str=item_id)
+    """Deprecated, use ItemIdListDepend and parser_str_set_list instead"""
+    warnings.warn(
+        "Deprecated, use ItemIdListDepend and parser_str_set_list instead",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return parser_str_set_list(item_id)
 
 
 def get_engine_db(engine: SqlalchemyDatabase) -> Union[Database, AsyncDatabase]:
     if isinstance(engine, (Database, AsyncDatabase)):
         return engine
     if isinstance(engine, Engine):
         return Database(engine)
```

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/base.pot` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/base.pot`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/models/fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.6.0a2/fastapi_amis_admin/utils/translation.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.0a1/pyproject.toml` & `fastapi_amis_admin-0.6.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "fastapi>=0.68.0",
+    "fastapi>=0.97.0",
     "sqlalchemy>=1.4.0",
     "python-multipart>=0.0.5",
     "sqlalchemy-database>=0.1.0,<0.2.0",
     "aiofiles>=0.17.0",
 ]
```

### Comparing `fastapi_amis_admin-0.6.0a1/PKG-INFO` & `fastapi_amis_admin-0.6.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
 Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
@@ -14,15 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi>=0.68.0
+Requires-Dist: fastapi>=0.97.0
 Requires-Dist: sqlalchemy>=1.4.0
 Requires-Dist: python-multipart>=0.0.5
 Requires-Dist: sqlalchemy-database>=0.1.0,<0.2.0
 Requires-Dist: aiofiles>=0.17.0
 Requires-Dist: fastapi-amis-admin-cli>=0.1.3,<0.2.0 ; extra == "cli"
 Requires-Dist: pre-commit>=2.20.0 ; extra == "dev"
 Requires-Dist: ruff>=0.0.261 ; extra == "dev"
@@ -271,15 +271,15 @@
 # mount AdminSite instance
 site.mount_app(app)
 
 
 # create initial database table
 @app.on_event("startup")
 async def startup():
-    await site.db.async_run_sync(SQLModel.metadata.create_all, is_session=False)
+    await site.db.async_run_sync(Base.metadata.create_all, is_session=False)
 
 
 if __name__ == '__main__':
     import uvicorn
 
     uvicorn.run(app)
 ```
@@ -366,15 +366,16 @@
 
 - [`Amis-Admin-Theme-Editor`](https://github.com/swelcker/amis-admin-theme-editor):Theme-Editor for the fastapi-amis-admin.
   Allows to add custom css styles and to apply theme --vars change on the fly.
 - [`FastAPI-User-Auth`](https://github.com/amisadmin/fastapi_user_auth): A simple and powerful `FastAPI` user `RBAC`
   authentication and authorization library.
 - [`FastAPI-Scheduler`](https://github.com/amisadmin/fastapi_scheduler): A simple scheduled task management `FastAPI` extension
   based on `APScheduler`.
-- [`FastAPI-Config`](https://github.com/amisadmin/fastapi-config): A visual dynamic configuration management extension package based on `FastAPI-Amis-Admin`.
+- [`FastAPI-Config`](https://github.com/amisadmin/fastapi-config): A visual dynamic configuration management extension package
+  based on `FastAPI-Amis-Admin`.
 - [`FastAPI-Amis-Admin-Demo`](https://github.com/amisadmin/fastapi_amis_admin_demo): An example `FastAPI-Amis-Admin` application.
 - [`FastAPI-User-Auth-Demo`](https://github.com/amisadmin/fastapi_user_auth_demo): An example `FastAPI-User-Auth` application.
 
 ## License
 
 - According to the `Apache2.0` protocol, `fastapi-amis-admin` is free and open source. It can be used for commercial for
   free, but please clearly display copyright information about `FastAPI-Amis-Admin` on the display interface.
```

