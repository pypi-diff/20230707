# Comparing `tmp/hspylib-cfman-0.9.98.tar.gz` & `tmp/hspylib-cfman-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.98.tar", last modified: Fri Jul  7 03:27:28 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.99.tar", last modified: Fri Jul  7 17:28:55 2023, max compression
```

## Comparing `hspylib-cfman-0.9.98.tar` & `hspylib-cfman-0.9.99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.398333 hspylib-cfman-0.9.98/
--rw-r--r--   0 hugo       (503) staff       (20)       49 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.98/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 03:27:28.397602 hspylib-cfman-0.9.98/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      677 2023-07-07 03:27:27.000000 hspylib-cfman-0.9.98/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.391098 hspylib-cfman-0.9.98/cfman/
--rw-r--r--   0 hugo       (503) staff       (20)        7 2023-07-07 03:27:27.000000 hspylib-cfman-0.9.98/cfman/.version
--rw-r--r--   0 hugo       (503) staff       (20)      783 2023-07-07 02:18:47.000000 hspylib-cfman-0.9.98/cfman/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3471 2023-07-04 00:05:40.000000 hspylib-cfman-0.9.98/cfman/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.393334 hspylib-cfman-0.9.98/cfman/core/
--rw-r--r--   0 hugo       (503) staff       (20)      238 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     7707 2023-07-07 03:26:59.000000 hspylib-cfman-0.9.98/cfman/core/cf.py
--rw-r--r--   0 hugo       (503) staff       (20)     2937 2023-07-07 03:25:43.000000 hspylib-cfman-0.9.98/cfman/core/cf_application.py
--rw-r--r--   0 hugo       (503) staff       (20)     5570 2023-07-07 03:24:42.000000 hspylib-cfman-0.9.98/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hugo       (503) staff       (20)     1234 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/cfman/core/cf_endpoint.py
--rw-r--r--   0 hugo       (503) staff       (20)    16985 2023-07-07 03:10:40.000000 hspylib-cfman-0.9.98/cfman/core/cf_manager.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.394079 hspylib-cfman-0.9.98/cfman/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      845 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/cfman/exception/exceptions.py
--rw-r--r--   0 hugo       (503) staff       (20)      204 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.98/cfman/welcome.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.396630 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      520 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)       28 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)        6 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2023-07-07 03:27:28.398479 hspylib-cfman-0.9.98/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     1934 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 17:28:55.446386 hspylib-cfman-0.9.99/
+-rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.99/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-07 17:28:55.445071 hspylib-cfman-0.9.99/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-07 17:28:54.000000 hspylib-cfman-0.9.99/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 17:28:55.410608 hspylib-cfman-0.9.99/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-07 17:28:54.000000 hspylib-cfman-0.9.99/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      783 2023-07-07 16:00:13.000000 hspylib-cfman-0.9.99/cfman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-07 17:28:54.000000 hspylib-cfman-0.9.99/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.99/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 17:28:55.426695 hspylib-cfman-0.9.99/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-07 17:28:54.000000 hspylib-cfman-0.9.99/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7674 2023-07-07 16:14:22.000000 hspylib-cfman-0.9.99/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2935 2023-07-07 17:00:07.000000 hspylib-cfman-0.9.99/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5829 2023-07-07 16:58:24.000000 hspylib-cfman-0.9.99/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.99/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    16925 2023-07-07 17:00:07.000000 hspylib-cfman-0.9.99/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 17:28:55.433077 hspylib-cfman-0.9.99/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-07 17:28:54.000000 hspylib-cfman-0.9.99/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.99/cfman/exception/exceptions.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.99/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 17:28:55.443197 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-07 17:28:55.000000 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-07 17:28:55.000000 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-07 17:28:55.000000 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-07 17:28:55.000000 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-07 17:28:55.000000 hspylib-cfman-0.9.99/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-07 17:28:55.446583 hspylib-cfman-0.9.99/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.99/setup.py
```

### Comparing `hspylib-cfman-0.9.98/PKG-INFO` & `hspylib-cfman-0.9.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.98
+Version: 0.9.99
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.98/cfman/__classpath__.py` & `hspylib-cfman-0.9.99/cfman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.98/cfman/__main__.py` & `hspylib-cfman-0.9.99/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.98/cfman/core/cf.py` & `hspylib-cfman-0.9.99/cfman/core/cf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,16 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-from collections import namedtuple
-
 from clitt.core.term.terminal import Terminal
+from collections import namedtuple
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.modules.application.exit_status import ExitStatus
 from typing import List, Optional
 
 import os
 
 CFTarget = namedtuple("CFTarget", ["user", "org", "space", "connected"])
@@ -104,17 +103,15 @@
             if org:
                 target_params.append("-o")
                 target_params.append(kwargs["org"])
             if space:
                 target_params.append("-s")
                 target_params.append(kwargs["space"])
             Terminal.echo(
-                f"%BLUE%Targeting"
-                f"{'  ORG=' + org if org else ''}"
-                f"{'  SPACE=' + space if space else ''}" "..."
+                f"%BLUE%Targeting" f"{'  ORG=' + org if org else ''}" f"{'  SPACE=' + space if space else ''}" "..."
             )
             self._target = CFTarget(
                 kwargs["user"] if "user" in kwargs else None,
                 kwargs["org"] if "org" in kwargs else None,
                 kwargs["space"] if "space" in kwargs else None,
                 self._check_result(self._exec(" ".join(target_params))) is not None,
             )
```

### Comparing `hspylib-cfman-0.9.98/cfman/core/cf_application.py` & `hspylib-cfman-0.9.99/cfman/core/cf_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def of(cls, app_line: str):
         """Create a cf application entry from the cf apps output line."""
         parts = re.split(r" {2,}", app_line)
         # format: name | state | instances | memory | disk | urls
         if len(parts) == 6:  # Old CF command output
             return CFApplication(parts[0], parts[1], parts[2], parts[3], parts[4], parts[5].split(", "))
         # format: name | requested state | processes | routes
-        elif len(parts) == 4:  # New CF command output
+        if len(parts) == 4:  # New CF command output
             if not (mat := re.search(r"(\w+):(\d+/\d+)", parts[2])):
                 raise InvalidArgumentError(f'Invalid application line: "{app_line}"')
             instances = mat.group(2)
             memory = disk = "-"
             return CFApplication(parts[0], parts[1], instances, memory, disk, parts[3].split(","))
 
         raise InvalidArgumentError(
```

### Comparing `hspylib-cfman-0.9.98/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.99/cfman/core/cf_blue_green_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
+import re
+from typing import Dict, List, Tuple
+
 from clitt.core.term.terminal import Terminal
 
 from cfman.core.cf_application import CFApplication
-from typing import Dict, List
-
-import re
 
 
 class CFBlueGreenChecker:
     """Blue/Green deployment checker."""
 
     @staticmethod
     def _is_green(cf_application: CFApplication) -> bool:
@@ -94,30 +94,18 @@
             f"{'-=' * 60 + '%EOL%'}"
             f"{'Color':^11}{'Status':<10}{'Instances (MEM)':<27}Routes:{'Alerts':>13}%EOL%"
         )
         for name, app in mapped_apps.items():
             app_green = app["green"]
             app_blue = app["blue"]
             Terminal.echo(f"%CYAN%\\-{name}")
-            Terminal.echo(
-                "{} |-GREEN: {}".format(
-                    "%YELLOW%"
-                    if app_green is None or app_blue is None or len(app_green.routes) > len(app_blue.routes)
-                    else "%NC%",
-                    cls._app_info(app_green, app_blue) if app_green else "%RED%Missing green pair!",
-                )
-            )
-            Terminal.echo(
-                "{} |-BLUE : {}".format(
-                    "%YELLOW%"
-                    if app_green is None or app_blue is None or len(app_blue.routes) > len(app_green.routes)
-                    else "%NC%",
-                    cls._app_info(app_blue, app_green) if app_blue else "%RED%Missing blue pair!",
-                )
-            )
+            color, info = cls._match_green(app_green, app_blue)
+            Terminal.echo(f"{color} |-GREEN: {info}")
+            color, info = cls._match_blue(app_blue, app_green)
+            Terminal.echo(f"{color} |-BLUE : {info}")
             Terminal.echo("%NC%%EOL%" + "-" * 120)
 
     @classmethod
     def _app_info(cls, active_app: CFApplication, idle_app: CFApplication) -> str:
         """
         :param active_app: the active cf application.
         :param idle_app: the inactive cf application.
@@ -131,7 +119,25 @@
         app_routes = len(active_app.routes)
 
         return (
             f"{active_app.colored_state:<16}  "
             f"{active_app.instances + f' ({active_app.memory})':<25}  "
             f"ROUTES: ({app_routes}) {alerts_str:^2}"
         )
+
+    @classmethod
+    def _match_green(cls, app_green: CFApplication, app_blue: CFApplication) -> Tuple[str, str]:
+        return (
+            "%YELLOW%"
+            if app_green is None or app_blue is None or len(app_green.routes) > len(app_blue.routes)
+            else "%NC%",
+            cls._app_info(app_green, app_blue) if app_green else "%RED%Missing green pair!"
+        )
+
+    @classmethod
+    def _match_blue(cls, app_blue: CFApplication, app_green: CFApplication) -> Tuple[str, str]:
+        return (
+            "%YELLOW%"
+            if app_green is None or app_blue is None or len(app_blue.routes) > len(app_green.routes)
+            else "%NC%",
+            cls._app_info(app_blue, app_green) if app_blue else "%RED%Missing blue pair!"
+        )
```

### Comparing `hspylib-cfman-0.9.98/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.99/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.98/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.99/cfman/core/cf_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,22 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-from clitt.core.term.cursor import Cursor
-from clitt.core.term.screen import Screen
-from clitt.core.term.terminal import Terminal
-
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
 from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
+from clitt.core.term.cursor import Cursor
+from clitt.core.term.screen import Screen
+from clitt.core.term.terminal import Terminal
 from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.minput.minput import MenuInput, minput
 from clitt.core.tui.mselect.mselect import mselect
 from functools import partial
 from hspylib.core.enums.http_code import HttpCode
 from hspylib.core.preconditions import check_state
 from hspylib.modules.cache.ttl_cache import TTLCache
@@ -81,23 +80,15 @@
             case "start":
                 return "stopped"
             case "logs" | "stop" | "restart":
                 return "started"
             case _:
                 return "started", "stopped"
 
-    def __init__(
-        self, api: str,
-        org: str,
-        space: str,
-        username: str,
-        password: str,
-        no_cache: str,
-        cf_endpoints: str):
-
+    def __init__(self, api: str, org: str, space: str, username: str, password: str, no_cache: str, cf_endpoints: str):
         self._terminal = Terminal.INSTANCE
         self._cf = CloudFoundry.INSTANCE or CloudFoundry()
         self._cache = TTLCache()
         self._api = api
         self._org = org
         self._space = space
         self._username = username
@@ -393,15 +384,15 @@
             list(map(CFApplication.print_status, apps))
             self.writeln("-=" * 60 + "%EOL%")
 
     def _blue_green_check(self) -> None:
         """Display all PCF space-application blue/green check."""
         if len(self.apps) > 0:
             self.screen.clear()
-            self.writeln(f"%BLUE%Checking blue/green deployments ...%EOL%")
+            self.writeln("%BLUE%Checking blue/green deployments ...%EOL%")
             CFBlueGreenChecker.check(self._org, self._space, self.apps)
 
     def _perform_callable(self, action: str) -> None:
         """Wrapper of the _perform method.
         :param action the action to perform.
         """
         act = action.lower()
```

### Comparing `hspylib-cfman-0.9.98/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.99/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.98/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.99/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.98
+Version: 0.9.99
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.99/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.98/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.99/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.98/setup.py` & `hspylib-cfman-0.9.99/setup.py`

 * *Files identical despite different names*

