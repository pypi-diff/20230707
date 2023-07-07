# Comparing `tmp/ckanext-federated-index-0.0.1.tar.gz` & `tmp/ckanext-federated-index-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-federated-index-0.0.1.tar", last modified: Fri Jul  7 19:30:11 2023, max compression
+gzip compressed data, was "ckanext-federated-index-0.0.2.tar", last modified: Fri Jul  7 20:11:58 2023, max compression
```

## Comparing `ckanext-federated-index-0.0.1.tar` & `ckanext-federated-index-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      222 2023-07-07 16:30:30.000000 ckanext-federated-index-0.0.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4004 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3427 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.529203 ckanext-federated-index-0.0.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-07-07 19:26:28.000000 ckanext-federated-index-0.0.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext/federated_index/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext/federated_index/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      178 2023-07-07 19:26:28.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      152 2023-07-07 19:12:25.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      321 2023-07-07 19:26:40.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:36:26.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4082 2023-07-07 19:27:54.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1017 2023-07-07 19:26:40.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2023-07-07 19:26:28.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2023-07-07 19:28:10.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/logic/validators.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3618 2023-07-07 19:26:40.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2092 2023-07-07 19:26:40.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.529203 ckanext-federated-index-0.0.1/ckanext/federated_index/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext/federated_index/templates/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      448 2023-07-07 19:23:35.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/templates/snippets/package_item.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext/federated_index/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:27:05.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:42:35.000000 ckanext-federated-index-0.0.1/ckanext/federated_index/types.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4004 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1173 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 19:30:11.000000 ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4200 2023-07-07 15:15:05.000000 ckanext-federated-index-0.0.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 16:30:15.000000 ckanext-federated-index-0.0.1/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1689 2023-07-07 19:30:11.539202 ckanext-federated-index-0.0.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-07-07 19:11:23.000000 ckanext-federated-index-0.0.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      222 2023-07-07 16:30:30.000000 ckanext-federated-index-0.0.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4004 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3427 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.595718 ckanext-federated-index-0.0.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-07-07 19:26:28.000000 ckanext-federated-index-0.0.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext/federated_index/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext/federated_index/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      152 2023-07-07 19:12:25.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      321 2023-07-07 19:26:40.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:36:26.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4365 2023-07-07 20:09:40.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1290 2023-07-07 20:09:39.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      812 2023-07-07 20:10:21.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      496 2023-07-07 20:09:40.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/logic/validators.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3866 2023-07-07 20:09:39.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2805 2023-07-07 20:11:35.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.595718 ckanext-federated-index-0.0.2/ckanext/federated_index/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext/federated_index/templates/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      448 2023-07-07 19:23:35.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/templates/snippets/package_item.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext/federated_index/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:29:16.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 19:27:05.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-07-07 14:42:35.000000 ckanext-federated-index-0.0.2/ckanext/federated_index/types.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4004 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1142 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 20:11:58.000000 ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4200 2023-07-07 15:15:05.000000 ckanext-federated-index-0.0.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-07 16:30:15.000000 ckanext-federated-index-0.0.2/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1689 2023-07-07 20:11:58.605718 ckanext-federated-index-0.0.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-07-07 19:11:23.000000 ckanext-federated-index-0.0.2/setup.py
```

### Comparing `ckanext-federated-index-0.0.1/LICENSE` & `ckanext-federated-index-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-federated-index-0.0.1/PKG-INFO` & `ckanext-federated-index-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-federated-index
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/DataShades/ckanext-federated-index
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-federated-index-0.0.1/README.md` & `ckanext-federated-index-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-federated-index-0.0.1/ckanext/federated_index/logic/action.py` & `ckanext-federated-index-0.0.2/ckanext/federated_index/logic/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 import logging
 from typing import Any
 
 from sqlalchemy.exc import IntegrityError
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
-from ckan import model, types
+from ckan import model
 from ckan.lib import redis, search
 from ckan.logic import validate
 
 from ckanext.federated_index import interfaces, shared
 
 from . import schema
 
 log = logging.getLogger(__name__)
 
 
+def get_actions():
+    return {
+        "federated_index_profile_refresh": federated_index_profile_refresh,
+        "federated_index_profile_list": federated_index_profile_list,
+        "federated_index_profile_index": federated_index_profile_index,
+        "federated_index_profile_clear": federated_index_profile_clear,
+    }
+
+
 @validate(schema.profile_refresh)
 def federated_index_profile_refresh(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
     tk.check_access("federated_index_profile_refresh", context, data_dict)
 
     conn: redis.Redis[bytes] = redis.connect_to_redis()
     key = _cache_key(data_dict["profile"])
     conn.delete(key)
@@ -42,15 +51,15 @@
 def _cache_key(profile: shared.Profile) -> str:
     site_id = tk.config["ckan.site_id"]
     return f"ckan:{site_id}:federated_index:profile:{profile.id}:datasets"
 
 
 @validate(schema.profile_list)
 def federated_index_profile_list(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
     tk.check_access("federated_index_profile_list", context, data_dict)
 
     conn: redis.Redis[bytes] = redis.connect_to_redis()
     key = _cache_key(data_dict["profile"])
 
@@ -61,15 +70,15 @@
         ],
         "count": conn.llen(key),
     }
 
 
 @validate(schema.profile_index)
 def federated_index_profile_index(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
     tk.check_access("federated_index_profile_index", context, data_dict)
 
     profile: shared.Profile = data_dict["profile"]
     conn: redis.Redis[bytes] = redis.connect_to_redis()
     key = _cache_key(profile)
@@ -126,15 +135,15 @@
         "key": key,
         "size": conn.llen(key),
     }
 
 
 @validate(schema.profile_clear)
 def federated_index_profile_clear(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
 ) -> dict[str, Any]:
     tk.check_access("federated_index_profile_clear", context, data_dict)
     profile: shared.Profile = data_dict["profile"]
 
     conn = search.make_connection()
     query = f"+{profile.index_profile_field}:{profile.id}"
```

### Comparing `ckanext-federated-index-0.0.1/ckanext/federated_index/logic/auth.py` & `ckanext-federated-index-0.0.2/ckanext/federated_index/logic/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from __future__ import annotations
 
 from typing import Any
 
-from ckan import authz, types
+from ckan import authz
+
+
+def get_auth_functions():
+    return {
+        "federated_index_access": federated_index_access,
+        "federated_index_profile_refresh": federated_index_profile_refresh,
+        "federated_index_profile_list": federated_index_profile_list,
+        "federated_index_profile_index": federated_index_profile_index,
+        "federated_index_profile_clear": federated_index_profile_clear,
+    }
 
 
 def federated_index_access(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
-) -> types.AuthResult:
+) -> Any:
     return {"success": False}
 
 
 def federated_index_profile_refresh(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
-) -> types.AuthResult:
+) -> Any:
     return authz.is_authorized("federated_index_access", context, data_dict)
 
 
 def federated_index_profile_list(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
-) -> types.AuthResult:
+) -> Any:
     return authz.is_authorized("federated_index_access", context, data_dict)
 
 
 def federated_index_profile_index(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
-) -> types.AuthResult:
+) -> Any:
     return authz.is_authorized("federated_index_access", context, data_dict)
 
 
 def federated_index_profile_clear(
-    context: types.Context,
+    context: Any,
     data_dict: dict[str, Any],
-) -> types.AuthResult:
+) -> Any:
     return authz.is_authorized("federated_index_access", context, data_dict)
```

### Comparing `ckanext-federated-index-0.0.1/ckanext/federated_index/plugin.py` & `ckanext-federated-index-0.0.2/ckanext/federated_index/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urljoin
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 
 from . import interfaces, shared
+from .logic import action, auth, validators
 
 if TYPE_CHECKING:
     from ckan.common import CKANConfig
 
 PKG_MANDATORY_FIELDS: list[str] = [
     "id",
     "extras",
@@ -28,23 +29,27 @@
 RES_MANDATORY_FIELDS: list[str] = [
     "id",
     "created",
     "metadata_modified",
 ]
 
 
-@tk.blanket.config_declarations
-@tk.blanket.auth_functions
-@tk.blanket.actions
-@tk.blanket.validators
-@tk.blanket.cli
+# @tk.blanket.config_declarations
 class FederatedIndexPlugin(p.SingletonPlugin):
     p.implements(p.IConfigurer, inherit=True)
     p.implements(interfaces.IFederatedIndex, inherit=True)
 
+    p.implements(p.IActions)
+    p.implements(p.IAuthFunctions)
+    p.implements(p.IValidators)
+
+    get_validators = staticmethod(validators.get_validators)
+    get_actions = staticmethod(action.get_actions)
+    get_auth_functions = staticmethod(auth.get_auth_functions)
+
     def update_config(self, config: CKANConfig) -> None:
         tk.add_template_directory(config, "templates")
 
     def federated_index_before_index(
         self,
         pkg_dict: dict[str, Any],
         profile: shared.Profile,
@@ -62,15 +67,15 @@
                         profile.url,
                         f"/{pkg_dict['type']}/{pkg_dict['id']}",
                     ),
                 },
             ],
         )
 
-        if tk.config["ckanext.federated_index.align_with_local_schema"]:
+        if tk.asbool(tk.config.get("ckanext.federated_index.align_with_local_schema")):
             _align_with_local_schema(pkg_dict)
 
         return pkg_dict
 
 
 def _align_with_local_schema(dataset: dict[str, Any]) -> None:
     """Throw away fields that doesn't exist in our local dataset schema"""
```

### Comparing `ckanext-federated-index-0.0.1/ckanext/federated_index/shared.py` & `ckanext-federated-index-0.0.2/ckanext/federated_index/shared.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 import dataclasses
 import json
 import logging
 from collections import defaultdict
 from typing import Any, Iterable
 
+import requests
 from ckanapi import RemoteCKAN
 
 import ckan.plugins.toolkit as tk
 
 PROFILE_PREFIX: str = "ckanext.federated_index.profile."
 
 log = logging.getLogger(__name__)
+NUMBER_OF_ATTEMPTS = 5
 
 
 @dataclasses.dataclass
 class Profile:
     id: str
     url: str
     api_key: str = ""
@@ -25,34 +27,59 @@
     timeout: int = 10
 
     def __post_init__(self):
         if isinstance(self.extras, str):
             self.extras = json.loads(self.extras)
 
     def get_client(self):
-        return RemoteCKAN(self.url, self.api_key)
+        return RemoteCKAN(
+            self.url,
+            self.api_key,
+            user_agent=(
+                "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
+                " AppleWebKit/537.36 (KHTML, like Gecko)"
+                " Chrome/117.0.0.0 Safari/537.36",
+            ),
+        )
 
     def fetch_packages(self) -> Iterable[dict[str, Any]]:
         payload = self.extras.get("search_payload", {})
         payload.setdefault("start", 0)
 
         client = self.get_client()
 
+        attempt = 0
+
         while True:
             log.debug(
                 "Fetch packages for profile %s starting from %s",
                 self.id,
                 payload["start"],
             )
 
-            result: dict[str, Any] = client.call_action(
-                "package_search",
-                payload,
-                requests_kwargs={"timeout": self.timeout},
-            )
+            try:
+                result: dict[str, Any] = client.call_action(
+                    "package_search",
+                    payload,
+                    requests_kwargs={"timeout": self.timeout},
+                )
+            except requests.RequestException:
+                log.exception(
+                    "Cannot pull datasets for profile %s: %s",
+                    self.id,
+                    payload,
+                )
+                attempt += 1
+
+                if attempt > NUMBER_OF_ATTEMPTS:
+                    break
+
+                continue
+
+            attempt = 0
             yield from result["results"]
 
             payload["start"] += len(result["results"])
 
             if result["count"] <= payload["start"]:
                 break
```

### Comparing `ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/PKG-INFO` & `ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-federated-index
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/DataShades/ckanext-federated-index
 Author: Alexandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-federated-index-0.0.1/ckanext_federated_index.egg-info/SOURCES.txt` & `ckanext-federated-index-0.0.2/ckanext_federated_index.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/federated_index/__init__.py
-ckanext/federated_index/cli.py
 ckanext/federated_index/config_declaration.yaml
 ckanext/federated_index/interfaces.py
 ckanext/federated_index/plugin.py
 ckanext/federated_index/shared.py
 ckanext/federated_index/types.py
 ckanext/federated_index/assets/script.js
 ckanext/federated_index/assets/style.css
```

### Comparing `ckanext-federated-index-0.0.1/pyproject.toml` & `ckanext-federated-index-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-federated-index-0.0.1/setup.cfg` & `ckanext-federated-index-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-federated-index
-version = 0.0.1
+version = 0.0.2
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-federated-index
 author = Alexandr Cherniavskyi
 author_email = mutantsan@gmail.com
 license = AGPL
```

