# Comparing `tmp/venture-3.0.0.tar.gz` & `tmp/venture-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venture-3.0.0.tar", max compression
+gzip compressed data, was "venture-3.1.0.tar", max compression
```

## Comparing `venture-3.0.0.tar` & `venture-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      481 2021-09-21 03:23:21.536216 venture-3.0.0/README.md
--rw-r--r--   0        0        0      630 2023-02-10 05:53:29.068140 venture-3.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 05:45:23.880376 venture-3.0.0/venture/__init__.py
--rw-r--r--   0        0        0     3685 2023-02-10 01:57:36.407218 venture-3.0.0/venture/browse.py
--rw-r--r--   0        0        0     2578 2023-02-10 05:52:13.201133 venture-3.0.0/venture/cli.py
--rw-r--r--   0        0        0     2572 2023-02-10 02:28:48.209928 venture-3.0.0/venture/config.py
--rw-r--r--   0        0        0      570 2023-02-10 00:27:00.356725 venture-3.0.0/venture/ext.py
--rw-r--r--   0        0        0    16975 2023-02-10 00:55:37.250475 venture-3.0.0/venture/icons.py
--rw-r--r--   0        0        0      391 2023-02-09 23:52:30.367348 venture-3.0.0/venture/pango.py
--rw-r--r--   0        0        0        0 2023-02-06 05:05:18.612176 venture-3.0.0/venture/py.typed
--rw-r--r--   0        0        0      570 2023-02-10 01:53:26.612618 venture-3.0.0/venture/quicklaunch.py
--rw-r--r--   0        0        0     2625 2023-02-06 05:41:53.216230 venture-3.0.0/venture/util.py
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 venture-3.0.0/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 venture-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      418 2023-07-07 02:14:21.346567 venture-3.1.0/README.md
+-rw-r--r--   0        0        0      631 2023-07-07 02:14:42.059721 venture-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 02:14:21.349900 venture-3.1.0/venture/__init__.py
+-rw-r--r--   0        0        0     3721 2023-07-07 02:14:21.349900 venture-3.1.0/venture/browse.py
+-rw-r--r--   0        0        0     2549 2023-07-07 02:14:21.349900 venture-3.1.0/venture/cli.py
+-rw-r--r--   0        0        0     2607 2023-07-07 02:14:21.349900 venture-3.1.0/venture/config.py
+-rw-r--r--   0        0        0      570 2023-07-07 02:14:21.349900 venture-3.1.0/venture/ext.py
+-rw-r--r--   0        0        0    16975 2023-07-07 02:14:21.349900 venture-3.1.0/venture/icons.py
+-rw-r--r--   0        0        0      391 2023-07-07 02:14:21.349900 venture-3.1.0/venture/pango.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:14:21.349900 venture-3.1.0/venture/py.typed
+-rw-r--r--   0        0        0      570 2023-07-07 02:14:21.349900 venture-3.1.0/venture/quicklaunch.py
+-rw-r--r--   0        0        0     2625 2023-07-07 02:14:21.349900 venture-3.1.0/venture/util.py
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 venture-3.1.0/setup.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 venture-3.1.0/PKG-INFO
```

### Comparing `venture-3.0.0/pyproject.toml` & `venture-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "venture"
-version = "3.0.0"
+version = "3.1.0"
 description = "Rofi / Wofi based project selector"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/venture"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-arc-cli = "8.0.0"
+arc-cli = "^8.0.0"
 ujson = "^4.0.2"
 pydantic = "^1.8.2"
 toml = "^0.10.2"
 xdg = "^5.1.1"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3.1"
```

### Comparing `venture-3.0.0/venture/browse.py` & `venture-3.1.0/venture/browse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as t
 from fnmatch import fnmatch
 import glob
 from typing import TypedDict
 from pathlib import Path
 import functools
```

### Comparing `venture-3.0.0/venture/cli.py` & `venture-3.1.0/venture/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from datetime import datetime
-import pkg_resources
+from importlib import metadata
 import typing as t
 from pathlib import Path
 import arc
 from xdg import xdg_config_home
 
 from venture import browse, ext, quicklaunch
 from venture.config import Config, UiConfig
 
 DEFAULT_CONFIG_FILE = xdg_config_home() / "venture.toml"
 
-arc.configure(version=pkg_resources.get_distribution("venture").version)
+arc.configure(version=metadata.version("venture"))
 
-
-@arc.command("venture")
-def cli():
-    ...
+cli = arc.namespace("venture")
 
 
 @arc.group
 class SharedArgs:
     config_path: Path = arc.Option(
         name="config",
         short="c",
         default=DEFAULT_CONFIG_FILE,
         desc="Path to the config file to load",
     )
 
 
-@cli.subcommand(("browse", "b"))
+@cli.subcommand("browse", "b")
 def browse_command(
     args: SharedArgs,
     ctx: arc.Context,
     profile_name: str = arc.Option(name="profile", short="p", default="default"),
 ) -> None:
     """Launch a particular browse profile"""
     start = datetime.now()
@@ -66,15 +63,15 @@
 
     if ctx.config.environment == "production":
         ext.run_exec(profile.exec, path)
     else:
         print(profile.exec.format(path=path))
 
 
-@cli.subcommand(("quicklaunch", "q"))
+@cli.subcommand("quicklaunch", "q")
 def quicklaunch_command(args: SharedArgs, ctx: arc.Context) -> None:
     config = Config.load(args.config_path)
     ql_config = config.quicklaunch
     mapping = {
         quicklaunch.format_option(config, ql_config, entry): entry
         for entry in ql_config.entries
     }
```

### Comparing `venture-3.0.0/venture/config.py` & `venture-3.1.0/venture/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import os
 from pathlib import Path
 
 from pydantic import BaseModel, ValidationError, validator
 import toml
 import arc
```

### Comparing `venture-3.0.0/venture/ext.py` & `venture-3.1.0/venture/ext.py`

 * *Files identical despite different names*

### Comparing `venture-3.0.0/venture/icons.py` & `venture-3.1.0/venture/icons.py`

 * *Files identical despite different names*

### Comparing `venture-3.0.0/venture/quicklaunch.py` & `venture-3.1.0/venture/quicklaunch.py`

 * *Files identical despite different names*

### Comparing `venture-3.0.0/venture/util.py` & `venture-3.1.0/venture/util.py`

 * *Files identical despite different names*

### Comparing `venture-3.0.0/setup.py` & `venture-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['venture']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['arc-cli==8.0.0',
+['arc-cli>=8.0.0,<9.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'toml>=0.10.2,<0.11.0',
  'ujson>=4.0.2,<5.0.0',
  'xdg>=5.1.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['venture = venture.cli:cli']}
 
 setup_kwargs = {
     'name': 'venture',
-    'version': '3.0.0',
+    'version': '3.1.0',
     'description': 'Rofi / Wofi based project selector',
-    'long_description': '# Venture\n\nA Dmenu / Rofi / Wofi menu to open projects and files in your favorite editor!\n\n\n\n### Dependancies\n- Venture supports three UI providers: dmenu, rofi, and wofi. It is expected that you have the one you intend to use installed.\n\n- Venture uses [Nerdfonts](https://www.nerdfonts.com/) for icons\n\n## Installation\n\n```\n$ pip install venture\n```\n\n## Docs\n[Here](./docs)\n\nNote this may installing into `~/.local/bin` which is not part of the default path on some Linux systems',
+    'long_description': '# Venture\n\nMake finding and opening your files / projects easier with Venture. Checkout the [configuration](docs/configuration.md) page for more information on how to configure Venture\n\n### Dependancies\nVenture uses [Nerdfonts](https://www.nerdfonts.com/) for icons\n\n## Installation\n\n```\n$ pip install venture\n```\n\nNote this may install into `~/.local/bin` which is not part of the default path on some Linux systems\n\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/venture',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `venture-3.0.0/PKG-INFO` & `venture-3.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 Metadata-Version: 2.1
 Name: venture
-Version: 3.0.0
+Version: 3.1.0
 Summary: Rofi / Wofi based project selector
 Home-page: https://github.com/seanrcollings/venture
 License: MIT
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arc-cli (==8.0.0)
+Requires-Dist: arc-cli (>=8.0.0,<9.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: ujson (>=4.0.2,<5.0.0)
 Requires-Dist: xdg (>=5.1.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Venture
 
-A Dmenu / Rofi / Wofi menu to open projects and files in your favorite editor!
-
-
+Make finding and opening your files / projects easier with Venture. Checkout the [configuration](docs/configuration.md) page for more information on how to configure Venture
 
 ### Dependancies
-- Venture supports three UI providers: dmenu, rofi, and wofi. It is expected that you have the one you intend to use installed.
-
-- Venture uses [Nerdfonts](https://www.nerdfonts.com/) for icons
+Venture uses [Nerdfonts](https://www.nerdfonts.com/) for icons
 
 ## Installation
 
 ```
 $ pip install venture
 ```
 
-## Docs
-[Here](./docs)
+Note this may install into `~/.local/bin` which is not part of the default path on some Linux systems
+
 
-Note this may installing into `~/.local/bin` which is not part of the default path on some Linux systems
```

