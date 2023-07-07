# Comparing `tmp/Zeraora-0.3.3.tar.gz` & `tmp/Zeraora-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.3.3.tar", last modified: Thu Jul  6 06:36:38 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.3.4.tar", last modified: Fri Jul  7 15:23:38 2023, max compression
```

## Comparing `Zeraora-0.3.3.tar` & `Zeraora-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-06 06:36:38.000000 Zeraora-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-06 06:36:21.000000 Zeraora-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 06:36:38.000000 Zeraora-0.3.3/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:36:38.000000 Zeraora-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 06:36:21.000000 Zeraora-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/constants/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/dj/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/dj/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:36:38.000000 Zeraora-0.3.3/zeraora/drf/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/gvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/throwables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-06 06:36:21.000000 Zeraora-0.3.3/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 15:23:38.000000 Zeraora-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-07 15:23:24.000000 Zeraora-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 15:23:38.000000 Zeraora-0.3.4/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:23:38.000000 Zeraora-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 15:23:24.000000 Zeraora-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/click/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/click/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/constants/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/dj/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:23:38.000000 Zeraora-0.3.4/zeraora/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/gvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/throwables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-07-07 15:23:24.000000 Zeraora-0.3.4/zeraora/utils.py
```

### Comparing `Zeraora-0.3.3/PKG-INFO` & `Zeraora-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.3
+Version: 0.3.4
 Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.4 Summary:
 ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
```

### Comparing `Zeraora-0.3.3/README.md` & `Zeraora-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.3.4/Zeraora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.3.3
+Version: 0.3.4
 Summary: 为了跨平台跨项目复用代码而开发的工具库。A utility Python package for our personal and corporate projects, with long time support.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.4 Summary:
 ä¸ºäºè·¨å¹³å°è·¨é¡¹ç®å¤ç¨ä»£ç èå¼åçå·¥å·åºãA utility Python
 package for our personal and corporate projects, with long time support. Home-
 page: https://github.com/aixcyi/zeraora Author: aixcyi Author-email:
 75880483+aixcyi@users.noreply.github.com License: MIT Project-URL: Source,
 https://github.com/aixcyi/zeraora Project-URL: Tracker, https://github.com/
 aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
```

### Comparing `Zeraora-0.3.3/Zeraora.egg-info/SOURCES.txt` & `Zeraora-0.3.4/Zeraora.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 zeraora/converters.py
 zeraora/generators.py
 zeraora/gvs.py
 zeraora/structures.py
 zeraora/throwables.py
 zeraora/typeclasses.py
 zeraora/utils.py
+zeraora/click/__init__.py
+zeraora/click/decorators.py
 zeraora/constants/__init__.py
 zeraora/constants/charsets.py
 zeraora/constants/configs.py
 zeraora/constants/enumerations.py
 zeraora/dj/__init__.py
 zeraora/dj/fields.py
 zeraora/dj/lookups.py
```

### Comparing `Zeraora-0.3.3/setup.py` & `Zeraora-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/constants/charsets.py` & `Zeraora-0.3.4/zeraora/constants/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/constants/configs.py` & `Zeraora-0.3.4/zeraora/constants/configs.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/constants/enumerations.py` & `Zeraora-0.3.4/zeraora/constants/enumerations.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/converters.py` & `Zeraora-0.3.4/zeraora/converters.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/dj/fields.py` & `Zeraora-0.3.4/zeraora/dj/fields.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 """
 定制的 Django ORM模型字段。
 """
-
-__all__ = [
-    'BizField',
-    'MoneyField',
-    'OSSPathField',
-]
-
 from decimal import Decimal
 
 try:
     from django.db import models
     from django.utils.translation import gettext_lazy
 except ImportError as e:
     raise ImportError('需要安装Django框架：\npip install django') from e
```

### Comparing `Zeraora-0.3.3/zeraora/dj/lookups.py` & `Zeraora-0.3.4/zeraora/dj/lookups.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,20 +3,14 @@
 
 这是什么？
 https://docs.djangoproject.com/zh-hans/4.2/ref/models/lookups/#lookup-reference
 
 如何自定义？
 https://docs.djangoproject.com/zh-hans/4.2/howto/custom-lookups/
 """
-
-__all__ = [
-    'BitsIn',
-    'BitsAllIn',
-]
-
 try:
     from django.db.models import Lookup
 except ImportError as e:
     raise ImportError('需要安装Django框架：\npip install django') from e
 
 
 class BitsIn(Lookup):
```

### Comparing `Zeraora-0.3.3/zeraora/dj/models.py` & `Zeraora-0.3.4/zeraora/dj/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 """
 对 Django ORM模型 的增强。
 """
 from __future__ import annotations
 
-__all__ = [
-    'SnakeModel', 'CreateTimeMixin',
-    'TimeMixin', 'ActiveStatusMixin', 'DeletionMixin',
-    'IndexMixin', 'ShortIndexMixin',
-    'UrgencyMixin', 'ImportanceMixin',
-    'AddressMixin', 'GlobalAddressMixin', 'BizMixin',
-]
-
 import re
 import uuid
 
 from .. import gvs
 from ..constants import Degree, Province
 from ..structures import DivisionCode
 from ..utils import warn_empty_ads
```

### Comparing `Zeraora-0.3.3/zeraora/drf/filters.py` & `Zeraora-0.3.4/zeraora/drf/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,14 @@
 
 这是什么？
 https://www.django-rest-framework.org/api-guide/filtering/
 
 如何自定义？
 https://www.django-rest-framework.org/api-guide/filtering/#custom-generic-filtering
 """
-
-__all__ = [
-    'ExistingFilterBackend',
-    'ActiveStatusFilterBackend',
-]
-
 try:
     from django.core.exceptions import FieldDoesNotExist
     from rest_framework.filters import BaseFilterBackend
 except ImportError as e:
     raise ImportError('需要安装Django以及DRF框架：\npip install django djangorestframework') from e
```

### Comparing `Zeraora-0.3.3/zeraora/drf/viewsets.py` & `Zeraora-0.3.4/zeraora/drf/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 """
 对 Django REST Framework 视图集（viewset）的增强。
 """
 from __future__ import annotations
 
-__all__ = [
-    'EasyViewSetMixin',
-    'SoftDeleteModelMixin',
-]
-
 from typing import Any
 
 try:
     from django.utils.decorators import classonlymethod
     from rest_framework import status
     from rest_framework.response import Response
     from rest_framework.viewsets import ViewSetMixin
```

### Comparing `Zeraora-0.3.3/zeraora/generators.py` & `Zeraora-0.3.4/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/structures.py` & `Zeraora-0.3.4/zeraora/structures.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/typeclasses.py` & `Zeraora-0.3.4/zeraora/typeclasses.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.3/zeraora/utils.py` & `Zeraora-0.3.4/zeraora/utils.py`

 * *Files identical despite different names*

