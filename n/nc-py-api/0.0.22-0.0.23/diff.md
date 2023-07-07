# Comparing `tmp/nc_py_api-0.0.22.tar.gz` & `tmp/nc_py_api-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.22.tar", last modified: Wed Jul  5 10:24:16 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.23.tar", last modified: Fri Jul  7 18:45:52 2023, max compression
```

## Comparing `nc_py_api-0.0.22.tar` & `nc_py_api-0.0.23.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12320 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 10:24:09.000000 nc_py_api-0.0.22/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12338 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 18:45:45.000000 nc_py_api-0.0.23/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/setup.py
```

### Comparing `nc_py_api-0.0.22/LICENSE` & `nc_py_api-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/PKG-INFO` & `nc_py_api-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc_py_api
-Version: 0.0.22
+Version: 0.0.23
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.22/README.md` & `nc_py_api-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/_session.py` & `nc_py_api-0.0.23/nc_py_api/_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     full_nc_url: str
     endpoint: str
     dav_endpoint: str
     dav_url_suffix: str
 
     def __init__(self, **kwargs):
         self.full_nc_url = self._get_value("nextcloud_url", **kwargs)
-        self.endpoint = self.full_nc_url.removesuffix("/index.php")
+        self.endpoint = self.full_nc_url.removesuffix("/index.php").removesuffix("/")
         self.dav_url_suffix = self._get_value("dav_url_suffix", raise_not_found=False, **kwargs)
         if not self.dav_url_suffix:
             self.dav_url_suffix = options.DAV_URL_SUFFIX
         self.dav_endpoint = self.endpoint + self.dav_url_suffix
 
     @staticmethod
     def _get_value(value_name: str, raise_not_found=True, **kwargs):
```

### Comparing `nc_py_api-0.0.22/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.23/nc_py_api/appconfig_preferences_ex.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/apps.py` & `nc_py_api-0.0.23/nc_py_api/apps.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/constants.py` & `nc_py_api-0.0.23/nc_py_api/constants.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/exceptions.py` & `nc_py_api-0.0.23/nc_py_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/files.py` & `nc_py_api-0.0.23/nc_py_api/files.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.23/nc_py_api/integration_fastapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Directly related stuff to FastAPI.
 """
 
-from typing import Annotated, Callable
+from typing import Annotated, Callable, Optional
 
 from fastapi import Depends, FastAPI, HTTPException, Request, status
 from fastapi.responses import JSONResponse
 
 from .constants import ApiScopesStruct
 from .nextcloud import NextcloudApp
 
@@ -35,11 +35,14 @@
         enabled: bool,
         nc: Annotated[NextcloudApp, Depends(nc_app)],
     ):
         r = callback(enabled, nc)
         return JSONResponse(content={"error": r}, status_code=200)
 
 
-def enable_heartbeat(fast_api_app: FastAPI):
+def enable_heartbeat(fast_api_app: FastAPI, callback: Optional[Callable[[], str]] = None):
     @fast_api_app.get("/heartbeat")
     def heartbeat_handler():
-        return JSONResponse(content={"status": "ok"}, status_code=200)
+        return_status = "ok"
+        if callback is not None:
+            return_status = callback()
+        return JSONResponse(content={"status": return_status}, status_code=200)
```

### Comparing `nc_py_api-0.0.22/nc_py_api/misc.py` & `nc_py_api-0.0.23/nc_py_api/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/nextcloud.py` & `nc_py_api-0.0.23/nc_py_api/nextcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.appconfig_ex_api = AppConfigExAPI(self._session)
         self.preferences_ex_api = PreferencesExAPI(self._session)
         self.ui_files_actions = UiFilesActionsAPI(self._session)
 
     def log(self, log_lvl: LogLvl, content: str):
         if self.check_capabilities("app_ecosystem_v2"):
             return
-        if int(log_lvl) < self.capabilities["app_ecosystem_v2"].get("loglevel", 4):
+        if int(log_lvl) < self.capabilities["app_ecosystem_v2"].get("loglevel", 0):
             return
         self._session.ocs(
             method="POST", path=f"{APP_V2_BASIC_URL}/log", json={"level": int(log_lvl), "message": content}
         )
 
     # def download_log(self) -> bytes:
     #     return self._session.ocs(method="GET", path=f"{APP_V2_BASIC_URL}/log")
```

### Comparing `nc_py_api-0.0.22/nc_py_api/preferences.py` & `nc_py_api-0.0.23/nc_py_api/preferences.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/theming.py` & `nc_py_api-0.0.23/nc_py_api/theming.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.23/nc_py_api/ui_files_actions_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/users.py` & `nc_py_api-0.0.23/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/users_groups.py` & `nc_py_api-0.0.23/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/users_status.py` & `nc_py_api-0.0.23/nc_py_api/users_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api/weather_status.py` & `nc_py_api-0.0.23/nc_py_api/weather_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.23/nc_py_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.0.22
+Version: 0.0.23
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.22/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.23/nc_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/pyproject.toml` & `nc_py_api-0.0.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.22/setup.cfg` & `nc_py_api-0.0.23/setup.cfg`

 * *Files identical despite different names*

