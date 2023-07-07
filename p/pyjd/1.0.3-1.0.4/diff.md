# Comparing `tmp/pyjd-1.0.3.tar.gz` & `tmp/pyjd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.3.tar", last modified: Fri Jul  7 06:34:40 2023, max compression
+gzip compressed data, was "pyjd-1.0.4.tar", last modified: Fri Jul  7 07:41:29 2023, max compression
```

## Comparing `pyjd-1.0.3.tar` & `pyjd-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 06:34:32.000000 pyjd-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 06:34:40.322980 pyjd-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-07 06:34:32.000000 pyjd-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/pyjd/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/direct_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/direct_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/jd_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/jd_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/linkgrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/myjd_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/myjd_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 06:34:32.000000 pyjd-1.0.3/pyjd/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:34:40.322980 pyjd-1.0.3/pyjd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 06:34:40.000000 pyjd-1.0.3/pyjd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:34:40.322980 pyjd-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-07 06:34:32.000000 pyjd-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:29.003286 pyjd-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 07:41:17.000000 pyjd-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 07:41:28.999286 pyjd-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 07:41:17.000000 pyjd-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:28.999286 pyjd-1.0.4/pyjd/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/direct_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/direct_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/jd_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/jd_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/linkgrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/myjd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 07:41:17.000000 pyjd-1.0.4/pyjd/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:41:28.999286 pyjd-1.0.4/pyjd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 07:41:28.000000 pyjd-1.0.4/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:41:29.003286 pyjd-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-07 07:41:17.000000 pyjd-1.0.4/setup.py
```

### Comparing `pyjd-1.0.3/LICENSE` & `pyjd-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.3/PKG-INFO` & `pyjd-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,26 @@
 
 # pyjd
 
 This is a wrapper for the JDownloader API.
 
 ## Installation
 
-Run `pip install .` in the repository folder.
+```shell
+pip install pyjd
+```
 
 ## Usage
 
 The documentation of the JDownloader API can be found here
 <https://my.jdownloader.org/developers/>. This library includes all of the
 documented functions (but uses underscores instead of CamelCase).
 
 For examples, check out the sample scripts in the repository
-([see here](https://git.sr.ht/~pglaum/pyjd/tree/master/item/examples)).
+([see here](https://github.com/pglaum/pyjd/tree/master/examples)).
 
 ## Building auto-docs
 
 ### Build
 
 Go to into the `docs` directory and run `make html`.
```

### Comparing `pyjd-1.0.3/README.md` & `pyjd-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # pyjd
 
 This is a wrapper for the JDownloader API.
 
 ## Installation
 
-Run `pip install .` in the repository folder.
+```shell
+pip install pyjd
+```
 
 ## Usage
 
 The documentation of the JDownloader API can be found here
 <https://my.jdownloader.org/developers/>. This library includes all of the
 documented functions (but uses underscores instead of CamelCase).
 
 For examples, check out the sample scripts in the repository
-([see here](https://git.sr.ht/~pglaum/pyjd/tree/master/item/examples)).
+([see here](https://github.com/pglaum/pyjd/tree/master/examples)).
 
 ## Building auto-docs
 
 ### Build
 
 Go to into the `docs` directory and run `make html`.
```

### Comparing `pyjd-1.0.3/pyjd/accounts.py` & `pyjd-1.0.4/pyjd/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .jd_types import Account, AccountQuery, BasicAuth, BasicAuthType
-from typing import Any, Dict, List, TYPE_CHECKING
+from typing import Optional, Any, Dict, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class Accounts:
     def __init__(self, device: "JDDevice"):
 
         self.device = device
         self.endpoint = "accountsV2"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def add_account(self, premium_hoster: str, username: str, password: str) -> None:
         """Add a premium hoster account.
 
         .. warning:: The password is used in plain text, so beware...
```

### Comparing `pyjd-1.0.3/pyjd/captcha.py` & `pyjd-1.0.4/pyjd/captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from .jd_types import CaptchaJob, SkipRequest
-from typing import Any, List, TYPE_CHECKING
+from typing import Optional, Any, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class Captcha:
     def __init__(self, device: "JDDevice") -> None:
 
         self.device = device
         self.endpoint = "captcha"
 
-    def action(self, route: str, params: Any = None, binary: bool = False) -> Any:
+    def action(self, route: str, params: Optional[Any] = None, binary: bool = False) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params, binary=binary)
 
-    def get(self, captcha_id: int, c_format: str = None) -> str:
+    def get(self, captcha_id: int, c_format: Optional[str] = None) -> str:
         """Get the base64 captcha image.
 
         The result is a captcha image as base64 encoded data url.
 
         :param captcha_id: The ID of the captcha.
         :type captcha_id: int
         :param format: The format
@@ -76,15 +76,15 @@
         :rtype: boolean
         """
 
         params = [captcha_id, skip_type.value]
         resp = self.action("/skip", params)
         return resp
 
-    def solve(self, captcha_id: int, result: str, result_format: str = None) -> bool:
+    def solve(self, captcha_id: int, result: str, result_format: Optional[str] = None) -> bool:
         """Solve a captcha.
 
         :param captcha_id: The ID of the captcha that is solved.
         :type captcha_id: int
         :param result: The solution of the captcha.
         :type result: str
         :param result_format: Format of the result
```

### Comparing `pyjd-1.0.3/pyjd/config.py` & `pyjd-1.0.4/pyjd/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .jd_types import AdvancedConfigAPIEntry, AdvancedConfigQuery, EnumOption
-from typing import Any, List, TYPE_CHECKING
+from typing import Optional, Any, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class Config:
     def __init__(self, device: "JDDevice") -> None:
         self.device = device
         self.endpoint = "config"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def get(self, interface_name: str, storage: str, key: str) -> Any:
         """Get value from interface by key.
 
         :param interface_name: The name of the JDownloader interface
```

### Comparing `pyjd-1.0.3/pyjd/content.py` & `pyjd-1.0.4/pyjd/content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .jd_types import IconDescriptor
-from typing import Any, TYPE_CHECKING
+from typing import Optional, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class Content:
     def __init__(self, device: "JDDevice") -> None:
         self.device = device
         self.endpoint = "contentV2"
 
-    def action(self, route: str, params: Any = None, binary: bool = False) -> Any:
+    def action(self, route: str, params: Optional[Any] = None, binary: bool = False) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params, binary=binary)
 
     def get_fav_icon(self, hostername: str) -> bytes:
         """Get the fav icon for a hoster.
 
         :param hostername: Name of the hoster for which the favicon will be
@@ -63,9 +63,10 @@
         :type key: str
         :returns: Description for the key
         :rtype: str
         """
 
         params = [key]
         resp = self.action("/getIconDescription", params)
+        print(resp)
         descriptor = IconDescriptor(**resp)
         return descriptor
```

### Comparing `pyjd-1.0.3/pyjd/direct_connection_helper.py` & `pyjd-1.0.4/pyjd/direct_connection_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any
+from typing import Optional, Any
 import json
 import requests
 
 
 class DirectConnectionHelper:
     def __init__(self, device):
 
         self.device = device
 
     def action(
         self,
         path: str,
-        params: Any = None,
+        params: Optional[Any] = None,
         http_action: str = "POST",
         binary: bool = False,
     ) -> Any:
         """Make the request to the JDownloader.
 
         :param path: The URL endpoint (excluding base_url) that is called.
         :type path: str
```

### Comparing `pyjd-1.0.3/pyjd/direct_connector.py` & `pyjd-1.0.4/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.3/pyjd/downloads.py` & `pyjd-1.0.4/pyjd/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class Downloads:
     def __init__(self, device):
         self.device = device
         self.endpoint = "downloadsV2"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def cleanup(
         self,
         link_ids: List[int],
         package_ids: List[int],
@@ -370,15 +370,15 @@
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         """
 
         params = [priority.value, link_ids, package_ids]
         self.action("/setPriority", params)
 
-    def set_stop_mark(self, link_id: int = None, package_id: int = None) -> None:
+    def set_stop_mark(self, link_id: Optional[int] = None, package_id: Optional[int] = None) -> None:
         """Set the stop mark to the specified id.
 
         Only one of link_id and package_id has to be given.
 
         :param link_id: A link id for the stop mark
         :type link_id: int
         :param package_id: A package id for the stop mark
```

### Comparing `pyjd-1.0.3/pyjd/events.py` & `pyjd-1.0.4/pyjd/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     subscribe _before_ you load your data. Otherwise it can happen, that there
     has been a change of content between you loading the data and then
     subscribing (especially if done over network).
 
 """
 
 from .jd_types import SubscriptionResponse, PublisherResponse
-from typing import Any, List
+from typing import Optional, Any, List
 
 
 class Events:
     def __init__(self, device):
         self.device = device
         self.endpoint = "events"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def add_subscription(
         self,
         subscription_id: int,
         subscriptions: List[str] = [],
```

### Comparing `pyjd-1.0.3/pyjd/extensions.py` & `pyjd-1.0.4/pyjd/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .jd_types import Extension, ExtensionQuery
-from typing import Any, List
+from typing import Optional, Any, List
 
 
 class Extensions:
     def __init__(self, device):
         self.device = device
         self.endpoint = "extensions"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def install(self, extension_id: str) -> bool:
         """Install the extension with extension_id.
 
         :param extension_id: The ID of the extension
```

### Comparing `pyjd-1.0.3/pyjd/jd_device.py` & `pyjd-1.0.4/pyjd/jd_device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.3/pyjd/jd_types.py` & `pyjd-1.0.4/pyjd/jd_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 These are the types and constants that are defined in JDownloader.
 
 For more information, see here:
     https://my.jdownloader.org/developers/index.html#tag_342
 """
 
+from __future__ import annotations
+
 from enum import Enum
 from pydantic import BaseModel
-from typing import Any, ForwardRef, List, Optional
+from typing import Any, List, Optional
 
 
 #
 # enums and constants
 #
 
 
@@ -186,28 +188,29 @@
     """Query for premium host accounts.
 
     The fields are booleans, that can be turned on or off, if you want to have
     query for the information or not.
     By default all possible data is queried.
     """
 
-    enabled: bool = (True,)
-    error: bool = (True,)
-    maxResults: int = (-1,)
-    startAt: int = (0,)
-    trafficLeft: bool = (True,)
-    trafficMax: bool = (True,)
-    userName: bool = (True,)
+    enabled: bool = True
+    error: bool = True
+    maxResults: int = -1
+    startAt: int = 0
+    trafficLeft: bool = True
+    trafficMax: bool = True
+    userName: bool = True
     uuidlist: Optional[List[int]]
-    valid: bool = (True,)
-    validUntil: bool = (True,)
+    valid: bool = True
+    validUntil: bool = True
 
     def __repr__(self):
-        return f"<AccountQuery ({self.uuid_list})>"
+        return f"<AccountQuery ({self.uuidlist})>"
 
+    @staticmethod
     def default():
         return AccountQuery(
             enabled=True,
             error=True,
             maxResults=-1,
             startAt=0,
             trafficLeft=True,
@@ -243,16 +246,17 @@
     description: bool
     enumInfo: bool
     includeExtensions: bool
     pattern: Optional[str]
     values: bool
 
     def __repr__(self):
-        return f"<AdvancedConfigQuery ({self.config_interface})>"
+        return f"<AdvancedConfigQuery ({self.configInterface})>"
 
+    @staticmethod
     def default():
         return AdvancedConfigQuery(
             configInterface=None,
             defaultValues=True,
             description=True,
             enumInfo=True,
             includeExtensions=True,
@@ -306,14 +310,15 @@
     forNullKey: Optional[str]
     maxResults: int
     startAt: int
 
     def __repr__(self):
         return "<APIQuery>"
 
+    @staticmethod
     def default():
         return APIQuery(empty=False, forNullKey="", maxResults=-1, startAt=0)
 
 
 class CaptchaJob(BaseModel):
 
     captchaCategory: Optional[str]
@@ -322,15 +327,15 @@
     hoster: Optional[str]
     id: Optional[int]
     link: Optional[int]
     timeout: Optional[int]
     type: Optional[str]
 
     def __repr__(self):
-        return f"<CaptchaJob ({self.captcha_id})>"
+        return f"<CaptchaJob ({self.id})>"
 
 
 class LinkVariant(BaseModel):
 
     iconKey: Optional[str]
     id: Optional[str]
     name: Optional[str]
@@ -378,14 +383,15 @@
     variantIcon: Optional[bool]
     variantName: Optional[bool]
     variants: Optional[bool]
 
     def __repr__(self):
         return "<CrawledLinkQuery>"
 
+    @staticmethod
     def default():
         return CrawledLinkQuery(
             availability=True,
             bytesTotal=True,
             comment=True,
             enabled=True,
             host=True,
@@ -442,14 +448,15 @@
     saveTo: Optional[bool]
     startAt: Optional[int]
     status: Optional[bool]
 
     def __repr__(self):
         return "<CrawledPackageQuery>"
 
+    @staticmethod
     def default():
         return CrawledPackageQuery(
             availableOfflineCount=True,
             availableOnlineCount=True,
             availableTempUnknownCount=True,
             availableUnknownCount=True,
             bytesTotal=True,
@@ -526,14 +533,15 @@
     installed: Optional[bool]
     name: Optional[bool]
     pattern: Optional[str]
 
     def __repr__(self):
         return "<ExtensionQuery>"
 
+    @staticmethod
     def default():
         return ExtensionQuery(
             configInterface=True,
             description=True,
             enabled=True,
             iconKey=True,
             installed=True,
@@ -563,23 +571,20 @@
     statusIconKey: Optional[str]
     uuid: Optional[int]
 
     def __repr__(self):
         return f"<FilePackage ({self.uuid})>"
 
 
-IconDescriptor = ForwardRef("IconDescriptor")
-
-
 class IconDescriptor(BaseModel):
 
     cls: Optional[str]
     key: Optional[str]
     prps: Optional[Any]
-    rsc: Optional[IconDescriptor]
+    rsc: Optional[List[IconDescriptor]]
 
     def __repr__(self):
         return f"<IconDescriptor ({self.key})>"
 
 
 class JobLinkCrawler(BaseModel):
 
@@ -589,28 +594,28 @@
     crawledId: Optional[int]
     crawling: Optional[bool]
     filtered: Optional[int]
     jobId: Optional[int]
     unhandled: Optional[int]
 
     def __repr__(self):
-        return f"<JobLinkCrawler ({self.crawlerId})>"
+        return f"<JobLinkCrawler ({self.crawledId})>"
 
 
 class LinkStatus(BaseModel):
 
     host: Optional[str]
     linkCheckID: Optional[str]
     name: Optional[str]
     size: Optional[int]
     status: Optional[AvailableLinkState]
     url: Optional[str]
 
     def __repr__(self):
-        return f"<LinkStatus ({self.link_check_id})>"
+        return f"<LinkStatus ({self.linkCheckID})>"
 
 
 class LinkCheckResult(BaseModel):
 
     link: Optional[List[LinkStatus]]
     status: Optional[Status]
 
@@ -630,14 +635,15 @@
 
     collectorInfo: Optional[bool]
     jobIds: Optional[List[int]]
 
     def __repr__(self):
         return "<LinkCrawlerJobsQuery>"
 
+    @staticmethod
     def default():
         return LinkCrawlerJobsQuery(collectorInfo=True, jobIds=None)
 
 
 class LinkQuery(BaseModel):
 
     addedDate: Optional[bool]
@@ -661,14 +667,15 @@
     startAt: Optional[int]
     status: Optional[bool]
     url: Optional[bool]
 
     def __repr__(self):
         return "<LinkQuery>"
 
+    @staticmethod
     def default():
         return LinkQuery(
             addedDate=True,
             bytesLoaded=True,
             bytesTotal=True,
             comment=True,
             enabled=True,
@@ -697,27 +704,24 @@
     current: Optional[bool]
     lastModified: Optional[int]
 
     def __repr__(self):
         return "<LogFolder>"
 
 
-MenuStructure = ForwardRef("MenuStructure")
-
-
 class MenuStructure(BaseModel):
 
     children: Optional[List[MenuStructure]]
     icon: Optional[str]
     id: Optional[str]
     name: Optional[str]
     type: Optional[MenuType]
 
     def __repr__(self):
-        return f"<MenuStructure ({self.menuId})>"
+        return f"<MenuStructure ({self.id})>"
 
 
 class PackageQuery(BaseModel):
 
     bytesLoaded: Optional[bool]
     bytesTotal: Optional[bool]
     childCount: Optional[bool]
@@ -734,14 +738,15 @@
     speed: Optional[bool]
     startAt: Optional[int]
     status: Optional[bool]
 
     def __repr__(self):
         return "<PackageQuery>"
 
+    @staticmethod
     def default():
         return PackageQuery(
             bytesLoaded=True,
             bytesTotal=True,
             childCount=True,
             comment=True,
             enabled=True,
@@ -784,14 +789,15 @@
 
     pattern: Optional[str]
     version: Optional[str]
 
     def __repr__(self):
         return f"<PluginsQuery ({self.pattern})>"
 
+    @staticmethod
     def default():
         return PluginsQuery(pattern="", version=None)
 
 
 class PublisherResponse(BaseModel):
 
     eventids: Optional[List[str]]
@@ -807,15 +813,15 @@
     maxKeepalive: Optional[int]
     maxPolltimeout: Optional[int]
     subscribed: Optional[bool]
     subscriptionid: Optional[int]
     subscriptions: Optional[List[str]]
 
     def __repr__(self):
-        return f"<SubscriptionResponse ({self.subscription_id})>"
+        return f"<SubscriptionResponse ({self.subscriptionid})>"
 
 
 class IPandPort(BaseModel):
 
     port: int
     ip: str
```

### Comparing `pyjd-1.0.3/pyjd/linkgrabber.py` & `pyjd-1.0.4/pyjd/linkgrabber.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,37 +6,37 @@
     CrawledPackageQuery,
     DeleteAction,
     JobLinkCrawler,
     LinkCollectingJob,
     LinkCrawlerJobsQuery,
     LinkVariant,
 )
-from typing import Any
+from typing import Optional, Any
 
 
 class LinkGrabber:
     def __init__(self, device):
         self.device = device
         self.endpoint = "linkgrabberv2"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
-    def abort(self, job_id: int = None) -> bool:
+    def abort(self, job_id: int = -1) -> bool:
         """Abort one or all jobs.
 
         :param job_id: If this is given, only the job `job_id` will be aborted.
         :type job_id: int
         :return: Success
         :rtype: bool
         """
 
         params = None
-        if job_id:
+        if job_id > -1:
             params = [job_id]
 
         resp = self.action("/abort", params)
         return resp
 
     def add_container(self, container_type: str, content: str) -> LinkCollectingJob:
         """Add a container of type and content.
```

### Comparing `pyjd-1.0.3/pyjd/log.py` & `pyjd-1.0.4/pyjd/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .jd_types import LogFolder
-from typing import Any, List
+from typing import Optional, Any, List
 
 
 class Log:
     def __init__(self, device):
         self.device = device
         self.endpoint = "log"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def get_available_logs(self) -> List[LogFolder]:
         """Returns a list of available logs.
 
         :return: List of log folders
```

### Comparing `pyjd-1.0.3/pyjd/myjd_connection_helper.py` & `pyjd-1.0.4/pyjd/myjd_connection_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import time
-from typing import List, TYPE_CHECKING
+from typing import List, TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class MyJDConnectionHelper:
     def __init__(self, device: "JDDevice") -> None:
 
         self.device = device
 
-        self.__direct_connection_info = None
+        self.__direct_connection_info: Optional[list] = None
         self.__refresh_direct_connections()
         self.__direct_connection_enabled = True
         self.__direct_connection_cooldown = 0
         self.__direct_connection_consecutive_failures = 0
 
     def __refresh_direct_connections(self) -> None:
         """Check again if a direct connection is possible."""
@@ -28,15 +28,15 @@
             and "data" in response
             and "infos" in response["data"]
             and len(response["data"]["infos"]) != 0
         ):
 
             self.__update_direct_connections(response["data"]["infos"])
 
-    def __update_direct_connections(self, direct_info: dict) -> None:
+    def __update_direct_connections(self, direct_info: list) -> None:
         """Update the direct_connection info while keeping the correct order.
 
         :param direct_info: Information about direct connections
         :type direct_info: dict
         """
 
         tmp = []
@@ -74,15 +74,15 @@
 
     def action(
         self,
         path: str,
         params: List = [],
         http_action: str = "POST",
         binary: bool = False,
-    ) -> None:
+    ) -> Optional[dict]:
         """Execute any action for the device using the params.
 
         All the information about the parameters and their default values,
         types, etc. can be found in the API specification for MyJDownloader
         (https://my.jdownloader.org/developers/).
 
         :param path: The URL of the endpoint (excluding the base url)
@@ -109,15 +109,15 @@
 
             # No direct connection available, use the MyJD API
             response = self.device.connector.request_api(
                 path, http_action, params, action_url, binary=binary
             )
 
             if response is None:
-                return False
+                return None
             else:
                 if (
                     self.__direct_connection_enabled
                     and time.time() >= self.__direct_connection_cooldown
                 ):
                     self.__refresh_direct_connections()
 
@@ -152,25 +152,25 @@
 
                         # Don't try this connection for a minute.
                         conn["cooldown"] = time.time() + 60
 
             # None of the direct connections worked, set a cooldown for all
             # direct connections
             self.__direct_connection_consecutive_failures += 1
-            self.__direct_connection_cooldown = time.time() + (
-                60 * self.__direct_connection_consecutive_failures
+            self.__direct_connection_cooldown = int(
+                time.time() + (60 * self.__direct_connection_consecutive_failures)
             )
 
             # Use the MyJD API instead
             response = self.device.connector.request_api(
                 path, http_action, params, action_url, binary=binary
             )
 
             if response is None:
-                return False
+                return None
 
             self.__refresh_direct_connections()
 
             return response["data"]
 
     def __action_url(self) -> str:
         """Generate the action url for the device and session."""
```

### Comparing `pyjd-1.0.3/pyjd/myjd_connector.py` & `pyjd-1.0.4/pyjd/myjd_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .jd_device import JDDevice
 from .myjd_connection_helper import MyJDConnectionHelper
 from Crypto.Cipher import AES
-from typing import Any, Dict, List
+from typing import Optional, Any, Dict, List
 from urllib.parse import quote
 import base64
 import hashlib
 import hmac
 import json
 import requests
 import time
@@ -13,29 +13,29 @@
 BS = 16
 
 
 def PAD(s: bytes) -> bytes:
     """Pad a string
 
     :param s: String to pad
-    :type s: str
+    :type s: bytes
     :return: Padded ``s``.
-    :rtype: str
+    :rtype: bytes
     """
 
     return s + ((BS - len(s) % BS) * chr(BS - len(s) % BS)).encode()
 
 
 def UNPAD(s: bytes) -> bytes:
     """Unpad a string.
 
     :param s: String to unpad
-    :type s: str
+    :type s: bytes
     :return: Unpadded ``s``.
-    :rtype: str
+    :rtype: bytes
     """
 
     return s[0 : -s[-1]]
 
 
 class MyJDConnector:
     """Main class for connecting to the MyJD API."""
@@ -43,26 +43,26 @@
     def __init__(self) -> None:
         """Initialize MyJD connector."""
 
         self.__request_id = int(time.time() * 1000)
         self.__api_url = "https://api.jdownloader.org"
         self.__app_key = "https://pglaum.srht.site/pyjd-api"
         self.__api_version = 1
-        self.__devices = None
+        self.__devices: List[dict] = []
 
-        self.__login_secret = None
-        self.__device_secret = None
-        self.__session_token = None
+        self.__login_secret: Optional[bytes] = None
+        self.__device_secret: Optional[bytes] = None
+        self.__session_token: Optional[str] = None
         self.__regain_token = None
-        self.__server_encryption_token = None
-        self.__device_encryption_token = None
+        self.__server_encryption_token: Optional[bytes] = None
+        self.__device_encryption_token: Optional[bytes] = None
 
         self.__connected = False
 
-    def get_session_token(self) -> str:
+    def get_session_token(self) -> Optional[str]:
         """Get the session token
 
         :return: Returns ``self.__session_token``.
         :rtype: str
         """
 
         return self.__session_token
@@ -115,36 +115,46 @@
         ``device_encryption_token``.
         """
 
         if self.__server_encryption_token is None:
             old_token = self.__login_secret
         else:
             old_token = self.__server_encryption_token
+
+        if not old_token:
+            raise Exception("No old token available")
+
+        if not self.__session_token:
+            raise Exception("No session token available")
+
+        if not self.__device_secret:
+            raise Exception("No device secret available")
+
         new_token = hashlib.sha256()
         new_token.update(old_token + bytearray.fromhex(self.__session_token))
         self.__server_encryption_token = new_token.digest()
         new_token = hashlib.sha256()
         new_token.update(self.__device_secret + bytearray.fromhex(self.__session_token))
         self.__device_encryption_token = new_token.digest()
 
-    def __create_signature(self, key: str, data: str) -> bytes:
+    def __create_signature(self, key: bytes, data: str) -> str:
         """Calculate the signature for the data, given a key.
 
         :param key: Key for the signature
         :type key: str
         :param data: Data to sign
         :type data: str
         :return: The SHA256 signature
         :rtype: bytes
         """
 
         signature = hmac.new(key, data.encode("utf-8"), hashlib.sha256)
         return signature.hexdigest()
 
-    def __decrypt(self, secret_token: str, data: str) -> str:
+    def __decrypt(self, secret_token: bytes, data: str) -> bytes:
         """Decrypt data from the server using the provided token.
 
         :param secret_token: Token for the server
         :type secret_token: str
         :param data: The data to decrypt
         :type data: str
         :returns: Decrypted data
@@ -155,26 +165,26 @@
         key = secret_token[len(secret_token) // 2 :]
         decryptor = AES.new(key, AES.MODE_CBC, init_vector)
 
         decrypted_data = UNPAD(decryptor.decrypt(base64.b64decode(data)))
 
         return decrypted_data
 
-    def __encrypt(self, secret_token: str, data: str) -> str:
+    def __encrypt(self, secret_token: bytes, data: bytes) -> str:
         """Encrypt data for the server using the provided token.
 
         :param secret_token: Token for the server
         :type secret_token: str
         :param data: The data to decrypt
         :type data: str
         :returns: Decrypted data
         :rtype: str
         """
 
-        data = PAD(data.encode("utf-8"))
+        data = PAD(data)
         init_vector = secret_token[: len(secret_token) // 2]
         key = secret_token[len(secret_token) // 2 :]
         encryptor = AES.new(key, AES.MODE_CBC, init_vector)
         encrypted_data = base64.b64encode(encryptor.encrypt(data))
 
         return encrypted_data.decode("utf-8")
 
@@ -200,15 +210,15 @@
         self.update_request_id()
         self.__login_secret = None
         self.__device_secret = None
         self.__session_token = None
         self.__regain_token = None
         self.__server_encryption_token = None
         self.__device_encryption_token = None
-        self.__devices = None
+        self.__devices = []
         self.__connected = False
 
         self.__login_secret = self.__create_secret(email, password, "server")
         self.__device_secret = self.__create_secret(email, password, "device")
         response = self.request_api(
             "/my/connect", "GET", [("email", email), ("appkey", self.__app_key)]
         )
@@ -256,15 +266,15 @@
         self.update_request_id()
         self.__login_secret = None
         self.__device_secret = None
         self.__session_token = None
         self.__regain_token = None
         self.__server_encryption_token = None
         self.__device_encryption_token = None
-        self.__devices = None
+        self.__devices = []
         self.__connected = False
 
         return response
 
     def update_devices(self) -> bool:
         """Update available devices.
 
@@ -300,15 +310,17 @@
 
         :returns: List of devices
         :rtype: list[dict]
         """
 
         return self.__devices
 
-    def get_device(self, device_name: str = None, device_id: str = None) -> JDDevice:
+    def get_device(
+        self, device_name: Optional[str] = None, device_id: Optional[str] = None
+    ) -> JDDevice:
         """Get a JDDevice instance for a device
 
         Will search for ``device_id`` first and then for ``device_name``.
 
         :param device_name: Name of the device
         :type device_name: str
         :param device_id: ID of the device
@@ -332,17 +344,17 @@
 
         raise (Exception("Device not found\n"))
 
     def request_api(
         self,
         path: str,
         http_method: str = "GET",
-        params: Any = None,
-        action: str = None,
-        api: str = None,
+        params: Optional[Any] = None,
+        action: Optional[str] = None,
+        api: Optional[str] = None,
         binary: bool = False,
     ) -> Any:
         """Make a request to the MyJD API.
 
         The request goes to ``path``, using the ``http_method`` with the
         parameters ``params``.
 
@@ -367,28 +379,32 @@
         :rtype: Any
         """
 
         if not api:
             api = self.__api_url
 
         data = None
+        query = None
         if not self.is_connected() and path != "/my/connect":
             raise (Exception("No connection established\n"))
 
         if http_method == "GET":
             query = [path + "?"]
             if params is not None:
                 for param in params:
                     if param[0] != "encryptedLoginSecret":
                         query += ["%s=%s" % (param[0], quote(param[1]))]
                     else:
                         query += ["&%s=%s" % (param[0], param[1])]
             query += ["rid=" + str(self.__request_id)]
 
             if self.__server_encryption_token is None:
+                if not self.__login_secret:
+                    raise Exception("No login secret\n")
+
                 query += [
                     "signature="
                     + str(
                         self.__create_signature(
                             self.__login_secret, query[0] + "&".join(query[1:])
                         )
                     )
@@ -401,37 +417,41 @@
                         self.__create_signature(
                             self.__server_encryption_token,
                             query[0] + "&".join(query[1:]),
                         )
                     )
                 ]
 
-            query = query[0] + "&".join(query[1:])
-            encrypted_response = requests.get(api + query, timeout=3)
+            s_query = query[0] + "&".join(query[1:])
+            encrypted_response = requests.get(api + s_query, timeout=3)
         else:
-            params_request = []
+            params_list: List[Any] = []
             if params is not None:
                 for param in params:
                     if not isinstance(param, list):
-                        params_request += [json.dumps(param)]
+                        params_list += [json.dumps(param)]
                     else:
-                        params_request += [param]
+                        params_list += [param]
 
             params_request = {
                 "apiVer": self.__api_version,
                 "url": path,
-                "params": params_request,
+                "params": params_list,
                 "rid": self.__request_id,
             }
 
             data = json.dumps(params_request)
             # Removing quotes around null elements.
             data = data.replace('"null"', "null")
             data = data.replace("'null'", "null")
-            encrypted_data = self.__encrypt(self.__device_encryption_token, data)
+            b_data = data.encode("utf-8")
+            if not self.__device_encryption_token:
+                raise Exception("No device encryption token\n")
+
+            encrypted_data = self.__encrypt(self.__device_encryption_token, b_data)
 
             if action is not None:
                 request_url = api + action + path
             else:
                 request_url = api + path
 
             try:
@@ -446,14 +466,17 @@
                 return None
 
         if encrypted_response.status_code != 200:
             try:
                 error_msg = json.loads(encrypted_response.text)
             except json.JSONDecodeError:
                 try:
+                    if not self.__device_encryption_token:
+                        raise Exception("No device encryption token\n")
+
                     error_msg = json.loads(
                         self.__decrypt(
                             self.__device_encryption_token, encrypted_response.text
                         )
                     )
                 except json.JSONDecodeError:
                     raise Exception(
@@ -466,15 +489,15 @@
                 + "\n\tTYPE: "
                 + error_msg["type"]
                 + "\n------\nREQUEST_URL: "
                 + api
                 + path
             )
 
-            if http_method == "GET":
+            if http_method == "GET" and query:
                 msg += query
 
             msg += "\n"
             if data is not None:
                 msg += "DATA:\n" + data
 
             raise (Exception(msg))
@@ -484,21 +507,27 @@
             self.update_request_id()
 
             # Binary content is not encrypted
             return encrypted_response.content
 
         if action is None:
             if not self.__server_encryption_token:
+                if not self.__login_secret:
+                    raise Exception("No login secret\n")
+
                 response = self.__decrypt(self.__login_secret, encrypted_response.text)
             else:
                 response = self.__decrypt(
                     self.__server_encryption_token, encrypted_response.text
                 )
 
         else:
+            if not self.__device_encryption_token:
+                raise Exception("No device encryption token\n")
+
             response = self.__decrypt(
                 self.__device_encryption_token, encrypted_response.text
             )
 
         jsondata = json.loads(response.decode("utf-8"))
         if jsondata["rid"] != self.__request_id:
             self.update_request_id()
```

### Comparing `pyjd-1.0.3/pyjd/plugins.py` & `pyjd-1.0.4/pyjd/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .jd_types import AdvancedConfigQuery, AdvancedConfigAPIEntry, Plugin, PluginsQuery
-from typing import Any
+from typing import Optional, Any
 
 
 class Plugins:
     def __init__(self, device):
         self.device = device
         self.endpoint = "plugins"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def get(self, interface_name, display_name, key):
         """Get a plugin."""
 
         params = [interface_name, display_name, key]
```

### Comparing `pyjd-1.0.3/pyjd/system.py` & `pyjd-1.0.4/pyjd/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Any, TYPE_CHECKING
+from typing import Optional, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class System:
     def __init__(self, device: "JDDevice") -> None:
         self.device = device
         self.endpoint = "system"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def exit_jd(self) -> str:
         """Stop the JDownloader."""
 
         resp = self.action("/exitJD")
         return resp
 
-    def get_storage_infos(self, path: str = None) -> dict:
+    def get_storage_infos(self, path: Optional[str] = None) -> dict:
         """Get storage information."""
 
         params = [path]
         resp = self.action("/getStorageInfos", params)
         return resp
 
     def get_system_infos(self) -> dict:
```

### Comparing `pyjd-1.0.3/pyjd/toolbar.py` & `pyjd-1.0.4/pyjd/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .jd_types import LinkCheckResult
-from typing import Any
+from typing import Optional, Any
 
 
 class Toolbar:
     def __init__(self, device):
         self.device = device
         self.endpoint = "toolbar"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def add_links_from_dom(self):
         """Unknown."""
 
         resp = self.action("/addLinksFromDOM")
```

### Comparing `pyjd-1.0.3/pyjd/ui.py` & `pyjd-1.0.4/pyjd/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .jd_types import Context, MenuStructure
-from typing import Any, List, TYPE_CHECKING
+from typing import Optional, Any, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class UI:
     def __init__(self, device: "JDDevice") -> None:
         self.device = device
         self.endpoint = "ui"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def get_menu(self, context: Context) -> MenuStructure:
         """Get the custom menu structure for the desired context."""
 
         params = [context.value]
```

### Comparing `pyjd-1.0.3/pyjd/update.py` & `pyjd-1.0.4/pyjd/update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, TYPE_CHECKING
+from typing import Optional, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .jd_device import JDDevice
 
 
 class Update:
     def __init__(self, device: "JDDevice") -> None:
         self.device = device
         self.endpoint = "update"
 
-    def action(self, route: str, params: Any = None) -> Any:
+    def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def is_update_available(self) -> str:
         """Returns if an update is available."""
 
         resp = self.action("/isUpdateAvailable")
```

### Comparing `pyjd-1.0.3/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.4/pyjd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,26 @@
 
 # pyjd
 
 This is a wrapper for the JDownloader API.
 
 ## Installation
 
-Run `pip install .` in the repository folder.
+```shell
+pip install pyjd
+```
 
 ## Usage
 
 The documentation of the JDownloader API can be found here
 <https://my.jdownloader.org/developers/>. This library includes all of the
 documented functions (but uses underscores instead of CamelCase).
 
 For examples, check out the sample scripts in the repository
-([see here](https://git.sr.ht/~pglaum/pyjd/tree/master/item/examples)).
+([see here](https://github.com/pglaum/pyjd/tree/master/examples)).
 
 ## Building auto-docs
 
 ### Build
 
 Go to into the `docs` directory and run `make html`.
```

### Comparing `pyjd-1.0.3/pyjd.egg-info/SOURCES.txt` & `pyjd-1.0.4/pyjd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.3/setup.py` & `pyjd-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0.3",
+    version="1.0.4",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
-    install_required=["requests", "pydantic", "pycryptodome"],
+    install_required=["requests", "pydantic===1.10.10", "pycryptodome"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
```

