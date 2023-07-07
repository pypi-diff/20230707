# Comparing `tmp/hspylib-cfman-0.9.97.tar.gz` & `tmp/hspylib-cfman-0.9.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.97.tar", last modified: Fri Jul  7 01:48:25 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.98.tar", last modified: Fri Jul  7 03:27:28 2023, max compression
```

## Comparing `hspylib-cfman-0.9.97.tar` & `hspylib-cfman-0.9.98.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.272868 hspylib-cfman-0.9.97/
--rw-r--r--   0 hugo       (503) staff       (20)       49 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.97/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 01:48:25.272531 hspylib-cfman-0.9.97/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      677 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.267105 hspylib-cfman-0.9.97/cfman/
--rw-r--r--   0 hugo       (503) staff       (20)        7 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/.version
--rw-r--r--   0 hugo       (503) staff       (20)      716 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3471 2023-07-04 00:05:40.000000 hspylib-cfman-0.9.97/cfman/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.269539 hspylib-cfman-0.9.97/cfman/core/
--rw-r--r--   0 hugo       (503) staff       (20)      238 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     7673 2023-07-07 00:12:05.000000 hspylib-cfman-0.9.97/cfman/core/cf.py
--rw-r--r--   0 hugo       (503) staff       (20)     2950 2023-06-07 00:17:15.000000 hspylib-cfman-0.9.97/cfman/core/cf_application.py
--rw-r--r--   0 hugo       (503) staff       (20)     5534 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hugo       (503) staff       (20)     1234 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/core/cf_endpoint.py
--rw-r--r--   0 hugo       (503) staff       (20)    16919 2023-07-07 01:48:06.000000 hspylib-cfman-0.9.97/cfman/core/cf_manager.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.270272 hspylib-cfman-0.9.97/cfman/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      845 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/exception/exceptions.py
--rw-r--r--   0 hugo       (503) staff       (20)      204 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.97/cfman/welcome.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.272032 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)      520 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)       28 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)        6 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2023-07-07 01:48:25.272958 hspylib-cfman-0.9.97/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     1934 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.398333 hspylib-cfman-0.9.98/
+-rw-r--r--   0 hugo       (503) staff       (20)       49 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.98/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 03:27:28.397602 hspylib-cfman-0.9.98/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      677 2023-07-07 03:27:27.000000 hspylib-cfman-0.9.98/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.391098 hspylib-cfman-0.9.98/cfman/
+-rw-r--r--   0 hugo       (503) staff       (20)        7 2023-07-07 03:27:27.000000 hspylib-cfman-0.9.98/cfman/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      783 2023-07-07 02:18:47.000000 hspylib-cfman-0.9.98/cfman/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3471 2023-07-04 00:05:40.000000 hspylib-cfman-0.9.98/cfman/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.393334 hspylib-cfman-0.9.98/cfman/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      238 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7707 2023-07-07 03:26:59.000000 hspylib-cfman-0.9.98/cfman/core/cf.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2937 2023-07-07 03:25:43.000000 hspylib-cfman-0.9.98/cfman/core/cf_application.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5570 2023-07-07 03:24:42.000000 hspylib-cfman-0.9.98/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1234 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hugo       (503) staff       (20)    16985 2023-07-07 03:10:40.000000 hspylib-cfman-0.9.98/cfman/core/cf_manager.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.394079 hspylib-cfman-0.9.98/cfman/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/cfman/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      845 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/cfman/exception/exceptions.py
+-rw-r--r--   0 hugo       (503) staff       (20)      204 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.98/cfman/welcome.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 03:27:28.396630 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      520 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       28 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2023-07-07 03:27:28.000000 hspylib-cfman-0.9.98/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2023-07-07 03:27:28.398479 hspylib-cfman-0.9.98/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     1934 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.98/setup.py
```

### Comparing `hspylib-cfman-0.9.97/PKG-INFO` & `hspylib-cfman-0.9.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.97
+Version: 0.9.98
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
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.97/README.md` & `hspylib-cfman-0.9.98/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.97/cfman/__classpath__.py` & `hspylib-cfman-0.9.98/cfman/__classpath__.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     """TODO"""
 
     def __init__(self):
         super().__init__(get_path(__file__), get_path(run_dir()), (get_path(__file__) / "resources"))
 
 
 # Instantiate the classpath singleton
-_Classpath()
+assert _Classpath().INSTANCE is not None, "Failed to create Classpath instance"
```

### Comparing `hspylib-cfman-0.9.97/cfman/__main__.py` & `hspylib-cfman-0.9.98/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.97/cfman/core/cf.py` & `hspylib-cfman-0.9.98/cfman/core/cf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from collections import namedtuple
 
-from clitt.core.terminal import Terminal
+from clitt.core.term.terminal import Terminal
 from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.tools.commons import sysout
 from hspylib.modules.application.exit_status import ExitStatus
 from typing import List, Optional
 
 import os
 
 CFTarget = namedtuple("CFTarget", ["user", "org", "space", "connected"])
 
@@ -104,15 +103,19 @@
             space = kwargs["space"] if "space" in kwargs else None
             if org:
                 target_params.append("-o")
                 target_params.append(kwargs["org"])
             if space:
                 target_params.append("-s")
                 target_params.append(kwargs["space"])
-            sysout(f"%BLUE%Targeting" f"{'  ORG=' + org if org else ''}" f"{'  SPACE=' + space if space else ''}" "...")
+            Terminal.echo(
+                f"%BLUE%Targeting"
+                f"{'  ORG=' + org if org else ''}"
+                f"{'  SPACE=' + space if space else ''}" "..."
+            )
             self._target = CFTarget(
                 kwargs["user"] if "user" in kwargs else None,
                 kwargs["org"] if "org" in kwargs else None,
                 kwargs["space"] if "space" in kwargs else None,
                 self._check_result(self._exec(" ".join(target_params))) is not None,
             )
 
@@ -195,15 +198,14 @@
         """Execute the CF command.
         :param cmd_line: the cf command line string
         :param poll: whether to poll or execute the command. If poll is set I/O events can be registered for any number
                      of file descriptors and the output will be continuously printed. If [ENTER] is hit, the polling
                      will terminate.
         """
         self._last_output = None
-
         if poll:
-            sysout("%YELLOW%%EOL%Press [ENTER] to exit...%EOL%%NC%")
+            Terminal.echo("%YELLOW%%EOL%Press [ENTER] to exit...%EOL%%NC%")
             Terminal.shell_poll(f"cf {cmd_line}")
         else:
             self._last_output, self._last_exit_code = Terminal.shell_exec(f"cf {cmd_line}")
 
         return self._last_output
```

### Comparing `hspylib-cfman-0.9.97/cfman/core/cf_application.py` & `hspylib-cfman-0.9.98/cfman/core/cf_application.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
+from clitt.core.term.terminal import Terminal
 from clitt.core.tui.tui_preferences import TUIPreferences
 from hspylib.core.exception.exceptions import InvalidArgumentError
-from hspylib.core.tools.commons import sysout
 from typing import List
 
 import re
 
 
 class CFApplication:
     """Represent a PCF application."""
@@ -41,15 +41,15 @@
             return CFApplication(parts[0], parts[1], instances, memory, disk, parts[3].split(","))
 
         raise InvalidArgumentError(
             f"Invalid application line: " f"{app_line}" f"Probably CF APPS command changed the command output."
         )
 
     def __init__(self, name: str, state: str, instances: str, memory: str, disk: str, routes: List[str]) -> None:
-        self.prefs: TUIPreferences = TUIPreferences.INSTANCE or TUIPreferences()
+        self.prefs: TUIPreferences = TUIPreferences.INSTANCE
         self.name = name
         self.state = state
         self.instances = instances
         self.memory = memory
         self.disk = disk
         self.routes = routes
         self.max_name_length = max(self.max_name_length, len(self.name))
@@ -71,11 +71,11 @@
 
     @property
     def is_started(self) -> bool:
         return self.state.lower() == "started"
 
     def print_status(self) -> None:
         """Print the actual application status line."""
-        sysout(
+        Terminal.echo(
             f"%CYAN%{self.name:<{self.max_name_length + 2}}"
             f"{self.colored_state:}  %NC%{self.instances:<12}{self.memory:<6}{self.disk:<6}{len(self.routes)}"
         )
```

### Comparing `hspylib-cfman-0.9.97/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.98/cfman/core/cf_blue_green_checker.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,17 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
+from clitt.core.term.terminal import Terminal
+
 from cfman.core.cf_application import CFApplication
-from hspylib.core.tools.commons import sysout
 from typing import Dict, List
 
 import re
 
 
 class CFBlueGreenChecker:
     """Blue/Green deployment checker."""
@@ -84,40 +85,40 @@
     @classmethod
     def _list_blue_green_pairs(cls, org: str, space: str, mapped_apps: Dict[str, Dict[str, CFApplication]]) -> None:
         """
         List all apps from current cf space, grouped by blue/green envs.
         :param mapped_apps: The dict containing all CF blue and green apps.
         :return: None
         """
-        sysout(
+        Terminal.echo(
             f"%BLUE%Listing '{org}::{space}' applications grouped by blue/green pairs ...%EOL%%WHITE%"
             f"{'-=' * 60 + '%EOL%'}"
             f"{'Color':^11}{'Status':<10}{'Instances (MEM)':<27}Routes:{'Alerts':>13}%EOL%"
         )
         for name, app in mapped_apps.items():
             app_green = app["green"]
             app_blue = app["blue"]
-            sysout(f"%CYAN%\\-{name}")
-            sysout(
+            Terminal.echo(f"%CYAN%\\-{name}")
+            Terminal.echo(
                 "{} |-GREEN: {}".format(
                     "%YELLOW%"
                     if app_green is None or app_blue is None or len(app_green.routes) > len(app_blue.routes)
                     else "%NC%",
                     cls._app_info(app_green, app_blue) if app_green else "%RED%Missing green pair!",
                 )
             )
-            sysout(
+            Terminal.echo(
                 "{} |-BLUE : {}".format(
                     "%YELLOW%"
                     if app_green is None or app_blue is None or len(app_blue.routes) > len(app_green.routes)
                     else "%NC%",
                     cls._app_info(app_blue, app_green) if app_blue else "%RED%Missing blue pair!",
                 )
             )
-            sysout("%NC%%EOL%" + "-" * 120)
+            Terminal.echo("%NC%%EOL%" + "-" * 120)
 
     @classmethod
     def _app_info(cls, active_app: CFApplication, idle_app: CFApplication) -> str:
         """
         :param active_app: the active cf application.
         :param idle_app: the inactive cf application.
         :return: Information about the active_app.
```

### Comparing `hspylib-cfman-0.9.97/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.98/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.97/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.98/cfman/core/cf_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-from clitt.core.terminal import Terminal
-from clitt.core.tty.cursor import Cursor
-from clitt.core.tty.screen import Screen
+from clitt.core.term.cursor import Cursor
+from clitt.core.term.screen import Screen
+from clitt.core.term.terminal import Terminal
 
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
 from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
 from clitt.core.tui.mchoose.mchoose import mchoose
@@ -81,16 +81,24 @@
             case "start":
                 return "stopped"
             case "logs" | "stop" | "restart":
                 return "started"
             case _:
                 return "started", "stopped"
 
-    def __init__(self, api: str, org: str, space: str, username: str, password: str, no_cache: str, cf_endpoints: str):
-        self._screen = Screen.INSTANCE or Screen()
+    def __init__(
+        self, api: str,
+        org: str,
+        space: str,
+        username: str,
+        password: str,
+        no_cache: str,
+        cf_endpoints: str):
+
+        self._terminal = Terminal.INSTANCE
         self._cf = CloudFoundry.INSTANCE or CloudFoundry()
         self._cache = TTLCache()
         self._api = api
         self._org = org
         self._space = space
         self._username = username
         self._password = password
@@ -116,15 +124,15 @@
 
     @property
     def apps(self) -> List[CFApplication]:
         return self._get_apps() or []
 
     @property
     def screen(self) -> Screen:
-        return self._screen
+        return self._terminal.screen
 
     @property
     def cursor(self) -> Cursor:
         return self.screen.cursor
 
     def write(self, obj: Any) -> None:
         """Write the string representation of the object to the screen."""
```

### Comparing `hspylib-cfman-0.9.97/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.98/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.97/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.98/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.97
+Version: 0.9.98
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
-[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.98/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.97/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.98/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.97/setup.py` & `hspylib-cfman-0.9.98/setup.py`

 * *Files identical despite different names*

