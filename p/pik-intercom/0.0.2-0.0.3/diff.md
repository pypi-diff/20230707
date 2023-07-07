# Comparing `tmp/pik_intercom-0.0.2.tar.gz` & `tmp/pik_intercom-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pik_intercom-0.0.2.tar", last modified: Thu Jul  6 23:44:54 2023, max compression
+gzip compressed data, was "pik_intercom-0.0.3.tar", last modified: Fri Jul  7 00:57:32 2023, max compression
```

## Comparing `pik_intercom-0.0.2.tar` & `pik_intercom-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.817609 pik_intercom-0.0.2/pik_intercom/
--rw-r--r--   0 runner    (1001) docker     (123)    26869 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/icm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pik_intercom/iot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/pik_intercom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 23:44:54.000000 pik_intercom-0.0.2/pik_intercom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 23:44:54.821609 pik_intercom-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-06 23:44:44.000000 pik_intercom-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 00:57:32.960236 pik_intercom-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/pik_intercom/
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/icm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pik_intercom/iot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:57:32.956236 pik_intercom-0.0.3/pik_intercom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 00:57:32.000000 pik_intercom-0.0.3/pik_intercom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 00:57:32.960236 pik_intercom-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-07 00:57:17.000000 pik_intercom-0.0.3/setup.py
```

### Comparing `pik_intercom-0.0.2/LICENSE` & `pik_intercom-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.2/PKG-INFO` & `pik_intercom-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik_intercom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.2/pik_intercom/__init__.py` & `pik_intercom-0.0.3/pik_intercom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Pik Intercom API"""
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import json
 import random
 import string
 from typing import (
     TypeVar,
     ClassVar,
@@ -20,19 +20,21 @@
 
 from .base import *
 from .errors import *
 from .icm import *
 from .iot import *
 
 _LOGGER: Final = logging.getLogger(__name__)
+
 DEFAULT_DEVICE_MODEL: Final = "Python API"
 DEFAULT_USER_AGENT: Final = "okhttp/4.9.0"
 DEFAULT_CLIENT_APP: Final = "alfred"
 DEFAULT_CLIENT_VERSION: Final = "2023.5.1"
 DEFAULT_CLIENT_OS: Final = "Android"
+
 _TBaseObject = TypeVar("_TBaseObject", bound=BaseObject)
 
 
 @dataclass(slots=True)
 class PikAccount(BaseObject):
     """Placeholder for data related to user account."""
```

### Comparing `pik_intercom-0.0.2/pik_intercom/base.py` & `pik_intercom-0.0.3/pik_intercom/base.py`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.2/pik_intercom/icm.py` & `pik_intercom-0.0.3/pik_intercom/icm.py`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.2/pik_intercom/iot.py` & `pik_intercom-0.0.3/pik_intercom/iot.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,26 +101,26 @@
 
 @dataclass(slots=True)
 class BaseIotCamera(ObjectWithSnapshot, ABC):
     name: Optional[str] = None
     snapshot_url: Optional[str] = None
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
-        BaseIotCamera.update_from_dict(self, data)
+        ObjectWithSnapshot.update_from_dict(self, data)
 
         self.name = data.get("name") or None
         self.snapshot_url = data.get("live_snapshot_url") or None
 
 
 @dataclass(slots=True)
 class BaseIotCameraWithRTSP(BaseIotCamera, ObjectWithVideo, ABC):
     stream_url: Optional[str] = None
 
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
-        BaseIotCameraWithRTSP.update_from_dict(self, data)
+        BaseIotCamera.update_from_dict(self, data)
         ObjectWithVideo.update_from_dict(self, data)
 
         self.stream_url = data.get("rtsp_url") or None
 
 
 class IotIntercomStatus(StrEnum):
     ONLINE = "online"
```

### Comparing `pik_intercom-0.0.2/pik_intercom.egg-info/PKG-INFO` & `pik_intercom-0.0.3/pik_intercom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik-intercom
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.2/setup.py` & `pik_intercom-0.0.3/setup.py`

 * *Files identical despite different names*

