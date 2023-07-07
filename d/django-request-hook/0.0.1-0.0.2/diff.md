# Comparing `tmp/django-request-hook-0.0.1.tar.gz` & `tmp/django-request-hook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-request-hook-0.0.1.tar", last modified: Thu Jul  6 12:43:12 2023, max compression
+gzip compressed data, was "django-request-hook-0.0.2.tar", last modified: Fri Jul  7 07:17:27 2023, max compression
```

## Comparing `django-request-hook-0.0.1.tar` & `django-request-hook-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-06 12:43:12.305693 django-request-hook-0.0.1/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     1063 2023-07-06 08:58:06.000000 django-request-hook-0.0.1/LICENSE
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-07-06 09:44:31.000000 django-request-hook-0.0.1/MANIFEST.in
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2327 2023-07-06 12:43:12.305261 django-request-hook-0.0.1/PKG-INFO
--rw-r--r--   0 huangjianglin   (501) staff       (20)      554 2023-07-06 09:43:45.000000 django-request-hook-0.0.1/README.md
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-06 12:43:12.300201 django-request-hook-0.0.1/django_request_hook/
--rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-07-06 08:57:09.000000 django-request-hook-0.0.1/django_request_hook/__init__.py
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2038 2023-07-06 09:57:50.000000 django-request-hook-0.0.1/django_request_hook/middleware.py
-drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-06 12:43:12.304296 django-request-hook-0.0.1/django_request_hook.egg-info/
--rw-r--r--   0 huangjianglin   (501) staff       (20)     2327 2023-07-06 12:43:12.000000 django-request-hook-0.0.1/django_request_hook.egg-info/PKG-INFO
--rw-r--r--   0 huangjianglin   (501) staff       (20)      324 2023-07-06 12:43:12.000000 django-request-hook-0.0.1/django_request_hook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-07-06 12:43:12.000000 django-request-hook-0.0.1/django_request_hook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)       43 2023-07-06 12:43:12.000000 django-request-hook-0.0.1/django_request_hook.egg-info/requires.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)       20 2023-07-06 12:43:12.000000 django-request-hook-0.0.1/django_request_hook.egg-info/top_level.txt
--rw-r--r--   0 huangjianglin   (501) staff       (20)      825 2023-07-06 10:00:35.000000 django-request-hook-0.0.1/pyproject.toml
--rw-r--r--   0 huangjianglin   (501) staff       (20)       38 2023-07-06 12:43:12.305847 django-request-hook-0.0.1/setup.cfg
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-07 07:17:27.261492 django-request-hook-0.0.2/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     1063 2023-07-06 08:58:06.000000 django-request-hook-0.0.2/LICENSE
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-07-06 09:44:31.000000 django-request-hook-0.0.2/MANIFEST.in
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2325 2023-07-07 07:17:27.259774 django-request-hook-0.0.2/PKG-INFO
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      554 2023-07-06 09:43:45.000000 django-request-hook-0.0.2/README.md
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-07 07:17:27.249898 django-request-hook-0.0.2/django_request_hook/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        0 2023-07-06 08:57:09.000000 django-request-hook-0.0.2/django_request_hook/__init__.py
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2038 2023-07-06 09:57:50.000000 django-request-hook-0.0.2/django_request_hook/middleware.py
+drwxr-xr-x   0 huangjianglin   (501) staff       (20)        0 2023-07-07 07:17:27.252776 django-request-hook-0.0.2/django_request_hook.egg-info/
+-rw-r--r--   0 huangjianglin   (501) staff       (20)     2325 2023-07-07 07:17:27.000000 django-request-hook-0.0.2/django_request_hook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      324 2023-07-07 07:17:27.000000 django-request-hook-0.0.2/django_request_hook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)        1 2023-07-07 07:17:27.000000 django-request-hook-0.0.2/django_request_hook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       37 2023-07-07 07:17:27.000000 django-request-hook-0.0.2/django_request_hook.egg-info/requires.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       20 2023-07-07 07:17:27.000000 django-request-hook-0.0.2/django_request_hook.egg-info/top_level.txt
+-rw-r--r--   0 huangjianglin   (501) staff       (20)      815 2023-07-07 07:13:22.000000 django-request-hook-0.0.2/pyproject.toml
+-rw-r--r--   0 huangjianglin   (501) staff       (20)       38 2023-07-07 07:17:27.261599 django-request-hook-0.0.2/setup.cfg
```

### Comparing `django-request-hook-0.0.1/LICENSE` & `django-request-hook-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-request-hook-0.0.1/PKG-INFO` & `django-request-hook-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-request-hook
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django middlewares to track request logs
 Author-email: joneai <mxjoneai@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Joneai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/tacnaci/django-request-hook
 Keywords: django,request log,hook,api log track,middleware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Django Request Hook
 
 Django middlewares to track request/response logs. Catch the logs and send it to anywhere you want through HTTP.
```

### Comparing `django-request-hook-0.0.1/README.md` & `django-request-hook-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-request-hook-0.0.1/django_request_hook/middleware.py` & `django-request-hook-0.0.2/django_request_hook/middleware.py`

 * *Files identical despite different names*

### Comparing `django-request-hook-0.0.1/django_request_hook.egg-info/PKG-INFO` & `django-request-hook-0.0.2/django_request_hook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-request-hook
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django middlewares to track request logs
 Author-email: joneai <mxjoneai@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Joneai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/tacnaci/django-request-hook
 Keywords: django,request log,hook,api log track,middleware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Django Request Hook
 
 Django middlewares to track request/response logs. Catch the logs and send it to anywhere you want through HTTP.
```

### Comparing `django-request-hook-0.0.1/pyproject.toml` & `django-request-hook-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-request-hook"
-version = "0.0.1"
+version = "0.0.2"
 description = "Django middlewares to track request logs"
 readme = "README.md"
 authors = [{ name = "joneai", email = "mxjoneai@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["django", "request log", "hook", "api log track", "middleware"]
 dependencies = [
-    "Django >= 4.2",
-    "requests >= 2.31.0",
+    "Django >= 2.0.0",
+    "requests",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3"
 
 [project.optional-dependencies]
 dev = ["pytest"]
 
 [project.urls]
 Homepage = "https://github.com/tacnaci/django-request-hook"
```

