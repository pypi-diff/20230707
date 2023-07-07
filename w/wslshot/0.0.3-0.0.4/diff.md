# Comparing `tmp/wslshot-0.0.3.tar.gz` & `tmp/wslshot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslshot-0.0.3.tar", last modified: Fri Jul  7 18:51:25 2023, max compression
+gzip compressed data, was "wslshot-0.0.4.tar", last modified: Fri Jul  7 20:24:04 2023, max compression
```

## Comparing `wslshot-0.0.3.tar` & `wslshot-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.3/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:51:25.766511 wslshot-0.0.3/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6269 2023-07-07 18:35:06.000000 wslshot-0.0.3/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 18:51:25.766511 wslshot-0.0.3/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-07 18:50:11.000000 wslshot-0.0.3/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/wslshot/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.3/wslshot/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15377 2023-07-07 18:50:02.000000 wslshot-0.0.3/wslshot/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/wslshot.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:24:04.006499 wslshot-0.0.4/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.4/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6779 2023-07-07 20:24:04.006499 wslshot-0.0.4/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6339 2023-07-07 20:06:37.000000 wslshot-0.0.4/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 20:24:04.006499 wslshot-0.0.4/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-07 20:23:07.000000 wslshot-0.0.4/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:24:04.006499 wslshot-0.0.4/wslshot/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.4/wslshot/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15561 2023-07-07 20:22:56.000000 wslshot-0.0.4/wslshot/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:24:04.006499 wslshot-0.0.4/wslshot.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6779 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-07 20:24:03.000000 wslshot-0.0.4/wslshot.egg-info/top_level.txt
```

### Comparing `wslshot-0.0.3/LICENSE` & `wslshot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.3/PKG-INFO` & `wslshot-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-Metadata-Version: 2.1
-Name: wslshot
-Version: 0.0.3
-Home-page: https://github.com/sderev/wslshot
-Author: Sébastien De Revière
-License: Apache Licence, Version 2.0
-Project-URL: Documentation, https://github.com/sderev/wslshot
-Project-URL: Issues, http://github.com/sderev/wslshot/issues
-Project-URL: Changelog, https://github.com/sderev/wslshot/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Windows Screenshot for Linux
 
 `wslshot` is a CLI tool that fetches the most recent screenshot(s) from a shared directory with a Windows host, then copies it to a specified directory in a Linux VM.
 
+Simply capture a screenshot using the Windows Snipping tool (`win + shift + S`), and then activate `wslshot` in your terminal to seamlessly transfer the screenshot.
+
+![demo_0](https://github.com/sderev/wslshot/assets/24412384/656b0595-0c27-41fa-966a-d6ca39ec410a)
+
 <!-- TOC -->
 ## Table of Contents
 
 1. [Features](#features)
 1. [Installation](#installation)
     1. [Install with pip](#install-with-pip)
     1. [Install with pipx (recommended)](#install-with-pipx-recommended)
@@ -137,18 +128,26 @@
 * `/assets/images/`
 * `/img/`
 * `/images/`
 
 **You can also choose a specific number of screenshots**:
 
 ```bash
+wslshot -n 3
+```
+
+This will fetch the three most recent screenshots.
+
+**These are all the possible options**:
+
+```bash
 wslshot [--source /custom/source] [--destination /custom/destination] [--count 3] [--output HTML]
 ```
 
-This will fetch the three most recent screenshots from the source directory and copy them to the destination directory. You can specify a custom source or destination directory for this operation. You can also specify the number of recent screenshots to fetch (defaults to 1) and choose the output format for the operation, which overrides the default set in `config`.
+You can access the help message with `wslshot --help`.
 
 ## Integration in Vim
 
 If `wslshot` is in your PATH (this is by default if you installed it with `pipx`), you can easily call it with a shebang command.
 
 ```vim
 :.!wslshot
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wslshot-0.0.3/README.md` & `wslshot-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,28 @@
+Metadata-Version: 2.1
+Name: wslshot
+Version: 0.0.4
+Home-page: https://github.com/sderev/wslshot
+Author: Sébastien De Revière
+License: Apache Licence, Version 2.0
+Project-URL: Documentation, https://github.com/sderev/wslshot
+Project-URL: Issues, http://github.com/sderev/wslshot/issues
+Project-URL: Changelog, https://github.com/sderev/wslshot/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Windows Screenshot for Linux
 
 `wslshot` is a CLI tool that fetches the most recent screenshot(s) from a shared directory with a Windows host, then copies it to a specified directory in a Linux VM.
 
+Simply capture a screenshot using the Windows Snipping tool (`win + shift + S`), and then activate `wslshot` in your terminal to seamlessly transfer the screenshot.
+
+![demo_0](https://github.com/sderev/wslshot/assets/24412384/656b0595-0c27-41fa-966a-d6ca39ec410a)
+
 <!-- TOC -->
 ## Table of Contents
 
 1. [Features](#features)
 1. [Installation](#installation)
     1. [Install with pip](#install-with-pip)
     1. [Install with pipx (recommended)](#install-with-pipx-recommended)
@@ -124,18 +141,26 @@
 * `/assets/images/`
 * `/img/`
 * `/images/`
 
 **You can also choose a specific number of screenshots**:
 
 ```bash
+wslshot -n 3
+```
+
+This will fetch the three most recent screenshots.
+
+**These are all the possible options**:
+
+```bash
 wslshot [--source /custom/source] [--destination /custom/destination] [--count 3] [--output HTML]
 ```
 
-This will fetch the three most recent screenshots from the source directory and copy them to the destination directory. You can specify a custom source or destination directory for this operation. You can also specify the number of recent screenshots to fetch (defaults to 1) and choose the output format for the operation, which overrides the default set in `config`.
+You can access the help message with `wslshot --help`.
 
 ## Integration in Vim
 
 If `wslshot` is in your PATH (this is by default if you installed it with `pipx`), you can easily call it with a shebang command.
 
 ```vim
 :.!wslshot
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wslshot-0.0.3/setup.py` & `wslshot-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

### Comparing `wslshot-0.0.3/wslshot/cli.py` & `wslshot-0.0.4/wslshot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,28 +133,32 @@
     - count: The number of screenshots to fetch.
 
     Returns:
 
     - The screenshot(s)'s path.
     """
     # Get the most recent screenshot(s) from the source directory.
-    screenshots = sorted(
-        Path(source).glob("*.png"), key=os.path.getmtime, reverse=True
-    )[:count]
-
-    if len(screenshots) == 0:
-        click.echo(f"No screenshots found in the source directory: {source}.")
+    try:
+        screenshots = sorted(
+            Path(source).glob("*.png"), key=os.path.getmtime, reverse=True
+        )[:count]
+
+        if len(screenshots) == 0:
+            click.echo(f"No screenshots found in the source directory: {source}.")
+            sys.exit(1)
+
+        if len(screenshots) < count:
+            raise ValueError(
+                f"Only {len(screenshots)} screenshot(s) found in the source directory:"
+                f" {source}."
+            )
+    except ValueError as error:
+        print(f"An error occurred while fetching the screenshot(s):\n{error}")
         sys.exit(1)
 
-    if len(screenshots) < count:
-        raise ValueError(
-            f"Only {len(screenshots)} screenshot(s) found in the source directory:"
-            f" {source}."
-        )
-
     return tuple(screenshots)
 
 
 def copy_screenshots(screenshots: Tuple[Path], destination: str) -> Tuple[Path]:
     """
     Copy the screenshot(s) to the destination directory.
```

### Comparing `wslshot-0.0.3/wslshot.egg-info/PKG-INFO` & `wslshot-0.0.4/wslshot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Windows Screenshot for Linux
 
 `wslshot` is a CLI tool that fetches the most recent screenshot(s) from a shared directory with a Windows host, then copies it to a specified directory in a Linux VM.
 
+Simply capture a screenshot using the Windows Snipping tool (`win + shift + S`), and then activate `wslshot` in your terminal to seamlessly transfer the screenshot.
+
+![demo_0](https://github.com/sderev/wslshot/assets/24412384/656b0595-0c27-41fa-966a-d6ca39ec410a)
+
 <!-- TOC -->
 ## Table of Contents
 
 1. [Features](#features)
 1. [Installation](#installation)
     1. [Install with pip](#install-with-pip)
     1. [Install with pipx (recommended)](#install-with-pipx-recommended)
@@ -137,18 +141,26 @@
 * `/assets/images/`
 * `/img/`
 * `/images/`
 
 **You can also choose a specific number of screenshots**:
 
 ```bash
+wslshot -n 3
+```
+
+This will fetch the three most recent screenshots.
+
+**These are all the possible options**:
+
+```bash
 wslshot [--source /custom/source] [--destination /custom/destination] [--count 3] [--output HTML]
 ```
 
-This will fetch the three most recent screenshots from the source directory and copy them to the destination directory. You can specify a custom source or destination directory for this operation. You can also specify the number of recent screenshots to fetch (defaults to 1) and choose the output format for the operation, which overrides the default set in `config`.
+You can access the help message with `wslshot --help`.
 
 ## Integration in Vim
 
 If `wslshot` is in your PATH (this is by default if you installed it with `pipx`), you can easily call it with a shebang command.
 
 ```vim
 :.!wslshot
```

