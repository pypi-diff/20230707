# Comparing `tmp/unknown-cli-0.6.7.tar.gz` & `tmp/unknown-cli-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknown-cli-0.6.7.tar", last modified: Fri Jul  7 08:17:43 2023, max compression
+gzip compressed data, was "unknown-cli-0.6.8.tar", last modified: Fri Jul  7 12:04:00 2023, max compression
```

## Comparing `unknown-cli-0.6.7.tar` & `unknown-cli-0.6.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.163719 unknown-cli-0.6.7/
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 08:17:43.160706 unknown-cli-0.6.7/PKG-INFO
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       28 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/README.md
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       38 2023-07-07 08:17:43.164736 unknown-cli-0.6.7/setup.cfg
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     2558 2023-07-05 17:48:37.000000 unknown-cli-0.6.7/setup.py
-drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:42.962344 unknown-cli-0.6.7/unknown_cli.egg-info/
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      436 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        1 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       83 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      116 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/requires.txt
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       11 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/top_level.txt
-drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.038427 unknown-cli-0.6.7/unknowncli/
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        5 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknowncli/VERSION
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      390 2023-07-05 17:41:19.000000 unknown-cli-0.6.7/unknowncli/__init__.py
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     1468 2023-07-05 17:41:21.000000 unknown-cli-0.6.7/unknowncli/__main__.py
-drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.111652 unknown-cli-0.6.7/unknowncli/commands/
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/commands/__init__.py
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    11755 2023-07-05 17:41:23.000000 unknown-cli-0.6.7/unknowncli/commands/project.py
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    16722 2023-07-07 08:15:06.000000 unknown-cli-0.6.7/unknowncli/commands/task.py
-drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.137181 unknown-cli-0.6.7/unknowncli/data/
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     3408 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/data/.p4ignore.txt
--rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     8549 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/utils.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 12:04:00.491019 unknown-cli-0.6.8/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 12:04:00.488013 unknown-cli-0.6.8/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       28 2023-07-05 17:33:30.000000 unknown-cli-0.6.8/README.md
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       38 2023-07-07 12:04:00.492518 unknown-cli-0.6.8/setup.cfg
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     2558 2023-07-05 17:48:37.000000 unknown-cli-0.6.8/setup.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 12:04:00.282714 unknown-cli-0.6.8/unknown_cli.egg-info/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknown_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      436 2023-07-07 12:04:00.000000 unknown-cli-0.6.8/unknown_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        1 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknown_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       83 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknown_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      116 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknown_cli.egg-info/requires.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       11 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknown_cli.egg-info/top_level.txt
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 12:04:00.362413 unknown-cli-0.6.8/unknowncli/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        5 2023-07-07 12:03:59.000000 unknown-cli-0.6.8/unknowncli/VERSION
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      391 2023-07-07 09:48:20.000000 unknown-cli-0.6.8/unknowncli/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     1473 2023-07-07 09:48:20.000000 unknown-cli-0.6.8/unknowncli/__main__.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 12:04:00.438305 unknown-cli-0.6.8/unknowncli/commands/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-05 17:33:30.000000 unknown-cli-0.6.8/unknowncli/commands/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    11841 2023-07-07 09:48:20.000000 unknown-cli-0.6.8/unknowncli/commands/project.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    15938 2023-07-07 12:03:44.000000 unknown-cli-0.6.8/unknowncli/commands/task.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 12:04:00.464832 unknown-cli-0.6.8/unknowncli/data/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     3408 2023-07-05 17:33:30.000000 unknown-cli-0.6.8/unknowncli/data/.p4ignore.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     8629 2023-07-07 09:48:20.000000 unknown-cli-0.6.8/unknowncli/utils.py
```

### Comparing `unknown-cli-0.6.7/setup.py` & `unknown-cli-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.6.7/unknowncli/__main__.py` & `unknown-cli-0.6.8/unknowncli/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,32 @@
 base_path = pathlib.Path(os.path.dirname(__file__))
 commands_folder = base_path / "commands"
 
 from typer import Typer, Context, Argument, Option, echo, secho, confirm, prompt
 
 app = Typer(add_completion=False)
 
+
 @app.callback(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
 def cli(
     ctx: Context,
-    #verbose: str = Option(None, "-v", "--verbose", help="Verbose logging: info or debug"),
-    #output: str = Option("text", "-o", "--output", help="Output text or json"),
+    # verbose: str = Option(None, "-v", "--verbose", help="Verbose logging: info or debug"),
+    # output: str = Option("text", "-o", "--output", help="Output text or json"),
 ):
     """
     This tool handles the initial setup of Perforce Projects and helps you work with task streams.
     It creates workspaces for you according to naming conventions and sets up a virtual drive.
     Please run the 'project setup' command to get started.
     """
     # by default we log out to console WARN and higher but can view info with -v
-    #if verbose:
+    # if verbose:
     #    console_handler.setLevel(getattr(logging, verbose.upper()))
     check_version()
 
+
 check_p4config()
 
 
 from unknowncli.commands import project
 from unknowncli.commands import task
 
 app.add_typer(project.app, name="project", help="Manage initial project setup")
```

### Comparing `unknown-cli-0.6.7/unknowncli/commands/project.py` & `unknown-cli-0.6.8/unknowncli/commands/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time 
+import time
 import sys, os
 import requests
 import logging
 import socket
 from tabulate import tabulate
 from pathlib import Path
 from pprint import pprint
@@ -15,59 +15,65 @@
 
 from typer import Context, launch, echo, secho, Option, Typer, confirm, prompt, style, progressbar
 
 app = Typer()
 
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
-STREAMS = {
-    "sn2-main": "//project/sn2-main-ue", 
-    "sandbox" : "//project/sandbox"
-    }
-is_windows = (os.name == 'nt')
+STREAMS = {"sn2-main": "//project/sn2-main-ue", "sandbox": "//project/sandbox"}
+is_windows = os.name == "nt"
 DEFAULT_FOLDER = "C:\Work" if is_windows else "~/Work"
 MIN_FREE_GB = 200
 
+
 def get_clientspecs(p4):
     try:
         specs = p4.run_clients("-u", p4.user)
     except Exception as e:
         abort(str(e))
     ret = {}
     for s in specs:
         host = s["Host"].lower()
         if host == hostname or not host:
             ret[s["Stream"].lower()] = s
     return ret
 
+
 def get_sync_stats(p4, force=False):
     # gah, p4 wrapper just returns text
     if force:
         ret = p4.run_sync("-N", "-f")
     else:
         ret = p4.run_sync("-N")
     lst = ret[0].split("=")
-    ret = {"files": {"added": 0, "updated": 0, "deleted": 0, "total": 0}, "mbytes": {"added": 0, "updated": 0, "total": 0}}
+    ret = {
+        "files": {"added": 0, "updated": 0, "deleted": 0, "total": 0},
+        "mbytes": {"added": 0, "updated": 0, "total": 0},
+    }
     lst2 = [int(l) for l in lst[1].split(",")[0].split("/")]
     ret["files"]["added"] = lst2[0]
     ret["files"]["updated"] = lst2[1]
     ret["files"]["deleted"] = lst2[2]
     ret["files"]["total"] = sum(lst2)
 
     lst2 = [int(l) // 1024 // 1024 for l in lst[-1].split(",")[0].split("/")]
     ret["mbytes"]["added"] = lst2[0]
     ret["mbytes"]["updated"] = lst2[1]
     ret["mbytes"]["total"] = sum(lst2)
 
     return ret
 
+
 @app.command()
-def setup(perforce_path: str = Option(DEFAULT_FOLDER, prompt="Folder to keep your workspace"), force: bool = Option(False, help="Forcefully overwrite an existing setup")):
+def setup(
+    perforce_path: str = Option(DEFAULT_FOLDER, prompt="Folder to keep your workspace"),
+    force: bool = Option(False, help="Forcefully overwrite an existing setup"),
+):
     """
-    Creates the virtual drive and perforce workspaces from 
+    Creates the virtual drive and perforce workspaces from
     //Project/[stream] -> s:/[stream]
 
     Perforce Setup: https://www.notion.so/unknownworlds/How-To-Version-Control-Setup-0fc38f99d29a4558ac32b24bdfc6904f
 
     Unreal Game Sync: https://www.notion.so/unknownworlds/How-To-Setup-Unreal-Game-Sync-59cc3348cdde449d8fdc7f39ee60c8b3
     """
     p4 = P4()
@@ -100,24 +106,27 @@
                 p4.password = passwd
                 p4.run_login()
                 all_client_specs = p4.run_clients("-u", p4.user)
             except Exception as e:
                 abort(str(e))
         else:
             abort(f"Error fetching workspaces from Perforce: {e}")
-    
+
     secho("OK", fg="green")
     if " " in perforce_path:
         abort("Workspace path cannot include spaces (sorry)")
 
     perforce_path = Path(perforce_path).expanduser()
     _, _, free = shutil.disk_usage(perforce_path.drive)
     free_gb = free // 1024 // 1024 // 1024
     if free_gb < MIN_FREE_GB:
-        secho(f"You need to have at least {MIN_FREE_GB} GB free disk space but you have only {free_gb} GB on drive {perforce_path.drive}", fg="yellow")
+        secho(
+            f"You need to have at least {MIN_FREE_GB} GB free disk space but you have only {free_gb} GB on drive {perforce_path.drive}",
+            fg="yellow",
+        )
         y = confirm("Are you sure you want to continue?")
         if not y:
             abort("Aborted")
 
     config_filename = "p4config.txt"
 
     # ignore_path = Path("~").expanduser() / ".p4ignore.txt"
@@ -154,36 +163,39 @@
         s_path = Path(SUBST_DRIVE)
         if s_path.exists():
             s_path_resolve = str(s_path.resolve()).lower()
             if s_path_resolve == str(perforce_path).lower():
                 secho(f"{SUBST_DRIVE} virtual drive is already set up and pointing to {s_path_resolve}.", fg="green")
             elif not force:
                 abort(f"{SUBST_DRIVE} virtual drive is pointing to another folder: {s_path_resolve}.")
-        
+
         if not s_path.exists() or force:
             try:
                 call(f"subst {SUBST_DRIVE} /D")
             except:
                 pass
             check_call(subst_cmd)
 
         import winreg
+
         echo(f"Adding Virtual Drive {SUBST_DRIVE} -> {perforce_path} to startup")
         h = winreg.CreateKey(winreg.HKEY_CURRENT_USER, "Software\Microsoft\Windows\CurrentVersion\Run")
         winreg.SetValueEx(h, "Perforce Work Drive", 0, winreg.REG_SZ, subst_cmd)
         h = winreg.CreateKey(winreg.HKEY_CURRENT_USER, "SOFTWARE\perforce\environment")
         winreg.SetValueEx(h, "P4CONFIG", 0, winreg.REG_SZ, str(config_file))
 
         if not perforce_path.exists():
             abort(f"Failed to add subst for {SUBST_DRIVE}")
         root_path = SUBST_DRIVE
     else:
         root_path = str(perforce_path)
 
-    computer_name = prompt("What would you like to call this computer in Perforce (work, home, laptop, etc)", default="work")
+    computer_name = prompt(
+        "What would you like to call this computer in Perforce (work, home, laptop, etc)", default="work"
+    )
     if not computer_name.isalpha() or computer_name != computer_name.lower():
         abort("Computer name must be lowercase with no symbols")
     for stream_name, stream in STREAMS.items():
         mapping = f"{root_path}/{stream_name}"
         found = False
         for r in all_client_specs:
             root = r["Root"].lower()
@@ -205,26 +217,29 @@
             client = p4.fetch_client(client_spec)
             client["Root"] = mapping
             client["Stream"] = stream
             p4.save_client(client)
             p = Path(mapping)
             p.mkdir(parents=True, exist_ok=True)
 
-    
     secho("\nProject setup has been completed. Please sync your workspaces through p4v", fg="green")
-    secho("Unreal Game Sync documentation: https://www.notion.so/unknownworlds/How-To-Setup-Unreal-Game-Sync-59cc3348cdde449d8fdc7f39ee60c8b3")
-    #sync_workspaces()
+    secho(
+        "Unreal Game Sync documentation: https://www.notion.so/unknownworlds/How-To-Setup-Unreal-Game-Sync-59cc3348cdde449d8fdc7f39ee60c8b3"
+    )
+    # sync_workspaces()
+
 
 @app.command()
 def sync(stream: str = Option(""), force: bool = Option(False)):
     """
     Runs a full Perforce sync of the Project streams. Intented for initial project sync
     """
     sync_workspaces(stream, force)
 
+
 def sync_workspaces(stream="", force=False):
     files_completed = 0
     old_files_completed = 0
     files_remaining = 0
     num_files = 0
 
     p4 = P4()
@@ -259,38 +274,39 @@
     for stream_name, s in STREAMS.items():
         if stream not in s:
             continue
         folder = specs[s.lower()]["Root"]
         echo(f"Syncing {s} -> {folder}...")
         p4.client = specs[s]["client"]
         stats = get_sync_stats(p4, force)
-        num_files = stats['files']['total']
+        num_files = stats["files"]["total"]
         batch_size = 1000
         threads = 8
 
         if force:
             secho(f"Refetching all files in {s} (this will take a while)...")
             ret = p4.run_sync("--parallel", threads, "-f")
-            num_files = get_sync_stats(p4)['files']['total']
+            num_files = get_sync_stats(p4)["files"]["total"]
 
         if num_files > 0:
             echo(f"Syncing {num_files} files...")
             with progressbar(length=num_files, show_pos=True) as progress:
-                for i in range(num_files//batch_size):
+                for i in range(num_files // batch_size):
                     p4.run_sync("-m", batch_size, "--parallel", threads, "-q")
                     progress.update(batch_size)
             p4.run_sync()
-            files_remaining = get_sync_stats(p4)['files']['total']
+            files_remaining = get_sync_stats(p4)["files"]["total"]
             if files_remaining == 0:
                 secho(f"{s} is now up-to-date", fg="green")
             else:
                 abort(f"{s} is not up to date after sync. Please sync manually")
         else:
             secho(f"{s} is already up-to-date", fg="green")
 
+
 @app.command()
 def workspaces():
     """
     Shows a list of your perforce workspaces
     """
     p4 = P4()
     p4.connect()
```

### Comparing `unknown-cli-0.6.7/unknowncli/commands/task.py` & `unknown-cli-0.6.8/unknowncli/commands/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,120 @@
-import random
 import datetime
-import json
-import time 
-import sys, os
-import requests
 import logging
 import socket
-from tabulate import tabulate
-from pathlib import Path
-from pprint import pprint
-from ..utils import dumps, abort, get_datafile
-from subprocess import check_call, call
+from ..utils import abort
 from P4 import P4, P4Exception
-import shutil
 from typing import Optional
+
 log = logging.getLogger(__name__)
 
 from typer import echo, secho, Option, Typer, confirm, prompt
-from rich.progress import track, Progress, SpinnerColumn, MofNCompleteColumn, TimeRemainingColumn, TimeElapsedColumn, BarColumn
+from rich.progress import Progress, MofNCompleteColumn, TimeRemainingColumn, BarColumn
 
-from multiprocessing import Pool, Manager
-import multiprocessing
-from concurrent.futures import ProcessPoolExecutor
 app = Typer()
 
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
 path = f"{SUBST_DRIVE}\\sn2-main\\"
 BASE_STREAM = "//Project/SN2-Main"
 UE_STREAM = "//project/sn2-main-ue"
 
 p4 = None
 
+
 def connect_p4():
     p4_conn = P4()
     try:
         p4_conn.connect()
     except Exception as e:
         abort(f"Cannot establish connection with Perforce server: {e}...")
     return p4_conn
 
 
 @app.callback()
 def main():
     """
     Manage task streams.
-    
+
     This tool is highly opinionated and expects you to be using the //Project/SN2-Main-UE stream and be working in a workspace called <username>_<label>_sn2-main
     """
     global p4
     p4 = connect_p4()
     ret = get_current_stream()
     ignore_file = (path + ".p4ignore.txt").lower()
     if p4.ignore_file.lower() != ignore_file:
-        abort(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.\nPlease change the setting in your {p4.env('P4CONFIG')} file")
-    
+        abort(
+            f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.\nPlease change the setting in your {p4.env('P4CONFIG')} file"
+        )
+
     if "Stream" not in ret:
         abort("Invalid workspace. You must be working in Streams to use this tool")
     stream_name = ret["Stream"]
     parent = ret["Parent"]
     secho(f"You are currently working in stream: {stream_name}", fg="blue")
     if parent.lower() != UE_STREAM and stream_name.lower() != UE_STREAM:
-        abort(f"To use this tool you must be working in the {UE_STREAM} stream but your workspace is set on {stream_name}. Please change your workspace with 'p4 set'")
+        abort(
+            f"To use this tool you must be working in the {UE_STREAM} stream but your workspace is set on {stream_name}. Please change your workspace with 'p4 set'"
+        )
+
 
 def get_task_streams(owner):
     lst = p4.run_streams("-F", f"Owner={owner} Type=task baseParent={BASE_STREAM}")
     return lst
 
+
 def get_current_stream():
     try:
         ret = p4.run_stream("-o")[0]
     except P4Exception as e:
         client_name = "None"
         try:
             client = get_current_client()
             client_name = client["Client"]
         except:
             pass
-        abort(f"Unable to get a stream from your current workspace, {client_name}. Make sure you are working in the {BASE_STREAM} stream. Error: {e}")
+        abort(
+            f"Unable to get a stream from your current workspace, {client_name}. Make sure you are working in the {BASE_STREAM} stream. Error: {e}"
+        )
     return ret
 
+
 def get_current_client():
     ret = p4.run_client("-o")[0]
     return ret
 
+
 def get_clients():
     try:
         specs = p4.run_clients("-u", p4.user)
     except Exception as e:
         abort(str(e))
     ret = {}
     for s in specs:
         if "Stream" not in s:
             continue
         host = s["Host"].lower()
         if host == hostname or not host:
             ret[s["Stream"].lower()] = s
     return ret
 
+
 def sync():
     s = confirm("Sync latest?")
 
     if not s:
         return
-    
+
     secho(f"Syncing latest...")
     try:
         ret = p4.run_sync("-q", f"{path}UE/Subnautica2/...")
     except P4Exception as e:
         print(e)
 
+
 @app.command()
 def create(label: str = Option(None, prompt="Task branch label")):
     """
     Create a new task branch
     """
     if not label:
         abort("Aborted.")
@@ -125,22 +126,21 @@
     for k, c in clients.items():
         if k == UE_STREAM:
             ue_stream_client = c
     if not ue_stream_client:
         abort(f"You have no workspace mapped to the {UE_STREAM} stream. Please set one up.")
 
     ret = p4.run_opened()
-    if (len(ret)):
+    if len(ret):
         abort("You have opened files. Please revert or submit before creating new task stream.")
 
-
-    #print(ue_stream_client)
-    #task_client_name = ue_stream_client["client"] + "_task"
-    #task_client = None
-    #for k, c in clients.items():
+    # print(ue_stream_client)
+    # task_client_name = ue_stream_client["client"] + "_task"
+    # task_client = None
+    # for k, c in clients.items():
     #    if c["client"] == task_client_name:
     #        echo(f"Reusing existin workspace {k}")
     #        task_client = c
     #        break
     # sync latest from parent
     echo("Syncing parent branch...")
     try:
@@ -165,15 +165,15 @@
 Options:        allsubmit unlocked toparent fromparent mergedown
 ParentView:     inherit
 Paths:
     share ...
 """
     p4.input = args
     ret = p4.run_stream("-i", "-t", "task")
-    #print(ret[0])
+    # print(ret[0])
 
     secho(f"Populating stream {full_stream_name}...")
     try:
         ret = p4.run_populate("-o", "-S", full_stream_name, "-r", "-d", "Initial branch")
     except P4Exception as e:
         if e.errors:
             secho(e.errors[0], fg="yellow")
@@ -191,49 +191,50 @@
         abort(f"Something went wrong. Current stream {stream_name} is not a task stream")
 
     # update the server without syncing
     ret = p4.run_sync("-q", "-k", f"{path}...")
 
     secho(f"You are now working in task stream {stream_name} from parent {parent}", bold=True, fg="green")
 
+
 @app.command()
 def switch():
     """
     Lists your current task streams and lets you switch between them
     """
     stream = get_current_stream()
-    old_stream_name = stream['Stream']
+    old_stream_name = stream["Stream"]
     client = p4.run_client("-o")[0]
     client_owner = client["Owner"]
     task_streams = get_task_streams(client_owner)
     parent = None
     if stream["Type"] == "task":
         parent = stream["Parent"]
     for i, t in enumerate(task_streams):
         secho(f"{i+1} : {t['Stream']}")
     if parent:
         secho(f"0 : {parent}")
-    
+
     if not task_streams:
         abort("You have no task streams. You can create one with the 'create' command")
     n = prompt("\nSelect a stream to work in")
     if n is None:
         abort("No stream selected")
     try:
         n = int(n)
     except:
         abort("Aborted.")
     if n == 0:
         new_stream = parent
     else:
         try:
-            new_stream = task_streams[n-1]["Stream"]
+            new_stream = task_streams[n - 1]["Stream"]
         except:
             abort("Aborted.")
-    
+
     secho(f"\nSwitching to stream {new_stream}", bold=True)
     try:
         p4.run_client("-s", "-S", new_stream)
     except P4Exception as e:
         abort(e)
 
     secho(f"Running sync...")
@@ -248,25 +249,14 @@
                 p4.run_sync("-q", "-f")
                 return
         secho(f"Switching back to {old_stream_name}", fg="yellow")
         p4.run_client("-s", "-S", old_stream_name)
         secho(f"Aborted. {err}", fg="red")
 
 
-def resolve(progress, task_id, files):
-    p4 = connect_p4()
-    len_of_task = len(files)
-    for n, filename in enumerate(files):
-        progress[task_id] = {"progress": n + 1, "total": len_of_task}
-        try:
-            ret = p4.run_resolve("-f", "-am", "-as", filename)
-        except P4Exception as e:
-            echo(str(e))
-
-
 @app.command()
 def mergedown(nosubmit: Optional[bool] = Option(False, help="Do not submit the changelist after resolving")):
     """
     Merge from parent into your current task branch
     """
     ret = p4.run_stream("-o")[0]
     stream_name = ret["Stream"]
@@ -279,27 +269,16 @@
     client = ret["Client"]
 
     ret = p4.run_opened()
     for r in ret:
         if r["change"] == "default":
             abort("Your default changelist must be empty before merging down from main.")
 
-    secho(f"Integrating latest from parent {parent} to task stream {stream_name}...", bold=True)
-
-    p4.input = f"""
-Change: new
-Client:	{client}
-User:	{p4.user}
-
-Description:
-	Automatically merge {UE_STREAM} to {stream_name}
-
-"""
     secho(f"Merging files from {UE_STREAM} to {stream_name}...", bold=True)
-
+    merge_response = []
     try:
         cmd = ["-Af", "-S", stream_name, "-r", f"{stream_name}/..."]
         merge_response = p4.run_merge(*cmd)
     except P4Exception as e:
         if e.errors:
             secho(e.errors[0], fg="red")
         if e.warnings:
@@ -312,26 +291,26 @@
     with Progress(
         "[green]Resolving files...",
         BarColumn(),
         "[progress.percentage]{task.percentage:>3.0f}%",
         TimeRemainingColumn(),
         MofNCompleteColumn(),
         "{task.description}",
-        refresh_per_second=0.5,  # bit slower updates
+        refresh_per_second=10,  # bit slower updates
     ) as progress:
         task = progress.add_task("", total=num_files)
         for resp in merge_response:
             depotFile = resp["depotFile"]
             try:
                 ret = p4.run_resolve("-f", "-am", "-as", depotFile)
                 if ret:
                     resolves.append(ret)
             except P4Exception as e:
                 echo(str(e))
-            progress.update(task, advance=1, description="..."+depotFile[-50:])
+            progress.update(task, advance=1, description="..." + depotFile[-50:])
     try:
         ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
     except P4Exception as e:
         echo(str(e))
 
     if not ret:
         abort("Your task stream is up to date.")
@@ -339,42 +318,48 @@
     unresolved = []
     for r in ret:
         if "unresolved" in r:
             unresolved.append(r)
             secho(f"  {r['clientFile']}... conflict", fg="yellow")
         else:
             secho(f"  {r['clientFile']}... ok", fg="green")
-    
+
     if unresolved:
-        secho(f"\nThere are conflicting files where you have changed files which have also been changed in {UE_STREAM}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v.")
+        secho(
+            f"\nThere are conflicting files where you have changed files which have also been changed in {UE_STREAM}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v."
+        )
         overwrite_all = False
         overwrite_none = False
         num_skipped = 0
         for i, r in enumerate(unresolved):
             y = None
             if not overwrite_all and not overwrite_none:
                 y = prompt(f"[{i+1}/{len(unresolved)}] Overwrite {r['clientFile']} [Yes/No/None/All] ").upper()
             if y not in ("YES", "Y", "NO", "N", "NONE", "ALL"):
-                abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
+                abort(
+                    f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}"
+                )
             if y in ("ALL"):
                 overwrite_none = False
                 overwrite_all = True
             elif y in ("NONE"):
                 overwrite_none = True
                 overwrite_all = False
 
             if y in ("Y", "YES") or overwrite_all:
                 ret = p4.run_resolve("-f", "-at", f"{r['clientFile']}")
             if y in ("N", "NO") or overwrite_none:
                 secho(f"Skipping {r['clientFile']}...")
                 num_skipped += 1
-            
+
         if num_skipped:
-            abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
-            
+            abort(
+                f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}"
+            )
+
         secho("All Unresolved files have been overwritten by parent stream")
 
     try:
         ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
     except P4Exception as e:
         echo(str(e))
     filelist = ""
@@ -383,66 +368,69 @@
             abort("There are still unresolved files in your pending changelist. Please resolve them in p4v")
         filelist += f"    {r['depotFile']}\n"
 
     mr = ""
     if unresolved:
         mr = f"{len(unresolved)} unresolvable files were overwritten."
 
-
     if not nosubmit:
-
         txt = f"""
-    Change: new
-    Client:	{client}
-    User:	{p4.user}
-
-    Description:
-        Automatically merge {UE_STREAM} to {stream_name}. {mr}
-    Files:
-    {filelist}
+Change:	new
+Client:	{client}
+User:	{p4.user}
+
+Description:
+    Automatically merge {UE_STREAM} to {stream_name}. {mr}
+Files:
+{filelist}
     """
+        print(txt)
+        # return
         p4.input = txt
-        p4.run_submit('-i')
+        p4.run_submit("-i")
 
         try:
             ret = p4.run_resolve("-f", "-am", "-as", f"{root_path}/...")
         except P4Exception as e:
             if "no file(s) to resolve" not in str(e):
                 raise
         try:
             ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
         except P4Exception as e:
-            if 'not opened on this client.' in str(e) or "no such file(s)." in str(e):
+            if "not opened on this client." in str(e) or "no such file(s)." in str(e):
                 secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
                 return
             else:
                 echo(str(e))
         if not ret:
             secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
         else:
             abort("Something is amiss. Your task stream is not up to date after the merge. Take a look at p4v")
     else:
-        echo(f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {UE_STREAM} to {stream_name}. {mr}")
+        echo(
+            f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {UE_STREAM} to {stream_name}. {mr}"
+        )
+
 
 @app.command()
 def copyup():
     """
     Finish the task and copy into the parent stream
     """
     ret = p4.run_opened()
     if ret:
         abort("There are unsubmitted files in your workspace")
 
-## p4 copy -Af -S //Project/jonb-2023-03-03-plugin_functional_tests //Project/SN2-Main/...
+    ## p4 copy -Af -S //Project/jonb-2023-03-03-plugin_functional_tests //Project/SN2-Main/...
     ret = get_current_stream()
     stream_name = ret["Stream"]
     parent = ret["Parent"]
     if ret["Type"] != "task":
         abort(f"Current stream {stream_name} is not a task stream")
-    
+
     echo(f"Switching to parent stream {parent}...")
     p4.run_client("-s", "-S", parent)
 
     p4.run_sync("-q")
     echo(f"Performing copy from {stream_name} to {ret['baseParent']}...")
     try:
         copy_ret = p4.run_copy("-Af", "-S", stream_name, ret["baseParent"] + "/...")
@@ -455,14 +443,15 @@
     else:
         echo("Adding files...")
         for r in copy_ret:
             echo(f"  {r['fromFile']} -> {r['depotFile']}")
 
     secho(f"You can now submit your changelist to {parent} in p4v", fg="green")
 
+
 @app.command()
 def delete(current: Optional[bool] = Option(False, help="Delete the current task stream")):
     """
     Permanently delete a named task stream or your current one"""
 
     if current:
         ret = p4.run_stream("-o")[0]
@@ -475,26 +464,26 @@
     else:
         client = p4.run_client("-o")[0]
         client_owner = client["Owner"]
         task_streams = get_task_streams(client_owner)
         parent = None
         for i, t in enumerate(task_streams):
             secho(f"{i+1} : {t['Stream']}")
-        
+
         if not task_streams:
             abort("You have no task streams.")
         n = prompt("\nSelect a stream to delete")
         try:
             n = int(n)
         except:
             abort("Aborted.")
         if n < 0 or n > len(task_streams):
             abort("Aborted.")
-        stream_name = task_streams[n-1]["Stream"]
-        delete = confirm(f"Are you sure you want to delete the task stream {stream_name}?") 
+        stream_name = task_streams[n - 1]["Stream"]
+        delete = confirm(f"Are you sure you want to delete the task stream {stream_name}?")
 
     if delete:
         if current:
             secho(f"Switching to {parent}...")
             p4.run_client("-s", "-S", parent)
             ret = p4.run_sync("-q", f"{path}...")
 
@@ -502,9 +491,8 @@
         try:
             p4.run_stream("--obliterate", "-y", stream_name)
         except P4Exception as e:
             abort(str(e))
     else:
         abort("Aborted")
     ret = p4.run_sync("-q", "-k", f"{path}...")
-    #sync()
-
+    # sync()
```

### Comparing `unknown-cli-0.6.7/unknowncli/data/.p4ignore.txt` & `unknown-cli-0.6.8/unknowncli/data/.p4ignore.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.6.7/unknowncli/utils.py` & `unknown-cli-0.6.8/unknowncli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 
 def fmt_date(dt: str):
     try:
         return dateutil.parser.parse(dt).strftime("%Y-%m-%d %H:%M")
     except:
         return dt
 
+
 def check_version():
     """
     Check for new version on pypi every 10 minutes
     """
     try:
         version_check_file = Path("~/.unknown-cli-version").expanduser()
         check_version = True
@@ -224,29 +225,34 @@
                     pass
 
         if check_version:
             contents = requests.get("https://pypi.org/pypi/unknown-cli/json").json()
             v = contents["info"]["version"]
             my_version = read_version()
 
-            if (v != my_version):
-                secho(f"Version {v} of this tool is available while you are on version {my_version}. Please upgrade using: pip install unknown-cli -U", fg="green", bold=True)
+            if v != my_version:
+                secho(
+                    f"Version {v} of this tool is available while you are on version {my_version}. Please upgrade using: pip install unknown-cli -U",
+                    fg="green",
+                    bold=True,
+                )
             else:
                 with version_check_file.open("w") as f:
                     f.write(f"{fmt_date(datetime.utcnow())}")
     except:
         raise
 
+
 def check_p4config():
     try:
         is_changes = False
         p4 = P4()
         ignore_file = "s:\\sn2-main\\.p4ignore.txt".lower()
         p4_port = "ssl:perforce.reginald.cloud:1666"
-        cfg = Path(p4.env('P4CONFIG'))
+        cfg = Path(p4.env("P4CONFIG"))
         if p4.ignore_file.lower() != ignore_file:
             secho(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.", fg="yellow")
             y = confirm(f"Would you like to change the setting in your {cfg} file?")
             if y:
                 _lines = []
                 lines = []
                 with cfg.open() as f:
@@ -282,8 +288,8 @@
                 for l in lines:
                     secho(f"{l.strip()}")
 
             secho("\nYou're all set!", fg="green")
             exit(0)
 
     except Exception as e:
-        pass
+        pass
```

