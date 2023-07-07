# Comparing `tmp/railguns-0.68.tar.gz` & `tmp/railguns-0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "railguns-0.68.tar", last modified: Sat May 13 08:31:51 2023, max compression
+gzip compressed data, was "railguns-0.69.tar", last modified: Fri Jul  7 07:25:07 2023, max compression
```

## Comparing `railguns-0.68.tar` & `railguns-0.69.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.961647 railguns-0.68/
--rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.68/LICENSE
--rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.68/MANIFEST.in
--rw-r--r--   0 ny         (501) staff       (20)     3954 2023-05-13 08:31:51.961518 railguns-0.68/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1648 2022-06-18 13:16:59.000000 railguns-0.68/README.md
--rw-r--r--   0 ny         (501) staff       (20)     1687 2023-05-13 08:27:25.000000 railguns-0.68/pyproject.toml
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.955965 railguns-0.68/railguns/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.957106 railguns-0.68/railguns/cloudfile/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/cloudfile/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      470 2022-06-18 13:16:59.000000 railguns-0.68/railguns/cloudfile/fields.py
--rw-r--r--   0 ny         (501) staff       (20)     1137 2022-06-18 13:16:59.000000 railguns-0.68/railguns/cloudfile/widgets.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.957378 railguns-0.68/railguns/django/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.957605 railguns-0.68/railguns/django/contrib/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/contrib/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     2321 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/contrib/admin.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.957818 railguns-0.68/railguns/django/contrib/auth/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/contrib/auth/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      855 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/contrib/auth/backends.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.958116 railguns-0.68/railguns/django/db/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/db/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     3140 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/db/models.py
--rw-r--r--   0 ny         (501) staff       (20)     2190 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/db/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1776 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/generics.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.958469 railguns-0.68/railguns/django/utils/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/utils/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      459 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/utils/html.py
--rw-r--r--   0 ny         (501) staff       (20)      777 2022-06-18 13:16:59.000000 railguns-0.68/railguns/django/utils/translation.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.959370 railguns-0.68/railguns/rest_framework/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     1614 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/generics.py
--rw-r--r--   0 ny         (501) staff       (20)     2762 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/mixins.py
--rw-r--r--   0 ny         (501) staff       (20)      306 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/pagination.py
--rw-r--r--   0 ny         (501) staff       (20)     1750 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/permissions.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.959568 railguns-0.68/railguns/rest_framework/schemas/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/schemas/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/schemas/openapi.py
--rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/serializers.py
--rw-r--r--   0 ny         (501) staff       (20)      128 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     6642 2022-06-18 13:16:59.000000 railguns-0.68/railguns/rest_framework/views.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.954645 railguns-0.68/railguns/static/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.954590 railguns-0.68/railguns/static/cloudfile/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.959676 railguns-0.68/railguns/static/cloudfile/js/
--rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/cloudfile/js/scripts.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.954849 railguns-0.68/railguns/static/railguns/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.959870 railguns-0.68/railguns/static/railguns/es2015/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.959980 railguns-0.68/railguns/static/railguns/es2015/components/
--rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/es2015/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/es2015/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.960096 railguns-0.68/railguns/static/railguns/es2015/util/
--rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/es2015/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/es2015/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.960302 railguns-0.68/railguns/static/railguns/js/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.960409 railguns-0.68/railguns/static/railguns/js/components/
--rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/js/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/js/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.960539 railguns-0.68/railguns/static/railguns/js/util/
--rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/js/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.68/railguns/static/railguns/js/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.955059 railguns-0.68/railguns/templates/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.960779 railguns-0.68/railguns/templates/railguns/
--rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.68/railguns/templates/railguns/base.html
--rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.68/railguns/templates/railguns/base_quick.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.961140 railguns-0.68/railguns/templates/railguns/ui/
--rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.68/railguns/templates/railguns/ui/base.html
--rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.68/railguns/templates/railguns/ui/detail.html
--rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.68/railguns/templates/railguns/ui/list.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.961345 railguns-0.68/railguns/tools/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.68/railguns/tools/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      238 2022-06-18 13:16:59.000000 railguns-0.68/railguns/tools/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1653 2022-06-18 13:16:59.000000 railguns-0.68/railguns/urls.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-05-13 08:31:51.956633 railguns-0.68/railguns.egg-info/
--rw-r--r--   0 ny         (501) staff       (20)     3954 2023-05-13 08:31:51.000000 railguns-0.68/railguns.egg-info/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1787 2023-05-13 08:31:51.000000 railguns-0.68/railguns.egg-info/SOURCES.txt
--rw-r--r--   0 ny         (501) staff       (20)        1 2023-05-13 08:31:51.000000 railguns-0.68/railguns.egg-info/dependency_links.txt
--rw-r--r--   0 ny         (501) staff       (20)      285 2023-05-13 08:31:51.000000 railguns-0.68/railguns.egg-info/requires.txt
--rw-r--r--   0 ny         (501) staff       (20)        9 2023-05-13 08:31:51.000000 railguns-0.68/railguns.egg-info/top_level.txt
--rw-r--r--   0 ny         (501) staff       (20)       38 2023-05-13 08:31:51.961680 railguns-0.68/setup.cfg
--rw-r--r--   0 ny         (501) staff       (20)     1560 2023-05-13 08:25:53.000000 railguns-0.68/setup.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.058626 railguns-0.69/
+-rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.69/LICENSE
+-rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.69/MANIFEST.in
+-rw-r--r--   0 ny         (501) staff       (20)     3954 2023-07-07 07:25:07.058499 railguns-0.69/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1648 2022-06-18 13:16:59.000000 railguns-0.69/README.md
+-rw-r--r--   0 ny         (501) staff       (20)     1687 2023-07-07 01:19:16.000000 railguns-0.69/pyproject.toml
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.051340 railguns-0.69/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.052578 railguns-0.69/railguns/cloudfile/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/cloudfile/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      470 2022-06-18 13:16:59.000000 railguns-0.69/railguns/cloudfile/fields.py
+-rw-r--r--   0 ny         (501) staff       (20)     1137 2022-06-18 13:16:59.000000 railguns-0.69/railguns/cloudfile/widgets.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.052813 railguns-0.69/railguns/django/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.053075 railguns-0.69/railguns/django/contrib/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/contrib/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     2321 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/contrib/admin.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.053326 railguns-0.69/railguns/django/contrib/auth/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/contrib/auth/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      855 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/contrib/auth/backends.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.053671 railguns-0.69/railguns/django/db/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/db/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     3140 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/db/models.py
+-rw-r--r--   0 ny         (501) staff       (20)     2190 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/db/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1776 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/generics.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.054067 railguns-0.69/railguns/django/utils/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/utils/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      459 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/utils/html.py
+-rw-r--r--   0 ny         (501) staff       (20)      777 2022-06-18 13:16:59.000000 railguns-0.69/railguns/django/utils/translation.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.055484 railguns-0.69/railguns/rest_framework/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     1614 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/generics.py
+-rw-r--r--   0 ny         (501) staff       (20)     2762 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/mixins.py
+-rw-r--r--   0 ny         (501) staff       (20)      306 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/pagination.py
+-rw-r--r--   0 ny         (501) staff       (20)     1750 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/permissions.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.055841 railguns-0.69/railguns/rest_framework/schemas/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/schemas/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/schemas/openapi.py
+-rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/serializers.py
+-rw-r--r--   0 ny         (501) staff       (20)      128 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     6642 2022-06-18 13:16:59.000000 railguns-0.69/railguns/rest_framework/views.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.049911 railguns-0.69/railguns/static/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.049855 railguns-0.69/railguns/static/cloudfile/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.056002 railguns-0.69/railguns/static/cloudfile/js/
+-rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/cloudfile/js/scripts.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.050116 railguns-0.69/railguns/static/railguns/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.056403 railguns-0.69/railguns/static/railguns/es2015/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.056558 railguns-0.69/railguns/static/railguns/es2015/components/
+-rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/es2015/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/es2015/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.056824 railguns-0.69/railguns/static/railguns/es2015/util/
+-rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/es2015/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/es2015/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.057113 railguns-0.69/railguns/static/railguns/js/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.057242 railguns-0.69/railguns/static/railguns/js/components/
+-rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/js/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/js/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.057464 railguns-0.69/railguns/static/railguns/js/util/
+-rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/js/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.69/railguns/static/railguns/js/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.050330 railguns-0.69/railguns/templates/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.057735 railguns-0.69/railguns/templates/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.69/railguns/templates/railguns/base.html
+-rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.69/railguns/templates/railguns/base_quick.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.058116 railguns-0.69/railguns/templates/railguns/ui/
+-rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.69/railguns/templates/railguns/ui/base.html
+-rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.69/railguns/templates/railguns/ui/detail.html
+-rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.69/railguns/templates/railguns/ui/list.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.058327 railguns-0.69/railguns/tools/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.69/railguns/tools/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      238 2022-06-18 13:16:59.000000 railguns-0.69/railguns/tools/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1653 2022-06-18 13:16:59.000000 railguns-0.69/railguns/urls.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-07-07 07:25:07.052180 railguns-0.69/railguns.egg-info/
+-rw-r--r--   0 ny         (501) staff       (20)     3954 2023-07-07 07:25:07.000000 railguns-0.69/railguns.egg-info/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1787 2023-07-07 07:25:07.000000 railguns-0.69/railguns.egg-info/SOURCES.txt
+-rw-r--r--   0 ny         (501) staff       (20)        1 2023-07-07 07:25:07.000000 railguns-0.69/railguns.egg-info/dependency_links.txt
+-rw-r--r--   0 ny         (501) staff       (20)      285 2023-07-07 07:25:07.000000 railguns-0.69/railguns.egg-info/requires.txt
+-rw-r--r--   0 ny         (501) staff       (20)        9 2023-07-07 07:25:07.000000 railguns-0.69/railguns.egg-info/top_level.txt
+-rw-r--r--   0 ny         (501) staff       (20)       38 2023-07-07 07:25:07.058666 railguns-0.69/setup.cfg
+-rw-r--r--   0 ny         (501) staff       (20)     1560 2023-07-07 01:18:21.000000 railguns-0.69/setup.py
```

### Comparing `railguns-0.68/LICENSE` & `railguns-0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `railguns-0.68/PKG-INFO` & `railguns-0.69/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.68
+Version: 0.69
 Summary: Only My Railgun
 Home-page: https://github.com/nyssance/railguns
 Author: NY
 Author-email: nyssance@icloud.com
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
```

### Comparing `railguns-0.68/README.md` & `railguns-0.69/README.md`

 * *Files identical despite different names*

### Comparing `railguns-0.68/pyproject.toml` & `railguns-0.69/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "railguns"
-version = "0.68"
+version = "0.69"
 description = "Only My Railgun"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["django", "railguns"]
 authors = [
   {email = "nyssance@icloud.com"},
@@ -25,26 +25,26 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
-  "django[argon2]==4.2.1",
+  "django[argon2]==4.2.3",
   "djangorestframework==3.14.0",
   "djangorestframework_simplejwt==5.2.2",
   "gunicorn==20.1.0",
   "uvicorn==0.22.0",
   #
-  "django-ckeditor==6.5.1",
+  "django-ckeditor==6.6.1",
   "django-filter==23.2",
   "django-htmlmin==0.11.0",
   "hiredis==2.2.3",
-  "mysqlclient==2.1.1",
-  "redis==4.5.5"
+  "mysqlclient==2.2.0",
+  "redis==4.6.0"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest < 5.0.0",
   "pytest-cov[all]"
 ]
```

### Comparing `railguns-0.68/railguns/cloudfile/widgets.py` & `railguns-0.69/railguns/cloudfile/widgets.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/contrib/admin.py` & `railguns-0.69/railguns/django/contrib/admin.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/contrib/auth/backends.py` & `railguns-0.69/railguns/django/contrib/auth/backends.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/db/models.py` & `railguns-0.69/railguns/django/db/models.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/db/utils.py` & `railguns-0.69/railguns/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/generics.py` & `railguns-0.69/railguns/django/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/django/utils/translation.py` & `railguns-0.69/railguns/django/utils/translation.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/generics.py` & `railguns-0.69/railguns/rest_framework/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/mixins.py` & `railguns-0.69/railguns/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/permissions.py` & `railguns-0.69/railguns/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/schemas/openapi.py` & `railguns-0.69/railguns/rest_framework/schemas/openapi.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/serializers.py` & `railguns-0.69/railguns/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/rest_framework/views.py` & `railguns-0.69/railguns/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/cloudfile/js/scripts.js` & `railguns-0.69/railguns/static/cloudfile/js/scripts.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/es2015/components/weui-components.js` & `railguns-0.69/railguns/static/railguns/es2015/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/es2015/mixins.js` & `railguns-0.69/railguns/static/railguns/es2015/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/es2015/util/http-utils.js` & `railguns-0.69/railguns/static/railguns/es2015/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/es2015/vendor.js` & `railguns-0.69/railguns/static/railguns/es2015/vendor.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/js/components/weui-components.js` & `railguns-0.69/railguns/static/railguns/js/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/js/mixins.js` & `railguns-0.69/railguns/static/railguns/js/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/static/railguns/js/util/http-utils.js` & `railguns-0.69/railguns/static/railguns/js/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/templates/railguns/base.html` & `railguns-0.69/railguns/templates/railguns/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/templates/railguns/base_quick.html` & `railguns-0.69/railguns/templates/railguns/base_quick.html`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/templates/railguns/ui/base.html` & `railguns-0.69/railguns/templates/railguns/ui/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/templates/railguns/ui/detail.html` & `railguns-0.69/railguns/templates/railguns/ui/detail.html`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/templates/railguns/ui/list.html` & `railguns-0.69/railguns/templates/railguns/ui/list.html`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns/urls.py` & `railguns-0.69/railguns/urls.py`

 * *Files identical despite different names*

### Comparing `railguns-0.68/railguns.egg-info/PKG-INFO` & `railguns-0.69/railguns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.68
+Version: 0.69
 Summary: Only My Railgun
 Home-page: https://github.com/nyssance/railguns
 Author: NY
 Author-email: nyssance@icloud.com
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
```

### Comparing `railguns-0.68/railguns.egg-info/SOURCES.txt` & `railguns-0.69/railguns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `railguns-0.68/setup.py` & `railguns-0.69/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='RailgunS',
-    version='0.68',
+    version='0.69',
     author='NY',
     author_email='nyssance@icloud.com',
     description='Only My Railgun',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nyssance/railguns',
     project_urls={
@@ -30,25 +30,25 @@
     ],
     # package_dir={'': 'src'},
     packages=find_packages(exclude=['tests']),
     python_requires='>=3.10',
     # zip_safe=False,
     include_package_data=True,
     install_requires=[
-        'django[argon2]==4.2.1',
+        'django[argon2]==4.2.3',
         'djangorestframework==3.14.0',
         'djangorestframework_simplejwt==5.2.2',
         'gunicorn==20.1.0',
         'uvicorn==0.22.0',
         #
-        'django-ckeditor==6.5.1',
+        'django-ckeditor==6.6.1',
         'django-filter==23.2',
         'django-htmlmin==0.11.0',
         'hiredis==2.2.3',
-        'mysqlclient==2.1.1',
-        'redis==4.5.5'
+        'mysqlclient==2.2.0',
+        'redis==4.6.0'
     ],
     extras_require={
         'dev': [],
         'prod': []
     }
 )
```

