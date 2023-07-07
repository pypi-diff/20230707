# Comparing `tmp/django-stdimage2-0.1.12.tar.gz` & `tmp/django-stdimage2-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stdimage2-0.1.12.tar", last modified: Fri Jul  7 07:42:08 2023, max compression
+gzip compressed data, was "django-stdimage2-0.1.13.tar", last modified: Fri Jul  7 07:42:45 2023, max compression
```

## Comparing `django-stdimage2-0.1.12.tar` & `django-stdimage2-0.1.13.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/
--rw-rw-r--   0 username  (1000) username  (1000)       58 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/FUNDING.yml
--rw-rw-r--   0 username  (1000) username  (1000)     1081 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/LICENSE
--rw-rw-r--   0 username  (1000) username  (1000)      165 2023-07-06 12:34:18.000000 django-stdimage2-0.1.12/MANIFEST.in
--rw-rw-r--   0 username  (1000) username  (1000)     9404 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/PKG-INFO
--rw-rw-r--   0 username  (1000) username  (1000)     8209 2023-07-06 12:20:56.000000 django-stdimage2-0.1.12/README.md
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/django_stdimage2.egg-info/
--rw-rw-r--   0 username  (1000) username  (1000)     9404 2023-07-07 07:42:08.000000 django-stdimage2-0.1.12/django_stdimage2.egg-info/PKG-INFO
--rw-rw-r--   0 username  (1000) username  (1000)      642 2023-07-07 07:42:08.000000 django-stdimage2-0.1.12/django_stdimage2.egg-info/SOURCES.txt
--rw-rw-r--   0 username  (1000) username  (1000)        1 2023-07-07 07:42:08.000000 django-stdimage2-0.1.12/django_stdimage2.egg-info/dependency_links.txt
--rw-rw-r--   0 username  (1000) username  (1000)       99 2023-07-07 07:42:08.000000 django-stdimage2-0.1.12/django_stdimage2.egg-info/requires.txt
--rw-rw-r--   0 username  (1000) username  (1000)       10 2023-07-07 07:42:08.000000 django-stdimage2-0.1.12/django_stdimage2.egg-info/top_level.txt
--rw-rw-r--   0 username  (1000) username  (1000)     2112 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/setup.cfg
--rwxrwxr-x   0 username  (1000) username  (1000)     1566 2023-07-07 07:42:04.000000 django-stdimage2-0.1.12/setup.py
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/
--rw-rw-r--   0 username  (1000) username  (1000)       53 2023-07-06 12:34:16.000000 django-stdimage2-0.1.12/stdimage2/__init__.py
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.133315 django-stdimage2-0.1.12/stdimage2/locale/
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.133315 django-stdimage2-0.1.12/stdimage2/locale/de/
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/locale/de/LC_MESSAGES/
--rw-rw-r--   0 username  (1000) username  (1000)     1106 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.133315 django-stdimage2-0.1.12/stdimage2/locale/fr/
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 username  (1000) username  (1000)     1108 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.133315 django-stdimage2-0.1.12/stdimage2/locale/sr/
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 username  (1000) username  (1000)     1231 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.133315 django-stdimage2-0.1.12/stdimage2/locale/sr_Latn/
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/locale/sr_Latn/LC_MESSAGES/
--rw-rw-r--   0 username  (1000) username  (1000)     1140 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/locale/sr_Latn/LC_MESSAGES/django.po
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/management/
--rw-rw-r--   0 username  (1000) username  (1000)        0 2023-07-06 12:34:17.000000 django-stdimage2-0.1.12/stdimage2/management/__init__.py
-drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:08.137315 django-stdimage2-0.1.12/stdimage2/management/commands/
--rw-rw-r--   0 username  (1000) username  (1000)        0 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/management/commands/__init__.py
--rw-rw-r--   0 username  (1000) username  (1000)     4057 2023-07-06 12:20:56.000000 django-stdimage2-0.1.12/stdimage2/management/commands/rendervariations.py
--rw-rw-r--   0 username  (1000) username  (1000)    14422 2023-07-06 12:20:56.000000 django-stdimage2-0.1.12/stdimage2/models.py
--rw-rw-r--   0 username  (1000) username  (1000)      409 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/utils.py
--rw-rw-r--   0 username  (1000) username  (1000)     1907 2023-07-06 11:49:43.000000 django-stdimage2-0.1.12/stdimage2/validators.py
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/
+-rw-rw-r--   0 username  (1000) username  (1000)       58 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/FUNDING.yml
+-rw-rw-r--   0 username  (1000) username  (1000)     1081 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/LICENSE
+-rw-rw-r--   0 username  (1000) username  (1000)      165 2023-07-06 12:34:18.000000 django-stdimage2-0.1.13/MANIFEST.in
+-rw-rw-r--   0 username  (1000) username  (1000)     9404 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/PKG-INFO
+-rw-rw-r--   0 username  (1000) username  (1000)     8209 2023-07-06 12:20:56.000000 django-stdimage2-0.1.13/README.md
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/django_stdimage2.egg-info/
+-rw-rw-r--   0 username  (1000) username  (1000)     9404 2023-07-07 07:42:45.000000 django-stdimage2-0.1.13/django_stdimage2.egg-info/PKG-INFO
+-rw-rw-r--   0 username  (1000) username  (1000)      642 2023-07-07 07:42:45.000000 django-stdimage2-0.1.13/django_stdimage2.egg-info/SOURCES.txt
+-rw-rw-r--   0 username  (1000) username  (1000)        1 2023-07-07 07:42:45.000000 django-stdimage2-0.1.13/django_stdimage2.egg-info/dependency_links.txt
+-rw-rw-r--   0 username  (1000) username  (1000)       99 2023-07-07 07:42:45.000000 django-stdimage2-0.1.13/django_stdimage2.egg-info/requires.txt
+-rw-rw-r--   0 username  (1000) username  (1000)       10 2023-07-07 07:42:45.000000 django-stdimage2-0.1.13/django_stdimage2.egg-info/top_level.txt
+-rw-rw-r--   0 username  (1000) username  (1000)     2112 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/setup.cfg
+-rwxrwxr-x   0 username  (1000) username  (1000)     1566 2023-07-07 07:42:43.000000 django-stdimage2-0.1.13/setup.py
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/
+-rw-rw-r--   0 username  (1000) username  (1000)       53 2023-07-06 12:34:16.000000 django-stdimage2-0.1.13/stdimage2/__init__.py
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.181989 django-stdimage2-0.1.13/stdimage2/locale/
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.181989 django-stdimage2-0.1.13/stdimage2/locale/de/
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 username  (1000) username  (1000)     1106 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.181989 django-stdimage2-0.1.13/stdimage2/locale/fr/
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 username  (1000) username  (1000)     1108 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.181989 django-stdimage2-0.1.13/stdimage2/locale/sr/
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 username  (1000) username  (1000)     1231 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/locale/sr/LC_MESSAGES/django.po
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.181989 django-stdimage2-0.1.13/stdimage2/locale/sr_Latn/
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/locale/sr_Latn/LC_MESSAGES/
+-rw-rw-r--   0 username  (1000) username  (1000)     1140 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/locale/sr_Latn/LC_MESSAGES/django.po
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/management/
+-rw-rw-r--   0 username  (1000) username  (1000)        0 2023-07-06 12:34:17.000000 django-stdimage2-0.1.13/stdimage2/management/__init__.py
+drwxrwxr-x   0 username  (1000) username  (1000)        0 2023-07-07 07:42:45.185989 django-stdimage2-0.1.13/stdimage2/management/commands/
+-rw-rw-r--   0 username  (1000) username  (1000)        0 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/management/commands/__init__.py
+-rw-rw-r--   0 username  (1000) username  (1000)     4057 2023-07-06 12:20:56.000000 django-stdimage2-0.1.13/stdimage2/management/commands/rendervariations.py
+-rw-rw-r--   0 username  (1000) username  (1000)    14422 2023-07-06 12:20:56.000000 django-stdimage2-0.1.13/stdimage2/models.py
+-rw-rw-r--   0 username  (1000) username  (1000)      409 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/utils.py
+-rw-rw-r--   0 username  (1000) username  (1000)     1907 2023-07-06 11:49:43.000000 django-stdimage2-0.1.13/stdimage2/validators.py
```

### Comparing `django-stdimage2-0.1.12/LICENSE` & `django-stdimage2-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/PKG-INFO` & `django-stdimage2-0.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stdimage2
-Version: 0.1.12
+Version: 0.1.13
 Summary: Django Standarized Image Field
 Home-page: https://github.com/codingjoe/django-stdimage2
 Author: Johannes Hoppe
 Author-email: info@johanneshoppe.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 7 - Inactive
```

### Comparing `django-stdimage2-0.1.12/README.md` & `django-stdimage2-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/django_stdimage2.egg-info/PKG-INFO` & `django-stdimage2-0.1.13/django_stdimage2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stdimage2
-Version: 0.1.12
+Version: 0.1.13
 Summary: Django Standarized Image Field
 Home-page: https://github.com/codingjoe/django-stdimage2
 Author: Johannes Hoppe
 Author-email: info@johanneshoppe.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 7 - Inactive
```

### Comparing `django-stdimage2-0.1.12/django_stdimage2.egg-info/SOURCES.txt` & `django-stdimage2-0.1.13/django_stdimage2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/setup.cfg` & `django-stdimage2-0.1.13/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/setup.py` & `django-stdimage2-0.1.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,14 @@
         ("compile_translations", None),
     ]
 
 
 setup(
     name="django-stdimage2",
     # use_scm_version=True,
-    version='0.1.12',
+    version='0.1.13',
     cmdclass={
         "build": build,
         "install": install,
         "compile_translations": compile_translations,
     },
 )
```

### Comparing `django-stdimage2-0.1.12/stdimage2/locale/de/LC_MESSAGES/django.po` & `django-stdimage2-0.1.13/stdimage2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/locale/fr/LC_MESSAGES/django.po` & `django-stdimage2-0.1.13/stdimage2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/locale/sr/LC_MESSAGES/django.po` & `django-stdimage2-0.1.13/stdimage2/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/locale/sr_Latn/LC_MESSAGES/django.po` & `django-stdimage2-0.1.13/stdimage2/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/management/commands/rendervariations.py` & `django-stdimage2-0.1.13/stdimage2/management/commands/rendervariations.py`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/models.py` & `django-stdimage2-0.1.13/stdimage2/models.py`

 * *Files identical despite different names*

### Comparing `django-stdimage2-0.1.12/stdimage2/validators.py` & `django-stdimage2-0.1.13/stdimage2/validators.py`

 * *Files identical despite different names*

