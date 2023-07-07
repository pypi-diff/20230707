# Comparing `tmp/django-learngual-0.13.5.tar.gz` & `tmp/django-learngual-0.13.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.5.tar", last modified: Tue Jul  4 13:07:20 2023, max compression
+gzip compressed data, was "django-learngual-0.13.6.tar", last modified: Fri Jul  7 14:31:01 2023, max compression
```

## Comparing `django-learngual-0.13.5.tar` & `django-learngual-0.13.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-04 13:06:29.000000 django-learngual-0.13.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 13:06:29.000000 django-learngual-0.13.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 13:07:20.167372 django-learngual-0.13.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 13:06:29.000000 django-learngual-0.13.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.163372 django-learngual-0.13.5/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 13:07:20.000000 django-learngual-0.13.5/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:20.167372 django-learngual-0.13.5/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-04 13:07:15.000000 django-learngual-0.13.5/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-04 13:07:20.171372 django-learngual-0.13.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:06:29.000000 django-learngual-0.13.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-07 14:30:06.000000 django-learngual-0.13.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 14:30:06.000000 django-learngual-0.13.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-07 14:31:01.199071 django-learngual-0.13.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-07 14:30:06.000000 django-learngual-0.13.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 14:31:01.199071 django-learngual-0.13.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:30:06.000000 django-learngual-0.13.6/setup.py
```

### Comparing `django-learngual-0.13.5/LICENSE` & `django-learngual-0.13.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/PKG-INFO` & `django-learngual-0.13.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.5
+Version: 0.13.6
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.5/README.rst` & `django-learngual-0.13.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.6/django_learngual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.5
+Version: 0.13.6
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.5/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.6/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/apps.py` & `django-learngual-0.13.6/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/authentication.py` & `django-learngual-0.13.6/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/permissions.py` & `django-learngual-0.13.6/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/tests/request_mock.py` & `django-learngual-0.13.6/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/tests/test_authentication.py` & `django-learngual-0.13.6/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/tests/test_utils.py` & `django-learngual-0.13.6/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.5/learngual/utils.py` & `django-learngual-0.13.6/learngual/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,19 +91,17 @@
                     start, stop = map(int, index_or_slice.split(":"))
                     value = value[key][start:stop]
                 else:
                     index = int(index_or_slice)
                     value = value[key][index]
             else:
                 value = value[key]
-    except (KeyError, TypeError, IndexError, ValueError) as e:
+    except (KeyError, TypeError, IndexError, ValueError):
         value = None
-        logging.warning(
-            f"An error occurred while retrieving nested value from path '{path}': {e}"
-        )
+        logging.warning(f"Could not retrieve path:'{path}'.")
 
     return value
 
 
 def update_nested_value(data: dict[str, Any], path: str, value: Any) -> dict[str, Any]:
     """
     Update a nested dictionary value using a dot path and return the modified dictionary.
@@ -404,14 +402,20 @@
 
         Raises:
             requests.exceptions.RequestException: _description_
 
         Returns:
             _type_: _description_
         """
+        if "localhost" in base_url:
+            return {
+                "id": "test-local",
+                "metadata": {"request_count": True, "messages": True},
+            }
+
         params = params.strip("?")
         params = dict([x.split("=") for x in params.split("&")])
 
         url_path = f"/{service}/v1/permission/{permission_id}/"
         res = requests.patch(
             base_url.rstrip("/") + url_path + get_service_request_params(**params),
             json=permmission_data,
@@ -455,14 +459,22 @@
             base_url (str):
             dot_path (str):Default:None, e.g metadata.request_count.value
             headers (dict):Default:{}
             params (str):Default:"", e.g name=ann&age=102
             cache_timeout (float):Default:timezone.timedelta(hours=1).total_seconds()
         """
         url_path = f"/{service}/v1/service/permission/{permission_id}/"
+        if "localhost" in base_url:
+            if dot_path:
+                return True
+            else:
+                return {
+                    "id": "test-local",
+                    "metadata": {"request_count": True, "messages": True},
+                }
         data = cache.get(url_path)
 
         params = params.strip("?")
         params = dict([x.split("=") for x in params.split("&") if x])
 
         if not data:
             res = requests.get(
```

### Comparing `django-learngual-0.13.5/setup.cfg` & `django-learngual-0.13.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.5
+version = 0.13.6
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

