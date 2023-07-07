# Comparing `tmp/django-authlib-0.9.6.tar.gz` & `tmp/django-authlib-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-authlib-0.9.6.tar", last modified: Tue Aug 11 16:59:30 2020, max compression
+gzip compressed data, was "dist/django-authlib-0.9.7.tar", last modified: Thu Sep 17 15:13:13 2020, max compression
```

## Comparing `django-authlib-0.9.6.tar` & `django-authlib-0.9.7.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.575408 django-authlib-0.9.6/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1078 2019-01-31 22:04:56.000000 django-authlib-0.9.6/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      109 2019-01-31 22:04:56.000000 django-authlib-0.9.6/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     8328 2020-08-11 16:59:30.575408 django-authlib-0.9.6/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6073 2019-01-31 22:06:15.000000 django-authlib-0.9.6/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2020-08-11 16:58:28.000000 django-authlib-0.9.6/authlib/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/admin_oauth/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      666 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/admin_oauth/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1027 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/admin_oauth/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/admin_oauth/templates/admin/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      654 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/admin_oauth/templates/admin/login.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      165 2020-06-05 11:37:17.000000 django-authlib-0.9.6/authlib/admin_oauth/urls.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1921 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/admin_oauth/views.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      479 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/backends.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1465 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/base_user.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4848 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/email.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1392 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/facebook.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1716 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/google.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/little_auth/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       65 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      684 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/admin.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/apps.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/little_auth/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/little_auth/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/little_auth/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      771 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/little_auth/migrations/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3388 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/migrations/0001_initial.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/little_auth/migrations/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2020-08-11 16:51:00.000000 django-authlib-0.9.6/authlib/little_auth/models.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.565408 django-authlib-0.9.6/authlib/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1578 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2460 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2020-04-27 07:16:39.000000 django-authlib-0.9.6/authlib/normalize.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2449 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/twitter.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6059 2020-06-04 09:21:24.000000 django-authlib-0.9.6/authlib/views.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-08-11 16:59:30.575408 django-authlib-0.9.6/django_authlib.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     8328 2020-08-11 16:59:30.000000 django-authlib-0.9.6/django_authlib.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1081 2020-08-11 16:59:30.000000 django-authlib-0.9.6/django_authlib.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2020-08-11 16:59:30.000000 django-authlib-0.9.6/django_authlib.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2020-03-08 17:10:25.000000 django-authlib-0.9.6/django_authlib.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       18 2020-08-11 16:59:30.000000 django-authlib-0.9.6/django_authlib.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        8 2020-08-11 16:59:30.000000 django-authlib-0.9.6/django_authlib.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      292 2020-08-11 16:59:30.575408 django-authlib-0.9.6/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)     1223 2020-08-11 16:53:56.000000 django-authlib-0.9.6/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1078 2020-02-14 21:38:54.000000 django-authlib-0.9.7/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      109 2020-02-14 21:38:54.000000 django-authlib-0.9.7/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     8328 2020-09-17 15:13:13.030000 django-authlib-0.9.7/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6073 2020-02-14 21:38:54.000000 django-authlib-0.9.7/README.rst
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2020-09-17 15:12:33.000000 django-authlib-0.9.7/authlib/__init__.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/admin_oauth/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/admin_oauth/__init__.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/admin_oauth/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/admin_oauth/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/admin_oauth/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      666 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/admin_oauth/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1027 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/admin_oauth/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/admin_oauth/templates/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/admin_oauth/templates/admin/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      654 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/admin_oauth/templates/admin/login.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      165 2020-07-24 16:01:42.000000 django-authlib-0.9.7/authlib/admin_oauth/urls.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1921 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/admin_oauth/views.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      479 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/backends.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1465 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/base_user.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4848 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/email.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1392 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/facebook.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1724 2020-09-17 15:11:29.000000 django-authlib-0.9.7/authlib/google.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/little_auth/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       65 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      684 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/admin.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/apps.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/little_auth/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/little_auth/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/little_auth/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      771 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/little_auth/migrations/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3388 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/migrations/0001_initial.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/little_auth/migrations/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      771 2020-09-17 15:10:58.000000 django-authlib-0.9.7/authlib/little_auth/models.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.020000 django-authlib-0.9.7/authlib/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/authlib/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1578 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2460 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2449 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/twitter.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6059 2020-02-17 19:32:57.000000 django-authlib-0.9.7/authlib/views.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2020-09-17 15:13:13.030000 django-authlib-0.9.7/django_authlib.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     8328 2020-09-17 15:13:12.000000 django-authlib-0.9.7/django_authlib.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1060 2020-09-17 15:13:12.000000 django-authlib-0.9.7/django_authlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2020-09-17 15:13:12.000000 django-authlib-0.9.7/django_authlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2020-03-05 16:29:51.000000 django-authlib-0.9.7/django_authlib.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       18 2020-09-17 15:13:12.000000 django-authlib-0.9.7/django_authlib.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        8 2020-09-17 15:13:12.000000 django-authlib-0.9.7/django_authlib.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      292 2020-09-17 15:13:13.040000 django-authlib-0.9.7/setup.cfg
+-rwxrwxr-x   0 matthias  (1000) matthias  (1000)     1223 2020-09-17 15:10:42.000000 django-authlib-0.9.7/setup.py
```

### Comparing `django-authlib-0.9.6/LICENSE` & `django-authlib-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/PKG-INFO` & `django-authlib-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-authlib
-Version: 0.9.6
+Version: 0.9.7
 Summary: Authentication utils for Django
 Home-page: http://github.com/matthiask/django-authlib/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: MIT License
 Description: ================================================
         django-authlib - Authentication utils for Django
```

### Comparing `django-authlib-0.9.6/README.rst` & `django-authlib-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/admin_oauth/locale/de/LC_MESSAGES/django.mo` & `django-authlib-0.9.7/authlib/admin_oauth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/admin_oauth/locale/de/LC_MESSAGES/django.po` & `django-authlib-0.9.7/authlib/admin_oauth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/admin_oauth/templates/admin/login.html` & `django-authlib-0.9.7/authlib/admin_oauth/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/admin_oauth/views.py` & `django-authlib-0.9.7/authlib/admin_oauth/views.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/base_user.py` & `django-authlib-0.9.7/authlib/base_user.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/email.py` & `django-authlib-0.9.7/authlib/email.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/facebook.py` & `django-authlib-0.9.7/authlib/facebook.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/google.py` & `django-authlib-0.9.7/authlib/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 class GoogleOAuth2Client(object):
     authorization_base_url = "https://accounts.google.com/o/oauth2/v2/auth"
     token_url = "https://www.googleapis.com/oauth2/v4/token"
     scope = ["openid", "email", "profile"]
     client_id = settings.GOOGLE_CLIENT_ID
     client_secret = settings.GOOGLE_CLIENT_SECRET
 
-    def __init__(self, request, *, login_hint=None, authorization_params={}):
+    def __init__(self, request, *, login_hint=None, authorization_params=None):
         # let oauthlib be less strict on scope mismatch
         os.environ["OAUTHLIB_RELAX_TOKEN_SCOPE"] = "1"
 
         self._request = request
         self._session = OAuth2Session(
             self.client_id,
             scope=self.scope,
             redirect_uri=request.build_absolute_uri("."),
         )
         self._login_hint = login_hint
-        self._authorization_params = authorization_params
+        self._authorization_params = authorization_params or {}
 
     def get_authentication_url(self):
         self._authorization_params.setdefault("login_hint", self._login_hint)
         authorization_url, self._state = self._session.authorization_url(
             self.authorization_base_url, **self._authorization_params
         )
```

### Comparing `django-authlib-0.9.6/authlib/little_auth/admin.py` & `django-authlib-0.9.7/authlib/little_auth/admin.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/little_auth/locale/de/LC_MESSAGES/django.po` & `django-authlib-0.9.7/authlib/little_auth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/little_auth/migrations/0001_initial.py` & `django-authlib-0.9.7/authlib/little_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/little_auth/models.py` & `django-authlib-0.9.7/authlib/little_auth/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from authlib.base_user import BaseUser
 
 
 def _obfuscate(email):
     user, _sep, domain = email.partition("@")
     return (
         "%s%s@***.%s"
-        % (user[:3], "***" if len(user) > 3 else "", domain.rsplit(".", 1)[-1],)
+        % (
+            user[:3],
+            "***" if len(user) > 3 else "",
+            domain.rsplit(".", 1)[-1],
+        )
         if domain
         else "%s***" % (user[:3],)
     )
 
 
 class User(BaseUser):
     full_name = models.CharField(_("full name"), max_length=200)
```

### Comparing `django-authlib-0.9.6/authlib/locale/de/LC_MESSAGES/django.mo` & `django-authlib-0.9.7/authlib/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/locale/de/LC_MESSAGES/django.po` & `django-authlib-0.9.7/authlib/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/twitter.py` & `django-authlib-0.9.7/authlib/twitter.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/authlib/views.py` & `django-authlib-0.9.7/authlib/views.py`

 * *Files identical despite different names*

### Comparing `django-authlib-0.9.6/django_authlib.egg-info/PKG-INFO` & `django-authlib-0.9.7/django_authlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-authlib
-Version: 0.9.6
+Version: 0.9.7
 Summary: Authentication utils for Django
 Home-page: http://github.com/matthiask/django-authlib/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: MIT License
 Description: ================================================
         django-authlib - Authentication utils for Django
```

### Comparing `django-authlib-0.9.6/django_authlib.egg-info/SOURCES.txt` & `django-authlib-0.9.7/django_authlib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.py
 authlib/__init__.py
 authlib/backends.py
 authlib/base_user.py
 authlib/email.py
 authlib/facebook.py
 authlib/google.py
-authlib/normalize.py
 authlib/twitter.py
 authlib/views.py
 authlib/admin_oauth/__init__.py
 authlib/admin_oauth/urls.py
 authlib/admin_oauth/views.py
 authlib/admin_oauth/locale/de/LC_MESSAGES/django.mo
 authlib/admin_oauth/locale/de/LC_MESSAGES/django.po
```

### Comparing `django-authlib-0.9.6/setup.py` & `django-authlib-0.9.7/setup.py`

 * *Files identical despite different names*

