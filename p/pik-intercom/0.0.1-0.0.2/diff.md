# Comparing `tmp/pik_intercom-0.0.1.tar.gz` & `tmp/pik_intercom-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pik_intercom-0.0.1.tar", last modified: Thu Jul  6 14:12:49 2023, max compression
+gzip compressed data, was "pik_intercom-0.0.2.tar", last modified: Thu Jul  6 23:44:54 2023, max compression
```

## Comparing `pik_intercom-0.0.1.tar` & `pik_intercom-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:12:49.187169 pik_intercom-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 14:12:49.187169 pik_intercom-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:12:49.187169 pik_intercom-0.0.1/pik_intercom/
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pik_intercom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pik_intercom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pik_intercom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pik_intercom/icm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pik_intercom/iot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:12:49.187169 pik_intercom-0.0.1/pik_intercom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 14:12:49.000000 pik_intercom-0.0.1/pik_intercom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 14:12:49.000000 pik_intercom-0.0.1/pik_intercom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:12:49.000000 pik_intercom-0.0.1/pik_intercom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:12:49.000000 pik_intercom-0.0.1/pik_intercom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 14:12:49.187169 pik_intercom-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-06 14:12:39.000000 pik_intercom-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.817609 pik_intercom-0.0.2/pik_intercom/
+-rw-r--r--   0 runner    (1001) docker     (123)    26869 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/icm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/iot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/pik_intercom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/setup.py
```

### Comparing `pik_intercom-0.0.1/LICENSE` & `pik_intercom-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.1/PKG-INFO` & `pik_intercom-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pik_intercom
-Version: 0.0.1
-Summary: Example PyPI (Python Package Index) Package
+Version: 0.0.2
+Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
-Keywords: example,pypi,package
+Keywords: pypi,package,pik,intercom
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pik_intercom-0.0.1/pik_intercom/__init__.py` & `pik_intercom-0.0.2/pik_intercom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Pik Intercom API"""
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 import json
 import random
 import string
 from typing import (
     TypeVar,
     ClassVar,
@@ -30,39 +30,49 @@
 DEFAULT_CLIENT_VERSION: Final = "2023.5.1"
 DEFAULT_CLIENT_OS: Final = "Android"
 _TBaseObject = TypeVar("_TBaseObject", bound=BaseObject)
 
 
 @dataclass(slots=True)
 class PikAccount(BaseObject):
+    """Placeholder for data related to user account."""
+
     phone: Optional[str] = None
     email: Optional[str] = None
     apartment_id: Optional[int] = None
     number: Optional[str] = None
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     middle_name: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(PikAccount, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseObject.update_from_dict(self, data)
 
         self.phone = data.get("phone") or None
         self.email = data.get("email") or None
         self.number = data.get("number") or None
         self.apartment_id = data.get("apartment_id") or None
         self.first_name = data.get("first_name") or None
         self.last_name = data.get("last_name") or None
         self.middle_name = data.get("middle_name") or None
 
 
 @dataclass(slots=True)
 class CustomerDevice(ObjectWithSIP):
+    """Placeholder for data related to customer device."""
+
     account_id: Optional[int] = None
+    """Account identifier"""
+
     uid: Optional[str] = None
+    """Unique identifier"""
+
     apartment_id: Optional[int] = None
+    """Apartment identifier (for installed devices)"""
+
     model: Optional[str] = None
     kind: Optional[str] = None
     firmware_version: Optional[str] = None
     mac_address: Optional[str] = None
     os: Optional[str] = None
     deleted_at: Any = None
 
@@ -71,16 +81,16 @@
     sip_proxy: Optional[str] = None
     sip_realm: Optional[str] = None
     sip_enable: bool = False
     sip_alias: Optional[str] = None
     sip_status: Optional[str] = None
     sip_password: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(CustomerDevice, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        ObjectWithSIP.update_from_dict(self, data)
 
         self.apartment_id = data.get("apartment_id") or None
         self.model = data.get("model") or None
         self.kind = data.get("kind") or None
         self.firmware_version = data.get("firmware_version") or None
         self.mac_address = data.get("mac_address") or None
         self.os = data.get("os") or None
```

### Comparing `pik_intercom-0.0.1/pik_intercom/base.py` & `pik_intercom-0.0.2/pik_intercom/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class BaseObject(ABC):
     """Base class for PIK Intercom Objects"""
 
     api: "PikIntercomAPI"
     id: int
     source_data: Any = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
         """Update object attributes from provided source dictionary."""
         self.source_data = data
 
     @classmethod
     def get_id_from_data(cls, data: Mapping[str, Any]) -> int:
         return int(data["id"])
 
@@ -128,25 +128,26 @@
                 if device.sip_user == user and (
                     password := device.sip_password
                 ):
                     return password
 
 
 @dataclass(slots=True)
-class BaseCallSession(ObjectWithSnapshot, ABC):
+class BaseCallSession(ObjectWithSnapshot, ObjectWithUnlocker, ABC):
     intercom_id: Optional[int] = None
     # property_id: Optional[int] = None
     notified_at: Optional[datetime] = None
     pickedup_at: Optional[datetime] = None
     finished_at: Optional[datetime] = None
     created_at: Optional[datetime] = None
     deleted_at: Optional[datetime] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(BaseCallSession, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        ObjectWithSnapshot.update_from_dict(self, data)
+        ObjectWithUnlocker.update_from_dict(self, data)
 
         self.intercom_id = (
             int(data["intercom_id"]) if data.get("intercom_id") else None
         )
         for timestamp in (
             "notified_at",
             "pickedup_at",
```

### Comparing `pik_intercom-0.0.1/pik_intercom/icm.py` & `pik_intercom-0.0.2/pik_intercom/icm.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     building_id: Optional[int] = None
     district_id: Optional[int] = None
     account_number: Optional[str] = None
 
     # Externally set properties
     category: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IcmProperty, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseObject.update_from_dict(self, data)
 
         self.scheme_id = data.get("scheme_id") or None
         self.number = data.get("number") or None
         self.section = data.get("section") or None
         self.building_id = data.get("building_id") or None
         self.district_id = data.get("district_id") or None
         self.account_number = data.get("account_number") or None
@@ -45,23 +45,26 @@
         }
 
     async def update_intercoms(self) -> None:
         await self.api.icm_update_intercoms(self.id)
 
 
 @dataclass(slots=True)
-class BaseIcmCallSession(BaseCallSession, ObjectWithSnapshot):
+class BaseIcmCallSession(BaseCallSession):
     intercom_name: Optional[str] = None
     snapshot_url: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(BaseIcmCallSession, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseCallSession.update_from_dict(self, data)
         self.intercom_name = data.get("intercom_name") or None
         self.snapshot_url = data.get("photo_url") or None
 
+    async def async_unlock(self, mode: Optional[str] = None) -> None:
+        await self.api.icm_intercoms[self.intercom_id].async_unlock()
+
 
 @dataclass(slots=True)
 class IcmCallSession(BaseIcmCallSession):
     # From call session
     call_number: Optional[str] = None
 
     # From root
@@ -69,18 +72,18 @@
     hangup: bool = False
 
     @classmethod
     def get_id_from_data(cls, data: Mapping[str, Any]) -> int:
         """Call session identifier is embedded in a sub-dict."""
         return int(data["call_session"]["id"])
 
-    def update_from_dict(self, data: Mapping[str, Any]):
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
         # This call session type holds call session data in a sub-dict
         call_session_data = data.get("call_session") or {}
-        super(IcmCallSession, self).update_from_dict(call_session_data)
+        BaseIcmCallSession.update_from_dict(self, call_session_data)
 
         self.call_number = call_session_data.get("call_number")
         self.answered_customer_device_ids = tuple(
             map(int, data.get("answered_customer_device_ids") or ())
         )
         self.hangup = bool(data.get("hangup"))
 
@@ -91,16 +94,16 @@
     call_id: Optional[str] = None
     call_from: Optional[int] = None
     mode: Optional[str] = None
     session_id: Optional[int] = None
     sip_proxy: Optional[str] = None
     property_id: Optional[int] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IcmActiveCallSession, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIcmCallSession.update_from_dict(self, data)
 
         self.call_duration = data.get("call_duration") or None
         self.call_id = data.get("call_id") or None
         self.call_from = data.get("from") or None
         self.mode = data.get("mode") or None
         self.session_id = data.get("session_id") or None
         self.sip_proxy = data.get("proxy") or None
@@ -140,16 +143,19 @@
     # From sip_account parameter
     sip_account_proxy: Optional[str] = None
     sip_account_ex_user: Optional[str] = None
 
     # Non-standard attribute
     property_ids: Set[int] = field(default_factory=set)
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IcmIntercom, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        ObjectWithSnapshot.update_from_dict(self, data)
+        ObjectWithVideo.update_from_dict(self, data)
+        ObjectWithUnlocker.update_from_dict(self, data)
+        ObjectWithSIP.update_from_dict(self, data)
 
         self.scheme_id = data.get("scheme_id") or None
         self.building_id = data.get("building_id") or None
         self.kind = data.get("kind") or None
         self.device_category = data.get("device_category") or None
         self.mode = data.get("mode") or None
         self.name = data.get("name") or None
```

### Comparing `pik_intercom-0.0.1/pik_intercom/iot.py` & `pik_intercom-0.0.2/pik_intercom/iot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import asyncio
 import logging
 from abc import ABC
 from dataclasses import dataclass
-from enum import StrEnum
 from typing import Optional, Any, List, Mapping, Final
 
+try:
+    from enum import StrEnum
+except ImportError:
+    from strenum import StrEnum
+
 from .base import (
     BaseObject,
     ObjectWithSnapshot,
     ObjectWithVideo,
     ObjectWithUnlocker,
     ObjectWithSIP,
     BaseCallSession,
@@ -18,16 +22,42 @@
 )
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 @dataclass(slots=True)
 class IotMeter(BaseObject):
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotMeter, self).update_from_dict(data)
+    """IoT meter representation."""
+
+    serial: Optional[str] = None
+    """Meter serial number"""
+
+    kind: Optional[str] = None
+    """Type of meter"""
+
+    pipe_identifier: Optional[int] = None
+    """Identifier of pipe (for water meters)"""
+
+    status: Optional[str] = None
+    """Current status (for meters with communication)"""
+
+    title: Optional[str] = None
+    """Meter name"""
+
+    current_value: Optional[str] = None
+    """Current (total) value"""
+
+    month_value: Optional[str] = None
+    """Total usage this month"""
+
+    geo_unit_short_name: Optional[str] = None
+    """Location short name"""
+
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseObject.update_from_dict(self, data)
 
         try:
             pipe_identifier = int(data.get("pipe_identifier"))
         except (TypeError, ValueError):
             pipe_identifier = None
 
         self.serial = data.get("serial") or None
@@ -35,66 +65,63 @@
         self.pipe_identifier = pipe_identifier
         self.status = data.get("status") or None
         self.title = data.get("title") or None
         self.current_value = data.get("current_value") or None
         self.month_value = data.get("month_value") or None
         self.geo_unit_short_name = data.get("geo_unit_short_name") or None
 
-        return self
-
-    serial: Optional[str] = None
-    kind: Optional[str] = None
-    pipe_identifier: Optional[int] = None
-    status: Optional[str] = None
-    title: Optional[str] = None
-    current_value: Optional[str] = None
-    month_value: Optional[str] = None
-    geo_unit_short_name: Optional[str] = None
-
     @staticmethod
     def _convert_value(value: Any) -> float:
+        """
+        Convert incoming value formatted as human-readable string.
+        :param value: Incoming value
+        :return: Numeric representation (float)
+        """
         if value is None:
             raise TypeError("cannot convert NoneType to float")
         return float(str(value).rpartition(" ")[0].replace(" ", ""))
 
     @property
     def current_value_numeric(self) -> Optional[float]:
+        """Convert current value to numeric representation."""
         return (
             IotMeter._convert_value(value)
             if (value := self.current_value)
             else None
         )
 
     @property
     def month_value_numeric(self) -> Optional[float]:
+        """Convert month value to numeric representation."""
         return (
             IotMeter._convert_value(value)
             if (value := self.month_value)
             else None
         )
 
 
 @dataclass(slots=True)
 class BaseIotCamera(ObjectWithSnapshot, ABC):
     name: Optional[str] = None
     snapshot_url: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(BaseIotCamera, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCamera.update_from_dict(self, data)
 
         self.name = data.get("name") or None
         self.snapshot_url = data.get("live_snapshot_url") or None
 
 
 @dataclass(slots=True)
 class BaseIotCameraWithRTSP(BaseIotCamera, ObjectWithVideo, ABC):
     stream_url: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(BaseIotCameraWithRTSP, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCameraWithRTSP.update_from_dict(self, data)
+        ObjectWithVideo.update_from_dict(self, data)
 
         self.stream_url = data.get("rtsp_url") or None
 
 
 class IotIntercomStatus(StrEnum):
     ONLINE = "online"
     OFFLINE = "offline"
@@ -115,16 +142,18 @@
     sip_proxy: Optional[str] = None
     sip_user: Optional[str] = None
 
     # Non-expected properties
     status: Optional[IotIntercomStatus | str] = None
     webrtc_supported: Optional[bool] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotIntercom, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCamera.update_from_dict(self, data)
+        ObjectWithSIP.update_from_dict(self, data)
+        ObjectWithUnlocker.update_from_dict(self, data)
 
         self.client_id = data.get("client_id") or None
         self.is_face_detection = bool(data.get("is_face_detection"))
         self.status = data.get("status") or None
         self.webrtc_supported = (
             bool(data["webrtc_supported"])
             if "webrtc_supported" in data
@@ -217,16 +246,17 @@
     def friendly_name(self) -> str:
         return self.custom_name or self.name
 
     async def async_unlock(self) -> None:
         """Unlock IoT relay"""
         return await self.api.iot_unlock_relay(self.id)
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotRelay, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCameraWithRTSP.update_from_dict(self, data)
+        ObjectWithUnlocker.update_from_dict(self, data)
 
         # Parse geo_unit parameter
         geo_unit_data = data.get("geo_unit") or {}
         self.geo_unit_id = geo_unit_data.get("id") or None
         self.geo_unit_full_name = geo_unit_data.get("full_name") or None
 
         # Parse user_settings parameter
@@ -236,70 +266,58 @@
         self.is_hidden = bool(relay_settings_data.get("is_hidden"))
 
 
 @dataclass(slots=True)
 class IotCamera(BaseIotCameraWithRTSP):
     geo_unit_short_name: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotCamera, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseIotCameraWithRTSP.update_from_dict(self, data)
+
         self.geo_unit_short_name = data.get("geo_unit_short_name") or None
-        return self
 
 
 @dataclass(slots=True)
-class IotCallSession(BaseCallSession, ObjectWithSnapshot):
+class IotCallSession(BaseCallSession):
     geo_unit_id: Optional[int] = None
     geo_unit_short_name: Optional[str] = None
     snapshot_url: Optional[str] = None
     identifier: Optional[str] = None
     provider: Optional[str] = None
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotCallSession, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        BaseCallSession.update_from_dict(self, data)
 
         self.geo_unit_id = data.get("geo_unit_id") or None
         self.geo_unit_short_name = data.get("geo_unit_short_name") or None
         self.snapshot_url = data.get("snapshot_url") or None
         self.identifier = data.get("identifier") or None
         self.provider = data.get("iot_pik") or None
 
         # Bypass lack of attribute
         if self.created_at is None and (notified_at := self.notified_at):
             self.created_at = notified_at
 
+    async def async_unlock(self) -> None:
+        await self.api.iot_intercoms[self.intercom_id].async_unlock()
+
 
 @dataclass(slots=True)
-class IotActiveCallSession(
-    BaseCallSession, ObjectWithUnlocker, ObjectWithSnapshot
-):
+class IotActiveCallSession(IotCallSession):
     intercom_name: Optional[str] = None
     property_name: Optional[str] = None
-    geo_unit_id: Optional[int] = None
-    geo_unit_short_name: Optional[str] = None
-    identifier: Optional[str] = None
-    provider: Optional[str] = None
-    proxy: Optional[str] = None
-    snapshot_url: Optional[str] = None
+    sip_proxy: Optional[str] = None
     target_relay_ids: tuple[int, ...] = ()
 
-    def update_from_dict(self, data: Mapping[str, Any]):
-        super(IotActiveCallSession, self).update_from_dict(data)
+    def update_from_dict(self, data: Mapping[str, Any]) -> None:
+        IotCallSession.update_from_dict(self, data)
 
         self.intercom_name = data.get("intercom_name") or None
         self.property_name = data.get("property_name") or None
-
-        self.geo_unit_id = (
-            int(data["geo_unit_id"]) if data.get("geo_unit_id") else None
-        )
-        self.geo_unit_short_name = data.get("geo_unit_name") or None
-        self.identifier = data.get("identifier") or None
-        self.provider = data.get("provider") or None
-        self.proxy = data.get("proxy") or None
-        self.snapshot_url = data.get("snapshot_url")
+        self.sip_proxy = data.get("proxy") or None
         self.target_relay_ids = (
             (
                 int(relay_data["id"])
                 for relay_data in data["target_relays"]
                 if relay_data
             )
             if data.get("target_relays")
```

### Comparing `pik_intercom-0.0.1/setup.py` & `pik_intercom-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 GITHUB_URL: Final = "https://github.com/alryaz/pik-intercom-python"
 
 setuptools.setup(
     name="pik_intercom",
     author="Alexander Ryazanov",
     author_email="alryaz@alryaz.com",
-    description="Example PyPI (Python Package Index) Package",
-    keywords="example, pypi, package",
+    description="Pik Intercom API for Python",
+    keywords="pypi, package, pik, intercom",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=GITHUB_URL,
     project_urls={
         "Documentation": GITHUB_URL,
         "Bug Reports": GITHUB_URL + "/issues",
         "Source Code": GITHUB_URL,
```

