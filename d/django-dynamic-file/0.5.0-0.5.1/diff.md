# Comparing `tmp/django-dynamic-file-0.5.0.tar.gz` & `tmp/django-dynamic-file-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-file-0.5.0.tar", last modified: Fri Jul  7 11:03:28 2023, max compression
+gzip compressed data, was "django-dynamic-file-0.5.1.tar", last modified: Fri Jul  7 11:38:58 2023, max compression
```

## Comparing `django-dynamic-file-0.5.0.tar` & `django-dynamic-file-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.861457 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 11:03:28.000000 django-dynamic-file-0.5.0/django_dynamic_file.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.861457 django-dynamic-file-0.5.0/dynamic_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/models/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/models/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/serializers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/dynamic_file/views/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/dynamic_file/views/serve_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:03:28.865458 django-dynamic-file-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_model_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_serializer_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-07 11:03:06.000000 django-dynamic-file-0.5.0/tests/test_view_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.368602 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-07 11:38:58.000000 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-07 11:38:58.000000 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:38:58.000000 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 11:38:58.000000 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 11:38:58.000000 django-dynamic-file-0.5.1/django_dynamic_file.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/dynamic_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/dynamic_file/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/migrations/0002_alter_dynamicfile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/migrations/0004_dynamicfile_created_at_dynamicfile_updated_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/dynamic_file/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/models/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/dynamic_file/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/serializers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/dynamic_file/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/dynamic_file/views/serve_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:38:58.372602 django-dynamic-file-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/tests/test_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/tests/test_serializer_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-07 11:38:40.000000 django-dynamic-file-0.5.1/tests/test_view_serve.py
```

### Comparing `django-dynamic-file-0.5.0/LICENSE` & `django-dynamic-file-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/PKG-INFO` & `django-dynamic-file-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.5.0
+Version: 0.5.1
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.5.0/README.rst` & `django-dynamic-file-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/django_dynamic_file.egg-info/PKG-INFO` & `django-dynamic-file-0.5.1/django_dynamic_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-file
-Version: 0.5.0
+Version: 0.5.1
 Summary: A flexible approach to handling and serving files with django
 Author-email: Philipp Hafner <philipp@hafner.xyz>
 License: MIT License
         
         Copyright (c) 2022 Philipp Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-dynamic-file-0.5.0/django_dynamic_file.egg-info/SOURCES.txt` & `django-dynamic-file-0.5.1/django_dynamic_file.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 dynamic_file/admin.py
 dynamic_file/apps.py
 dynamic_file/config.py
 dynamic_file/storage.py
 dynamic_file/migrations/0001_initial.py
 dynamic_file/migrations/0002_alter_dynamicfile_file.py
 dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py
+dynamic_file/migrations/0004_dynamicfile_created_at_dynamicfile_updated_at.py
 dynamic_file/migrations/__init__.py
 dynamic_file/models/__init__.py
 dynamic_file/models/base.py
 dynamic_file/models/file.py
 dynamic_file/serializers/__init__.py
 dynamic_file/serializers/fields.py
 dynamic_file/views/__init__.py
```

### Comparing `django-dynamic-file-0.5.0/dynamic_file/admin.py` & `django-dynamic-file-0.5.1/dynamic_file/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/dynamic_file/migrations/0001_initial.py` & `django-dynamic-file-0.5.1/dynamic_file/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/dynamic_file/migrations/0002_alter_dynamicfile_file.py` & `django-dynamic-file-0.5.1/dynamic_file/migrations/0002_alter_dynamicfile_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py` & `django-dynamic-file-0.5.1/dynamic_file/migrations/0003_alter_dynamicfile_uploaded_by.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/dynamic_file/models/base.py` & `django-dynamic-file-0.5.1/dynamic_file/models/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,32 @@
     Specifies the uploader of this file. This foreign key defaults to ``AUTH_USER_MODEL``
     but can be customized by changing ``DYNAMIC_FILE_UPLOADED_BY_MODEL``.
     The reverse accessor is unused.
 
     NOTE: Changing those settings is only supported _before_ running the first migration
     '''
 
+    created_at = models.DateTimeField(
+        auto_now_add=True,
+        blank=True,
+        help_text=_('The creation date of this file')
+    )
+    '''
+    Read-only field, specifying the upload date of this file.
+    '''
+
+    updated_at = models.DateTimeField(
+        auto_now=True,
+        blank=True,
+        help_text=_('The last update date of this file')
+    )
+    '''
+    Read-only field, specifying the update date of this file.
+    '''
+
     @property
     def name(self):
         '''
         Returns the filename of this instance. If ``file`` is ``None``, an empty string is returned.
         '''
         if self.file:
             return self.file.name
```

### Comparing `django-dynamic-file-0.5.0/dynamic_file/serializers/fields.py` & `django-dynamic-file-0.5.1/dynamic_file/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/dynamic_file/views/serve_file.py` & `django-dynamic-file-0.5.1/dynamic_file/views/serve_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/pyproject.toml` & `django-dynamic-file-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-dynamic-file"
-version = "0.5.0"
+version = "0.5.1"
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
-current_version = "0.5.0"
+current_version = "0.5.1"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `django-dynamic-file-0.5.0/tests/test_admin.py` & `django-dynamic-file-0.5.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/tests/test_model_file.py` & `django-dynamic-file-0.5.1/tests/test_model_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/tests/test_serializer_file.py` & `django-dynamic-file-0.5.1/tests/test_serializer_file.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-file-0.5.0/tests/test_view_serve.py` & `django-dynamic-file-0.5.1/tests/test_view_serve.py`

 * *Files identical despite different names*

