# Comparing `tmp/django_titofisto-1.0.0.tar.gz` & `tmp/django_titofisto-1.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_titofisto-1.0.0.tar", max compression
+gzip compressed data, was "django_titofisto-1.0.0.post0.tar", max compression
```

## Comparing `django_titofisto-1.0.0.tar` & `django_titofisto-1.0.0.post0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1737 2023-07-07 19:37:58.513308 django_titofisto-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11373 2021-12-07 10:10:52.592509 django_titofisto-1.0.0/LICENSE
--rw-r--r--   0        0        0     4519 2023-07-07 20:07:12.751646 django_titofisto-1.0.0/README.rst
--rw-r--r--   0        0        0      863 2023-07-07 20:16:42.207155 django_titofisto-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       38 2021-12-07 10:10:52.592509 django_titofisto-1.0.0/titofisto/__init__.py
--rw-r--r--   0        0        0      472 2023-07-07 19:50:59.996547 django_titofisto-1.0.0/titofisto/settings.py
--rw-r--r--   0        0        0     1672 2023-07-07 17:40:15.939074 django_titofisto-1.0.0/titofisto/storage.py
--rw-r--r--   0        0        0      733 2023-07-07 19:51:17.780528 django_titofisto-1.0.0/titofisto/test_settings.py
--rw-r--r--   0        0        0      165 2023-07-07 17:48:02.146669 django_titofisto-1.0.0/titofisto/test_urls.py
--rw-r--r--   0        0        0     7870 2023-07-07 20:12:59.283346 django_titofisto-1.0.0/titofisto/tests.py
--rw-r--r--   0        0        0      460 2023-07-07 18:57:09.038691 django_titofisto-1.0.0/titofisto/urls.py
--rw-r--r--   0        0        0     3948 2023-07-07 20:11:36.535417 django_titofisto-1.0.0/titofisto/views.py
--rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 django_titofisto-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1737 2023-07-07 20:17:56.135063 django_titofisto-1.0.0.post0/CHANGELOG.md
+-rw-r--r--   0        0        0    11373 2021-12-07 10:10:52.592509 django_titofisto-1.0.0.post0/LICENSE
+-rw-r--r--   0        0        0     4519 2023-07-07 20:07:12.751646 django_titofisto-1.0.0.post0/README.rst
+-rw-r--r--   0        0        0      869 2023-07-07 20:18:08.079040 django_titofisto-1.0.0.post0/pyproject.toml
+-rw-r--r--   0        0        0       38 2021-12-07 10:10:52.592509 django_titofisto-1.0.0.post0/titofisto/__init__.py
+-rw-r--r--   0        0        0      472 2023-07-07 19:50:59.996547 django_titofisto-1.0.0.post0/titofisto/settings.py
+-rw-r--r--   0        0        0     1672 2023-07-07 17:40:15.939074 django_titofisto-1.0.0.post0/titofisto/storage.py
+-rw-r--r--   0        0        0      733 2023-07-07 19:51:17.780528 django_titofisto-1.0.0.post0/titofisto/test_settings.py
+-rw-r--r--   0        0        0      165 2023-07-07 17:48:02.146669 django_titofisto-1.0.0.post0/titofisto/test_urls.py
+-rw-r--r--   0        0        0     7870 2023-07-07 20:12:59.283346 django_titofisto-1.0.0.post0/titofisto/tests.py
+-rw-r--r--   0        0        0      460 2023-07-07 18:57:09.038691 django_titofisto-1.0.0.post0/titofisto/urls.py
+-rw-r--r--   0        0        0     3948 2023-07-07 20:11:36.535417 django_titofisto-1.0.0.post0/titofisto/views.py
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 django_titofisto-1.0.0.post0/PKG-INFO
```

### Comparing `django_titofisto-1.0.0/CHANGELOG.md` & `django_titofisto-1.0.0.post0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.3.0] - 2023-07-07
+## [1.0.0] - 2023-07-07
 ### Added
 - Time-constrained upload slot handling
 
 ### Changed
 - Use Django's Signer for token generation and verification
 
 ## [0.2.2] - 2022-02-03
@@ -44,8 +44,8 @@
 [0.1.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.0
 [0.1.1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.1
 [0.1.2]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.2
 [0.1.2.post1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.1.2.post1
 [0.2.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.0
 [0.2.1]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.1
 [0.2.2]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.2.2
-[0.3.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/0.3.0
+[1.0.0]: https://edugit.org/AlekSIS/libs/django-titofisto/-/tags/1.0.0
```

### Comparing `django_titofisto-1.0.0/LICENSE` & `django_titofisto-1.0.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/README.rst` & `django_titofisto-1.0.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/pyproject.toml` & `django_titofisto-1.0.0.post0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-titofisto"
-version = "1.0.0"
+version = "1.0.0.post0"
 description = "Django Time-Token File Storage"
 authors = ["Dominik George <dominik.george@teckids.org>", "Jonathan Weth <dev@jonathanweth.de>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://edugit.org/AlekSIS/libs/django-titofisto"
 keywords = ["django", "storage", "media", "secure"]
 classifiers = [
```

### Comparing `django_titofisto-1.0.0/titofisto/storage.py` & `django_titofisto-1.0.0.post0/titofisto/storage.py`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/titofisto/test_settings.py` & `django_titofisto-1.0.0.post0/titofisto/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/titofisto/tests.py` & `django_titofisto-1.0.0.post0/titofisto/tests.py`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/titofisto/views.py` & `django_titofisto-1.0.0.post0/titofisto/views.py`

 * *Files identical despite different names*

### Comparing `django_titofisto-1.0.0/PKG-INFO` & `django_titofisto-1.0.0.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-titofisto
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: Django Time-Token File Storage
 Home-page: https://edugit.org/AlekSIS/libs/django-titofisto
 License: Apache-2.0
 Keywords: django,storage,media,secure
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
```

