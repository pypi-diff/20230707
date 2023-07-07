# Comparing `tmp/metadata_inspector-2023.7.6.tar.gz` & `tmp/metadata_inspector-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata_inspector-2023.7.6.tar", last modified: Thu Jul  6 12:08:50 2023, max compression
+gzip compressed data, was "metadata_inspector-2023.7.7.tar", last modified: Fri Jul  7 08:13:22 2023, max compression
```

## Comparing `metadata_inspector-2023.7.6.tar` & `metadata_inspector-2023.7.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1516 2022-10-05 16:26:44.000000 metadata_inspector-2023.7.6/LICENSE
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1304 2022-10-12 08:55:23.000000 metadata_inspector-2023.7.6/README.md
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       38 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/setup.cfg
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2673 2023-07-05 07:58:41.000000 metadata_inspector-2023.7.6/setup.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/metadata_inspector/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7735 2023-07-06 09:23:24.000000 metadata_inspector-2023.7.6/src/metadata_inspector/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6041 2023-07-06 09:23:24.000000 metadata_inspector-2023.7.6/src/metadata_inspector/_slk.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       58 2023-07-06 09:23:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector/_version.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      405 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       62 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/entry_points.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      240 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/requires.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       19 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:13:22.202906 metadata_inspector-2023.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-07 08:13:22.202906 metadata_inspector-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:13:22.202906 metadata_inspector-2023.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:13:22.198906 metadata_inspector-2023.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:13:22.202906 metadata_inspector-2023.7.7/src/metadata_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/src/metadata_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/src/metadata_inspector/_slk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 08:13:10.000000 metadata_inspector-2023.7.7/src/metadata_inspector/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:13:22.202906 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 08:13:22.000000 metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/top_level.txt
```

### Comparing `metadata_inspector-2023.7.6/LICENSE` & `metadata_inspector-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.7.6/PKG-INFO` & `metadata_inspector-2023.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata_inspector
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: Inspect metadata of weather/climate datasets
 Home-page: https://github.com/FREVA-CLINT/metadata-inspektor.git
 Author: Martin Bergemann
 Author-email: bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/FREVA-CLINT/metadata-inspektor
```

### Comparing `metadata_inspector-2023.7.6/README.md` & `metadata_inspector-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.7.6/setup.py` & `metadata_inspector-2023.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.7.6/src/metadata_inspector/__init__.py` & `metadata_inspector-2023.7.7/src/metadata_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.7.6/src/metadata_inspector/_slk.py` & `metadata_inspector-2023.7.7/src/metadata_inspector/_slk.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,57 +8,38 @@
 from __future__ import annotations
 import base64
 from datetime import datetime, timedelta
 from getpass import getuser
 import json
 from pathlib import Path
 import os
-import re
 import shutil
 import warnings
-from subprocess import run, PIPE, SubprocessError, CalledProcessError
+from subprocess import run, PIPE, SubprocessError
 
 from hurry.filesize import alternative, size
 import requests
 
-MODULES_CMD_ENV = "MODULES_CMD"
+SLK_HELPERS_BIN = "/sw/spack-levante/slk_helpers-1.9.3-5hmec4/bin"
+SLK_BIN = "/sw/spack-levante/slk-3.3.91-wuylnb/bin/slk"
+JDK_BIN = "/sw/spack-levante/openjdk-17.0.0_35-k5o6dr/bin"
+JAVA_HOME = "/sw/spack-levante/openjdk-17.0.0_35-k5o6dr"
 SLK = "slk"
 
 SESSION_PATH = Path("~").expanduser() / ".slk" / "config.json"
 
 
-def load_module() -> dict[str, str]:
+def get_env() -> dict[str, str]:
     """Load the slk module."""
-    module_path = os.environ.get(
-        MODULES_CMD_ENV, "/usr/share/Modules/libexec/modulecmd.tcl"
-    )
+    env: dict[str, str] = os.environ.copy()
     if shutil.which("slk") is not None:
-        return os.environ.copy()
-    _env: dict[str, str] = {}
-    try:
-        res = (
-            run(
-                [module_path, "python", "load", SLK],
-                check=True,
-                stdout=PIPE,
-                stderr=PIPE,
-            )
-            .stdout.decode()
-            .split("\n")
-        )
-    except (FileNotFoundError, CalledProcessError) as error:
-        warnings.warn(f"Could not load {SLK}: {error}")
-        return _env
-    for line in res:
-        if "=" in line:
-            key, _, value = line.partition("=")
-            new_key = (re.findall(r"\['([^']*)", key.strip()) or [""])[0]
-            if new_key.strip():
-                _env[new_key.strip()] = value.strip().replace("'", "")
-    return _env
+        return env  # pragma: no cover
+    env["PATH"] = f"{SLK_BIN}:{SLK_HELPERS_BIN}:{JDK_BIN}:{env['PATH']}"
+    env["JAVA_HOME"] = JAVA_HOME
+    return env
 
 
 def get_file_size(input_path: str) -> str:
     """Extract the size of an object on the HSM store.
 
     Parameters
     ----------
@@ -67,17 +48,15 @@
 
     Returns
     -------
     str: A string representation of the size of the ojbect
     """
     command = ["slk_helpers", "size", input_path]
     try:
-        res = run(
-            command, env=load_module(), check=True, stdout=PIPE, stderr=PIPE
-        )
+        res = run(command, env=get_env(), check=True, stdout=PIPE, stderr=PIPE)
     except SubprocessError as error:  # pragma: no cover
         warnings.warn(
             f"Error: could not get meta-data: {error}"
         )  # pragma: no cover
         return "unkown"  # pragma: no cover
     try:
         fsize = int(res.stdout.decode().strip())
@@ -97,17 +76,15 @@
 
     Returns
     -------
     str: string representation of the metdata
     """
     command = ["slk_helpers", "metadata", input_path]
     try:
-        res = run(
-            command, env=load_module(), check=True, stdout=PIPE, stderr=PIPE
-        )
+        res = run(command, env=get_env(), check=True, stdout=PIPE, stderr=PIPE)
     except SubprocessError as error:  # pragma: no cover
         warnings.warn(
             f"Error: could not get meta-data: {error}"
         )  # pragma: no cover
         return {}  # pragma: no cover
     # This needs to be done because the output of the command is only nearly
     # yaml. That is the ":" for the first keys are missing:
@@ -143,16 +120,16 @@
     for fmt in ("%a %b %d %H:%M:%S %Z %Y", "%a %b %d %H:%M:%S %Y"):
         try:
             with session_path.open() as f_obj:
                 date = json.load(f_obj).get("expireDate", now.strftime(fmt))
             return datetime.strptime(date, fmt)
         except FileNotFoundError:  # pragma: no cover
             break  # pragma: no cover
-        except ValueError:
-            pass
+        except ValueError:  # pragma: no cover
+            pass  # pragma: no cover
     return now
 
 
 def _login_via_request(passwd: str) -> None:
     data = {
         "data": {
             "attributes": {
@@ -188,8 +165,8 @@
     exp_date = get_expiration_date()
     diff = (exp_date - now).total_seconds()
     if passwd:
         passwd = base64.b64decode(passwd.encode()).decode()
         _login_via_request(passwd)
     elif diff <= 0:
         print("Your session has expired, login to slk")
-        run(["slk", "login"], shell=False, check=True, env=load_module())
+        run(["slk", "login"], shell=False, check=True, env=get_env())
```

### Comparing `metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/PKG-INFO` & `metadata_inspector-2023.7.7/src/metadata_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-inspector
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: Inspect metadata of weather/climate datasets
 Home-page: https://github.com/FREVA-CLINT/metadata-inspektor.git
 Author: Martin Bergemann
 Author-email: bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/FREVA-CLINT/metadata-inspektor
```

