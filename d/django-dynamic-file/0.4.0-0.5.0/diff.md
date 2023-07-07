# Comparing `tmp/django-dynamic-file-0.4.0.tar.gz` & `tmp/django-dynamic-file-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-file-0.4.0.tar", last modified: Mon May 22 16:34:49 2023, max compression
+gzip compressed data, was "django-dynamic-file-0.5.0.tar", last modified: Fri Jul  7 11:03:28 2023, max compression
```

## Comparing `django-dynamic-file-0.4.0.tar` & `django-dynamic-file-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 16:34:49.000000 django-dynamic-file-0.4.0/django_dynamic_file.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/models/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/models/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/dynamic_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/serializers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/dynamic_file/views/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/dynamic_file/views/serve_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:34:49.076432 django-dynamic-file-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_model_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_serializer_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-22 16:34:33.000000 django-dynamic-file-0.4.0/tests/test_view_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.861457 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.861457 django-dynamic-file-0.5.0/dynamic_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/serializers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/views/serve_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_serializer_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_view_serve.py
```

### Comparing `django-dynamic-file-0.4.0/LICENSE` & `django-dynamic-file-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.4.0/PKG-INFO` & `django-dynamic-file-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.4.0
+Version: 0.5.0
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.4.0/README.rst` & `django-dynamic-file-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.4.0/django_dynamic_file.egg-info/PKG-INFO` & `django-dynamic-file-0.5.0/django_dynamic_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.4.0
+Version: 0.5.0
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.4.0/django_dynamic_file.egg-info/SOURCES.txt` & `django-dynamic-file-0.5.0/django_dynamic_file.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 dynamic_file/__init__.py
 dynamic_file/admin.py
 dynamic_file/apps.py
 dynamic_file/config.py
 dynamic_file/storage.py
 dynamic_file/migrations/0001_initial.py
 dynamic_file/migrations/0002_alter_dynamicfile_file.py
+dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py
 dynamic_file/migrations/__init__.py
 dynamic_file/models/__init__.py
 dynamic_file/models/base.py
 dynamic_file/models/file.py
 dynamic_file/serializers/__init__.py
-dynamic_file/serializers/dynamic_file.py
 dynamic_file/serializers/fields.py
 dynamic_file/views/__init__.py
 dynamic_file/views/serve_file.py
+tests/test_admin.py
 tests/test_model_file.py
 tests/test_serializer_file.py
 tests/test_view_serve.py
```

### Comparing `django-dynamic-file-0.4.0/dynamic_file/migrations/0001_initial.py` & `django-dynamic-file-0.5.0/dynamic_file/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.conf import settings
 
 from dynamic_file import config
 
 # Heavily inspired by https://github.com/dj-stripe/dj-stripe/blob/master/djstripe/migrations/0001_initial.py
 
 DYNAMIC_FILE_UPLOADED_BY_MODEL = settings.DYNAMIC_FILE_UPLOADED_BY_MODEL
-DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME = settings.DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME
+DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME = '+'
 DYNAMIC_FILE_UPLOADED_BY_MODEL_MIGRATION_DEPENDENCY = settings.DYNAMIC_FILE_UPLOADED_BY_MIGRATION_DEPENDENCY
 
 
 DYNAMIC_FILE_UPLOADED_BY_MODEL_DEPENDENCY = migrations.swappable_dependency(
     DYNAMIC_FILE_UPLOADED_BY_MODEL
 )
 
@@ -23,14 +23,15 @@
         (
             DYNAMIC_FILE_UPLOADED_BY_MODEL.split('.', 1)[0],
             DYNAMIC_FILE_UPLOADED_BY_MODEL_MIGRATION_DEPENDENCY,
         ),
         DYNAMIC_FILE_UPLOADED_BY_MODEL,
     )
 
+
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         DYNAMIC_FILE_UPLOADED_BY_MODEL_DEPENDENCY
     ]
@@ -38,14 +39,15 @@
     operations = [
         migrations.CreateModel(
             name='DynamicFile',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('description', models.TextField(blank=True, help_text='A description for this file')),
                 ('file', models.FileField(help_text='The uploaded file', upload_to='')),
-                ('uploaded_by', models.ForeignKey(help_text='The owner/uploader of this file', null=True, on_delete=django.db.models.deletion.SET_NULL, related_name=DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME, to=DYNAMIC_FILE_UPLOADED_BY_MODEL)),
+                ('uploaded_by', models.ForeignKey(help_text='The owner/uploader of this file', null=True,
+                 on_delete=django.db.models.deletion.SET_NULL, related_name=DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME, to=DYNAMIC_FILE_UPLOADED_BY_MODEL)),
             ],
             options={
                 'abstract': False,
             },
         ),
     ]
```

### Comparing `django-dynamic-file-0.4.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py` & `django-dynamic-file-0.5.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.4.0/dynamic_file/serializers/fields.py` & `django-dynamic-file-0.5.0/dynamic_file/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.4.0/dynamic_file/views/serve_file.py` & `django-dynamic-file-0.5.0/dynamic_file/views/serve_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 from django.conf import settings
 from django.http.response import FileResponse
 from django.http.response import HttpResponse
 
-# from rest_framework.generics import RetrieveUpdateDestroyAPIView
 from rest_framework.views import APIView
+from rest_framework import status
+from rest_framework.exceptions import NotFound
 
 from dynamic_file.models import DynamicFile
 
 from rest_framework.settings import api_settings
+from rest_framework.permissions import IsAuthenticated
+from rest_framework.permissions import IsAdminUser
 
 import mimetypes
 import os
 
 
 class _DynamicContentMixin():
     _Model = DynamicFile
     permission_classes = api_settings.DEFAULT_PERMISSION_CLASSES
 
     lookup_field = 'pk'
     lookup_url_kwarg = 'pk'
 
-    def get_file_name(self, file, _):
-        _, ext = os.path.splitext(file.name)
-        if not ext:
-            return file.name + mimetypes.guess_extension(file.content_type)
-        else:  # pragma: no cover
-            return file.name
-
-    def get_parent(self):
-        return None
-
     def get_object(self):
         filter_kwargs = {self.lookup_field: self.kwargs[self.lookup_url_kwarg]}
-        return self._Model.objects.filter(**filter_kwargs).first()
+        instance = self._Model.objects.filter(**filter_kwargs).first()
+        self.check_object_permissions(self.request, instance)
+        return instance
 
 
 class ServeDynamicFile(_DynamicContentMixin, APIView):
     def get(self, request, *args, **kwargs):
         instance = self.get_object()
         filename = None
         if instance:
             filename = instance.file.name
-
-        # fallback would go here.
+        else:
+            raise NotFound()
 
         content_type, encoding = mimetypes.guess_type(filename)
         path = os.path.join(settings.DYNAMIC_FILE_STORAGE_LOCATION, filename)
 
-        # TODO check if exists and add fallback
-
-        if settings.DEBUG:
-            fp = open(path, 'rb')
-            response = FileResponse(fp)
-            response.filename = filename
-
-        else:  # for now, nginx will suffice
-            response = HttpResponse(content_type=content_type)
-            response['Content-Disposition'] = 'inline; filename={0}'.format(filename)
-            response['Content-Encoding'] = encoding
-
-            location = os.path.normpath(path)
-            response['X-Accel-Redirect'] = location
-
-        return response
+        try:
+            if settings.DEBUG:
+                fp = open(path, 'rb')
+                response = FileResponse(fp)
+                response.filename = filename
+
+            else:  # for now, nginx will suffice
+                response = HttpResponse(content_type=content_type)
+                response['Content-Disposition'] = 'inline; filename={0}'.format(filename)
+                response['Content-Encoding'] = encoding
+
+                location = os.path.normpath(path)
+                response['X-Accel-Redirect'] = location
+
+            return response
+        except Exception as e:
+            print(e)
+            return HttpResponse('File not found', status=status.HTTP_404_NOT_FOUND)
+
+
+class ServeDynamicFileAdmin(ServeDynamicFile):
+    permission_classes = [IsAuthenticated, IsAdminUser]
+    lookup_field = 'file'
+    lookup_url_kwarg = 'name'
```

### Comparing `django-dynamic-file-0.4.0/pyproject.toml` & `django-dynamic-file-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-dynamic-file"
-version = "0.4.0"
+version = "0.5.0"
 description = "A flexible approach to handling and serving files with django"
 readme = "README.rst"
 authors = [{ name = "Philipp Hafner", email = "philipp@hafner.xyz" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 
 [tool.setuptools]
 package-dir = {"dynamic_file" = "dynamic_file"}
 
 
 [tool.bumpver]
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
-current_version = "0.4.0"
+current_version = "0.5.0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `django-dynamic-file-0.4.0/tests/test_model_file.py` & `django-dynamic-file-0.5.0/tests/test_model_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,76 @@
 from django.test import TestCase
 from django.apps import apps
 from django.conf import settings
 
 from dynamic_file.models import DynamicFile
 
 import helpers
+import base64
 
 UploadedByModel = apps.get_model(settings.DYNAMIC_FILE_UPLOADED_BY_MODEL)
 
 
 class DynamicFileModelTestCase(TestCase):
 
     def test_create_default(self):
         instance = DynamicFile.objects.create()
 
         assert instance.description == ''
         assert instance.uploaded_by is None
         instance.file.name == ''
 
-    def test_reverse_accessor(self):
-        uploader = UploadedByModel.objects.create()
-        instance = DynamicFile.objects.create(uploaded_by=uploader)
-
-        assert instance in getattr(uploader, settings.DYNAMIC_FILE_UPLOADED_BY_RELATED_NAME).all()
-
     def test_description(self):
         desc = 'A sample description for this file'
         instance = DynamicFile.objects.create(description=desc)
 
         assert instance.description == desc
 
     def test_name(self):
         instance = DynamicFile.objects.create(file=helpers.create_dummy_gif())
-
         assert instance.name == instance.file.name
 
     def test_storage_location(self):
         instance = DynamicFile.objects.create(file=helpers.create_dummy_gif())
 
         assert instance.file.name != ''
         assert instance.file.read() == helpers.create_dummy_gif().read()
+
+    def test_read(self):
+        instance = DynamicFile.objects.create(file=helpers.create_dummy_gif())
+        assert instance.read == instance.file.read
+
+    def test_mimetype(self):
+        instance = DynamicFile.objects.create(file=helpers.create_dummy_gif('image.gif'))
+        mimetype = instance.mimetype
+        assert mimetype
+        assert mimetype == 'image/gif'
+
+    def test_to_base64(self):
+        file = helpers.create_dummy_gif('image.gif')
+        instance = DynamicFile.objects.create(file=file)
+
+        assert base64.b64encode(helpers.SMALL_GIF) == instance.to_base64()
+
+    def test_to_base64_utf8(self):
+        file = helpers.create_dummy_gif('image.gif')
+        instance = DynamicFile.objects.create(file=file)
+
+        assert base64.b64encode(helpers.SMALL_GIF).decode('utf-8') == instance.to_base64_utf8()
+
+    def test_to_base64_src(self):
+        file = helpers.create_dummy_gif('image.gif')
+        instance = DynamicFile.objects.create(file=file)
+
+        b64 = base64.b64encode(helpers.SMALL_GIF).decode('utf-8')
+        expected = f'data:;base64,{b64}'
+        assert expected == instance.to_base64_src()
+
+    def test_str(self):
+        instance = DynamicFile.objects.create(file=None)
+        assert str(instance.pk) in str(instance)
+
+        instance = DynamicFile.objects.create(display_name='test')
+        assert instance.display_name == str(instance)
+
+        instance = DynamicFile.objects.create(file=helpers.create_dummy_gif('image.gif'))
+        assert instance.name == str(instance)
```

### Comparing `django-dynamic-file-0.4.0/tests/test_serializer_file.py` & `django-dynamic-file-0.5.0/tests/test_serializer_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.4.0/tests/test_view_serve.py` & `django-dynamic-file-0.5.0/tests/test_view_serve.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         assert 'Content-Disposition' in response.headers.keys()
         assert 'Content-Encoding' in response.headers.keys()
         assert response.headers['X-Accel-Redirect'] == expected_path
 
         with open(response.headers['X-Accel-Redirect'], 'rb') as file:
             assert file.read() == self.instance_1.file.read()
 
+    def test_not_found(self):
+        factory = APIRequestFactory()
+        request = factory.get('')
+
+        response = self.view(request, pk=-1)
+
+        assert response.status_code is status.HTTP_404_NOT_FOUND
+
 
 class ServeCustomDynamicFileTestCase(TestCase):
 
     @classmethod
     def setUpTestData(cls):
         cls.view = ServeTestFile.as_view()
         cls.instance_1 = DynamicFile.objects.create(file=helpers.create_dummy_gif())
```

