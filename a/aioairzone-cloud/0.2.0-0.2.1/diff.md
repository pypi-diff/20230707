# Comparing `tmp/aioairzone-cloud-0.2.0.tar.gz` & `tmp/aioairzone-cloud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.2.0.tar", last modified: Tue Jun 27 18:41:21 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.2.1.tar", last modified: Fri Jul  7 09:18:46 2023, max compression
```

## Comparing `aioairzone-cloud-0.2.0.tar` & `aioairzone-cloud-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      936 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    21059 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1800 2023-06-26 18:43:43.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     7503 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4886 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    23649 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-06-25 08:46:58.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1605 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5294 2023-06-25 08:46:58.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3091 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-06-27 18:41:21.000000 aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.0/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.0/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-06-27 18:41:21.365568 aioairzone-cloud-0.2.0/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-07-07 09:18:46.669276 aioairzone-cloud-0.2.1/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.1/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.1/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-07-07 09:18:46.669276 aioairzone-cloud-0.2.1/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.1/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-07-07 09:18:46.665276 aioairzone-cloud-0.2.1/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      936 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    22746 2023-07-07 09:17:15.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1800 2023-06-26 18:43:43.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     7693 2023-07-07 09:17:15.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5391 2023-07-06 17:06:19.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11161 2023-07-07 09:17:15.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    23460 2023-07-06 17:06:19.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-06-25 08:46:58.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1605 2023-06-27 18:40:36.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5665 2023-07-06 17:06:19.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3091 2023-07-06 16:58:06.000000 aioairzone-cloud-0.2.1/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-07-07 09:18:46.669276 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      696 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-07-07 09:18:46.000000 aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-07-07 09:17:57.000000 aioairzone-cloud-0.2.1/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.2.1/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-07-07 09:18:46.669276 aioairzone-cloud-0.2.1/setup.cfg
```

### Comparing `aioairzone-cloud-0.2.0/LICENSE` & `aioairzone-cloud-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/PKG-INFO` & `aioairzone-cloud-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.2.0/README.md` & `aioairzone-cloud-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/aidoo.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/aidoo.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/cloudapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     API_AZ_SYSTEM,
     API_AZ_ZONE,
     API_CONFIG,
     API_DEVICE_ID,
     API_DEVICE_TYPE,
     API_DEVICES,
     API_EMAIL,
+    API_GROUP,
     API_GROUPS,
     API_INSTALLATION_ID,
     API_INSTALLATIONS,
     API_OPTS,
     API_PARAM,
     API_PASSWORD,
     API_REFRESH_TOKEN,
@@ -37,14 +38,15 @@
     API_USER,
     API_USER_LOGOUT,
     API_V1,
     API_VALUE,
     API_WS,
     API_WS_ID,
     AZD_AIDOOS,
+    AZD_GROUPS,
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
     HEADER_AUTHORIZATION,
     HEADER_BEARER,
     HTTP_CALL_TIMEOUT,
@@ -61,14 +63,15 @@
     AirzoneCloudError,
     APIError,
     AuthError,
     LoginError,
     TokenRefreshError,
     TooManyRequests,
 )
+from .group import Group
 from .installation import Installation
 from .system import System
 from .webserver import WebServer
 from .zone import Zone
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -86,14 +89,15 @@
             RAW_DEVICES_CONFIG: {},
             RAW_DEVICES_STATUS: {},
             RAW_INSTALLATIONS: {},
             RAW_WEBSERVERS: {},
         }
         self.aidoos: dict[str, Aidoo] = {}
         self.aiohttp_session = aiohttp_session
+        self.groups: dict[str, Group] = {}
         self.installations: dict[str, Installation] = {}
         self.options = options
         self.refresh_time: datetime | None = None
         self.refresh_token: str | None = None
         self.systems: dict[str, System] = {}
         self.token: str | None = None
         self.webservers: dict[str, WebServer] = {}
@@ -240,14 +244,27 @@
 
         return await self.api_request(
             "PATCH",
             f"{API_V1}/{API_DEVICES}/{url_id}",
             json,
         )
 
+    async def api_put_group(self, group: Group, json: dict[str, Any]) -> dict[str, Any]:
+        """Perform a PUT request to update group parameters."""
+        grp_id = group.get_id()
+        grp_url = urllib.parse.quote(grp_id)
+        inst_id = group.get_installation()
+        inst_url = urllib.parse.quote(inst_id)
+
+        return await self.api_request(
+            "PUT",
+            f"{API_V1}/{API_INSTALLATIONS}/{inst_url}/{API_GROUP}/{grp_url}",
+            json,
+        )
+
     async def api_set_device_param(
         self, device: Device, param: str, data: dict[str, Any]
     ) -> None:
         """Set device parameter."""
         json = {
             API_PARAM: param,
             API_VALUE: data[API_VALUE],
@@ -268,14 +285,20 @@
         tasks = []
 
         for param, data in params.items():
             tasks += [self.api_set_device_param(device, param, data)]
 
         await asyncio.gather(*tasks)
 
+    async def api_set_group_params(self, group: Group, params: dict[str, Any]) -> None:
+        """Set group parameters."""
+        await self.api_put_group(group, params)
+
+        group.set_params(params)
+
     async def api_set_aidoo_id_params(
         self, aidoo_id: str, params: dict[str, Any]
     ) -> None:
         """Set aidoo parameters."""
         aidoo = self.get_aidoo_id(aidoo_id)
         if aidoo is not None:
             await self.api_set_device_params(aidoo, params)
@@ -288,14 +311,22 @@
             self.get_aidoo_id(device_id)
             or self.get_system_id(device_id)
             or self.get_zone_id(device_id)
         )
         if device is not None:
             await self.api_set_device_params(device, params)
 
+    async def api_set_group_id_params(
+        self, group_id: str, params: dict[str, Any]
+    ) -> None:
+        """Set group parameters."""
+        group = self.get_group_id(group_id)
+        if group is not None:
+            await self.api_set_group_params(group, params)
+
     async def api_set_system_id_params(
         self, system_id: str, params: dict[str, Any]
     ) -> None:
         """Set system parameters."""
         system = self.get_system_id(system_id)
         if system is not None:
             await self.api_set_device_params(system, params)
@@ -367,14 +398,20 @@
 
         if len(self.aidoos) > 0:
             aidoos: dict[str, Any] = {}
             for key, aidoo in self.aidoos.items():
                 aidoos[key] = aidoo.data()
             data[AZD_AIDOOS] = aidoos
 
+        if len(self.groups) > 0:
+            groups: dict[str, Any] = {}
+            for key, group in self.groups.items():
+                groups[key] = group.data()
+            data[AZD_GROUPS] = groups
+
         if len(self.installations) > 0:
             installations: dict[str, Any] = {}
             for key, installation in self.installations.items():
                 installations[key] = installation.data()
             data[AZD_INSTALLATIONS] = installations
 
         if len(self.systems) > 0:
@@ -397,14 +434,18 @@
 
         return data
 
     def get_aidoo_id(self, aidoo_id: str) -> Aidoo | None:
         """Return Airzone Cloud Aidoo by ID."""
         return self.aidoos.get(aidoo_id)
 
+    def get_group_id(self, group_id: str) -> Group | None:
+        """Return Airzone Cloud Group by ID."""
+        return self.groups.get(group_id)
+
     def get_installation_id(self, inst_id: str) -> Installation | None:
         """Return Airzone Cloud Installation by ID."""
         return self.installations.get(inst_id)
 
     def get_system_id(self, sys_id: str) -> System | None:
         """Return Airzone Cloud System by ID."""
         return self.systems.get(sys_id)
@@ -468,35 +509,40 @@
             tasks += [self.update_aidoo(aidoo)]
 
         await asyncio.gather(*tasks)
 
     async def update_installation(self, inst: Installation) -> None:
         """Update Airzone Cloud installation from API."""
         installation_data = await self.api_get_installation(inst)
-        for group in installation_data[API_GROUPS]:
-            for device_data in group[API_DEVICES]:
+        for group_data in installation_data[API_GROUPS]:
+            group = Group(inst.get_id(), group_data)
+            self.groups[group.get_id()] = group
+            for device_data in group_data[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_TYPE]:
                     if self.get_zone_id(device_data[API_DEVICE_ID]) is None:
                         zone = Zone(inst.get_id(), device_data[API_WS_ID], device_data)
                         if zone is not None:
                             self.zones[zone.get_id()] = zone
+                            group.add_zone(zone)
                 elif API_AZ_SYSTEM == device_data[API_TYPE]:
                     if self.get_system_id(device_data[API_DEVICE_ID]) is None:
                         system = System(
                             inst.get_id(), device_data[API_WS_ID], device_data
                         )
                         if system is not None:
                             self.systems[system.get_id()] = system
+                            group.add_system(system)
                 elif API_AZ_AIDOO == device_data[API_TYPE]:
                     if self.get_aidoo_id(device_data[API_DEVICE_ID]) is None:
                         aidoo = Aidoo(
                             inst.get_id(), device_data[API_WS_ID], device_data
                         )
                         if aidoo is not None:
                             self.aidoos[aidoo.get_id()] = aidoo
+                            group.add_aidoo(aidoo)
 
     async def update_installations(self) -> None:
         """Update Airzone Cloud installations from API."""
         installations_data = await self.api_get_installations()
         for installation_data in installations_data[API_INSTALLATIONS]:
             if self.get_installation_id(installation_data[API_INSTALLATION_ID]) is None:
                 installation = Installation(installation_data)
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/common.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/const.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 from datetime import timedelta
 from typing import Final
 
 API_ACTIVE: Final[str] = "active"
 API_AUTH_LOGIN: Final[str] = "auth/login"
 API_AUTH_REFRESH_TOKEN: Final[str] = "auth/refreshToken"
+API_AUTO_MODE: Final[str] = "auto_mode"
 API_CELSIUS: Final[str] = "celsius"
 API_CITY: Final[str] = "city"
 API_CONFIG: Final[str] = "config"
 API_CONNECTION_DATE: Final[str] = "connection_date"
 API_DEVICE_ID: Final[str] = "device_id"
 API_DEVICE_TYPE: Final[str] = "device_type"
 API_DEVICES: Final[str] = "devices"
 API_DISCONNECTION_DATE: Final[str] = "disconnection_date"
 API_ECO_CONF: Final[str] = "eco_conf"
 API_EMAIL: Final[str] = "email"
 API_ERRORS: Final[str] = "errors"
 API_FAH: Final[str] = "fah"
+API_GROUP: Final[str] = "group"
 API_GROUP_ID: Final[str] = "group_id"
 API_GROUPS: Final[str] = "groups"
 API_HUMIDITY: Final[str] = "humidity"
 API_INSTALLATION_ID: Final[str] = "installation_id"
 API_INSTALLATIONS: Final[str] = "installations"
 API_IS_CONNECTED: Final[str] = "isConnected"
 API_LOCAL_TEMP: Final[str] = "local_temp"
@@ -101,23 +103,26 @@
 AZD_ACTIVE: Final[str] = "active"
 AZD_AIDOOS: Final[str] = "aidoos"
 AZD_AVAILABLE: Final[str] = "available"
 AZD_CONNECTION_DATE: Final[str] = "connection-date"
 AZD_DISCONNECTION_DATE: Final[str] = "disconnection-date"
 AZD_ERRORS: Final[str] = "errors"
 AZD_FIRMWARE: Final[str] = "firmware"
+AZD_GROUPS: Final[str] = "groups"
 AZD_HUMIDITY: Final[str] = "humidity"
 AZD_ID: Final[str] = "id"
 AZD_INSTALLATION: Final[str] = "installation"
 AZD_INSTALLATIONS: Final[str] = "installations"
 AZD_IS_CONNECTED: Final[str] = "is-connected"
 AZD_MASTER: Final[str] = "master"
 AZD_MODE: Final[str] = "mode"
+AZD_MODE_AUTO: Final[str] = "mode-auto"
 AZD_MODES: Final[str] = "modes"
 AZD_NAME: Final[str] = "name"
+AZD_NUM_DEVICES: Final[str] = "num-devices"
 AZD_POWER: Final[str] = "power"
 AZD_PROBLEMS: Final[str] = "problems"
 AZD_SYSTEM: Final[str] = "system"
 AZD_SYSTEM_ID: Final[str] = "system-id"
 AZD_SYSTEMS: Final[str] = "systems"
 AZD_TEMP: Final[str] = "temperature"
 AZD_TEMP_STEP: Final[str] = "temperature-step"
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/device.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     API_WS_CONNECTED,
     AZD_AVAILABLE,
     AZD_ERRORS,
     AZD_ID,
     AZD_INSTALLATION,
     AZD_IS_CONNECTED,
     AZD_MODE,
+    AZD_MODE_AUTO,
     AZD_MODES,
     AZD_NAME,
     AZD_PROBLEMS,
     AZD_WARNINGS,
     AZD_WEBSERVER,
     AZD_WS_CONNECTED,
 )
@@ -34,14 +35,15 @@
 class Device(ABC):
     """Airzone Cloud Device."""
 
     name: str
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud Device init."""
+        self.auto_mode: OperationMode | None = None
         self.errors: list[str] = []
         self.id = str(device_data[API_DEVICE_ID])
         self.installation_id = inst_id
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
         self.name: str = "Device"
         self.warnings: list[str] = []
@@ -67,14 +69,18 @@
             AZD_WS_CONNECTED: self.get_ws_connected(),
         }
 
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
+        mode_auto = self.get_mode_auto()
+        if mode_auto is not None:
+            data[AZD_MODE_AUTO] = mode_auto
+
         modes = self.get_modes()
         if modes is not None:
             data[AZD_MODES] = modes
 
         warnings = self.get_warnings()
         if len(warnings) > 0:
             data[AZD_WARNINGS] = warnings
@@ -101,14 +107,18 @@
         """Return Device connection status."""
         return self.is_connected
 
     def get_mode(self) -> OperationMode | None:
         """Return Device mode."""
         return self.mode
 
+    def get_mode_auto(self) -> OperationMode | None:
+        """Return current auto mode."""
+        return self.auto_mode
+
     def get_modes(self) -> list[OperationMode] | None:
         """Return Device modes."""
         if len(self.modes) > 0:
             return self.modes
         return None
 
     def get_name(self) -> str:
@@ -141,29 +151,35 @@
 
     @abstractmethod
     def set_param(self, param: str, data: dict[str, Any]) -> None:
         """Update device parameter from API request."""
 
     def update(self, data: dict[str, Any]) -> None:
         """Update Device data."""
-        if API_IS_CONNECTED in data:
-            self.is_connected = bool(data[API_IS_CONNECTED])
-        if API_WS_CONNECTED in data:
-            self.ws_connected = bool(data[API_WS_CONNECTED])
+        is_connected = data.get(API_IS_CONNECTED)
+        if is_connected is not None:
+            self.is_connected = bool(is_connected)
+        ws_connected = data.get(API_WS_CONNECTED)
+        if ws_connected is not None:
+            self.ws_connected = bool(ws_connected)
 
-        if API_ERRORS in data:
+        errors = data.get(API_ERRORS)
+        if errors is not None:
             self.errors = []
-            for error in data[API_ERRORS]:
+            for error in errors:
                 self.errors += [error]
 
-        if API_MODE in data:
-            self.mode = OperationMode(data[API_MODE])
-        if API_MODE_AVAIL in data and len(data[API_MODE_AVAIL]) > 0:
+        mode = data.get(API_MODE)
+        if mode is not None:
+            self.mode = OperationMode(mode)
+        mode_avail = data.get(API_MODE_AVAIL)
+        if mode_avail is not None and len(mode_avail) > 0:
             modes = []
-            for mode in data[API_MODE_AVAIL]:
+            for mode in mode_avail:
                 modes += [OperationMode(mode)]
             self.modes = modes
 
-        if API_WARNINGS in data:
+        warnings = data.get(API_WARNINGS)
+        if warnings is not None:
             self.warnings = []
-            for warning in data[API_WARNINGS]:
+            for warning in warnings:
                 self.warnings += [warning]
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/hvac.py`

 * *Files 10% similar despite different names*

```diff
@@ -188,78 +188,57 @@
         if temp_set_vent_air is not None:
             data[AZD_TEMP_SET_VENT_AIR] = temp_set_vent_air
 
         return data
 
     def get_action(self) -> OperationAction:
         """Return HVAC action."""
-
         if self.get_power():
             if self.get_active():
                 mode = self.get_mode() or OperationMode.STOP
                 if mode.is_cool():
                     action = OperationAction.COOLING
                 elif mode.is_heat():
                     action = OperationAction.HEATING
                 elif mode.is_vent():
                     action = OperationAction.FAN
                 elif mode.is_dry():
                     action = OperationAction.DRYING
                 elif mode.is_auto():
-                    action = self.get_auto_mode()
+                    action = self.get_action_auto()
                 else:
                     action = OperationAction.OFF
             else:
                 action = OperationAction.IDLE
         else:
             action = OperationAction.OFF
+        return action
 
+    def get_action_auto(self) -> OperationAction:
+        """Return current Auto action."""
+        mode = self.get_mode_auto()
+        if mode is not None:
+            if mode.is_cool():
+                action = OperationAction.COOLING
+            elif mode.is_heat():
+                action = OperationAction.HEATING
+            elif mode.is_vent():
+                action = OperationAction.FAN
+            elif mode.is_dry():
+                action = OperationAction.DRYING
+            else:
+                action = OperationAction.IDLE
+        else:
+            action = OperationAction.IDLE
         return action
 
     def get_active(self) -> bool | None:
         """Return HVAC device active status."""
         return self.active
 
-    def get_auto_mode(self) -> OperationAction:
-        """Return action from auto mode."""
-        temp_sp = self.get_temp_set()
-        temp_min = self.temp_set_min
-        temp_max = self.temp_set_max
-        cool_sp = self.get_temp_set_cool_air()
-        cool_max = self.get_temp_set_max_cool_air()
-        cool_min = self.get_temp_set_min_cool_air()
-        heat_sp = self.get_temp_set_hot_air()
-        heat_max = self.get_temp_set_max_hot_air()
-        heat_min = self.get_temp_set_min_hot_air()
-
-        if (
-            cool_max is not None
-            and cool_min is not None
-            and heat_max is not None
-            and heat_min is not None
-        ):
-            cool_match = cool_max == temp_max and cool_min == temp_min
-            heat_match = heat_max == temp_max and heat_min == temp_min
-
-            if cool_match and not heat_match:
-                return OperationAction.COOLING
-            if heat_match and not cool_match:
-                return OperationAction.HEATING
-
-        if cool_sp is not None and heat_sp is not None:
-            cool_match = cool_sp == temp_sp
-            heat_match = heat_sp == temp_sp
-
-            if cool_match and not heat_match:
-                return OperationAction.COOLING
-            if heat_match and not cool_match:
-                return OperationAction.HEATING
-
-        return OperationAction.IDLE
-
     def get_humidity(self) -> int | None:
         """Return HVAC device humidity."""
         return self.humidity
 
     def get_power(self) -> bool | None:
         """Return HVAC device power."""
         return self.power
@@ -472,117 +451,119 @@
         if self.temp_set_vent_air is not None:
             self.temp_set_vent_air = setpoint
 
     def update(self, data: dict[str, Any]) -> None:
         """Update HVAC device data."""
         super().update(data)
 
-        if API_ACTIVE in data:
-            self.active = bool(data[API_ACTIVE])
-
-        if API_HUMIDITY in data:
-            self.humidity = int(data[API_HUMIDITY])
-
-        if API_LOCAL_TEMP in data:
-            if API_CELSIUS in data[API_LOCAL_TEMP]:
-                self.temp = float(data[API_LOCAL_TEMP][API_CELSIUS])
-
-        if API_POWER in data:
-            self.power = bool(data[API_POWER])
-
-        if API_RANGE_MAX_AIR in data:
-            if API_CELSIUS in data[API_RANGE_MAX_AIR]:
-                self.temp_set_max = float(data[API_RANGE_MAX_AIR][API_CELSIUS])
-        if API_RANGE_SP_MAX_AUTO_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_AUTO_AIR]:
-                self.temp_set_max_auto_air = float(
-                    data[API_RANGE_SP_MAX_AUTO_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_COOL_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_COOL_AIR]:
-                self.temp_set_max_cool_air = float(
-                    data[API_RANGE_SP_MAX_COOL_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_DRY_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_DRY_AIR]:
-                self.temp_set_max_dry_air = float(
-                    data[API_RANGE_SP_MAX_DRY_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_EMERHEAT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_EMERHEAT_AIR]:
+        active = data.get(API_ACTIVE)
+        if active is not None:
+            self.active = bool(active)
+
+        humidity = data.get(API_HUMIDITY)
+        if humidity is not None:
+            self.humidity = int(humidity)
+
+        local_temp = data.get(API_LOCAL_TEMP)
+        if local_temp is not None:
+            if API_CELSIUS in local_temp:
+                self.temp = float(local_temp[API_CELSIUS])
+
+        power = data.get(API_POWER)
+        if power is not None:
+            self.power = bool(power)
+
+        range_max_air = data.get(API_RANGE_MAX_AIR)
+        if range_max_air is not None:
+            if API_CELSIUS in range_max_air:
+                self.temp_set_max = float(range_max_air[API_CELSIUS])
+        range_sp_max_auto_air = data.get(API_RANGE_SP_MAX_AUTO_AIR)
+        if range_sp_max_auto_air is not None:
+            if API_CELSIUS in range_sp_max_auto_air:
+                self.temp_set_max_auto_air = float(range_sp_max_auto_air[API_CELSIUS])
+        range_sp_max_cool_air = data.get(API_RANGE_SP_MAX_COOL_AIR)
+        if range_sp_max_cool_air is not None:
+            if API_CELSIUS in range_sp_max_cool_air:
+                self.temp_set_max_cool_air = float(range_sp_max_cool_air[API_CELSIUS])
+        range_sp_max_dry_air = data.get(API_RANGE_SP_MAX_DRY_AIR)
+        if range_sp_max_dry_air is not None:
+            if API_CELSIUS in range_sp_max_dry_air:
+                self.temp_set_max_dry_air = float(range_sp_max_dry_air[API_CELSIUS])
+        range_sp_max_emerheat_air = data.get(API_RANGE_SP_MAX_EMERHEAT_AIR)
+        if range_sp_max_emerheat_air is not None:
+            if API_CELSIUS in range_sp_max_emerheat_air:
                 self.temp_set_max_emerheat_air = float(
-                    data[API_RANGE_SP_MAX_EMERHEAT_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_HOT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_HOT_AIR]:
-                self.temp_set_max_hot_air = float(
-                    data[API_RANGE_SP_MAX_HOT_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_STOP_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_STOP_AIR]:
-                self.temp_set_max_stop_air = float(
-                    data[API_RANGE_SP_MAX_STOP_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MAX_VENT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MAX_VENT_AIR]:
-                self.temp_set_max_vent_air = float(
-                    data[API_RANGE_SP_MAX_VENT_AIR][API_CELSIUS]
-                )
-
-        if API_RANGE_MIN_AIR in data:
-            if API_CELSIUS in data[API_RANGE_MIN_AIR]:
-                self.temp_set_min = float(data[API_RANGE_MIN_AIR][API_CELSIUS])
-        if API_RANGE_SP_MIN_AUTO_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_AUTO_AIR]:
-                self.temp_set_min_auto_air = float(
-                    data[API_RANGE_SP_MIN_AUTO_AIR][API_CELSIUS]
+                    range_sp_max_emerheat_air[API_CELSIUS]
                 )
-        if API_RANGE_SP_MIN_COOL_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_COOL_AIR]:
-                self.temp_set_min_cool_air = float(
-                    data[API_RANGE_SP_MIN_COOL_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MIN_DRY_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_DRY_AIR]:
-                self.temp_set_min_dry_air = float(
-                    data[API_RANGE_SP_MIN_DRY_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MIN_EMERHEAT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_EMERHEAT_AIR]:
+        range_sp_max_hot_air = data.get(API_RANGE_SP_MAX_HOT_AIR)
+        if range_sp_max_hot_air is not None:
+            if API_CELSIUS in range_sp_max_hot_air:
+                self.temp_set_max_hot_air = float(range_sp_max_hot_air[API_CELSIUS])
+        range_sp_max_stop_air = data.get(API_RANGE_SP_MAX_STOP_AIR)
+        if range_sp_max_stop_air is not None:
+            if API_CELSIUS in range_sp_max_stop_air:
+                self.temp_set_max_stop_air = float(range_sp_max_stop_air[API_CELSIUS])
+        range_sp_max_vent_air = data.get(API_RANGE_SP_MAX_VENT_AIR)
+        if range_sp_max_vent_air is not None:
+            if API_CELSIUS in range_sp_max_vent_air:
+                self.temp_set_max_vent_air = float(range_sp_max_vent_air[API_CELSIUS])
+
+        range_min_air = data.get(API_RANGE_MIN_AIR)
+        if range_min_air is not None:
+            if API_CELSIUS in range_min_air:
+                self.temp_set_min = float(range_min_air[API_CELSIUS])
+        range_sp_min_auto_air = data.get(API_RANGE_SP_MIN_AUTO_AIR)
+        if range_sp_min_auto_air is not None:
+            if API_CELSIUS in range_sp_min_auto_air:
+                self.temp_set_min_auto_air = float(range_sp_min_auto_air[API_CELSIUS])
+        range_sp_min_cool_air = data.get(API_RANGE_SP_MIN_COOL_AIR)
+        if range_sp_min_cool_air is not None:
+            if API_CELSIUS in range_sp_min_cool_air:
+                self.temp_set_min_cool_air = float(range_sp_min_cool_air[API_CELSIUS])
+        range_sp_min_dry_air = data.get(API_RANGE_SP_MIN_DRY_AIR)
+        if range_sp_min_dry_air is not None:
+            if API_CELSIUS in range_sp_min_dry_air:
+                self.temp_set_min_dry_air = float(range_sp_min_dry_air[API_CELSIUS])
+        range_sp_min_emerheat_air = data.get(API_RANGE_SP_MIN_EMERHEAT_AIR)
+        if range_sp_min_emerheat_air is not None:
+            if API_CELSIUS in range_sp_min_emerheat_air:
                 self.temp_set_min_emerheat_air = float(
-                    data[API_RANGE_SP_MIN_EMERHEAT_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MIN_HOT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_HOT_AIR]:
-                self.temp_set_min_hot_air = float(
-                    data[API_RANGE_SP_MIN_HOT_AIR][API_CELSIUS]
+                    range_sp_min_emerheat_air[API_CELSIUS]
                 )
-        if API_RANGE_SP_MIN_STOP_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_STOP_AIR]:
-                self.temp_set_min_stop_air = float(
-                    data[API_RANGE_SP_MIN_STOP_AIR][API_CELSIUS]
-                )
-        if API_RANGE_SP_MIN_VENT_AIR in data:
-            if API_CELSIUS in data[API_RANGE_SP_MIN_VENT_AIR]:
-                self.temp_set_min_vent_air = float(
-                    data[API_RANGE_SP_MIN_VENT_AIR][API_CELSIUS]
-                )
-
-        if API_SP_AIR_COOL in data:
-            if API_CELSIUS in data[API_SP_AIR_COOL]:
-                self.temp_set_cool_air = float(data[API_SP_AIR_COOL][API_CELSIUS])
-        if API_SP_AIR_DRY in data:
-            if API_CELSIUS in data[API_SP_AIR_DRY]:
+        range_sp_min_hot_air = data.get(API_RANGE_SP_MIN_HOT_AIR)
+        if range_sp_min_hot_air is not None:
+            if API_CELSIUS in range_sp_min_hot_air:
+                self.temp_set_min_hot_air = float(range_sp_min_hot_air[API_CELSIUS])
+        range_sp_min_stop_air = data.get(API_RANGE_SP_MIN_STOP_AIR)
+        if range_sp_min_stop_air is not None:
+            if API_CELSIUS in range_sp_min_stop_air:
+                self.temp_set_min_stop_air = float(range_sp_min_stop_air[API_CELSIUS])
+        range_sp_min_vent_air = data.get(API_RANGE_SP_MIN_VENT_AIR)
+        if range_sp_min_vent_air is not None:
+            if API_CELSIUS in range_sp_min_vent_air:
+                self.temp_set_min_vent_air = float(range_sp_min_vent_air[API_CELSIUS])
+
+        sp_air_cool = data.get(API_SP_AIR_COOL)
+        if sp_air_cool is not None:
+            if API_CELSIUS in sp_air_cool:
+                self.temp_set_cool_air = float(sp_air_cool[API_CELSIUS])
+        sp_air_dry = data.get(API_SP_AIR_DRY)
+        if sp_air_dry is not None:
+            if API_CELSIUS in sp_air_dry:
                 self.temp_set_dry_air = float(data[API_SP_AIR_DRY][API_CELSIUS])
-        if API_SP_AIR_HEAT in data:
-            if API_CELSIUS in data[API_SP_AIR_HEAT]:
-                self.temp_set_hot_air = float(data[API_SP_AIR_HEAT][API_CELSIUS])
-        if API_SP_AIR_STOP in data:
-            if API_CELSIUS in data[API_SP_AIR_STOP]:
-                self.temp_set_stop_air = float(data[API_SP_AIR_STOP][API_CELSIUS])
-        if API_SP_AIR_VENT in data:
-            if API_CELSIUS in data[API_SP_AIR_VENT]:
-                self.temp_set_vent_air = float(data[API_SP_AIR_VENT][API_CELSIUS])
-
-        if API_STEP in data:
-            if API_CELSIUS in data[API_STEP]:
-                self.temp_step = float(data[API_STEP][API_CELSIUS])
+        sp_air_heat = data.get(API_SP_AIR_HEAT)
+        if sp_air_heat is not None:
+            if API_CELSIUS in sp_air_heat:
+                self.temp_set_hot_air = float(sp_air_heat[API_CELSIUS])
+        sp_air_stop = data.get(API_SP_AIR_STOP)
+        if sp_air_stop is not None:
+            if API_CELSIUS in sp_air_stop:
+                self.temp_set_stop_air = float(sp_air_stop[API_CELSIUS])
+        sp_air_vent = data.get(API_SP_AIR_VENT)
+        if sp_air_vent is not None:
+            if API_CELSIUS in sp_air_vent:
+                self.temp_set_vent_air = float(sp_air_vent[API_CELSIUS])
+
+        step = data.get(API_STEP)
+        if step is not None:
+            if API_CELSIUS in step:
+                self.temp_step = float(step[API_CELSIUS])
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/system.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/webserver.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,40 +51,50 @@
         self.wifi_quality: int | None = None
         self.wifi_rssi: int | None = None
         self.wifi_ssid: str | None = None
 
     def update(self, data: dict[str, Any]) -> None:
         """Update WebServer data."""
 
-        if API_WS_TYPE in data:
-            self.type = str(data[API_WS_TYPE])
+        ws_type = data.get(API_WS_TYPE)
+        if ws_type is not None:
+            self.type = str(ws_type)
 
         ws_config = data.get(API_CONFIG)
         if ws_config is not None:
-            if API_STAT_AP_MAC in ws_config:
-                self.wifi_mac = str(ws_config[API_STAT_AP_MAC])
-            if API_STAT_CHANNEL in ws_config:
-                self.wifi_channel = int(ws_config[API_STAT_CHANNEL])
-            if API_STAT_SSID in ws_config:
-                self.wifi_ssid = str(ws_config[API_STAT_SSID])
-            if API_WS_FW in ws_config:
-                self.firmware = str(ws_config[API_WS_FW])
+            stat_ap_mac = ws_config.get(API_STAT_AP_MAC)
+            if stat_ap_mac is not None:
+                self.wifi_mac = str(stat_ap_mac)
+            stat_channel = ws_config.get(API_STAT_CHANNEL)
+            if stat_channel is not None:
+                self.wifi_channel = int(stat_channel)
+            stat_ssid = ws_config.get(API_STAT_SSID)
+            if stat_ssid is not None:
+                self.wifi_ssid = str(stat_ssid)
+            ws_fw = ws_config.get(API_WS_FW)
+            if ws_fw is not None:
+                self.firmware = str(ws_fw)
 
         ws_status = data.get(API_STATUS)
         if ws_status is not None:
-            if API_CONNECTION_DATE in ws_status:
-                self.connection_date = str(ws_status[API_CONNECTION_DATE])
-            if API_DISCONNECTION_DATE in ws_status:
-                self.disconnection_date = str(ws_status[API_DISCONNECTION_DATE])
-            if API_IS_CONNECTED in ws_status:
-                self.is_connected = bool(ws_status[API_IS_CONNECTED])
-            if API_STAT_QUALITY in ws_status:
-                self.wifi_quality = int(ws_status[API_STAT_QUALITY])
-            if API_STAT_RSSI in ws_status:
-                self.wifi_rssi = int(ws_status[API_STAT_RSSI])
+            connection_date = ws_status.get(API_CONNECTION_DATE)
+            if connection_date is not None:
+                self.connection_date = str(connection_date)
+            disconnection_date = ws_status.get(API_DISCONNECTION_DATE)
+            if disconnection_date is not None:
+                self.disconnection_date = str(disconnection_date)
+            is_connected = ws_status.get(API_IS_CONNECTED)
+            if is_connected is not None:
+                self.is_connected = bool(is_connected)
+            stat_quality = ws_status.get(API_STAT_QUALITY)
+            if stat_quality is not None:
+                self.wifi_quality = int(stat_quality)
+            stat_rssi = ws_status.get(API_STAT_RSSI)
+            if stat_rssi is not None:
+                self.wifi_rssi = int(stat_rssi)
 
     def data(self) -> dict[str, Any]:
         """Return WebServer data."""
         data: dict[str, Any] = {
             AZD_AVAILABLE: self.get_available(),
             AZD_CONNECTION_DATE: self.get_connection_date(),
             AZD_DISCONNECTION_DATE: self.get_disconnection_date(),
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.2.1/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.2.0/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.2.1/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 aioairzone_cloud/__init__.py
 aioairzone_cloud/aidoo.py
 aioairzone_cloud/cloudapi.py
 aioairzone_cloud/common.py
 aioairzone_cloud/const.py
 aioairzone_cloud/device.py
 aioairzone_cloud/exceptions.py
+aioairzone_cloud/group.py
 aioairzone_cloud/hvac.py
 aioairzone_cloud/installation.py
 aioairzone_cloud/py.typed
 aioairzone_cloud/system.py
 aioairzone_cloud/webserver.py
 aioairzone_cloud/zone.py
 aioairzone_cloud.egg-info/PKG-INFO
```

### Comparing `aioairzone-cloud-0.2.0/pyproject.toml` & `aioairzone-cloud-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

