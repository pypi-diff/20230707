# Comparing `tmp/django_quanttide-0.1.0b1.tar.gz` & `tmp/django_quanttide-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_quanttide-0.1.0b1.tar", max compression
+gzip compressed data, was "django_quanttide-0.1.0b2.tar", max compression
```

## Comparing `django_quanttide-0.1.0b1.tar` & `django_quanttide-0.1.0b2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       39 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/__init__.py
--rw-r--r--   0        0        0      104 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/apps.py
--rw-r--r--   0        0        0      494 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/models/__init__.py
--rw-r--r--   0        0        0      414 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/models/choices.py
--rw-r--r--   0        0        0     6929 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/models/fields.py
--rw-r--r--   0        0        0      275 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/django_quanttide/models/models.py
--rw-r--r--   0        0        0      531 2023-07-05 07:17:46.658199 django_quanttide-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 django_quanttide-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-07-07 13:38:26.758218 django_quanttide-0.1.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 13:38:26.758218 django_quanttide-0.1.0b2/django_quanttide/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-07 13:38:26.758218 django_quanttide-0.1.0b2/django_quanttide/apps.py
+-rw-r--r--   0        0        0      654 2023-07-07 13:38:26.758218 django_quanttide-0.1.0b2/django_quanttide/models/__init__.py
+-rw-r--r--   0        0        0      414 2023-07-07 13:38:26.758218 django_quanttide-0.1.0b2/django_quanttide/models/choices.py
+-rw-r--r--   0        0        0     9596 2023-07-07 13:38:26.762218 django_quanttide-0.1.0b2/django_quanttide/models/fields.py
+-rw-r--r--   0        0        0     1823 2023-07-07 13:38:26.762218 django_quanttide-0.1.0b2/django_quanttide/models/models.py
+-rw-r--r--   0        0        0      561 2023-07-07 13:38:26.762218 django_quanttide-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 django_quanttide-0.1.0b2/PKG-INFO
```

### Comparing `django_quanttide-0.1.0b1/django_quanttide/models/fields.py` & `django_quanttide-0.1.0b2/django_quanttide/models/fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 数据模型字段
 """
 
 import uuid
 
 from django.db import models
+from django.contrib.auth import get_user_model
 
 
 class IDField(models.UUIDField):
     """
     ID字段
 
     微服务系统内全局唯一。
@@ -32,14 +33,40 @@
         options.setdefault('primary_key', True)
         options.setdefault('editable', not options['primary_key'])
         options.setdefault('default', uuid.uuid4)
         options.setdefault('verbose_name', 'ID')
         super().__init__(**options)
 
 
+class NumberField(models.IntegerField):
+    """
+    编号字段
+    """
+    description = "编号字段"
+
+    def __init__(self, **options):
+        options['editable'] = False
+        options['unique'] = True
+        options.setdefault('verbose_name', '编号')
+        super().__init__(**options)
+
+    def pre_save(self, model_instance, add):
+        value = getattr(model_instance, self.attname)
+        if not value:
+            # 如果字段值为空，则生成一个自增的值
+            queryset = model_instance.__class__.objects.all()
+            if queryset:
+                last_object = queryset.latest(self.attname)
+                value = getattr(last_object, self.attname) + 1
+            else:
+                value = 1
+            setattr(model_instance, self.attname, value)
+        return value
+
+
 class NameField(models.SlugField):
     """
     标识字段
 
     租户内同模型唯一。
 
     用于表示名称或标题的标识符字段，通常用于生成URL Slug。
@@ -210,7 +237,57 @@
     """
     description = "更新时间字段"
 
     def __init__(self, **options):
         options.setdefault('auto_now', True)
         options.setdefault('verbose_name', '更新时间')
         super().__init__(**options)
+
+
+class CreatedByField(models.ForeignKey):
+    """
+    创建者字段
+
+    该字段用于记录创建该记录的用户。
+
+    :param to: 外键关联的用户模型。默认为 settings.AUTH_USER_MODEL。
+    :type to: str
+    :param on_delete: 外键关联的删除行为。默认为 PROTECT。
+    :type on_delete: ~typing.Optional[Callable[[], Any]]
+    :param null: 是否允许为空。默认为 True。
+    :type null: bool
+    :param verbose_name: 字段的可读名称。默认为“创建者”。
+    :type verbose_name: str
+    """
+    description = "创建者字段"
+
+    def __init__(self, **options):
+        user_model = options.pop('to', get_user_model())
+        on_delete = options.pop('on_delete', models.PROTECT)
+        options.setdefault('null', True)
+        options.setdefault('verbose_name', '创建者')
+        super().__init__(user_model, on_delete, **options)
+
+
+class UpdatedByField(models.ForeignKey):
+    """
+    更新者字段
+
+    该字段用于记录最后一次更新该记录的用户。
+
+    :param to: 外键关联的用户模型。默认为 settings.AUTH_USER_MODEL。
+    :type to: str
+    :param on_delete: 外键关联的删除行为。默认为 PROTECT。
+    :type on_delete: ~typing.Optional[Callable[[], Any]]
+    :param null: 是否允许为空。默认为 True。
+    :type null: bool
+    :param verbose_name: 字段的可读名称。默认为“更新者”。
+    :type verbose_name: str
+    """
+    description = "更新者字段"
+
+    def __init__(self, **options):
+        user_model = options.pop('to', get_user_model())
+        on_delete = options.pop('on_delete', models.PROTECT)
+        options.setdefault('null', True)
+        options.setdefault('verbose_name', '更新者')
+        super().__init__(user_model, on_delete, **options)
```

### Comparing `django_quanttide-0.1.0b1/pyproject.toml` & `django_quanttide-0.1.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-quanttide"
-version = "0.1.0-beta.1"
+version = "0.1.0-beta.2"
 description = "量潮Django SDK"
 authors = ["QuantTide Inc. <opensource@quanttide.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "django_quanttide"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = ">=3.1"
 djangorestframework = ">=3.0"
+django-polymorphic = "^3.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 coverage = "^7.2.7"
 pre-commit = "^3.3.3"
 tox = "^4.6.3"
```

### Comparing `django_quanttide-0.1.0b1/PKG-INFO` & `django_quanttide-0.1.0b2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-quanttide
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: 量潮Django SDK
 License: Apache 2.0
 Author: QuantTide Inc.
 Author-email: opensource@quanttide.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3.1)
+Requires-Dist: django-polymorphic (>=3.1.0,<4.0.0)
 Requires-Dist: djangorestframework (>=3.0)
 Description-Content-Type: text/markdown
 
 # `django-quanttide`
 
 量潮Django SDK
```

