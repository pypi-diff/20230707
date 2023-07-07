# Comparing `tmp/pik_intercom-0.0.3.tar.gz` & `tmp/pik_intercom-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pik_intercom-0.0.3.tar", last modified: Fri Jul  7 00:57:32 2023, max compression
+gzip compressed data, was "pik_intercom-0.0.4.tar", last modified: Fri Jul  7 03:59:37 2023, max compression
```

## Comparing `pik_intercom-0.0.3.tar` & `pik_intercom-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 00:57:32.960236 pik_intercom-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/pik_intercom/
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/icm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/iot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/pik_intercom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 00:57:32.960236 pik_intercom-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/pik_intercom/
+-rw-r--r--   0 runner    (1001) docker     (123)    30170 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/icm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/iot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/pik_intercom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/setup.py
```

### Comparing `pik_intercom-0.0.3/LICENSE` & `pik_intercom-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.3/PKG-INFO` & `pik_intercom-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik_intercom
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.3/pik_intercom/__init__.py` & `pik_intercom-0.0.4/pik_intercom/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Pik Intercom API"""
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import json
 import random
 import string
 from typing import (
     TypeVar,
     ClassVar,
     Tuple,
     MutableMapping,
     Iterable,
     Type,
-    Union,
 )
 
 import aiohttp
 from multidict import CIMultiDict, CIMultiDictProxy
 
 from .base import *
 from .errors import *
@@ -24,15 +23,15 @@
 from .iot import *
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 DEFAULT_DEVICE_MODEL: Final = "Python API"
 DEFAULT_USER_AGENT: Final = "okhttp/4.9.0"
 DEFAULT_CLIENT_APP: Final = "alfred"
-DEFAULT_CLIENT_VERSION: Final = "2023.5.1"
+DEFAULT_CLIENT_VERSION: Final = "2023.6.1"
 DEFAULT_CLIENT_OS: Final = "Android"
 
 _TBaseObject = TypeVar("_TBaseObject", bound=BaseObject)
 
 
 @dataclass(slots=True)
 class PikAccount(BaseObject):
@@ -107,17 +106,45 @@
             self.sip_status = (
                 sip_account_data.get("remote_request_status") or None
             )
             self.sip_password = sip_account_data.get("password") or None
 
 
 class PikIntercomAPI:
+    """HTTP API for Pik Intercom"""
+
     BASE_ICM_URL: ClassVar[str] = "https://intercom.rubetek.com"
     BASE_IOT_URL: ClassVar[str] = "https://iot.rubetek.com"
 
+    __slots__ = (
+        "account",
+        "authorization",
+        "client_app",
+        "client_os",
+        "client_version",
+        "customer_devices",
+        "device_id",
+        "device_model",
+        "icm_buildings",
+        "icm_call_sessions",
+        "icm_intercoms",
+        "icm_properties",
+        "iot_call_sessions",
+        "iot_cameras",
+        "iot_intercoms",
+        "iot_meters",
+        "iot_relays",
+        "password",
+        "refresh_token",
+        "request_counter",
+        "session",
+        "user_agent",
+        "username",
+    )
+
     def __init__(
         self,
         username: str,
         password: str,
         session: aiohttp.ClientSession,
         device_id: Optional[str] = None,
         *,
@@ -134,39 +161,40 @@
 
         self.device_id = device_id or "".join(
             random.choices(
                 string.ascii_uppercase + string.digits,
                 k=16,
             )
         )
-        self.device_model = device_model
-        self.user_agent = user_agent
         self.client_app = client_app
-        self.client_version = client_version
         self.client_os = client_os
+        self.client_version = client_version
+        self.device_model = device_model
+        self.user_agent = user_agent
 
         self.authorization: Optional[str] = None
         self.refresh_token: Optional[str] = None
         self.request_counter: int = 0
 
         # General
         self.account: Optional[PikAccount] = None
-        self.icm_properties: dict[int, IcmProperty] = {}
         self.customer_devices: dict[int, CustomerDevice] = {}
 
         # Placeholders for ICM requests
+        self.icm_buildings: dict[int, IcmBuilding] = {}
+        self.icm_call_sessions: dict[int, IcmCallSession] = {}
         self.icm_intercoms: dict[int, IcmIntercom] = {}
+        self.icm_properties: dict[int, IcmProperty] = {}
 
         # Placeholders for IoT requests
-        self.iot_intercoms: dict[int, IotIntercom] = {}
-        self.iot_relays: dict[int, IotRelay] = {}
+        self.iot_call_sessions: dict[int, IotCallSession] = {}
         self.iot_cameras: dict[int, IotCamera] = {}
+        self.iot_intercoms: dict[int, IotIntercom] = {}
         self.iot_meters: dict[int, IotMeter] = {}
-        self.icm_call_sessions: dict[int, IcmCallSession] = {}
-        self.iot_call_sessions: dict[int, IotCallSession] = {}
+        self.iot_relays: dict[int, IotRelay] = {}
 
         # @TODO: add other properties
 
     @property
     def is_authenticated(self) -> bool:
         """Whether an authorization token is already present."""
         return self.authorization is not None
@@ -174,15 +202,25 @@
     @property
     def customer_device(self) -> Optional["CustomerDevice"]:
         """Return current customer device object."""
         for device in self.customer_devices.values():
             if device.uid == self.device_id:
                 return device
 
-    def get_last_call_session(self) -> Union[IotCallSession, IcmCallSession]:
+    def get_last_call_session(
+        self,
+    ) -> Optional[Union[IotCallSession, IcmCallSession]]:
+        """
+        Find last call session.
+
+        It will search both IoT and ICM call session stores
+        to fetch whatever call session is more recent.
+
+        :return: The most recent call session, if found
+        """
         last_call_session = None
         for source in (self.iot_call_sessions, self.icm_call_sessions):
             iterator = iter(source.values())
             if last_call_session is None:
                 try:
                     last_call_session = next(iterator)
                 except StopIteration:
@@ -198,19 +236,34 @@
         return request_counter
 
     async def make_request(
         self,
         method: str,
         url: str,
         headers: Optional[CIMultiDict] = None,
-        authenticated: bool = False,
+        authenticated: bool = True,
         title: str = "request",
         api_version: int = 2,
         **kwargs: Any,
     ) -> Tuple[Any, CIMultiDictProxy[str], int]:
+        """
+        Request wrapper.
+
+        This injects necessary authentication and validation
+        before making an aiohttp request. It is a helper method.
+
+        :param method: HTTP method
+        :param url: URL of API endpoint
+        :param headers: Request headers (optional)
+        :param authenticated: Use authentication (true by default)
+        :param title: Logging title ("request" by default)
+        :param api_version: API version for request (2 by default)
+        :param kwargs: Additional aiohttp.ClientSession.request keyword arguments
+        :return: Tuple of (Response data, Response headers, Request counter value)
+        """
         if headers is None:
             headers = CIMultiDict()
         elif not isinstance(headers, MutableMapping):
             headers = CIMultiDict(headers)
 
         headers.update(
             {
@@ -276,49 +329,102 @@
             _LOGGER.debug(log_prefix + f"Response data: {resp_data}")
 
             return resp_data, request.headers, request_counter
 
     async def iterate_paginated_request(
         self,
         url: str,
-        title: str,
+        title: str = "paginated request",
         method: str = aiohttp.hdrs.METH_GET,
-        authenticated: bool = True,
         params: Optional[Mapping[str, Any]] = None,
         max_pages: Optional[int] = None,
         **kwargs,
     ):
+        """
+        Asynchronous generator to iterate paginated requests.
+
+        Perform requests until it meets 'no data' condition,
+        or max requested pages limit is reached.
+
+        :param url: URL of API endpoint
+        :param title:
+        :param method: HTTP method ("GET" by default)
+        :param params: Query parameters (none by default)
+        :param max_pages: Max pages to request (unlimited by default)
+        :param kwargs: Additional PikIntercomAPI.make_request keyword arguments
+        :return: Generator of response data per each page with data
+        """
         params = {} if params is None else dict(params)
         page_number = 0
 
         while max_pages is None or (page_number < max_pages):
             page_number += 1
             params["page"] = page_number
-            (
-                resp_data,
-                headers,
-                request_counter,
-            ) = await self.make_request(
+            (resp_data, headers, request_counter,) = await self.make_request(
                 method,
                 url,
                 title=title,
-                authenticated=authenticated,
                 params=params,
                 **kwargs,
             )
 
             if not resp_data:
                 _LOGGER.debug(
                     f"[{request_counter}] Page does not contain data, stopping"
                 )
                 break
 
             _LOGGER.debug(f"page {resp_data}")
             yield resp_data
 
+    async def update_single_item_from_request(
+        self,
+        url: str,
+        container: MutableMapping[int, _TBaseObject],
+        data_cls: Type[_TBaseObject],
+        title: str = "single item request",
+        method: str = aiohttp.hdrs.METH_GET,
+        item_id: Optional[int] = None,
+        **kwargs,
+    ) -> _TBaseObject:
+        """
+        Perform single request and update single item.
+
+        This is a shorthand to avoid mistakes and reuse code.
+
+        :param url: URL of API endpoint
+        :param title:
+        :param container:
+        :param data_cls:
+        :param method:
+        :param item_id:
+        :param kwargs:
+        :return:
+        """
+        resp_data, _, __ = await self.make_request(
+            method,
+            url,
+            title=title,
+            **kwargs,
+        )
+
+        if item_id is None:
+            item_id = data_cls.get_id_from_data(resp_data)
+
+        try:
+            item = container[item_id]
+        except KeyError:
+            container[item_id] = item = data_cls.create_from_dict(
+                self, resp_data
+            )
+        else:
+            item.update_from_dict(resp_data)
+
+        return item
+
     def iterate_data_list_and_update(
         self,
         container: MutableMapping[int, _TBaseObject],
         data_list: Iterable[Mapping[str, Any]],
         data_cls: Type[_TBaseObject],
     ):
         if not data_list:
@@ -365,14 +471,15 @@
                         "password": self.password,
                     },
                     "customer_device": {
                         "uid": self.device_id,
                     },
                 },
                 title="authentication",
+                authenticated=False,
             )
         except aiohttp.ClientResponseError as exc:
             _LOGGER.debug(f"Client response: {exc.headers}")
             raise
 
         if not (authorization := headers.get(aiohttp.hdrs.AUTHORIZATION)):
             _LOGGER.error(
@@ -399,37 +506,27 @@
 
         _LOGGER.debug(f"[{request_counter}] Authentication successful")
 
     async def update_customer_device(self) -> Any:
         if not (device_id := self.device_id):
             raise PikIntercomException("device ID not set")
         try:
-            (
-                resp_data,
-                headers,
-                request_counter,
-            ) = await self.make_request(
+            (resp_data, headers, request_counter,) = await self.make_request(
                 aiohttp.hdrs.METH_GET,
                 f"{self.BASE_ICM_URL}/api/customers/devices/lookup",
                 title="customer device lookup",
-                authenticated=True,
                 params={"customer_device[uid]": device_id},
             )
         except aiohttp.ClientResponseError as exc:
             if exc.status != 404:
                 raise
-            (
-                resp_data,
-                headers,
-                request_counter,
-            ) = await self.make_request(
+            (resp_data, headers, request_counter,) = await self.make_request(
                 aiohttp.hdrs.METH_POST,
                 f"{self.BASE_ICM_URL}/api/customers/devices",
                 title="customer device initialization",
-                authenticated=True,
                 params={
                     "customer_device[model]": self.device_model,
                     "customer_device[kind]": "mobile",
                     "customer_device[uid]": device_id,
                     "customer_device[os]": self.client_os.lower(),
                     "customer_device[push_version]": "2.0.0",
                 },
@@ -445,21 +542,20 @@
                 break
         if customer_device_id is None:
             raise PikIntercomException("device by id not found")
         await self.make_request(
             aiohttp.hdrs.METH_PATCH,
             f"/api/customers/devices/{customer_device_id}",
             title="customer device push token update",
-            authenticated=True,
             params={"customer_device[push_token]": push_token},
         )
 
     async def fetch_last_active_session(
         self,
-    ) -> IcmActiveCallSession | IotActiveCallSession | None:
+    ) -> Optional[Union[IcmActiveCallSession, IotActiveCallSession]]:
         # Current call session is None
         create_task = asyncio.get_running_loop().create_task
         tasks = [
             create_task(self.iot_fetch_last_active_session()),
             create_task(self.icm_fetch_last_active_session()),
         ]
 
@@ -509,26 +605,39 @@
         Retrieve properties from ICM API.
         :return:
         """
         resp_data, _, __ = await self.make_request(
             aiohttp.hdrs.METH_GET,
             f"{self.BASE_ICM_URL}/api/customers/properties",
             title="properties fetching",
-            authenticated=True,
         )
 
         retrieved_objects = {}
         for property_type, properties_data in resp_data.items():
             for obj_id, obj, _ in self.iterate_data_list_and_update(
                 self.icm_properties, properties_data, IcmProperty
             ):
                 retrieved_objects[obj_id] = obj
                 obj.category = property_type
         return retrieved_objects
 
+    async def icm_update_building(self, building_id: int) -> IcmBuilding:
+        """
+        Update data about a single ICM building.
+        :param building_id: ICM building identifier
+        :return: Updated ICM building object
+        """
+        return await self.update_single_item_from_request(
+            f"{self.BASE_ICM_URL}/api/buildings/{building_id}",
+            container=self.icm_buildings,
+            data_cls=IcmBuilding,
+            title="building fetching",
+            item_id=building_id,
+        )
+
     async def icm_update_intercoms(
         self, property_id: Optional[int] = None
     ) -> dict[int, IcmIntercom]:
         """
         Retrieve intercoms from ICM API.
         :param property_id: Property identifier.
         :return:
@@ -566,54 +675,48 @@
                 self.icm_intercoms, resp_data, IcmIntercom
             ):
                 obj.property_ids.add(property_id)
                 retrieved_objects[obj_id] = obj
         return retrieved_objects
 
     async def icm_update_intercom(self, intercom_id: int) -> IcmIntercom:
-        resp_data, headers, request_counter = await self.make_request(
-            aiohttp.hdrs.METH_GET,
+        """
+        Update data about a single ICM intercom device.
+        :param intercom_id: ICM intercom identifier
+        :return: Updated ICM intercom object
+        """
+        return await self.update_single_item_from_request(
             f"{self.BASE_ICM_URL}/api/intercoms/{intercom_id}",
-            title="single intercom retrieval",
-            authenticated=True,
+            container=self.icm_intercoms,
+            data_cls=IcmIntercom,
+            title="building fetching",
+            item_id=intercom_id,
         )
 
-        try:
-            intercom = self.icm_intercoms[intercom_id]
-        except KeyError:
-            self.icm_intercoms = intercom = IcmIntercom.create_from_dict(
-                self, resp_data
-            )
-        else:
-            intercom.update_from_dict(resp_data)
-
-        return intercom
-
     async def icm_unlock_intercom(self, intercom_id: int, mode: str) -> None:
         """
         Send command to property device to unlock.
         :param intercom_id: Property device identifier
         :param mode: <unknown parameter, comes from PropertyDevice data object>
         """
         resp_data, headers, request_counter = await self.make_request(
             aiohttp.hdrs.METH_POST,
             f"{self.BASE_ICM_URL}/api/customers/intercoms/{intercom_id}/unlock",
             data={"id": intercom_id, "door": mode},
             title="intercom unlocking",
-            authenticated=True,
         )
 
         if resp_data.get("request") is not True:
             _LOGGER.error(f"[{request_counter}] Timed out unlocking intercom")
             raise PikIntercomException("Timed out unlocking intercom")
 
         _LOGGER.debug(f"[{request_counter}] Intercom unlocking successful")
 
     async def icm_update_call_sessions(
-        self, max_pages: int | None = 10
+        self, max_pages: Optional[int] = 10
     ) -> dict[int, IcmCallSession]:
         retrieved_objects = {}
         async for resp_data in self.iterate_paginated_request(
             f"{self.BASE_ICM_URL}/api/call_sessions",
             f"intercom call sessions fetching",
             max_pages=max_pages,
         ):
@@ -632,15 +735,14 @@
         self,
     ) -> Optional["IcmActiveCallSession"]:
         try:
             resp_data, _, __ = await self.make_request(
                 aiohttp.hdrs.METH_GET,
                 f"{self.BASE_ICM_URL}/api/call_sessions/last_open",
                 title="current call session",
-                authenticated=True,
             )
         except aiohttp.ClientResponseError as exc:
             if exc.status == 404:
                 return None
             raise
 
         return (
@@ -717,15 +819,14 @@
         Send command to IoT relay to unlock.
         :param iot_relay_id: IoT relay identifier.
         """
         resp_data, headers, request_counter = await self.make_request(
             aiohttp.hdrs.METH_POST,
             f"{self.BASE_IOT_URL}/api/alfred/v1/personal/relays/{iot_relay_id}/unlock",
             title="IoT relay unlocking",
-            authenticated=True,
         )
 
         # @TODO: rule out correct response
 
         _LOGGER.debug(
             f"[{request_counter}] Intercom unlocking successful (assumed)"
         )
@@ -734,15 +835,14 @@
         self,
     ) -> Optional["IotActiveCallSession"]:
         try:
             resp_data, _, __ = await self.make_request(
                 aiohttp.hdrs.METH_GET,
                 f"{self.BASE_IOT_URL}/api/alfred/v1/personal/call_sessions/current",
                 title="current call session",
-                authenticated=True,
             )
         except aiohttp.ClientResponseError as exc:
             if exc.status == 404:
                 return None
             raise
 
         return IotActiveCallSession.create_from_dict(self, resp_data)
```

### Comparing `pik_intercom-0.0.3/pik_intercom/base.py` & `pik_intercom-0.0.4/pik_intercom/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def snapshot_url(self) -> Optional[str]:
         raise NotImplementedError
 
     @property
     def has_camera(self) -> bool:
         return bool(self.snapshot_url) or getattr(super(), "has_camera", False)
 
-    async def async_get_snapshot(self) -> bytes:
+    async def get_snapshot(self) -> bytes:
         snapshot_url = self.snapshot_url
         api = self.api
 
         if not snapshot_url:
             # @TODO: add diversion to get snapshot off RTSP
             raise PikIntercomException("Photo URL is empty")
 
@@ -107,15 +107,15 @@
     @property
     def has_camera(self) -> bool:
         return bool(self.stream_url) or getattr(super(), "has_camera", False)
 
 
 class ObjectWithUnlocker(BaseObject, ABC):
     @abstractmethod
-    async def async_unlock(self) -> None:
+    async def unlock(self) -> None:
         raise NotImplementedError
 
 
 class ObjectWithSIP(BaseObject, ABC):
     @property
     @abstractmethod
     def sip_user(self) -> Optional[str]:
```

### Comparing `pik_intercom-0.0.3/pik_intercom/icm.py` & `pik_intercom-0.0.4/pik_intercom/icm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import ABC
 from dataclasses import dataclass, field
 from enum import StrEnum
 from typing import Optional, Mapping, Dict, Any, Set
 
 from multidict import MultiDict
 
 from .base import (
@@ -11,32 +12,111 @@
     ObjectWithVideo,
     ObjectWithUnlocker,
     ObjectWithSIP,
 )
 
 
 @dataclass(slots=True)
-class IcmProperty(BaseObject):
+class IcmBuilding(BaseObject):
+    building: Optional[str] = None
+    district_id: Optional[int] = None
+    entrances_count: Optional[int] = None
+    house: Optional[str] = None
+    housing: Optional[str] = None
+    latitude: Optional[float] = None
+    longitude: Optional[float] = None
+    street: Optional[str] = None
+
+    @property
+    def address(self) -> Optional[str]:
+        parts = []
+        if part := self.street:
+            parts.append(part)
+        if part := self.house:
+            parts.append(f"д. {part}")
+        if part := self.building:
+            parts.append(f"ст. {part}")
+        return ", ".join(parts) if parts else None
+
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseObject.update_from_dict(self, data)
+
+        self.district_id = data.get("district_id") or None
+        self.entrances_count = data.get("entrances_count") or None
+        self.house = data.get("house") or None
+        self.housing = data.get("housing") or None
+        self.street = data.get("street") or None
+
+        try:
+            self.latitude, self.longitude = map(float, data["location"])
+        except (TypeError, ValueError, LookupError):
+            pass
+
+
+@dataclass(slots=True)
+class ObjectWithBuilding(BaseObject, ABC):
+    building_id: Optional[int] = None
+
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseObject.update_from_dict(self, data)
+
+        self.building_id = (
+            int(data["building_id"]) if data.get("building_id") else None
+        )
+
+    @property
+    def building(self) -> Optional[IcmBuilding]:
+        return self.api.icm_buildings.get(self.building_id)
+
+
+class IcmPropertyCategory(StrEnum):
+    APARTMENT = "apartment"
+    PARKING_PLACE = "parking_place"
+    STOREROOM = "storeroom"
+    BKFN = "bkfn"
+
+
+@dataclass(slots=True)
+class IcmProperty(ObjectWithBuilding):
     scheme_id: Optional[int] = None
     number: Optional[str] = None
     section: Optional[int] = None
-    building_id: Optional[int] = None
     district_id: Optional[int] = None
     account_number: Optional[str] = None
 
     # Externally set properties
-    category: Optional[str] = None
+    category: Optional[IcmPropertyCategory] = None
+
+    @property
+    def address(self) -> Optional[str]:
+        if not (category := self.category):
+            return
+        if not (building := self.building):
+            return
+        if not (address := building.address):
+            return
+        address += ","
+        if category == IcmPropertyCategory.APARTMENT:
+            address += " кв."
+        elif category == IcmPropertyCategory.STOREROOM:
+            address += " кл."
+        elif category == IcmPropertyCategory.PARKING_PLACE:
+            address += " мм."
+        elif category == IcmPropertyCategory.BKFN:
+            address += " БКФН."
+        if number := self.number:
+            address += " " + str(number)
+        return address
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
-        BaseObject.update_from_dict(self, data)
+        ObjectWithBuilding.update_from_dict(self, data)
 
         self.scheme_id = data.get("scheme_id") or None
         self.number = data.get("number") or None
         self.section = data.get("section") or None
-        self.building_id = data.get("building_id") or None
         self.district_id = data.get("district_id") or None
         self.account_number = data.get("account_number") or None
 
     @property
     def intercoms(self) -> Mapping[int, "IcmIntercom"]:
         return {
             intercom_id: intercom_device
@@ -54,16 +134,16 @@
     snapshot_url: Optional[str] = None
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         BaseCallSession.update_from_dict(self, data)
         self.intercom_name = data.get("intercom_name") or None
         self.snapshot_url = data.get("photo_url") or None
 
-    async def async_unlock(self, mode: Optional[str] = None) -> None:
-        await self.api.icm_intercoms[self.intercom_id].async_unlock()
+    async def unlock(self, mode: Optional[str] = None) -> None:
+        await self.api.icm_intercoms[self.intercom_id].unlock()
 
 
 @dataclass(slots=True)
 class IcmCallSession(BaseIcmCallSession):
     # From call session
     call_number: Optional[str] = None
 
@@ -118,17 +198,17 @@
 
 @dataclass(slots=True)
 class IcmIntercom(
     ObjectWithSnapshot,
     ObjectWithVideo,
     ObjectWithUnlocker,
     ObjectWithSIP,
+    ObjectWithBuilding,
 ):
     scheme_id: Optional[int] = None
-    building_id: Optional[int] = None
     kind: Optional[str] = None
     device_category: Optional[str] = None
     mode: Optional[str] = None
     name: Optional[str] = None
     human_name: Optional[str] = None
     renamed_name: Optional[str] = None
     relays: Optional[Dict[str, str]] = None
@@ -148,17 +228,17 @@
     property_ids: Set[int] = field(default_factory=set)
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         ObjectWithSnapshot.update_from_dict(self, data)
         ObjectWithVideo.update_from_dict(self, data)
         ObjectWithUnlocker.update_from_dict(self, data)
         ObjectWithSIP.update_from_dict(self, data)
+        ObjectWithBuilding.update_from_dict(self, data)
 
         self.scheme_id = data.get("scheme_id") or None
-        self.building_id = data.get("building_id") or None
         self.kind = data.get("kind") or None
         self.device_category = data.get("device_category") or None
         self.mode = data.get("mode") or None
         self.name = data.get("name") or None
         self.human_name = data.get("human_name") or None
         self.renamed_name = data.get("renamed_name") or None
         self.checkpoint_relay_index = data.get("checkpoint_relay_index")
@@ -194,10 +274,10 @@
 
         return next(iter(video_streams.values()))
 
     @property
     def snapshot_url(self) -> Optional[str]:
         return self.photo_url
 
-    async def async_unlock(self) -> None:
+    async def unlock(self) -> None:
         """Unlock intercom"""
         await self.api.icm_unlock_intercom(self.id, self.mode)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pik_intercom-0.0.3/pik_intercom/iot.py` & `pik_intercom-0.0.4/pik_intercom/iot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import logging
 from abc import ABC
 from dataclasses import dataclass
-from typing import Optional, Any, List, Mapping, Final
+from types import MappingProxyType
+from typing import Optional, Any, List, Mapping, Final, Union, Tuple
 
 try:
     from enum import StrEnum
 except ImportError:
     from strenum import StrEnum
 
 from .base import (
@@ -20,22 +21,31 @@
 from .errors import (
     PikIntercomException,
 )
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
+class IotMeterKind(StrEnum):
+    """Known kinds of IoT meters."""
+
+    HOT = "hot"
+    COLD = "cold"
+    HEAT = "heat"
+    ELECTRO = "electro"
+
+
 @dataclass(slots=True)
 class IotMeter(BaseObject):
     """IoT meter representation."""
 
     serial: Optional[str] = None
     """Meter serial number"""
 
-    kind: Optional[str] = None
+    kind: Optional[IotMeterKind] = None
     """Type of meter"""
 
     pipe_identifier: Optional[int] = None
     """Identifier of pipe (for water meters)"""
 
     status: Optional[str] = None
     """Current status (for meters with communication)"""
@@ -139,15 +149,15 @@
     geo_unit_full_name: Optional[str] = None
 
     # From sip_account parameter
     sip_proxy: Optional[str] = None
     sip_user: Optional[str] = None
 
     # Non-expected properties
-    status: Optional[IotIntercomStatus | str] = None
+    status: Optional[Union[IotIntercomStatus, str]] = None
     webrtc_supported: Optional[bool] = None
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         BaseIotCamera.update_from_dict(self, data)
         ObjectWithSIP.update_from_dict(self, data)
         ObjectWithUnlocker.update_from_dict(self, data)
 
@@ -200,34 +210,63 @@
                     return relay.stream_url
 
         # Return first relay
         for relay in self.relays:
             if relay.stream_url:
                 return relay.stream_url
 
-    async def async_unlock(self) -> None:
+    async def unlock(self) -> None:
         if not (relay_ids := self.relay_ids):
             raise RuntimeError("intercom does not have any relays")
         await asyncio.gather(*map(self.api.iot_unlock_relay, relay_ids))
 
 
 @dataclass(slots=True)
 class IotRelay(BaseIotCameraWithRTSP, ObjectWithUnlocker):
     # From geo_unit parameter
     geo_unit_id: Optional[int] = None
     geo_unit_full_name: Optional[str] = None
+    property_geo_units: Optional[Mapping[int, Tuple[str, str]]] = None
 
     # From user_settings parameter
     custom_name: Optional[str] = None
     is_favorite: bool = False
     is_hidden: bool = False
 
     # Propagated from parent intercom
     geo_unit_short_name: Optional[str] = None
 
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCameraWithRTSP.update_from_dict(self, data)
+        ObjectWithUnlocker.update_from_dict(self, data)
+
+        if property_geo_units := data.get("property_geo_units"):
+            units = {}
+            for geo_unit_data in property_geo_units:
+                units[geo_unit_data["id"]] = (geo_unit_data["post_name"], geo_unit_data["type"])
+            self.property_geo_units = MappingProxyType(units)
+        else:
+            self.property_geo_units = None
+
+        # Parse geo_unit parameter
+        geo_unit_data = data.get("geo_unit") or {}
+        self.geo_unit_id = geo_unit_data.get("id") or None
+        self.geo_unit_full_name = geo_unit_data.get("full_name") or None
+
+        # Parse user_settings parameter
+        relay_settings_data = data.get("user_settings") or {}
+        self.custom_name = relay_settings_data.get("custom_name") or None
+        self.is_favorite = bool(relay_settings_data.get("is_favorite"))
+        self.is_hidden = bool(relay_settings_data.get("is_hidden"))
+
+    @property
+    def property_geo_unit(self) -> Optional[Tuple[int, str, str]]:
+        for geo_unit_id, (geo_unit_name, geo_unit_type) in self.property_geo_units.items():
+            return geo_unit_id, geo_unit_name, geo_unit_type
+
     @property
     def intercoms(self) -> List["IotIntercom"]:
         """Retrieve list of related intercoms."""
         relay_id = self.id
         return [
             intercom
             for intercom in self.api.iot_intercoms.values()
@@ -242,33 +281,18 @@
             if relay_id in intercom.relay_ids:
                 return intercom
 
     @property
     def friendly_name(self) -> str:
         return self.custom_name or self.name
 
-    async def async_unlock(self) -> None:
+    async def unlock(self) -> None:
         """Unlock IoT relay"""
         return await self.api.iot_unlock_relay(self.id)
 
-    def update_from_dict(self, data: Mapping[str, Any]) -> None:
-        BaseIotCameraWithRTSP.update_from_dict(self, data)
-        ObjectWithUnlocker.update_from_dict(self, data)
-
-        # Parse geo_unit parameter
-        geo_unit_data = data.get("geo_unit") or {}
-        self.geo_unit_id = geo_unit_data.get("id") or None
-        self.geo_unit_full_name = geo_unit_data.get("full_name") or None
-
-        # Parse user_settings parameter
-        relay_settings_data = data.get("user_settings") or {}
-        self.custom_name = relay_settings_data.get("custom_name") or None
-        self.is_favorite = bool(relay_settings_data.get("is_favorite"))
-        self.is_hidden = bool(relay_settings_data.get("is_hidden"))
-
 
 @dataclass(slots=True)
 class IotCamera(BaseIotCameraWithRTSP):
     geo_unit_short_name: Optional[str] = None
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         BaseIotCameraWithRTSP.update_from_dict(self, data)
@@ -293,16 +317,16 @@
         self.identifier = data.get("identifier") or None
         self.provider = data.get("iot_pik") or None
 
         # Bypass lack of attribute
         if self.created_at is None and (notified_at := self.notified_at):
             self.created_at = notified_at
 
-    async def async_unlock(self) -> None:
-        await self.api.iot_intercoms[self.intercom_id].async_unlock()
+    async def unlock(self) -> None:
+        await self.api.iot_intercoms[self.intercom_id].unlock()
 
 
 @dataclass(slots=True)
 class IotActiveCallSession(IotCallSession):
     intercom_name: Optional[str] = None
     property_name: Optional[str] = None
     sip_proxy: Optional[str] = None
@@ -329,23 +353,23 @@
         relay_ids = self.target_relay_ids
         return [
             relay
             for key, relay in self.api.iot_relays.items()
             if key in relay_ids
         ]
 
-    async def async_unlock(self) -> None:
+    async def unlock(self) -> None:
         if not self.target_relays:
             raise PikIntercomException("no target relays provided")
 
         errors = []
         for task in (
             await asyncio.wait(
                 [
-                    asyncio.create_task(relay.async_unlock())
+                    asyncio.create_task(relay.unlock())
                     for relay in self.target_relays
                 ],
                 return_when=asyncio.ALL_COMPLETED,
             )
         )[0]:
             if (exc := task.exception()) and not isinstance(
                 exc, asyncio.CancelledError
```

### Comparing `pik_intercom-0.0.3/pik_intercom.egg-info/PKG-INFO` & `pik_intercom-0.0.4/pik_intercom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik-intercom
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.3/setup.py` & `pik_intercom-0.0.4/setup.py`

 * *Files identical despite different names*

