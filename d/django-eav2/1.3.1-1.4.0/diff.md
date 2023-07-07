# Comparing `tmp/django_eav2-1.3.1.tar.gz` & `tmp/django_eav2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eav2-1.3.1.tar", max compression
+gzip compressed data, was "django_eav2-1.4.0.tar", max compression
```

## Comparing `django_eav2-1.3.1.tar` & `django_eav2-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      844 2023-02-22 17:39:25.125577 django_eav2-1.3.1/LICENSE
--rw-r--r--   0        0        0    10157 2023-02-22 17:39:25.125577 django_eav2-1.3.1/README.md
--rw-r--r--   0        0        0      229 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/__init__.py
--rw-r--r--   0        0        0     3184 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/admin.py
--rw-r--r--   0        0        0      683 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/decorators.py
--rw-r--r--   0        0        0       54 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/exceptions.py
--rw-r--r--   0        0        0     2378 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/fields.py
--rw-r--r--   0        0        0     5187 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/forms.py
--rw-r--r--   0        0        0     4608 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5523 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4273 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5715 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/logic/__init__.py
--rw-r--r--   0        0        0      371 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/logic/entity_pk.py
--rw-r--r--   0        0        0      695 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/logic/slug.py
--rw-r--r--   0        0        0     1561 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/managers.py
--rw-r--r--   0        0        0     7597 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0001_initial.py
--rw-r--r--   0        0        0      469 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0002_add_entity_ct_field.py
--rw-r--r--   0        0        0     1250 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0003_auto_20210404_2209.py
--rw-r--r--   0        0        0      393 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0004_alter_value_value_bool.py
--rw-r--r--   0        0        0     1102 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0005_auto_20210510_1305.py
--rw-r--r--   0        0        0      559 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0006_add_entity_uuid.py
--rw-r--r--   0        0        0      395 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0007_alter_value_value_int.py
--rw-r--r--   0        0        0      514 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0008_use_native_slugfield.py
--rw-r--r--   0        0        0     5326 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/0009_enchance_naming.py
--rw-r--r--   0        0        0        0 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/migrations/__init__.py
--rw-r--r--   0        0        0    24634 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/models.py
--rw-r--r--   0        0        0    13067 2023-02-22 17:39:25.125577 django_eav2-1.3.1/eav/queryset.py
--rw-r--r--   0        0        0     7206 2023-02-22 17:39:25.129577 django_eav2-1.3.1/eav/registry.py
--rw-r--r--   0        0        0     3103 2023-02-22 17:39:25.129577 django_eav2-1.3.1/eav/validators.py
--rw-r--r--   0        0        0     1348 2023-02-22 17:39:25.129577 django_eav2-1.3.1/eav/widgets.py
--rw-r--r--   0        0        0     2046 2023-02-22 17:39:25.129577 django_eav2-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    11345 1970-01-01 00:00:00.000000 django_eav2-1.3.1/setup.py
--rw-r--r--   0        0        0    11772 1970-01-01 00:00:00.000000 django_eav2-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      844 2023-07-07 20:15:43.589037 django_eav2-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10157 2023-07-07 20:15:43.589037 django_eav2-1.4.0/README.md
+-rw-r--r--   0        0        0      229 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/admin.py
+-rw-r--r--   0        0        0      683 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/decorators.py
+-rw-r--r--   0        0        0       54 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/exceptions.py
+-rw-r--r--   0        0        0     2378 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/fields.py
+-rw-r--r--   0        0        0     5187 2023-07-07 20:15:43.589037 django_eav2-1.4.0/eav/forms.py
+-rw-r--r--   0        0        0     6113 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4608 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5523 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4273 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5715 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/logic/__init__.py
+-rw-r--r--   0        0        0      371 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/logic/entity_pk.py
+-rw-r--r--   0        0        0      695 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/logic/slug.py
+-rw-r--r--   0        0        0     1561 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/managers.py
+-rw-r--r--   0        0        0     7597 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0001_initial.py
+-rw-r--r--   0        0        0      469 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0002_add_entity_ct_field.py
+-rw-r--r--   0        0        0     1250 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0003_auto_20210404_2209.py
+-rw-r--r--   0        0        0      393 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0004_alter_value_value_bool.py
+-rw-r--r--   0        0        0     1102 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0005_auto_20210510_1305.py
+-rw-r--r--   0        0        0      559 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0006_add_entity_uuid.py
+-rw-r--r--   0        0        0      395 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0007_alter_value_value_int.py
+-rw-r--r--   0        0        0      514 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0008_use_native_slugfield.py
+-rw-r--r--   0        0        0     5326 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/0009_enchance_naming.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/migrations/__init__.py
+-rw-r--r--   0        0        0    24634 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/models.py
+-rw-r--r--   0        0        0    13067 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/queryset.py
+-rw-r--r--   0        0        0     7206 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/registry.py
+-rw-r--r--   0        0        0     3103 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/validators.py
+-rw-r--r--   0        0        0     1348 2023-07-07 20:15:43.593037 django_eav2-1.4.0/eav/widgets.py
+-rw-r--r--   0        0        0     2274 2023-07-07 20:15:43.593037 django_eav2-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 django_eav2-1.4.0/PKG-INFO
```

### Comparing `django_eav2-1.3.1/LICENSE` & `django_eav2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/README.md` & `django_eav2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/admin.py` & `django_eav2-1.4.0/eav/admin.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/decorators.py` & `django_eav2-1.4.0/eav/decorators.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/fields.py` & `django_eav2-1.4.0/eav/fields.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/forms.py` & `django_eav2-1.4.0/eav/forms.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/locale/ru/LC_MESSAGES/django.mo` & `django_eav2-1.4.0/eav/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/locale/ru/LC_MESSAGES/django.po` & `django_eav2-1.4.0/eav/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_eav2-1.4.0/eav/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/locale/zh_Hans/LC_MESSAGES/django.po` & `django_eav2-1.4.0/eav/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/logic/slug.py` & `django_eav2-1.4.0/eav/logic/slug.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/managers.py` & `django_eav2-1.4.0/eav/managers.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0001_initial.py` & `django_eav2-1.4.0/eav/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0003_auto_20210404_2209.py` & `django_eav2-1.4.0/eav/migrations/0003_auto_20210404_2209.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0005_auto_20210510_1305.py` & `django_eav2-1.4.0/eav/migrations/0005_auto_20210510_1305.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0006_add_entity_uuid.py` & `django_eav2-1.4.0/eav/migrations/0006_add_entity_uuid.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0008_use_native_slugfield.py` & `django_eav2-1.4.0/eav/migrations/0008_use_native_slugfield.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/migrations/0009_enchance_naming.py` & `django_eav2-1.4.0/eav/migrations/0009_enchance_naming.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/models.py` & `django_eav2-1.4.0/eav/models.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/queryset.py` & `django_eav2-1.4.0/eav/queryset.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/registry.py` & `django_eav2-1.4.0/eav/registry.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/validators.py` & `django_eav2-1.4.0/eav/validators.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/eav/widgets.py` & `django_eav2-1.4.0/eav/widgets.py`

 * *Files identical despite different names*

### Comparing `django_eav2-1.3.1/pyproject.toml` & `django_eav2-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 skip-string-normalization = true
 include = '\.pyi?$'
 
 
 [tool.poetry]
 name = "django-eav2"
 description = "Entity-Attribute-Value storage for Django"
-version = "1.3.1"
+version = "1.4.0"
 license = "GNU Lesser General Public License (LGPL), Version 3"
 packages = [
   { include = "eav" }
 ]
 
 
 authors = [
@@ -48,43 +48,53 @@
   "Programming Language :: Python",
   "Topic :: Database",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 
+[tool.semantic_release]
+version_variable = [
+    "pyproject.toml:version"
+]
+branch = "master"
+upload_to_pypi = false
+upload_to_release = false
+build_command = "pip install poetry && poetry build"
+
 [tool.poetry.dependencies]
 python = "^3.8"
-django = ">=3.2, <4.2"
+django = ">=3.2,<4.3"
 
 # Docs extra:
 sphinx = { version = ">=5,<7", optional = true }
 sphinx-autodoc-typehints = { version = "^1.12", optional = true }
 m2r2 = { version = "^0.3", optional = true }
 tomlkit = { version = "^0.11", optional = true }
 sphinx-rtd-theme = { version = "^1.0.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.0"
+mypy = "^1.4"
 
 wemake-python-styleguide = "^0.17"
 flake8-pytest-style = "^1.7"
-nitpick = "^0.32"
+nitpick = "^0.33"
 black = "^22.12"
 
 safety = "^2.3"
 
 pytest = "^6.2"
-pytest-cov = "^4.0"
+pytest-cov = "^4.1"
 pytest-randomly = "^3.12"
 pytest-pythonpath = "^0.7.4"
 pytest-django = "^4.5.2"
-hypothesis = "^6.68.2"
+hypothesis = "^6.80.1"
 
 doc8 = "^0.11.2"
 
 [tool.poetry.extras]
 docs = [
   "sphinx",
   "sphinx-autodoc-typehints",
```

### Comparing `django_eav2-1.3.1/setup.py` & `django_eav2-1.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,202 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-eav2
+Version: 1.4.0
+Summary: Entity-Attribute-Value storage for Django
+Home-page: https://github.com/jazzband/django-eav2
+License: GNU Lesser General Public License (LGPL), Version 3
+Keywords: django,django-eav2,database,eav,sql
+Author: Mauro Lizaur
+Author-email: mauro@sdf.org
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs
+Requires-Dist: django (>=3.2,<4.3)
+Requires-Dist: m2r2 (>=0.3,<0.4) ; extra == "docs"
+Requires-Dist: sphinx (>=5,<7) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.12,<2.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
+Requires-Dist: tomlkit (>=0.11,<0.12) ; extra == "docs"
+Project-URL: Repository, https://github.com/jazzband/django-eav2
+Description-Content-Type: text/markdown
 
-packages = \
-['eav', 'eav.logic', 'eav.migrations']
+[![Build Status](https://github.com/jazzband/django-eav2/actions/workflows/test.yml/badge.svg)](https://github.com/jazzband/django-eav2/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/jazzband/django-eav2/branch/master/graph/badge.svg?token=BJk3zS22BS)](https://codecov.io/gh/jazzband/django-eav2)
+[![Python Version](https://img.shields.io/pypi/pyversions/django-eav2.svg)](https://pypi.org/project/django-eav2/)
+[![Django Version](https://img.shields.io/pypi/djversions/django-eav2.svg?color=green)](https://pypi.org/project/django-eav2/)
+[![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)
 
-package_data = \
-{'': ['*'], 'eav': ['locale/ru/LC_MESSAGES/*', 'locale/zh_Hans/LC_MESSAGES/*']}
+## Django EAV 2 - Entity-Attribute-Value storage for Django
 
-install_requires = \
-['django>=3.2,<4.2']
-
-extras_require = \
-{'docs': ['sphinx>=5,<7',
-          'sphinx-autodoc-typehints>=1.12,<2.0',
-          'm2r2>=0.3,<0.4',
-          'tomlkit>=0.11,<0.12',
-          'sphinx-rtd-theme>=1.0.0,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'django-eav2',
-    'version': '1.3.1',
-    'description': 'Entity-Attribute-Value storage for Django',
-    'long_description': '[![Build Status](https://github.com/jazzband/django-eav2/actions/workflows/test.yml/badge.svg)](https://github.com/jazzband/django-eav2/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/jazzband/django-eav2/branch/master/graph/badge.svg?token=BJk3zS22BS)](https://codecov.io/gh/jazzband/django-eav2)\n[![Python Version](https://img.shields.io/pypi/pyversions/django-eav2.svg)](https://pypi.org/project/django-eav2/)\n[![Django Version](https://img.shields.io/pypi/djversions/django-eav2.svg?color=green)](https://pypi.org/project/django-eav2/)\n[![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)\n\n## Django EAV 2 - Entity-Attribute-Value storage for Django\n\nDjango EAV 2 is a fork of django-eav (which itself was derived from eav-django).\nYou can find documentation <a href="https://django-eav2.rtfd.io">here</a>.\n\n## What is EAV anyway?\n\n> Entity–attribute–value model (EAV) is a data model to encode, in a space-efficient manner, entities where the number of attributes (properties, parameters) that can be used to describe them is potentially vast, but the number that will actually apply to a given entity is relatively modest. Such entities correspond to the mathematical notion of a sparse matrix. (Wikipedia)\n\nData in EAV is stored as a 3-tuple (typically corresponding to three distinct tables):\n\n- The entity: the item being described, e.g. `Person(name=\'Mike\')`.\n- The attribute: often a foreign key into a table of attributes, e.g. `Attribute(slug=\'height\', datatype=FLOAT)`.\n- The value of the attribute, with links both an attribute and an entity, e.g. `Value(value_float=15.5, person=mike, attr=height)`.\n\nEntities in **django-eav2** are your typical Django model instances. Attributes (name and type) are stored in their own table, which makes it easy to manipulate the list of available attributes in the system. Values are an intermediate table between attributes and entities, each instance holding a single value.\nThis implementation also makes it easy to edit attributes in Django Admin and form instances.\n\nYou will find detailed description of the EAV here:\n\n- [Wikipedia - Entity–attribute–value model](https://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model)\n\n## EAV - The Good, the Bad or the Ugly?\n\nEAV is a trade-off between flexibility and complexity. As such, it should not be thought of as either an amelioration pattern, nor an anti-pattern. It is more of a [gray pattern](https://wiki.c2.com/?GreyPattern) - it exists in some context, to solve certain set of problems. When used appropriately, it can introduce great flexibility, cut prototyping time or deacrease complexity. When used carelessly, however, it can complicate database schema, degrade the performance and make maintainance hard. **As with every tool, it should not be overused.** In the following paragraphs we briefly discuss the pros, the cons and pointers to keep in mind when using EAV.\n\n### When to use EAV?\n\nOriginally, EAV was introduced to workaround a problem which cannot be easily solved within relational model. In order to achieve this, EAV bypasses normal schema restrictions. Some refer to this as an example of the [inner-platform effect](https://en.wikipedia.org/wiki/Inner-platform_effect#Examples). Naturally, in such scenarios RDMS resources cannot be used efficiently.\n\nTypical application of the EAV model sets to solve the problem of sparse data with a large number of applicable attributes, but only a small fraction that applies to a given entity that may not be known beforehand. Consider the classic example:\n\n> A problem that data modelers commonly encounter in the biomedical domain is organizing and storing highly diverse and heterogeneous data. For example, a single patient may have thousands of applicable descriptive parameters, all of which need to be easily accessible in an electronic patient record system. These requirements pose significant modeling and implementation challenges. [1]\n\nAnd:\n\n> [...] what do you do when you have customers that demand real-time, on-demand addition of attributes that they want to store? In one of the systems I manage, our customers wanted to do exactly this. Since we run a SaaS (software as a service) application, we have many customers across several different industries, who in turn want to use our system to store different types of information about _their_ customers. A salon chain might want to record facts such as \'hair color,\' \'hair type,\' and \'haircut frequency\'; while an investment company might want to record facts such as \'portfolio name,\' \'last portfolio adjustment date,\' and \'current portfolio balance.\' [2]\n\nIn both of these problems we have to deal with sparse and heterogeneous properties that apply only to potentially different subsets of particular entities. Applying EAV to a sub-schema of the database allows to model the desired behaviour. Traditional solution would involves wide tables with many columns storing NULL values for attributes that don\'t apply to an entity.\n\nVery common use case for EAV are custom product attributes in E-commerce implementations, such as Magento. [3]\n\nAs a rule of thumb, EAV can be used when:\n\n- Model attributes are to be added and removed by end users (or are unknowable in some different way). EAV supports these without ALTER TABLE statements and allows the attributes to be strongly typed and easily searchable.\n- There will be many attributes and values are sparse, in contrast to having tables with mostly-null columns.\n- The data is highly dynamic/volatile/vulnerable to change. This problem is present in the second example given above. Other example would be rapidly evolving system, such as a prototype with constantly changing requirements.\n- We want to store meta-data or supporting information, e.g. to customize system\'s behavior.\n- Numerous classes of data need to be represented, each class has a limited number of attributes, but the number of instances of each class is very small.\n- We want to minimise programmer\'s input when changing the data model.\n\nFor more throughout discussion on the appriopriate use-cases see:\n\n1. [Wikipedia - Scenarios that are appropriate for EAV modeling](https://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model#Scenarios_that_are_appropriate_for_EAV_modeling)\n2. [StackOverflow - Entity Attribute Value Database vs. strict Relational Model E-commerce](https://stackoverflow.com/questions/870808/entity-attribute-value-database-vs-strict-relational-model-ecommerce)\n3. [WikiWikiWeb - Generic Data Model](https://wiki.c2.com/?GenericDataModel)\n\n## When to avoid it?\n\nAs we outlined in the opening section, EAV is a trade-off. It should not be used when:\n\n##### 1. System is performance critical\n\n> Attribute-centric query is inherently more difficult when data are stored in EAV form than when they are stored conventionally. [4]\n\nIn general, the more structured your data model, the more efficiently you can deal with it. Therefore, loose data storage such as EAV has obvious trade-off in performance. Specifically, application of the EAV model makes performing JOINs on tables more complicated.\n\n##### 2. Low complexity/low maintenance cost is of priority\n\nEAV complicates data model by splitting information across tables. This increases conceptual complexity as well as SQL statements required to query the data. In consequence, optimization in one area that also makes the system harder to understand and maintain.\n\nHowever, it is important to note that:\n\n> An EAV design should be employed only for that sub-schema of a database where sparse attributes need to be modeled: even here, they need to be supported by third normal form metadata tables. There are relatively few database-design problems where sparse attributes are encountered: this is why the circumstances where EAV design is applicable are relatively rare. [1]\n\n## Alternatives\n\nIn some use-cases, JSONB (binary JSON data) datatype (Postgres 9.4+ and analogous in other RDMSs) can be used as an alternative to EAV. JSONB supports indexing, which amortizes performance trade-off. It\'s important to keep in mind that JSONB is not RDMS-agnostic solution and has it\'s own problems, such as typing.\n\n## Installation\n\nInstall with pip\n\n```bash\npip install django-eav2\n```\n\n## Configuration\n\nAdd `eav` to `INSTALLED_APPS` in your settings.\n\n```python\nINSTALLED_APPS = [\n    ...\n    \'eav\',\n]\n```\n\n### Note: Django 2.2 Users\n\nSince `models.JSONField()` isn\'t supported in Django 2.2, we use [django-jsonfield-backport](https://github.com/laymonage/django-jsonfield-backport) to provide [JSONField](https://docs.djangoproject.com/en/dev/releases/3.1/#jsonfield-for-all-supported-database-backends) functionality.\n\nThis requires adding `django_jsonfield_backport` to your `INSTALLED_APPS` as well.\n\n```python\nINSTALLED_APPS = [\n    ...\n    \'eav\',\n    \'django_jsonfield_backport\',\n]\n```\n\n## Getting started\n\n**Step 1.** Register a model:\n\n```python\nimport eav\neav.register(Supplier)\n```\n\nor with decorators:\n\n```python\nfrom eav.decorators import register_eav\n\n@register_eav\nclass Supplier(models.Model):\n    ...\n```\n\n**Step 2.** Create an attribute:\n\n```python\nAttribute.objects.create(name=\'City\', datatype=Attribute.TYPE_TEXT)\n```\n\n**Step 3.** That’s it! You’re ready to go:\n\n```python\nsupplier.eav.city = \'London\'\nsupplier.save()\n\nSupplier.objects.filter(eav__city=\'London\')\n# = <EavQuerySet [<Supplier: Supplier object (1)>]>\n```\n\n**What next? Check out the <a href="https://django-eav2.readthedocs.io/en/latest/#documentation">documentation</a>.**\n\n---\n\n### References\n\n[1] Exploring Performance Issues for a Clinical Database Organized Using an Entity-Attribute-Value Representation, https://doi.org/10.1136/jamia.2000.0070475 <br>\n[2] What is so bad about EAV, anyway?, https://sqlblog.org/2009/11/19/what-is-so-bad-about-eav-anyway <br>\n[3] Magento for Developers: Part 7—Advanced ORM: Entity Attribute Value, https://devdocs.magento.com/guides/m1x/magefordev/mage-for-dev-7.html <br>\n[4] Data Extraction and Ad Hoc Query of an Entity— Attribute— Value Database, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC61332/\n',
-    'author': 'Mauro Lizaur',
-    'author_email': 'mauro@sdf.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jazzband/django-eav2',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+Django EAV 2 is a fork of django-eav (which itself was derived from eav-django).
+You can find documentation <a href="https://django-eav2.rtfd.io">here</a>.
 
+## What is EAV anyway?
+
+> Entity–attribute–value model (EAV) is a data model to encode, in a space-efficient manner, entities where the number of attributes (properties, parameters) that can be used to describe them is potentially vast, but the number that will actually apply to a given entity is relatively modest. Such entities correspond to the mathematical notion of a sparse matrix. (Wikipedia)
+
+Data in EAV is stored as a 3-tuple (typically corresponding to three distinct tables):
+
+- The entity: the item being described, e.g. `Person(name='Mike')`.
+- The attribute: often a foreign key into a table of attributes, e.g. `Attribute(slug='height', datatype=FLOAT)`.
+- The value of the attribute, with links both an attribute and an entity, e.g. `Value(value_float=15.5, person=mike, attr=height)`.
+
+Entities in **django-eav2** are your typical Django model instances. Attributes (name and type) are stored in their own table, which makes it easy to manipulate the list of available attributes in the system. Values are an intermediate table between attributes and entities, each instance holding a single value.
+This implementation also makes it easy to edit attributes in Django Admin and form instances.
+
+You will find detailed description of the EAV here:
+
+- [Wikipedia - Entity–attribute–value model](https://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model)
+
+## EAV - The Good, the Bad or the Ugly?
+
+EAV is a trade-off between flexibility and complexity. As such, it should not be thought of as either an amelioration pattern, nor an anti-pattern. It is more of a [gray pattern](https://wiki.c2.com/?GreyPattern) - it exists in some context, to solve certain set of problems. When used appropriately, it can introduce great flexibility, cut prototyping time or deacrease complexity. When used carelessly, however, it can complicate database schema, degrade the performance and make maintainance hard. **As with every tool, it should not be overused.** In the following paragraphs we briefly discuss the pros, the cons and pointers to keep in mind when using EAV.
+
+### When to use EAV?
+
+Originally, EAV was introduced to workaround a problem which cannot be easily solved within relational model. In order to achieve this, EAV bypasses normal schema restrictions. Some refer to this as an example of the [inner-platform effect](https://en.wikipedia.org/wiki/Inner-platform_effect#Examples). Naturally, in such scenarios RDMS resources cannot be used efficiently.
+
+Typical application of the EAV model sets to solve the problem of sparse data with a large number of applicable attributes, but only a small fraction that applies to a given entity that may not be known beforehand. Consider the classic example:
+
+> A problem that data modelers commonly encounter in the biomedical domain is organizing and storing highly diverse and heterogeneous data. For example, a single patient may have thousands of applicable descriptive parameters, all of which need to be easily accessible in an electronic patient record system. These requirements pose significant modeling and implementation challenges. [1]
+
+And:
+
+> [...] what do you do when you have customers that demand real-time, on-demand addition of attributes that they want to store? In one of the systems I manage, our customers wanted to do exactly this. Since we run a SaaS (software as a service) application, we have many customers across several different industries, who in turn want to use our system to store different types of information about _their_ customers. A salon chain might want to record facts such as 'hair color,' 'hair type,' and 'haircut frequency'; while an investment company might want to record facts such as 'portfolio name,' 'last portfolio adjustment date,' and 'current portfolio balance.' [2]
+
+In both of these problems we have to deal with sparse and heterogeneous properties that apply only to potentially different subsets of particular entities. Applying EAV to a sub-schema of the database allows to model the desired behaviour. Traditional solution would involves wide tables with many columns storing NULL values for attributes that don't apply to an entity.
+
+Very common use case for EAV are custom product attributes in E-commerce implementations, such as Magento. [3]
+
+As a rule of thumb, EAV can be used when:
+
+- Model attributes are to be added and removed by end users (or are unknowable in some different way). EAV supports these without ALTER TABLE statements and allows the attributes to be strongly typed and easily searchable.
+- There will be many attributes and values are sparse, in contrast to having tables with mostly-null columns.
+- The data is highly dynamic/volatile/vulnerable to change. This problem is present in the second example given above. Other example would be rapidly evolving system, such as a prototype with constantly changing requirements.
+- We want to store meta-data or supporting information, e.g. to customize system's behavior.
+- Numerous classes of data need to be represented, each class has a limited number of attributes, but the number of instances of each class is very small.
+- We want to minimise programmer's input when changing the data model.
+
+For more throughout discussion on the appriopriate use-cases see:
+
+1. [Wikipedia - Scenarios that are appropriate for EAV modeling](https://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model#Scenarios_that_are_appropriate_for_EAV_modeling)
+2. [StackOverflow - Entity Attribute Value Database vs. strict Relational Model E-commerce](https://stackoverflow.com/questions/870808/entity-attribute-value-database-vs-strict-relational-model-ecommerce)
+3. [WikiWikiWeb - Generic Data Model](https://wiki.c2.com/?GenericDataModel)
+
+## When to avoid it?
+
+As we outlined in the opening section, EAV is a trade-off. It should not be used when:
+
+##### 1. System is performance critical
+
+> Attribute-centric query is inherently more difficult when data are stored in EAV form than when they are stored conventionally. [4]
+
+In general, the more structured your data model, the more efficiently you can deal with it. Therefore, loose data storage such as EAV has obvious trade-off in performance. Specifically, application of the EAV model makes performing JOINs on tables more complicated.
+
+##### 2. Low complexity/low maintenance cost is of priority
+
+EAV complicates data model by splitting information across tables. This increases conceptual complexity as well as SQL statements required to query the data. In consequence, optimization in one area that also makes the system harder to understand and maintain.
+
+However, it is important to note that:
+
+> An EAV design should be employed only for that sub-schema of a database where sparse attributes need to be modeled: even here, they need to be supported by third normal form metadata tables. There are relatively few database-design problems where sparse attributes are encountered: this is why the circumstances where EAV design is applicable are relatively rare. [1]
+
+## Alternatives
+
+In some use-cases, JSONB (binary JSON data) datatype (Postgres 9.4+ and analogous in other RDMSs) can be used as an alternative to EAV. JSONB supports indexing, which amortizes performance trade-off. It's important to keep in mind that JSONB is not RDMS-agnostic solution and has it's own problems, such as typing.
+
+## Installation
+
+Install with pip
+
+```bash
+pip install django-eav2
+```
+
+## Configuration
+
+Add `eav` to `INSTALLED_APPS` in your settings.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'eav',
+]
+```
+
+### Note: Django 2.2 Users
+
+Since `models.JSONField()` isn't supported in Django 2.2, we use [django-jsonfield-backport](https://github.com/laymonage/django-jsonfield-backport) to provide [JSONField](https://docs.djangoproject.com/en/dev/releases/3.1/#jsonfield-for-all-supported-database-backends) functionality.
+
+This requires adding `django_jsonfield_backport` to your `INSTALLED_APPS` as well.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'eav',
+    'django_jsonfield_backport',
+]
+```
+
+## Getting started
+
+**Step 1.** Register a model:
+
+```python
+import eav
+eav.register(Supplier)
+```
+
+or with decorators:
+
+```python
+from eav.decorators import register_eav
+
+@register_eav
+class Supplier(models.Model):
+    ...
+```
+
+**Step 2.** Create an attribute:
+
+```python
+Attribute.objects.create(name='City', datatype=Attribute.TYPE_TEXT)
+```
+
+**Step 3.** That’s it! You’re ready to go:
+
+```python
+supplier.eav.city = 'London'
+supplier.save()
+
+Supplier.objects.filter(eav__city='London')
+# = <EavQuerySet [<Supplier: Supplier object (1)>]>
+```
+
+**What next? Check out the <a href="https://django-eav2.readthedocs.io/en/latest/#documentation">documentation</a>.**
+
+---
+
+### References
+
+[1] Exploring Performance Issues for a Clinical Database Organized Using an Entity-Attribute-Value Representation, https://doi.org/10.1136/jamia.2000.0070475 <br>
+[2] What is so bad about EAV, anyway?, https://sqlblog.org/2009/11/19/what-is-so-bad-about-eav-anyway <br>
+[3] Magento for Developers: Part 7—Advanced ORM: Entity Attribute Value, https://devdocs.magento.com/guides/m1x/magefordev/mage-for-dev-7.html <br>
+[4] Data Extraction and Ad Hoc Query of an Entity— Attribute— Value Database, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC61332/
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,149 +1,154 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['eav',
-'eav.logic', 'eav.migrations'] package_data = \ {'': ['*'], 'eav': ['locale/ru/
-LC_MESSAGES/*', 'locale/zh_Hans/LC_MESSAGES/*']} install_requires = \
-['django>=3.2,<4.2'] extras_require = \ {'docs': ['sphinx>=5,<7', 'sphinx-
-autodoc-typehints>=1.12,<2.0', 'm2r2>=0.3,<0.4', 'tomlkit>=0.11,<0.12',
-'sphinx-rtd-theme>=1.0.0,<2.0.0']} setup_kwargs = { 'name': 'django-eav2',
-'version': '1.3.1', 'description': 'Entity-Attribute-Value storage for Django',
-'long_description': '[![Build Status](https://github.com/jazzband/django-eav2/
-actions/workflows/test.yml/badge.svg)](https://github.com/jazzband/django-eav2/
-actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/jazzband/django-
-eav2/branch/master/graph/badge.svg?token=BJk3zS22BS)](https://codecov.io/gh/
-jazzband/django-eav2)\n[![Python Version](https://img.shields.io/pypi/
-pyversions/django-eav2.svg)](https://pypi.org/project/django-eav2/)\n[![Django
-Version](https://img.shields.io/pypi/djversions/django-eav2.svg?color=green)]
-(https://pypi.org/project/django-eav2/)\n[![Jazzband](https://jazzband.co/
-static/img/badge.svg)](https://jazzband.co/)\n\n## Django EAV 2 - Entity-
-Attribute-Value storage for Django\n\nDjango EAV 2 is a fork of django-eav
-(which itself was derived from eav-django).\nYou can find documentation
-here.\n\n## What is EAV anyway?\n\n> Entityâattributeâvalue model (EAV) is
-a data model to encode, in a space-efficient manner, entities where the number
-of attributes (properties, parameters) that can be used to describe them is
-potentially vast, but the number that will actually apply to a given entity is
-relatively modest. Such entities correspond to the mathematical notion of a
-sparse matrix. (Wikipedia)\n\nData in EAV is stored as a 3-tuple (typically
-corresponding to three distinct tables):\n\n- The entity: the item being
-described, e.g. `Person(name=\'Mike\')`.\n- The attribute: often a foreign key
-into a table of attributes, e.g. `Attribute(slug=\'height\',
-datatype=FLOAT)`.\n- The value of the attribute, with links both an attribute
-and an entity, e.g. `Value(value_float=15.5, person=mike,
-attr=height)`.\n\nEntities in **django-eav2** are your typical Django model
+Metadata-Version: 2.1 Name: django-eav2 Version: 1.4.0 Summary: Entity-
+Attribute-Value storage for Django Home-page: https://github.com/jazzband/
+django-eav2 License: GNU Lesser General Public License (LGPL), Version 3
+Keywords: django,django-eav2,database,eav,sql Author: Mauro Lizaur Author-
+email: mauro@sdf.org Requires-Python: >=3.8,<4.0 Classifier: Development Status
+:: 3 - Alpha Classifier: Environment :: Web Environment Classifier: Framework
+:: Django Classifier: Framework :: Django :: 3.2 Classifier: Framework ::
+Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
+Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Classifier: License :: Other/Proprietary License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Database
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: docs Requires-Dist: django (>=3.2,<4.3) Requires-Dist: m2r2
+(>=0.3,<0.4) ; extra == "docs" Requires-Dist: sphinx (>=5,<7) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.12,<2.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs" Requires-
+Dist: tomlkit (>=0.11,<0.12) ; extra == "docs" Project-URL: Repository, https:/
+/github.com/jazzband/django-eav2 Description-Content-Type: text/markdown [!
+[Build Status](https://github.com/jazzband/django-eav2/actions/workflows/
+test.yml/badge.svg)](https://github.com/jazzband/django-eav2/actions/workflows/
+test.yml) [![codecov](https://codecov.io/gh/jazzband/django-eav2/branch/master/
+graph/badge.svg?token=BJk3zS22BS)](https://codecov.io/gh/jazzband/django-eav2)
+[![Python Version](https://img.shields.io/pypi/pyversions/django-eav2.svg)]
+(https://pypi.org/project/django-eav2/) [![Django Version](https://
+img.shields.io/pypi/djversions/django-eav2.svg?color=green)](https://pypi.org/
+project/django-eav2/) [![Jazzband](https://jazzband.co/static/img/badge.svg)]
+(https://jazzband.co/) ## Django EAV 2 - Entity-Attribute-Value storage for
+Django Django EAV 2 is a fork of django-eav (which itself was derived from eav-
+django). You can find documentation here. ## What is EAV anyway? >
+Entityâattributeâvalue model (EAV) is a data model to encode, in a space-
+efficient manner, entities where the number of attributes (properties,
+parameters) that can be used to describe them is potentially vast, but the
+number that will actually apply to a given entity is relatively modest. Such
+entities correspond to the mathematical notion of a sparse matrix. (Wikipedia)
+Data in EAV is stored as a 3-tuple (typically corresponding to three distinct
+tables): - The entity: the item being described, e.g. `Person(name='Mike')`. -
+The attribute: often a foreign key into a table of attributes, e.g. `Attribute
+(slug='height', datatype=FLOAT)`. - The value of the attribute, with links both
+an attribute and an entity, e.g. `Value(value_float=15.5, person=mike,
+attr=height)`. Entities in **django-eav2** are your typical Django model
 instances. Attributes (name and type) are stored in their own table, which
 makes it easy to manipulate the list of available attributes in the system.
 Values are an intermediate table between attributes and entities, each instance
-holding a single value.\nThis implementation also makes it easy to edit
-attributes in Django Admin and form instances.\n\nYou will find detailed
-description of the EAV here:\n\n- [Wikipedia - Entityâattributeâvalue
-model](https://en.wikipedia.org/wiki/
-Entity%E2%80%93attribute%E2%80%93value_model)\n\n## EAV - The Good, the Bad or
-the Ugly?\n\nEAV is a trade-off between flexibility and complexity. As such, it
-should not be thought of as either an amelioration pattern, nor an anti-
-pattern. It is more of a [gray pattern](https://wiki.c2.com/?GreyPattern) - it
-exists in some context, to solve certain set of problems. When used
-appropriately, it can introduce great flexibility, cut prototyping time or
-deacrease complexity. When used carelessly, however, it can complicate database
-schema, degrade the performance and make maintainance hard. **As with every
-tool, it should not be overused.** In the following paragraphs we briefly
-discuss the pros, the cons and pointers to keep in mind when using EAV.\n\n###
-When to use EAV?\n\nOriginally, EAV was introduced to workaround a problem
-which cannot be easily solved within relational model. In order to achieve
-this, EAV bypasses normal schema restrictions. Some refer to this as an example
-of the [inner-platform effect](https://en.wikipedia.org/wiki/Inner-
+holding a single value. This implementation also makes it easy to edit
+attributes in Django Admin and form instances. You will find detailed
+description of the EAV here: - [Wikipedia - Entityâattributeâvalue model]
+(https://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model) ##
+EAV - The Good, the Bad or the Ugly? EAV is a trade-off between flexibility and
+complexity. As such, it should not be thought of as either an amelioration
+pattern, nor an anti-pattern. It is more of a [gray pattern](https://
+wiki.c2.com/?GreyPattern) - it exists in some context, to solve certain set of
+problems. When used appropriately, it can introduce great flexibility, cut
+prototyping time or deacrease complexity. When used carelessly, however, it can
+complicate database schema, degrade the performance and make maintainance hard.
+**As with every tool, it should not be overused.** In the following paragraphs
+we briefly discuss the pros, the cons and pointers to keep in mind when using
+EAV. ### When to use EAV? Originally, EAV was introduced to workaround a
+problem which cannot be easily solved within relational model. In order to
+achieve this, EAV bypasses normal schema restrictions. Some refer to this as an
+example of the [inner-platform effect](https://en.wikipedia.org/wiki/Inner-
 platform_effect#Examples). Naturally, in such scenarios RDMS resources cannot
-be used efficiently.\n\nTypical application of the EAV model sets to solve the
+be used efficiently. Typical application of the EAV model sets to solve the
 problem of sparse data with a large number of applicable attributes, but only a
 small fraction that applies to a given entity that may not be known beforehand.
-Consider the classic example:\n\n> A problem that data modelers commonly
-encounter in the biomedical domain is organizing and storing highly diverse and
+Consider the classic example: > A problem that data modelers commonly encounter
+in the biomedical domain is organizing and storing highly diverse and
 heterogeneous data. For example, a single patient may have thousands of
 applicable descriptive parameters, all of which need to be easily accessible in
 an electronic patient record system. These requirements pose significant
-modeling and implementation challenges. [1]\n\nAnd:\n\n> [...] what do you do
-when you have customers that demand real-time, on-demand addition of attributes
-that they want to store? In one of the systems I manage, our customers wanted
-to do exactly this. Since we run a SaaS (software as a service) application, we
-have many customers across several different industries, who in turn want to
-use our system to store different types of information about _their_ customers.
-A salon chain might want to record facts such as \'hair color,\' \'hair type,\'
-and \'haircut frequency\'; while an investment company might want to record
-facts such as \'portfolio name,\' \'last portfolio adjustment date,\' and
-\'current portfolio balance.\' [2]\n\nIn both of these problems we have to deal
-with sparse and heterogeneous properties that apply only to potentially
-different subsets of particular entities. Applying EAV to a sub-schema of the
-database allows to model the desired behaviour. Traditional solution would
-involves wide tables with many columns storing NULL values for attributes that
-don\'t apply to an entity.\n\nVery common use case for EAV are custom product
-attributes in E-commerce implementations, such as Magento. [3]\n\nAs a rule of
-thumb, EAV can be used when:\n\n- Model attributes are to be added and removed
-by end users (or are unknowable in some different way). EAV supports these
-without ALTER TABLE statements and allows the attributes to be strongly typed
-and easily searchable.\n- There will be many attributes and values are sparse,
-in contrast to having tables with mostly-null columns.\n- The data is highly
-dynamic/volatile/vulnerable to change. This problem is present in the second
-example given above. Other example would be rapidly evolving system, such as a
-prototype with constantly changing requirements.\n- We want to store meta-data
-or supporting information, e.g. to customize system\'s behavior.\n- Numerous
+modeling and implementation challenges. [1] And: > [...] what do you do when
+you have customers that demand real-time, on-demand addition of attributes that
+they want to store? In one of the systems I manage, our customers wanted to do
+exactly this. Since we run a SaaS (software as a service) application, we have
+many customers across several different industries, who in turn want to use our
+system to store different types of information about _their_ customers. A salon
+chain might want to record facts such as 'hair color,' 'hair type,' and
+'haircut frequency'; while an investment company might want to record facts
+such as 'portfolio name,' 'last portfolio adjustment date,' and 'current
+portfolio balance.' [2] In both of these problems we have to deal with sparse
+and heterogeneous properties that apply only to potentially different subsets
+of particular entities. Applying EAV to a sub-schema of the database allows to
+model the desired behaviour. Traditional solution would involves wide tables
+with many columns storing NULL values for attributes that don't apply to an
+entity. Very common use case for EAV are custom product attributes in E-
+commerce implementations, such as Magento. [3] As a rule of thumb, EAV can be
+used when: - Model attributes are to be added and removed by end users (or are
+unknowable in some different way). EAV supports these without ALTER TABLE
+statements and allows the attributes to be strongly typed and easily
+searchable. - There will be many attributes and values are sparse, in contrast
+to having tables with mostly-null columns. - The data is highly dynamic/
+volatile/vulnerable to change. This problem is present in the second example
+given above. Other example would be rapidly evolving system, such as a
+prototype with constantly changing requirements. - We want to store meta-data
+or supporting information, e.g. to customize system's behavior. - Numerous
 classes of data need to be represented, each class has a limited number of
-attributes, but the number of instances of each class is very small.\n- We want
-to minimise programmer\'s input when changing the data model.\n\nFor more
-throughout discussion on the appriopriate use-cases see:\n\n1. [Wikipedia -
+attributes, but the number of instances of each class is very small. - We want
+to minimise programmer's input when changing the data model. For more
+throughout discussion on the appriopriate use-cases see: 1. [Wikipedia -
 Scenarios that are appropriate for EAV modeling](https://en.wikipedia.org/wiki/
-Entity%E2%80%93attribute%E2%80%93value_model#Scenarios_that_are_appropriate_for_EAV_modeling)\n2.
-[StackOverflow - Entity Attribute Value Database vs. strict Relational Model E-
-commerce](https://stackoverflow.com/questions/870808/entity-attribute-value-
-database-vs-strict-relational-model-ecommerce)\n3. [WikiWikiWeb - Generic Data
-Model](https://wiki.c2.com/?GenericDataModel)\n\n## When to avoid it?\n\nAs we
+Entity%E2%80%93attribute%E2%80%93value_model#Scenarios_that_are_appropriate_for_EAV_modeling)
+2. [StackOverflow - Entity Attribute Value Database vs. strict Relational Model
+E-commerce](https://stackoverflow.com/questions/870808/entity-attribute-value-
+database-vs-strict-relational-model-ecommerce) 3. [WikiWikiWeb - Generic Data
+Model](https://wiki.c2.com/?GenericDataModel) ## When to avoid it? As we
 outlined in the opening section, EAV is a trade-off. It should not be used
-when:\n\n##### 1. System is performance critical\n\n> Attribute-centric query
-is inherently more difficult when data are stored in EAV form than when they
-are stored conventionally. [4]\n\nIn general, the more structured your data
-model, the more efficiently you can deal with it. Therefore, loose data storage
-such as EAV has obvious trade-off in performance. Specifically, application of
-the EAV model makes performing JOINs on tables more complicated.\n\n##### 2.
-Low complexity/low maintenance cost is of priority\n\nEAV complicates data
-model by splitting information across tables. This increases conceptual
-complexity as well as SQL statements required to query the data. In
-consequence, optimization in one area that also makes the system harder to
-understand and maintain.\n\nHowever, it is important to note that:\n\n> An EAV
-design should be employed only for that sub-schema of a database where sparse
-attributes need to be modeled: even here, they need to be supported by third
-normal form metadata tables. There are relatively few database-design problems
-where sparse attributes are encountered: this is why the circumstances where
-EAV design is applicable are relatively rare. [1]\n\n## Alternatives\n\nIn some
-use-cases, JSONB (binary JSON data) datatype (Postgres 9.4+ and analogous in
-other RDMSs) can be used as an alternative to EAV. JSONB supports indexing,
-which amortizes performance trade-off. It\'s important to keep in mind that
-JSONB is not RDMS-agnostic solution and has it\'s own problems, such as
-typing.\n\n## Installation\n\nInstall with pip\n\n```bash\npip install django-
-eav2\n```\n\n## Configuration\n\nAdd `eav` to `INSTALLED_APPS` in your
-settings.\n\n```python\nINSTALLED_APPS = [\n ...\n \'eav\',\n]\n```\n\n###
-Note: Django 2.2 Users\n\nSince `models.JSONField()` isn\'t supported in Django
-2.2, we use [django-jsonfield-backport](https://github.com/laymonage/django-
-jsonfield-backport) to provide [JSONField](https://docs.djangoproject.com/en/
-dev/releases/3.1/#jsonfield-for-all-supported-database-backends)
-functionality.\n\nThis requires adding `django_jsonfield_backport` to your
-`INSTALLED_APPS` as well.\n\n```python\nINSTALLED_APPS = [\n ...\n \'eav\',\n
-\'django_jsonfield_backport\',\n]\n```\n\n## Getting started\n\n**Step 1.**
-Register a model:\n\n```python\nimport eav\neav.register(Supplier)\n```\n\nor
-with decorators:\n\n```python\nfrom eav.decorators import
-register_eav\n\n@register_eav\nclass Supplier(models.Model):\n
-...\n```\n\n**Step 2.** Create an attribute:
-\n\n```python\nAttribute.objects.create(name=\'City\',
-datatype=Attribute.TYPE_TEXT)\n```\n\n**Step 3.** Thatâs it! Youâre ready
-to go:\n\n```python\nsupplier.eav.city = \'London\'\nsupplier.save
-()\n\nSupplier.objects.filter(eav__city=\'London\')\n# =
-1)>]>\n```\n\n**What next? Check out the documentation.**\n\n---\n\n###
-References\n\n[1] Exploring Performance Issues for a Clinical Database
-Organized Using an Entity-Attribute-Value Representation, https://doi.org/
-10.1136/jamia.2000.0070475
-\n[2] What is so bad about EAV, anyway?, https://sqlblog.org/2009/11/19/what-
-is-so-bad-about-eav-anyway
-\n[3] Magento for Developers: Part 7âAdvanced ORM: Entity Attribute Value,
+when: ##### 1. System is performance critical > Attribute-centric query is
+inherently more difficult when data are stored in EAV form than when they are
+stored conventionally. [4] In general, the more structured your data model, the
+more efficiently you can deal with it. Therefore, loose data storage such as
+EAV has obvious trade-off in performance. Specifically, application of the EAV
+model makes performing JOINs on tables more complicated. ##### 2. Low
+complexity/low maintenance cost is of priority EAV complicates data model by
+splitting information across tables. This increases conceptual complexity as
+well as SQL statements required to query the data. In consequence, optimization
+in one area that also makes the system harder to understand and maintain.
+However, it is important to note that: > An EAV design should be employed only
+for that sub-schema of a database where sparse attributes need to be modeled:
+even here, they need to be supported by third normal form metadata tables.
+There are relatively few database-design problems where sparse attributes are
+encountered: this is why the circumstances where EAV design is applicable are
+relatively rare. [1] ## Alternatives In some use-cases, JSONB (binary JSON
+data) datatype (Postgres 9.4+ and analogous in other RDMSs) can be used as an
+alternative to EAV. JSONB supports indexing, which amortizes performance trade-
+off. It's important to keep in mind that JSONB is not RDMS-agnostic solution
+and has it's own problems, such as typing. ## Installation Install with pip
+```bash pip install django-eav2 ``` ## Configuration Add `eav` to
+`INSTALLED_APPS` in your settings. ```python INSTALLED_APPS = [ ... 'eav', ]
+``` ### Note: Django 2.2 Users Since `models.JSONField()` isn't supported in
+Django 2.2, we use [django-jsonfield-backport](https://github.com/laymonage/
+django-jsonfield-backport) to provide [JSONField](https://
+docs.djangoproject.com/en/dev/releases/3.1/#jsonfield-for-all-supported-
+database-backends) functionality. This requires adding
+`django_jsonfield_backport` to your `INSTALLED_APPS` as well. ```python
+INSTALLED_APPS = [ ... 'eav', 'django_jsonfield_backport', ] ``` ## Getting
+started **Step 1.** Register a model: ```python import eav eav.register
+(Supplier) ``` or with decorators: ```python from eav.decorators import
+register_eav @register_eav class Supplier(models.Model): ... ``` **Step 2.**
+Create an attribute: ```python Attribute.objects.create(name='City',
+datatype=Attribute.TYPE_TEXT) ``` **Step 3.** Thatâs it! Youâre ready to
+go: ```python supplier.eav.city = 'London' supplier.save()
+Supplier.objects.filter(eav__city='London') # =
+1)>]> ``` **What next? Check out the documentation.** --- ### References [1]
+Exploring Performance Issues for a Clinical Database Organized Using an Entity-
+Attribute-Value Representation, https://doi.org/10.1136/jamia.2000.0070475
+[2] What is so bad about EAV, anyway?, https://sqlblog.org/2009/11/19/what-is-
+so-bad-about-eav-anyway
+[3] Magento for Developers: Part 7âAdvanced ORM: Entity Attribute Value,
 https://devdocs.magento.com/guides/m1x/magefordev/mage-for-dev-7.html
-\n[4] Data Extraction and Ad Hoc Query of an Entityâ Attributeâ Value
-Database, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC61332/\n', 'author':
-'Mauro Lizaur', 'author_email': 'mauro@sdf.org', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/jazzband/django-eav2',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+[4] Data Extraction and Ad Hoc Query of an Entityâ Attributeâ Value
+Database, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC61332/
```

