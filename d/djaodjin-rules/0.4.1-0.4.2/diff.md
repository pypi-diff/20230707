# Comparing `tmp/djaodjin-rules-0.4.1.tar.gz` & `tmp/djaodjin-rules-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-rules-0.4.1.tar", last modified: Fri Dec 16 04:58:02 2022, max compression
+gzip compressed data, was "djaodjin-rules-0.4.2.tar", last modified: Fri Jul  7 15:04:57 2023, max compression
```

## Comparing `djaodjin-rules-0.4.1.tar` & `djaodjin-rules-0.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.513462 djaodjin-rules-0.4.1/
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1759 2022-12-16 04:58:02.513341 djaodjin-rules-0.4.1/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1420 2022-12-16 04:56:17.000000 djaodjin-rules-0.4.1/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.505772 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1759 2022-12-16 04:58:02.000000 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1031 2022-12-16 04:58:02.000000 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2022-12-16 04:58:02.000000 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      109 2022-12-16 04:58:02.000000 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        6 2022-12-16 04:58:02.000000 djaodjin-rules-0.4.1/djaodjin_rules.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      109 2022-11-15 18:07:07.000000 djaodjin-rules-0.4.1/requirements.txt
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.508618 djaodjin-rules-0.4.1/rules/
--rw-r--r--   0 smirolo    (501) staff       (20)     1434 2022-12-16 04:56:31.000000 djaodjin-rules-0.4.1/rules/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.509733 djaodjin-rules-0.4.1/rules/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4627 2022-11-22 21:34:31.000000 djaodjin-rules-0.4.1/rules/api/keys.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14588 2022-11-23 08:32:55.000000 djaodjin-rules-0.4.1/rules/api/rules.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8966 2022-11-22 21:34:56.000000 djaodjin-rules-0.4.1/rules/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3520 2022-08-18 22:52:58.000000 djaodjin-rules-0.4.1/rules/api/sessions.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4116 2022-11-22 21:39:21.000000 djaodjin-rules-0.4.1/rules/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2787 2022-11-22 20:39:30.000000 djaodjin-rules-0.4.1/rules/decorators.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3493 2022-11-22 20:38:03.000000 djaodjin-rules-0.4.1/rules/extras.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7975 2022-12-16 04:52:23.000000 djaodjin-rules-0.4.1/rules/middleware.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7435 2022-11-04 16:48:37.000000 djaodjin-rules-0.4.1/rules/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11898 2022-11-22 21:38:55.000000 djaodjin-rules-0.4.1/rules/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8463 2022-11-22 21:17:58.000000 djaodjin-rules-0.4.1/rules/perms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6317 2022-11-22 21:23:14.000000 djaodjin-rules-0.4.1/rules/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1543 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.504568 djaodjin-rules-0.4.1/rules/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.510633 djaodjin-rules-0.4.1/rules/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    50139 2022-12-07 06:05:31.000000 djaodjin-rules-0.4.1/rules/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     4881 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/static/js/djaodjin-resources.js
--rw-r--r--   0 smirolo    (501) staff       (20)     9738 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/static/js/djaodjin-rules-angular.js
--rw-r--r--   0 smirolo    (501) staff       (20)     8414 2022-11-15 17:57:27.000000 djaodjin-rules-0.4.1/rules/static/js/djaodjin-rules-vue.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.504660 djaodjin-rules-0.4.1/rules/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.511335 djaodjin-rules-0.4.1/rules/templates/rules/
--rw-r--r--   0 smirolo    (501) staff       (20)     9020 2022-11-15 17:53:58.000000 djaodjin-rules-0.4.1/rules/templates/rules/app_dashboard.html
--rw-r--r--   0 smirolo    (501) staff       (20)      949 2022-11-15 18:47:22.000000 djaodjin-rules-0.4.1/rules/templates/rules/engagement.html
--rw-r--r--   0 smirolo    (501) staff       (20)      751 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/templates/rules/forward_error.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9160 2022-11-22 21:38:20.000000 djaodjin-rules-0.4.1/rules/urldecorators.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.511755 djaodjin-rules-0.4.1/rules/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1551 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.512140 djaodjin-rules-0.4.1/rules/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1477 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2528 2022-08-10 04:42:14.000000 djaodjin-rules-0.4.1/rules/urls/api/proxy.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1513 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/rules/urls/apply.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1803 2022-11-16 20:10:48.000000 djaodjin-rules-0.4.1/rules/urls/configure.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4604 2022-11-22 21:01:08.000000 djaodjin-rules-0.4.1/rules/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2022-12-16 04:58:02.513014 djaodjin-rules-0.4.1/rules/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1763 2022-11-22 20:38:48.000000 djaodjin-rules-0.4.1/rules/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    18928 2022-11-16 20:12:05.000000 djaodjin-rules-0.4.1/rules/views/app.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4413 2022-11-22 21:34:13.000000 djaodjin-rules-0.4.1/rules/views/download.py
--rw-r--r--   0 smirolo    (501) staff       (20)       38 2022-12-16 04:58:02.513497 djaodjin-rules-0.4.1/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     2374 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.1/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.321417 djaodjin-rules-0.4.2/
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     2010 2023-07-07 15:04:57.321287 djaodjin-rules-0.4.2/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1251 2023-07-07 13:28:17.000000 djaodjin-rules-0.4.2/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.316909 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2010 2023-07-07 15:04:57.000000 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1029 2023-07-07 15:04:57.000000 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-07-07 15:04:57.000000 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      109 2023-07-07 15:04:57.000000 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        6 2023-07-07 15:04:57.000000 djaodjin-rules-0.4.2/djaodjin_rules.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1342 2023-07-07 13:20:24.000000 djaodjin-rules-0.4.2/pyproject.toml
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.318524 djaodjin-rules-0.4.2/rules/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1434 2023-07-07 15:04:02.000000 djaodjin-rules-0.4.2/rules/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.319139 djaodjin-rules-0.4.2/rules/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4627 2022-11-22 21:34:31.000000 djaodjin-rules-0.4.2/rules/api/keys.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14588 2023-07-07 14:46:04.000000 djaodjin-rules-0.4.2/rules/api/rules.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8966 2022-11-22 21:34:56.000000 djaodjin-rules-0.4.2/rules/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3520 2022-08-18 22:52:58.000000 djaodjin-rules-0.4.2/rules/api/sessions.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4116 2022-11-22 21:39:21.000000 djaodjin-rules-0.4.2/rules/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2787 2022-11-22 20:39:30.000000 djaodjin-rules-0.4.2/rules/decorators.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3493 2022-11-22 20:38:03.000000 djaodjin-rules-0.4.2/rules/extras.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7975 2023-03-24 18:42:51.000000 djaodjin-rules-0.4.2/rules/middleware.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7435 2022-11-04 16:48:37.000000 djaodjin-rules-0.4.2/rules/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11898 2022-11-22 21:38:55.000000 djaodjin-rules-0.4.2/rules/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8463 2022-11-22 21:17:58.000000 djaodjin-rules-0.4.2/rules/perms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6317 2023-03-03 05:27:25.000000 djaodjin-rules-0.4.2/rules/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1543 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.315525 djaodjin-rules-0.4.2/rules/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.319654 djaodjin-rules-0.4.2/rules/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    51677 2023-07-07 13:10:52.000000 djaodjin-rules-0.4.2/rules/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     4881 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/static/js/djaodjin-resources.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     9738 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/static/js/djaodjin-rules-angular.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     8414 2022-11-15 17:57:27.000000 djaodjin-rules-0.4.2/rules/static/js/djaodjin-rules-vue.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.315652 djaodjin-rules-0.4.2/rules/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.320075 djaodjin-rules-0.4.2/rules/templates/rules/
+-rw-r--r--   0 smirolo    (501) staff       (20)     8542 2023-07-07 14:33:41.000000 djaodjin-rules-0.4.2/rules/templates/rules/app_dashboard.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      949 2022-11-15 18:47:22.000000 djaodjin-rules-0.4.2/rules/templates/rules/engagement.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      751 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/templates/rules/forward_error.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9160 2022-11-22 21:38:20.000000 djaodjin-rules-0.4.2/rules/urldecorators.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.320469 djaodjin-rules-0.4.2/rules/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1551 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.320730 djaodjin-rules-0.4.2/rules/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1477 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2528 2022-08-10 04:42:14.000000 djaodjin-rules-0.4.2/rules/urls/api/proxy.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1513 2022-07-26 19:09:34.000000 djaodjin-rules-0.4.2/rules/urls/apply.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1803 2022-11-16 20:10:48.000000 djaodjin-rules-0.4.2/rules/urls/configure.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4604 2022-11-22 21:01:08.000000 djaodjin-rules-0.4.2/rules/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-07-07 15:04:57.321118 djaodjin-rules-0.4.2/rules/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1763 2022-11-22 20:38:48.000000 djaodjin-rules-0.4.2/rules/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    18928 2022-11-16 20:12:05.000000 djaodjin-rules-0.4.2/rules/views/app.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4413 2022-11-22 21:34:13.000000 djaodjin-rules-0.4.2/rules/views/download.py
+-rw-r--r--   0 smirolo    (501) staff       (20)       38 2023-07-07 15:04:57.321452 djaodjin-rules-0.4.2/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-07-07 13:21:24.000000 djaodjin-rules-0.4.2/setup.py
```

### Comparing `djaodjin-rules-0.4.1/PKG-INFO` & `djaodjin-rules-0.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: djaodjin-rules
-Version: 0.4.1
-Summary: HTTP proxy firewall Django App
-Home-page: https://github.com/djaodjin/djaodjin-rules/
-Download-URL: https://github.com/djaodjin/djaodjin-rules/tarball/0.4.1
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
+Version: 0.4.2
+Summary: Flexible framework to check permissions to URIs and forward HTTP requests
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-rules
+Project-URL: documentation, https://djaodjin-rules.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-rules/changelog
+Keywords: django,security,rules,proxy,rbac
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 Flexible framework to check permissions to URIs and forward HTTP requests
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.0 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 This project contains bare bone templates. To see it in action, integrated into
 a full-fledged subscription-based session proxy with bootstrap-styled
 dashboards, take a look at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 Development
 ===========
 
 After cloning the repository, create a virtualenv environment and install
 the prerequisites:
 
-    $ virtualenv _installTop_
-    $ source _installTop_/bin/activate
+    $ python -m venv .venv
+    $ source .venv/bin/activate
     $ pip install -r testsite/requirements.txt
 
 It remains to create the database and populate it with test data.
 
     $ python ./manage.py migrate --run-syncdb --noinput
     $ python ./manage.py loaddata testsite/fixtures/test_data.json
 
@@ -40,17 +41,20 @@
 
     $ python ./manage.py runserver
 
 
 Release Notes
 =============
 
-0.4.1
+Tested with
+
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.4.2
 
-  * adds toggle to enable/disable CORS checks
-  * selects rules.App based on path_prefix
-  * supports forwarded "OPTIONS" HTTP requests
-  * defaults new rule to authenticated and at the top of the list
-  * uses up/down arrows in rules dashboard
-  * downloads user engagement
+  * fixes error when OPTIONS on restframework View subclass
+  * removes dependency on vue-infinite-loading.js
+  * installs using pyproject.toml
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-rules-0.4.1/djaodjin_rules.egg-info/PKG-INFO` & `djaodjin-rules-0.4.2/djaodjin_rules.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: djaodjin-rules
-Version: 0.4.1
-Summary: HTTP proxy firewall Django App
-Home-page: https://github.com/djaodjin/djaodjin-rules/
-Download-URL: https://github.com/djaodjin/djaodjin-rules/tarball/0.4.1
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
+Version: 0.4.2
+Summary: Flexible framework to check permissions to URIs and forward HTTP requests
+Author-email: The DjaoDjin Team <help@djaodjin.com>
+Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
+License: BSD-2-Clause
+Project-URL: repository, https://github.com/djaodjin/djaodjin-rules
+Project-URL: documentation, https://djaodjin-rules.readthedocs.io/
+Project-URL: changelog, https://github.com/djaodjin/djaodjin-rules/changelog
+Keywords: django,security,rules,proxy,rbac
+Classifier: Framework :: Django
+Classifier: Environment :: Web Environment
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 Flexible framework to check permissions to URIs and forward HTTP requests
 
-Tested with
-
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.0 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
 This project contains bare bone templates. To see it in action, integrated into
 a full-fledged subscription-based session proxy with bootstrap-styled
 dashboards, take a look at [djaoapp](https://github.com/djaodjin/djaoapp/).
 
 Development
 ===========
 
 After cloning the repository, create a virtualenv environment and install
 the prerequisites:
 
-    $ virtualenv _installTop_
-    $ source _installTop_/bin/activate
+    $ python -m venv .venv
+    $ source .venv/bin/activate
     $ pip install -r testsite/requirements.txt
 
 It remains to create the database and populate it with test data.
 
     $ python ./manage.py migrate --run-syncdb --noinput
     $ python ./manage.py loaddata testsite/fixtures/test_data.json
 
@@ -40,17 +41,20 @@
 
     $ python ./manage.py runserver
 
 
 Release Notes
 =============
 
-0.4.1
+Tested with
+
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
+
+0.4.2
 
-  * adds toggle to enable/disable CORS checks
-  * selects rules.App based on path_prefix
-  * supports forwarded "OPTIONS" HTTP requests
-  * defaults new rule to authenticated and at the top of the list
-  * uses up/down arrows in rules dashboard
-  * downloads user engagement
+  * fixes error when OPTIONS on restframework View subclass
+  * removes dependency on vue-infinite-loading.js
+  * installs using pyproject.toml
 
 [previous release notes](changelog)
```

### Comparing `djaodjin-rules-0.4.1/djaodjin_rules.egg-info/SOURCES.txt` & `djaodjin-rules-0.4.2/djaodjin_rules.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
 djaodjin_rules.egg-info/PKG-INFO
 djaodjin_rules.egg-info/SOURCES.txt
 djaodjin_rules.egg-info/dependency_links.txt
 djaodjin_rules.egg-info/requires.txt
 djaodjin_rules.egg-info/top_level.txt
 rules/__init__.py
```

### Comparing `djaodjin-rules-0.4.1/rules/__init__.py` & `djaodjin-rules-0.4.2/rules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the rules django app.
 """
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
```

### Comparing `djaodjin-rules-0.4.1/rules/api/keys.py` & `djaodjin-rules-0.4.2/rules/api/keys.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/api/rules.py` & `djaodjin-rules-0.4.2/rules/api/rules.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/api/serializers.py` & `djaodjin-rules-0.4.2/rules/api/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/api/sessions.py` & `djaodjin-rules-0.4.2/rules/api/sessions.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/compat.py` & `djaodjin-rules-0.4.2/rules/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/decorators.py` & `djaodjin-rules-0.4.2/rules/decorators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/docs.py` & `djaodjin-rules-0.4.2/rules/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/extras.py` & `djaodjin-rules-0.4.2/rules/extras.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/middleware.py` & `djaodjin-rules-0.4.2/rules/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             LOGGER.debug("dont enforce csrf checks on %s %s because"\
                 " we have an authorization header",
                 request.method, request.path)
 
         # CORS will first send an OPTIONS request with no authorization header
         # and expect to get a 200 OK response.
         if request.method.lower() == 'options':
-            if view_class and isinstance(view_class, APIView):
+            if view_class and issubclass(view_class, APIView):
                 # Duplicates what Django does before calling `dispatch`
                 view = view_class(**callback.initkwargs)
                 view.setup(request, *callback_args, **callback_kwargs)
                 if not hasattr(view, 'request'):
                     raise AttributeError("%s instance has no 'request'"
                         " attribute. Did you override setup() and forget"
                         " to call super()?" % view_class.__name__)
```

### Comparing `djaodjin-rules-0.4.1/rules/mixins.py` & `djaodjin-rules-0.4.2/rules/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/models.py` & `djaodjin-rules-0.4.2/rules/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/perms.py` & `djaodjin-rules-0.4.2/rules/perms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/settings.py` & `djaodjin-rules-0.4.2/rules/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/signals.py` & `djaodjin-rules-0.4.2/rules/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/static/js/djaodjin-resources-vue.js` & `djaodjin-rules-0.4.2/rules/static/js/djaodjin-resources-vue.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -153,22 +153,151 @@
                     }
                 }
                 vm.showMessages(messages, "error");
             },
         }
     };
 
+
+    /** compute outdated based on `params`.
+
+        `params = {start_at, ends_at}` must exist in either the `props` or `data`
+        of the component.
+
+        A subclass of this mixin must define either the function `autoReload`
+        or `reload` in order to make updates as a user is typing in input fields
+        or when a button is pressed respectively.
+     */
+    var paramsMixin = {
+        data: function() {
+            var data = {
+                lastGetParams: {},
+            }
+            return data;
+        },
+        methods: {
+            asDateInputField: function(dateISOString) {
+                const dateValue = moment(dateISOString);
+                return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
+            },
+            asDateISOString: function(dateInputField) {
+                const dateValue = moment(dateInputField, "YYYY-MM-DD");
+                return dateValue.isValid() ? dateValue.toISOString() : null;
+            },
+            autoReload: function() {},
+            reload: function() {},
+            getParams: function(excludes) {
+                var vm = this;
+                var params = {};
+                for (var key in vm.params) {
+                    if (vm.params.hasOwnProperty(key) && vm.params[key]) {
+                        if (excludes && key in excludes) continue;
+                        params[key] = vm.params[key];
+                    }
+                }
+                return params;
+            },
+            getQueryString: function(excludes) {
+                var vm = this;
+                var sep = "";
+                var result = "";
+                var params = vm.getParams(excludes);
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        result += sep + key + '=' + encodeURIComponent(
+                            params[key].toString());
+                        sep = "&";
+                    }
+                }
+                if (result) {
+                    result = '?' + result;
+                }
+                return result;
+            },
+        },
+        computed: {
+            _start_at: {
+                get: function() {
+                    return this.asDateInputField(this.params.start_at);
+                },
+                set: function(newVal) {
+                    if (newVal) {
+                        // The setter might be call with `newVal === null`
+                        // when the date is incorrect (ex: 09/31/2022).
+                        this.$set(this.params, 'start_at',
+                            this.asDateISOString(newVal));
+                        if (this.outdated) this.debouncedAutoReload();
+                    }
+                }
+            },
+            _ends_at: {
+                get: function() {
+                    // form field input="date" will expect ends_at as a String
+                    // but will literally cut the hour part regardless of timezone.
+                    // We don't want an empty list as a result.
+                    // If we use moment `endOfDay` we get 23:59:59 so we
+                    // add a full day instead. It seemed clever to run the following
+                    // code but that prevented entering the year part in the input
+                    // field (as oppossed to use the widget).
+                    //
+                    // const dateValue = moment(this.params.ends_at).add(1,'days');
+                    // return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
+                    return this.asDateInputField(this.params.ends_at);
+                },
+                set: function(newVal) {
+                    if (newVal) {
+                        // The setter might be call with `newVal === null`
+                        // when the date is incorrect (ex: 09/31/2022).
+                        this.$set(this.params, 'ends_at',
+                            this.asDateISOString(newVal));
+                        if (this.outdated) this.debouncedAutoReload();
+                    }
+                }
+            },
+            outdated: function() {
+                var vm = this;
+                const params = vm.getParams();
+                for (var key in vm.lastGetParams) {
+                    if (vm.lastGetParams.hasOwnProperty(key)) {
+                        if (vm.lastGetParams[key] !== params[key]) {
+                            return true;
+                        }
+                    }
+                }
+                for (var key in params) {
+                    if (params.hasOwnProperty(key)) {
+                        if (params[key] !== vm.lastGetParams[key]) {
+                            return true;
+                        }
+                    }
+                }
+                return false;
+            }
+        },
+        created: function() {
+            // _.debounce is a function provided by lodash to limit how
+            // often a particularly expensive operation can be run.
+            if (typeof _ != 'undefined' && typeof _.debounce != 'undefined') {
+                this.debouncedAutoReload = _.debounce(this.autoReload, 500);
+            } else {
+                this.debouncedAutoReload = this.autoReload;
+            }
+        }
+    };
+
+
     /** A wrapper around jQuery ajax functions that adds authentication
         parameters as necessary.
 
         requires `jQuery`
     */
     var httpRequestMixin = {
         mixins: [
-            messagesMixin
+            messagesMixin,
+            paramsMixin
         ],
         // XXX conflitcs when params defined as props
         //    data: function() {
         //        return {
         //            params: {}
         //        }
         //    },
@@ -213,52 +342,41 @@
                 }
                 return "";
             },
 
             _safeUrl: function(base, path) {
                 if (!path) return base;
 
-                if (base && base[base.length - 1] == '/') {
-                    if (path && path[0] == '/') {
-                        return base + path.substring(1);
+                const parts = [base].concat(
+                    (typeof path === 'string') ? [path] : path);
+                var cleanParts = [];
+                var start, end;
+                for (var idx = 0; idx < parts.length; ++idx) {
+                    const part = parts[idx];
+                    for (start = 0; start < part.length; ++start) {
+                        if (part[start] !== '/') {
+                            break;
+                        }
                     }
-                    return base + path;
-                }
-                if (path && path[0] == '/') {
-                    return base + path;
-                }
-                return base + '/' + path;
-            },
-
-            getParams: function(excludes) {
-                var vm = this;
-                var params = {};
-                for (var key in vm.params) {
-                    if (vm.params.hasOwnProperty(key) && vm.params[key]) {
-                        if (excludes && key in excludes) continue;
-                        params[key] = vm.params[key];
+                    for (end = part.length - 1; end >= 0; --end) {
+                        if (part[end] !== '/') {
+                            break;
+                        }
                     }
-                }
-                return params;
-            },
-            getQueryString: function(excludes) {
-                var vm = this;
-                var sep = "";
-                var result = "";
-                var params = vm.getParams(excludes);
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        result += sep + key + '=' + params[key].toString();
-                        sep = "&";
+                    if (start < end) {
+                        cleanParts.push(part.slice(start, end + 1));
+                    } else {
+                        cleanParts.push(part);
                     }
                 }
-                if (result) {
-                    result = '?' + result;
+                var cleanUrl = cleanParts[0];
+                for (idx = 1; idx < cleanParts.length; ++idx) {
+                    cleanUrl += '/' + cleanParts[idx];
                 }
-                return result;
+                return cleanUrl.startsWith('http') ? cleanUrl[0] : '/' + cleanUrl;
             },
 
             /** This method generates a GET HTTP request to `url` with a query
                 string built of a `queryParams` dictionnary.
 
                 It supports the following prototypes:
 
@@ -709,38 +827,37 @@
                 if (!successCallback) {
                     successCallback = function() {};
                 }
                 if (!failureCallback) {
                     failureCallback = vm.showErrorMessages;
                 }
                 for (var idx = 0; idx < queryArray.length; ++idx) {
-                    ajaxCalls.push(function() {
-                        return $.ajax({
-                            method: queryArray[idx].method,
-                            url: queryArray[idx].url,
-                            data: JSON.stringify(queryArray[idx].data),
-                            beforeSend: function(xhr, settings) {
-                                var authToken = vm._getAuthToken();
-                                if (authToken) {
-                                    xhr.setRequestHeader("Authorization",
-                                        "Bearer " + authToken);
-                                } else {
-                                    if (!vm._csrfSafeMethod(settings.type)) {
-                                        var csrfToken = vm._getCSRFToken();
-                                        if (csrfToken) {
-                                            xhr.setRequestHeader("X-CSRFToken", csrfToken);
-                                        }
+                    ajaxCalls.push($.ajax({
+                        method: queryArray[idx].method,
+                        url: queryArray[idx].url,
+                        data: JSON.stringify(queryArray[idx].data),
+                        beforeSend: function(xhr, settings) {
+                            var authToken = vm._getAuthToken();
+                            if (authToken) {
+                                xhr.setRequestHeader("Authorization",
+                                    "Bearer " + authToken);
+                            } else {
+                                if (!vm._csrfSafeMethod(settings.type)) {
+                                    var csrfToken = vm._getCSRFToken();
+                                    if (csrfToken) {
+                                        xhr.setRequestHeader("X-CSRFToken", csrfToken);
                                     }
                                 }
-                            },
-                            contentType: 'application/json',
-                        });
-                    }());
+                            }
+                        },
+                        contentType: 'application/json',
+                    }));
                 }
-                jQuery.when(ajaxCalls).done(successCallback).fail(failureCallback);
+                jQuery.when.apply(jQuery, ajaxCalls).done(successCallback).fail(
+                    failureCallback);
             },
         }
     }
 
 
     var itemMixin = {
         mixins: [
@@ -791,83 +908,58 @@
                 }
                 return !isEmpty;
             },
         },
     }
 
 
-    var filterableMixin = {
-        data: function() {
-            return {
-                params: {
-                    q: '',
-                },
-                mixinFilterCb: 'get',
-            }
-        },
-        methods: {
-            filterList: function() {
-                if (this.params.q) {
-                    if ("page" in this.params) {
-                        this.params.page = 1;
-                    }
-                }
-                if (this[this.mixinFilterCb]) {
-                    this[this.mixinFilterCb]();
-                }
-            },
-        },
-    }
-
-
     var paginationMixin = {
         data: function() {
             return {
                 params: {
                     page: 1,
                 },
+                mergeResults: false,
                 itemsPerPage: this.$itemsPerPage,
                 ellipsisThreshold: 4,
+                preReload: ['resetPage'],
                 getCompleteCb: 'getCompleted',
                 getBeforeCb: 'resetPage',
-                qsCache: null,
-                isInfiniteScroll: false,
             }
         },
         methods: {
             resetPage: function() {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (vm.qsCache && vm.qsCache !== vm.qs) {
-                    vm.params.page = 1;
-                    vm.ISState.reset();
-                }
-                vm.qsCache = vm.qs;
+                vm.params.page = 1;
             },
             getCompleted: function() {
                 var vm = this;
-                if (!vm.ISState) return;
                 vm.mergeResults = false;
-                if (vm.pageCount > 0) {
-                    vm.ISState.loaded();
-                }
-                if (vm.params.page >= vm.pageCount) {
-                    vm.ISState.complete();
+            },
+            handleScroll: function(evt) {
+                var vm = this;
+                let element = this.$el;
+                if (element.getBoundingClientRect().bottom < window.innerHeight) {
+                    let menubar = vm.$el.querySelector('[role="pagination"]');
+                    if (menubar) {
+                        var style = window.getComputedStyle(menubar);
+                        if (style.display == 'none') {
+                            // We are not displaying the pagination menubar,
+                            // so let's scroll!
+                            vm.paginationHandler();
+                        }
+                    }
                 }
             },
             paginationHandler: function($state) {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (!vm.itemsLoaded) {
-                    // this handler is triggered on initial get too
+                if (!vm.itemsLoaded || vm.mergeResults) {
+                    // this handler is triggered on initial get() too.
                     return;
                 }
-                // rudimentary way to detect which type of pagination
-                // is active. ideally need to monitor resolution changes
-                vm.isInfiniteScroll = true;
                 var nxt = vm.params.page + 1;
                 if (nxt <= vm.pageCount) {
                     vm.$set(vm.params, 'page', nxt);
                     vm.mergeResults = true;
                     vm.get();
                 }
             },
@@ -923,23 +1015,21 @@
                 var vm = this;
                 var pages = [];
                 for (var idx = vm.minDirectPageLink; idx <= vm.maxDirectPageLink; ++idx) {
                     pages.push(idx);
                 }
                 return pages;
             },
-            ISState: function() {
-                if (!this.$refs.infiniteLoading) return;
-                return this.$refs.infiniteLoading.stateChanger;
-            },
-            qs: function() {
-                return this.getQueryString({
-                    page: null
-                });
-            },
+        },
+        mounted: function() {
+            var vm = this;
+            window.addEventListener("scroll", vm.handleScroll);
+        },
+        unmounted: function() {
+            window.removeEventListener("scroll", vm.handleScroll);
         }
     }
 
 
     var sortableMixin = {
         data: function() {
             var defaultDir = this.$sortDirection || 'desc';
@@ -1034,41 +1124,39 @@
     }
 
 
     var itemListMixin = {
         mixins: [
             httpRequestMixin,
             paginationMixin,
-            filterableMixin,
             sortableMixin
         ],
         data: function() {
             return this.getInitData();
         },
         methods: {
             getInitData: function() {
                 var data = {
                     url: null,
-                    itemsLoaded: false,
-                    items: {
-                        results: [],
-                        count: 0
-                    },
-                    mergeResults: false,
                     params: {
                         // The following dates will be stored as `String` objects
                         // as oppossed to `moment` or `Date` objects because this
                         // is how form fields input="date" will update them.
                         start_at: null,
                         ends_at: null,
                         // The timezone for both start_at and ends_at.
-                        timezone: 'local'
+                        timezone: 'local',
+                        q: '',
+                    },
+                    itemsLoaded: false,
+                    items: {
+                        results: [],
+                        count: 0
                     },
-                    lastGetParams: {},
-                    autoreload: true,
+                    mergeResults: false,
                     getCb: null,
                     getCompleteCb: null,
                     getBeforeCb: null,
                 }
                 if (this.$dateRange) {
                     if (this.$dateRange.start_at) {
                         data.params['start_at'] = this.$dateRange.start_at;
@@ -1118,89 +1206,33 @@
                             vm[vm.getCompleteCb]();
                         }
                     }
                 }
                 if (vm[vm.getBeforeCb]) {
                     vm[vm.getBeforeCb]();
                 }
+                vm.fetch(cb);
+            },
+            fetch: function(cb) {
+                let vm = this;
                 vm.lastGetParams = vm.getParams();
                 vm.reqGet(vm.url, vm.lastGetParams, cb);
             },
-            asDateInputField: function(dateISOString) {
-                const dateValue = moment(dateISOString);
-                return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
-            },
-            asDateISOString: function(dateInputField) {
-                const dateValue = moment(dateInputField, "YYYY-MM-DD");
-                return dateValue.isValid() ? dateValue.toISOString() : null;
-            }
-        },
-        computed: {
-            _start_at: {
-                get: function() {
-                    return this.asDateInputField(this.params.start_at);
-                },
-                set: function(newVal) {
-                    if (newVal) {
-                        // The setter might be call with `newVal === null`
-                        // when the date is incorrect (ex: 09/31/2022).
-                        this.$set(this.params, 'start_at',
-                            this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
-                    }
-                }
-            },
-            _ends_at: {
-                get: function() {
-                    // form field input="date" will expect ends_at as a String
-                    // but will literally cut the hour part regardless of timezone.
-                    // We don't want an empty list as a result.
-                    // If we use moment `endOfDay` we get 23:59:59 so we
-                    // add a full day instead. It seemed clever to run the following
-                    // code but that prevented entering the year part in the input
-                    // field (as oppossed to use the widget).
-                    //
-                    // const dateValue = moment(this.params.ends_at).add(1,'days');
-                    // return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
-                    return this.asDateInputField(this.params.ends_at);
-                },
-                set: function(newVal) {
-                    if (newVal) {
-                        // The setter might be call with `newVal === null`
-                        // when the date is incorrect (ex: 09/31/2022).
-                        this.$set(this.params, 'ends_at',
-                            this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
-                    }
+            reload: function() {
+                let vm = this;
+                for (let idx = 0; idx < vm.preReload.length; ++idx) {
+                    vm[vm.preReload[idx]]();
                 }
+                vm.get();
             },
-            outdated: function() {
-                var vm = this;
-                const params = vm.getParams();
-                for (var key in vm.lastGetParams) {
-                    if (vm.lastGetParams.hasOwnProperty(key)) {
-                        if (vm.lastGetParams[key] !== params[key]) {
-                            return true;
-                        }
-                    }
-                }
-                for (var key in params) {
-                    if (params.hasOwnProperty(key)) {
-                        if (params[key] !== vm.lastGetParams[key]) {
-                            return true;
-                        }
-                    }
-                }
-                return false;
-            }
-        }
+        },
     };
 
 
-    var TypeAhead = Vue.extend({
+    var typeAheadMixin = {
         mixins: [
             httpRequestMixin
         ],
         data: function data() {
             return {
                 url: null,
                 items: [],
@@ -1238,22 +1270,21 @@
                 var vm = this;
                 if (vm.current !== -1) {
                     vm.onHit(vm.items[vm.current]);
                 }
             },
 
             onHit: function onHit() {
-                Vue.util.warn('You need to implement the `onHit` method', this);
+                console.warn('You need to implement the `onHit` method', this);
             },
 
             reset: function() {
                 var vm = this;
-                vm.items = [];
+                vm.clear();
                 vm.query = '';
-                vm.loading = false;
             },
 
             setActive: function(index) {
                 var vm = this;
                 vm.current = index;
             },
 
@@ -1309,19 +1340,22 @@
                 return !this.query;
             },
             isDirty: function isDirty() {
                 return !!this.query;
             }
         },
         mounted: function() {
-            // do nothing.
+            if (this.$el.dataset && this.$el.dataset.url) {
+                this.url = this.$el.dataset.url;
+            }
         }
-    });
+    };
 
     // attach properties to the exports object to define
     // the exported module properties.
-    exports.messagesMixin = messagesMixin;
     exports.httpRequestMixin = httpRequestMixin;
-    exports.itemMixin = itemMixin;
     exports.itemListMixin = itemListMixin;
-    exports.TypeAhead = TypeAhead;
+    exports.itemMixin = itemMixin;
+    exports.messagesMixin = messagesMixin;
+    exports.paramsMixin = paramsMixin;
+    exports.typeAheadMixin = typeAheadMixin;
 }));
```

### Comparing `djaodjin-rules-0.4.1/rules/static/js/djaodjin-resources.js` & `djaodjin-rules-0.4.2/rules/static/js/djaodjin-resources.js`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/static/js/djaodjin-rules-angular.js` & `djaodjin-rules-0.4.2/rules/static/js/djaodjin-rules-angular.js`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/static/js/djaodjin-rules-vue.js` & `djaodjin-rules-0.4.2/rules/static/js/djaodjin-rules-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/templates/rules/app_dashboard.html` & `djaodjin-rules-0.4.2/rules/templates/rules/app_dashboard.html`

 * *Files 8% similar despite different names*

```diff
@@ -71,25 +71,15 @@
                      data-toggle="modal" data-target="#new-rule"
                      @click.prevent="ruleModalOpen=true">Add ...</a>
                 </td>
               </tr>
             </tbody>
           </table>
         </div>
-        <div v-show="itemsLoaded && totalItems > itemsPerPage">
-          <div v-show="pageCount > 1" class="d-md-none">
-            <infinite-loading @infinite="paginationHandler" ref="infiniteLoading" force-use-infinite-wrapper>
-              <div slot="no-more">
-                <div class="back-to-top my-4 text-center">
-                  <a href="#">Back to Top</a>
-                </div>
-              </div>
-            </infinite-loading>
-          </div>
-        </div>
+
         <!-- modal dialog for Adding a rule -->
         <div id="new-rule" class="modal fade" tabindex="-1" role="dialog"
              aria-labelledby="Add Access Rule" aria-hidden="true">
           <div>
             <h4>New Rule: path accessed ...</h4>
             <form ng-submit="create()"
                   @submit.prevent="create">
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
 {% extends "base.html" %} {% block content %}
 **** Domain ****
 The site is available at {{site_available_at_url}}.
 **** Access Rules ****
 Rank Path Access Rule Forward Engage tags
 click.prevent="ruleModalOpen=true">Add ...
-infinite="paginationHandler" ref="infiniteLoading" force-use-infinite-wrapper>
-Back_to_Top
 *** New Rule: path accessed ... ***
 submit.prevent="create">
 [new_rule_path       ]
 Your path should end with '/'. If not it will be automatically added.
 Create
 
 **** Web application ****
```

### Comparing `djaodjin-rules-0.4.1/rules/templates/rules/engagement.html` & `djaodjin-rules-0.4.2/rules/templates/rules/engagement.html`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/templates/rules/forward_error.html` & `djaodjin-rules-0.4.2/rules/templates/rules/forward_error.html`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urldecorators.py` & `djaodjin-rules-0.4.2/rules/urldecorators.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urls/__init__.py` & `djaodjin-rules-0.4.2/rules/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urls/api/__init__.py` & `djaodjin-rules-0.4.2/rules/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urls/api/proxy.py` & `djaodjin-rules-0.4.2/rules/urls/api/proxy.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urls/apply.py` & `djaodjin-rules-0.4.2/rules/urls/apply.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/urls/configure.py` & `djaodjin-rules-0.4.2/rules/urls/configure.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/utils.py` & `djaodjin-rules-0.4.2/rules/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/views/__init__.py` & `djaodjin-rules-0.4.2/rules/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/views/app.py` & `djaodjin-rules-0.4.2/rules/views/app.py`

 * *Files identical despite different names*

### Comparing `djaodjin-rules-0.4.1/rules/views/download.py` & `djaodjin-rules-0.4.2/rules/views/download.py`

 * *Files identical despite different names*

