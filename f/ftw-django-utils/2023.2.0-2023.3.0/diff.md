# Comparing `tmp/ftw_django_utils-2023.2.0.tar.gz` & `tmp/ftw_django_utils-2023.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftw_django_utils-2023.2.0.tar", max compression
+gzip compressed data, was "ftw_django_utils-2023.3.0.tar", max compression
```

## Comparing `ftw_django_utils-2023.2.0.tar` & `ftw_django_utils-2023.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-04-24 06:47:54.167855 ftw_django_utils-2023.2.0/LICENSE
--rw-r--r--   0        0        0    10043 2023-05-03 15:13:01.186342 ftw_django_utils-2023.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 11:53:42.866695 ftw_django_utils-2023.2.0/django_utils/__init__.py
--rw-r--r--   0        0        0      101 2023-04-24 06:47:54.168594 ftw_django_utils-2023.2.0/django_utils/apps.py
--rw-r--r--   0        0        0      931 2023-04-24 06:47:54.168843 ftw_django_utils-2023.2.0/django_utils/authentication/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.168986 ftw_django_utils-2023.2.0/django_utils/db/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169154 ftw_django_utils-2023.2.0/django_utils/db/fields/__init__.py
--rw-r--r--   0        0        0      579 2023-04-24 06:47:54.169320 ftw_django_utils-2023.2.0/django_utils/db/fields/text.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169464 ftw_django_utils-2023.2.0/django_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169619 ftw_django_utils-2023.2.0/django_utils/management/commands/__init__.py
--rw-r--r--   0        0        0      672 2023-04-24 06:47:54.169783 ftw_django_utils-2023.2.0/django_utils/management/commands/sentry_test.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.169954 ftw_django_utils-2023.2.0/django_utils/serializer/__init__.py
--rw-r--r--   0        0        0       70 2023-04-24 06:47:54.170297 ftw_django_utils-2023.2.0/django_utils/serializer/fields/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-27 12:17:15.591189 ftw_django_utils-2023.2.0/django_utils/serializer/fields/protected_image_field.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.170724 ftw_django_utils-2023.2.0/django_utils/settings/__init__.py
--rw-r--r--   0        0        0     2229 2023-04-24 06:47:54.170950 ftw_django_utils-2023.2.0/django_utils/settings/logging.py
--rw-r--r--   0        0        0      989 2023-04-24 06:47:54.171110 ftw_django_utils-2023.2.0/django_utils/settings/sentry.py
--rw-r--r--   0        0        0        0 2023-04-24 06:47:54.171273 ftw_django_utils-2023.2.0/django_utils/testing/__init__.py
--rw-r--r--   0        0        0      793 2023-04-24 06:47:54.171507 ftw_django_utils-2023.2.0/django_utils/testing/filestructure.py
--rw-r--r--   0        0        0      358 2023-04-27 12:17:15.591899 ftw_django_utils-2023.2.0/django_utils/testing/urls.py
--rw-r--r--   0        0        0     3701 2023-04-27 12:17:15.592407 ftw_django_utils-2023.2.0/django_utils/testing/views.py
--rw-r--r--   0        0        0       55 2023-04-24 06:47:54.171995 ftw_django_utils-2023.2.0/django_utils/views/__init__.py
--rw-r--r--   0        0        0     1520 2023-04-27 12:17:15.592903 ftw_django_utils-2023.2.0/django_utils/views/file_getter.py
--rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474048 ftw_django_utils-2023.2.0/django_utils/webhooks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 13:48:47.474359 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/__init__.py
--rw-r--r--   0        0        0       98 2023-04-25 13:48:47.475387 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/default_delete_hooks.py
--rw-r--r--   0        0        0      214 2023-04-25 13:48:47.476248 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/serializers.py
--rw-r--r--   0        0        0     1158 2023-04-25 13:48:47.476744 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/token_authentication.py
--rw-r--r--   0        0        0      259 2023-04-25 13:48:47.477333 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/urls.py
--rw-r--r--   0        0        0     1837 2023-04-27 12:17:15.593531 ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/views.py
--rw-r--r--   0        0        0     1404 2023-05-03 15:15:02.991709 ftw_django_utils-2023.2.0/pyproject.toml
--rw-r--r--   0        0        0    10741 1970-01-01 00:00:00.000000 ftw_django_utils-2023.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-16 16:36:40.055892 ftw_django_utils-2023.3.0/LICENSE
+-rw-r--r--   0        0        0    10043 2023-06-15 09:45:45.169734 ftw_django_utils-2023.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.056156 ftw_django_utils-2023.3.0/django_utils/__init__.py
+-rw-r--r--   0        0        0      101 2022-11-16 16:36:40.056265 ftw_django_utils-2023.3.0/django_utils/apps.py
+-rw-r--r--   0        0        0      931 2022-11-16 16:36:40.056445 ftw_django_utils-2023.3.0/django_utils/authentication/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.056548 ftw_django_utils-2023.3.0/django_utils/db/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.056657 ftw_django_utils-2023.3.0/django_utils/db/fields/__init__.py
+-rw-r--r--   0        0        0      579 2022-11-16 16:36:40.056777 ftw_django_utils-2023.3.0/django_utils/db/fields/text.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.056873 ftw_django_utils-2023.3.0/django_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.056987 ftw_django_utils-2023.3.0/django_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0      672 2022-11-16 16:36:40.057114 ftw_django_utils-2023.3.0/django_utils/management/commands/sentry_test.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.057217 ftw_django_utils-2023.3.0/django_utils/serializer/__init__.py
+-rw-r--r--   0        0        0       70 2022-11-16 16:36:40.057371 ftw_django_utils-2023.3.0/django_utils/serializer/fields/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-15 09:45:45.169971 ftw_django_utils-2023.3.0/django_utils/serializer/fields/protected_image_field.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.057710 ftw_django_utils-2023.3.0/django_utils/settings/__init__.py
+-rw-r--r--   0        0        0     2229 2023-02-03 13:51:24.363133 ftw_django_utils-2023.3.0/django_utils/settings/logging.py
+-rw-r--r--   0        0        0      989 2023-06-20 13:14:04.328261 ftw_django_utils-2023.3.0/django_utils/settings/sentry.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:36:40.058148 ftw_django_utils-2023.3.0/django_utils/testing/__init__.py
+-rw-r--r--   0        0        0      793 2022-11-16 16:36:40.058293 ftw_django_utils-2023.3.0/django_utils/testing/filestructure.py
+-rw-r--r--   0        0        0      358 2023-06-15 09:45:45.170051 ftw_django_utils-2023.3.0/django_utils/testing/urls.py
+-rw-r--r--   0        0        0     3701 2023-06-15 09:45:45.170138 ftw_django_utils-2023.3.0/django_utils/testing/views.py
+-rw-r--r--   0        0        0       55 2022-11-16 16:36:40.058730 ftw_django_utils-2023.3.0/django_utils/views/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-15 09:45:45.170242 ftw_django_utils-2023.3.0/django_utils/views/file_getter.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:45:45.170292 ftw_django_utils-2023.3.0/django_utils/webhooks/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:45:45.170348 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/__init__.py
+-rw-r--r--   0        0        0       98 2023-06-15 09:45:45.170404 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/default_delete_hooks.py
+-rw-r--r--   0        0        0      214 2023-06-15 09:45:45.170452 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/serializers.py
+-rw-r--r--   0        0        0     1158 2023-06-15 09:45:45.170506 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/token_authentication.py
+-rw-r--r--   0        0        0      259 2023-06-15 09:45:45.170553 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/urls.py
+-rw-r--r--   0        0        0     1837 2023-06-15 09:45:45.170602 ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/views.py
+-rw-r--r--   0        0        0     1403 2023-07-07 12:40:36.837641 ftw_django_utils-2023.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10732 1970-01-01 00:00:00.000000 ftw_django_utils-2023.3.0/PKG-INFO
```

### Comparing `ftw_django_utils-2023.2.0/LICENSE` & `ftw_django_utils-2023.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/README.md` & `ftw_django_utils-2023.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/authentication/__init__.py` & `ftw_django_utils-2023.3.0/django_utils/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/db/fields/text.py` & `ftw_django_utils-2023.3.0/django_utils/db/fields/text.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/management/commands/sentry_test.py` & `ftw_django_utils-2023.3.0/django_utils/management/commands/sentry_test.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/serializer/fields/protected_image_field.py` & `ftw_django_utils-2023.3.0/django_utils/serializer/fields/protected_image_field.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/settings/logging.py` & `ftw_django_utils-2023.3.0/django_utils/settings/logging.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/settings/sentry.py` & `ftw_django_utils-2023.3.0/django_utils/settings/sentry.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/testing/filestructure.py` & `ftw_django_utils-2023.3.0/django_utils/testing/filestructure.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/testing/views.py` & `ftw_django_utils-2023.3.0/django_utils/testing/views.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/views/file_getter.py` & `ftw_django_utils-2023.3.0/django_utils/views/file_getter.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/token_authentication.py` & `ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/token_authentication.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/django_utils/webhooks/delete_user/views.py` & `ftw_django_utils-2023.3.0/django_utils/webhooks/delete_user/views.py`

 * *Files identical despite different names*

### Comparing `ftw_django_utils-2023.2.0/pyproject.toml` & `ftw_django_utils-2023.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "ftw-django-utils"
-version = "2023.2.0"
+version = "2023.3.0"
 description = "A collection of utils used in our Django based web applications."
 authors = ["4teamwork AG"]
 readme = "README.md"
 packages = [{include = "django_utils"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4"
 django-configurations = "^2.4.1"
 django-extensions = "^3.2.1"
 sentry-sdk = "^1.21.0"
 djangorestframework = "^3"
-django = "^3"
+django = "*"
 django-sendfile2 = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 towncrier = "^22.12.0"
```

### Comparing `ftw_django_utils-2023.2.0/PKG-INFO` & `ftw_django_utils-2023.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ftw-django-utils
-Version: 2023.2.0
+Version: 2023.3.0
 Summary: A collection of utils used in our Django based web applications.
 Author: 4teamwork AG
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3,<4)
+Requires-Dist: django
 Requires-Dist: django-configurations (>=2.4.1,<3.0.0)
 Requires-Dist: django-extensions (>=3.2.1,<4.0.0)
 Requires-Dist: django-sendfile2 (>=0.7.0,<0.8.0)
 Requires-Dist: djangorestframework (>=3,<4)
 Requires-Dist: sentry-sdk (>=1.21.0,<2.0.0)
 Description-Content-Type: text/markdown
```

