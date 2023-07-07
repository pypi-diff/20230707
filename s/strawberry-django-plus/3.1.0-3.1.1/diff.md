# Comparing `tmp/strawberry_django_plus-3.1.0.tar.gz` & `tmp/strawberry_django_plus-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-3.1.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.1.1.tar", max compression
```

## Comparing `strawberry_django_plus-3.1.0.tar` & `strawberry_django_plus-3.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-07-05 14:49:08.966455 strawberry_django_plus-3.1.0/LICENSE
--rw-r--r--   0        0        0     3928 2023-07-05 14:49:08.966455 strawberry_django_plus-3.1.0/README.md
--rw-r--r--   0        0        0     4208 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     3088 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5649 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5800 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    30445 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3033 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1556 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     2060 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1920 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0      896 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    24115 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14791 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26973 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1340 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    28094 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0     2532 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1027 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2423 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    17118 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0     9889 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13343 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     6604 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    16377 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      951 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 strawberry_django_plus-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-07 14:06:41.538741 strawberry_django_plus-3.1.1/LICENSE
+-rw-r--r--   0        0        0     3928 2023-07-07 14:06:41.538741 strawberry_django_plus-3.1.1/README.md
+-rw-r--r--   0        0        0     4215 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3088 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5800 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    30445 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     2060 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1920 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    24115 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26973 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28094 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2423 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    17118 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13343 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     6604 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16377 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      951 2023-07-07 14:06:41.542742 strawberry_django_plus-3.1.1/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 strawberry_django_plus-3.1.1/PKG-INFO
```

### Comparing `strawberry_django_plus-3.1.0/LICENSE` & `strawberry_django_plus-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/README.md` & `strawberry_django_plus-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/pyproject.toml` & `strawberry_django_plus-3.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "3.1.0"
+version = "3.1.1"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -30,15 +30,15 @@
 packages = [{ include = "strawberry_django_plus" }]
 include = ["strawberry_django_plus/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">= 3.2"
 strawberry-graphql = ">=0.187.5"
-strawberry-graphql-django = ">= 0.9.4"
+strawberry-graphql-django = ">=0.9.4,<0.10.0"
 typing-extensions = ">= 4.2.0"
 django-choices-field = { version = ">=2.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 codecov = "^2.1.12"
 django-types = "^0.17.0"
```

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "3.1.0"  # x-release-please-version
+__version__ = "3.1.1"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/field.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/type.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/types.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.1.1/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.1.0/PKG-INFO` & `strawberry_django_plus-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 3.1.0
+Version: 3.1.1
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: enum
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-choices-field (>=2.0) ; extra == "enum"
 Requires-Dist: strawberry-graphql (>=0.187.5)
-Requires-Dist: strawberry-graphql-django (>=0.9.4)
+Requires-Dist: strawberry-graphql-django (>=0.9.4,<0.10.0)
 Requires-Dist: typing-extensions (>=4.2.0)
 Project-URL: Documentation, https://strawberry-django-plus.readthedocs.io
 Project-URL: Repository, https://github.com/blb-ventures/strawberry-django-plus
 Description-Content-Type: text/markdown
 
 # strawberry-django-plus
```

