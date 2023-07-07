# Comparing `tmp/unknown-cli-0.5.5.tar.gz` & `tmp/unknown-cli-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknown-cli-0.5.5.tar", last modified: Wed Mar 29 09:59:35 2023, max compression
+gzip compressed data, was "unknown-cli-0.6.7.tar", last modified: Fri Jul  7 08:17:43 2023, max compression
```

## Comparing `unknown-cli-0.5.5.tar` & `unknown-cli-0.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2023-03-29 09:59:35.259245 unknown-cli-0.5.5/
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)      474 2023-03-29 09:59:35.258246 unknown-cli-0.5.5/PKG-INFO
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)       30 2022-10-25 14:43:45.000000 unknown-cli-0.5.5/README.md
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)       38 2023-03-29 09:59:35.259746 unknown-cli-0.5.5/setup.cfg
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)     2640 2022-10-31 11:26:41.000000 unknown-cli-0.5.5/setup.py
-drwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2023-03-29 09:59:35.161219 unknown-cli-0.5.5/unknown_cli.egg-info/
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)      474 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknown_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)      436 2023-03-29 09:59:35.000000 unknown-cli-0.5.5/unknown_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        1 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknown_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)       83 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknown_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)      111 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknown_cli.egg-info/requires.txt
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)       11 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknown_cli.egg-info/top_level.txt
-drwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2023-03-29 09:59:35.200724 unknown-cli-0.5.5/unknowncli/
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        5 2023-03-29 09:59:34.000000 unknown-cli-0.5.5/unknowncli/VERSION
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)      405 2022-10-25 14:43:45.000000 unknown-cli-0.5.5/unknowncli/__init__.py
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)     1509 2023-03-24 11:49:34.000000 unknown-cli-0.5.5/unknowncli/__main__.py
-drwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2023-03-29 09:59:35.238745 unknown-cli-0.5.5/unknowncli/commands/
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2022-10-25 14:43:45.000000 unknown-cli-0.5.5/unknowncli/commands/__init__.py
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)    11755 2023-03-29 09:59:14.000000 unknown-cli-0.5.5/unknowncli/commands/project.py
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)    15826 2023-03-24 12:57:44.000000 unknown-cli-0.5.5/unknowncli/commands/task.py
-drwxrwxrwx   0 nonnib    (1001) nonnib    (1002)        0 2023-03-29 09:59:35.248745 unknown-cli-0.5.5/unknowncli/data/
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)     3560 2022-10-31 11:46:02.000000 unknown-cli-0.5.5/unknowncli/data/.p4ignore.txt
--rwxrwxrwx   0 nonnib    (1001) nonnib    (1002)     8896 2023-03-29 09:42:08.000000 unknown-cli-0.5.5/unknowncli/utils.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.163719 unknown-cli-0.6.7/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 08:17:43.160706 unknown-cli-0.6.7/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       28 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/README.md
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       38 2023-07-07 08:17:43.164736 unknown-cli-0.6.7/setup.cfg
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     2558 2023-07-05 17:48:37.000000 unknown-cli-0.6.7/setup.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:42.962344 unknown-cli-0.6.7/unknown_cli.egg-info/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      447 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      436 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        1 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       83 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      116 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/requires.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)       11 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknown_cli.egg-info/top_level.txt
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.038427 unknown-cli-0.6.7/unknowncli/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        5 2023-07-07 08:17:42.000000 unknown-cli-0.6.7/unknowncli/VERSION
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)      390 2023-07-05 17:41:19.000000 unknown-cli-0.6.7/unknowncli/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     1468 2023-07-05 17:41:21.000000 unknown-cli-0.6.7/unknowncli/__main__.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.111652 unknown-cli-0.6.7/unknowncli/commands/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/commands/__init__.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    11755 2023-07-05 17:41:23.000000 unknown-cli-0.6.7/unknowncli/commands/project.py
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)    16722 2023-07-07 08:15:06.000000 unknown-cli-0.6.7/unknowncli/commands/task.py
+drwxrwxrwx   0 nonnib    (1000) nonnib    (1000)        0 2023-07-07 08:17:43.137181 unknown-cli-0.6.7/unknowncli/data/
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     3408 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/data/.p4ignore.txt
+-rwxrwxrwx   0 nonnib    (1000) nonnib    (1000)     8549 2023-07-05 17:33:30.000000 unknown-cli-0.6.7/unknowncli/utils.py
```

### Comparing `unknown-cli-0.5.5/unknowncli/__main__.py` & `unknown-cli-0.6.7/unknowncli/__main__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os, sys
-import logging
-import pathlib
-import requests
-from .utils import console_handler, abort, check_version, check_p4config
-from pathlib import Path
-
-log = logging.getLogger(__name__)
-help_string = """A utility for managing Unknown projects"""
-
-base_path = pathlib.Path(os.path.dirname(__file__))
-commands_folder = base_path / "commands"
-
-from typer import Typer, Context, Argument, Option, echo, secho, confirm, prompt
-
-app = Typer(add_completion=False)
-
-@app.callback(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
-def cli(
-    ctx: Context,
-    #verbose: str = Option(None, "-v", "--verbose", help="Verbose logging: info or debug"),
-    #output: str = Option("text", "-o", "--output", help="Output text or json"),
-):
-    """
-    This tool handles the initial setup of Perforce Projects and helps you work with task streams.
-    It creates workspaces for you according to naming conventions and sets up a virtual drive.
-    Please run the 'project setup' command to get started.
-    """
-    # by default we log out to console WARN and higher but can view info with -v
-    #if verbose:
-    #    console_handler.setLevel(getattr(logging, verbose.upper()))
-    check_version()
-
-check_p4config()
-
-
-from unknowncli.commands import project
-from unknowncli.commands import task
-
-app.add_typer(project.app, name="project", help="Manage initial project setup")
-app.add_typer(task.app, name="task", help="Manage perforce task streams")
+import os, sys
+import logging
+import pathlib
+import requests
+from .utils import console_handler, abort, check_version, check_p4config
+from pathlib import Path
+
+log = logging.getLogger(__name__)
+help_string = """A utility for managing Unknown projects"""
+
+base_path = pathlib.Path(os.path.dirname(__file__))
+commands_folder = base_path / "commands"
+
+from typer import Typer, Context, Argument, Option, echo, secho, confirm, prompt
+
+app = Typer(add_completion=False)
+
+@app.callback(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
+def cli(
+    ctx: Context,
+    #verbose: str = Option(None, "-v", "--verbose", help="Verbose logging: info or debug"),
+    #output: str = Option("text", "-o", "--output", help="Output text or json"),
+):
+    """
+    This tool handles the initial setup of Perforce Projects and helps you work with task streams.
+    It creates workspaces for you according to naming conventions and sets up a virtual drive.
+    Please run the 'project setup' command to get started.
+    """
+    # by default we log out to console WARN and higher but can view info with -v
+    #if verbose:
+    #    console_handler.setLevel(getattr(logging, verbose.upper()))
+    check_version()
+
+check_p4config()
+
+
+from unknowncli.commands import project
+from unknowncli.commands import task
+
+app.add_typer(project.app, name="project", help="Manage initial project setup")
+app.add_typer(task.app, name="task", help="Manage perforce task streams")
```

### Comparing `unknown-cli-0.5.5/unknowncli/commands/project.py` & `unknown-cli-0.6.7/unknowncli/commands/project.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.5.5/unknowncli/commands/task.py` & `unknown-cli-0.6.7/unknowncli/commands/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,486 +1,510 @@
-import datetime
-import time 
-import sys, os
-import requests
-import logging
-import socket
-from tabulate import tabulate
-from pathlib import Path
-from pprint import pprint
-from ..utils import dumps, abort, get_datafile
-from subprocess import check_call, call
-from P4 import P4, P4Exception
-import shutil
-from typing import Optional
-log = logging.getLogger(__name__)
-
-from typer import Context, launch, echo, secho, Option, Typer, confirm, prompt, style, progressbar
-
-app = Typer()
-
-hostname = socket.gethostname().lower()
-SUBST_DRIVE = "S:"
-path = f"{SUBST_DRIVE}\\sn2-main\\"
-BASE_STREAM = "//Project/SN2-Main"
-UE_STREAM = "//project/sn2-main-ue"
-
-p4 = None
-
-def connect_p4():
-    p4_conn = P4()
-    try:
-        p4_conn.connect()
-    except Exception as e:
-        abort(f"Cannot establish connection with Perforce server: {e}...")
-    return p4_conn
-
-
-@app.callback()
-def main():
-    """
-    Manage task streams.
-    
-    This tool is highly opinionated and expects you to be using the //Project/SN2-Main-UE stream and be working in a workspace called <username>_<label>_sn2-main
-    """
-    global p4
-    p4 = connect_p4()
-    ret = get_current_stream()
-    ignore_file = (path + ".p4ignore.txt").lower()
-    if p4.ignore_file.lower() != ignore_file:
-        abort(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.\nPlease change the setting in your {p4.env('P4CONFIG')} file")
-    
-    if "Stream" not in ret:
-        abort("Invalid workspace. You must be working in Streams to use this tool")
-    stream_name = ret["Stream"]
-    parent = ret["Parent"]
-    secho(f"You are currently working in stream: {stream_name}", fg="blue")
-    if parent.lower() != UE_STREAM and stream_name.lower() != UE_STREAM:
-        abort(f"To use this tool you must be working in the {UE_STREAM} stream but your workspace is set on {stream_name}. Please change your workspace with 'p4 set'")
-
-def get_task_streams(owner):
-    lst = p4.run_streams("-F", f"Owner={owner} Type=task baseParent={BASE_STREAM}")
-    return lst
-
-def get_current_stream():
-    try:
-        ret = p4.run_stream("-o")[0]
-    except P4Exception as e:
-        client_name = "None"
-        try:
-            client = get_current_client()
-            client_name = client["Client"]
-        except:
-            pass
-        abort(f"Unable to get a stream from your current workspace, {client_name}. Make sure you are working in the {BASE_STREAM} stream. Error: {e}")
-    return ret
-
-def get_current_client():
-    ret = p4.run_client("-o")[0]
-    return ret
-
-def get_clients():
-    try:
-        specs = p4.run_clients("-u", p4.user)
-    except Exception as e:
-        abort(str(e))
-    ret = {}
-    for s in specs:
-        if "Stream" not in s:
-            continue
-        host = s["Host"].lower()
-        if host == hostname or not host:
-            ret[s["Stream"].lower()] = s
-    return ret
-
-def sync():
-    s = confirm("Sync latest?")
-
-    if not s:
-        return
-    
-    secho(f"Syncing latest...")
-    try:
-        ret = p4.run_sync("-q", f"{path}UE/Subnautica2/...")
-    except P4Exception as e:
-        print(e)
-
-@app.command()
-def create(label: str = Option(None, prompt="Task branch label")):
-    """
-    Create a new task branch
-    """
-    if not label:
-        abort("Aborted.")
-    clients = get_clients()
-    if get_current_stream()["Stream"].lower() != UE_STREAM:
-        abort(f"Please switch to the {UE_STREAM} before creating a new task stream")
-
-    ue_stream_client = None
-    for k, c in clients.items():
-        if k == UE_STREAM:
-            ue_stream_client = c
-    if not ue_stream_client:
-        abort(f"You have no workspace mapped to the {UE_STREAM} stream. Please set one up.")
-
-    ret = p4.run_opened()
-    if (len(ret)):
-        abort("You have opened files. Please revert or submit before creating new task stream.")
-
-
-    #print(ue_stream_client)
-    #task_client_name = ue_stream_client["client"] + "_task"
-    #task_client = None
-    #for k, c in clients.items():
-    #    if c["client"] == task_client_name:
-    #        echo(f"Reusing existin workspace {k}")
-    #        task_client = c
-    #        break
-    # sync latest from parent
-    echo("Syncing parent branch...")
-    try:
-        ret = p4.run_sync("-q", f"{path}...")
-    except P4Exception as e:
-        secho(str(e), fg="yellow")
-        abort("Please fix the issues above before continuing")
-
-    d = datetime.datetime.utcnow().isoformat().split("T")[0]
-    label = label.replace(" ", "_").lower()
-    stream_name = f"{p4.user}-{d}-{label}"
-    full_stream_name = f"//Project/{stream_name}"
-    secho(f"Creating task stream {stream_name} from {UE_STREAM}...")
-    args = f"""
-Stream: {full_stream_name}
-Owner:  {p4.user}
-Name:   {stream_name}
-Parent: {UE_STREAM}
-Type:   task
-Description:
-    Created by {p4.user}.
-Options:        allsubmit unlocked toparent fromparent mergedown
-ParentView:     inherit
-Paths:
-    share ...
-"""
-    p4.input = args
-    ret = p4.run_stream("-i", "-t", "task")
-    #print(ret[0])
-
-    secho(f"Populating stream {full_stream_name}...")
-    try:
-        ret = p4.run_populate("-o", "-S", full_stream_name, "-r", "-d", "Initial branch")
-    except P4Exception as e:
-        if e.errors:
-            secho(e.errors[0], fg="yellow")
-
-
-    if 0:#not task_client:
-        root = f"{ue_stream_client['Root']}_task"
-        echo("Creating new workspace {task_client_name} -> {root}...")
-        client_spec = f"""
-Client: {task_client_name}
-Owner:  {ue_stream_client['Owner']}
-Host:   {ue_stream_client['Host']}
-Description:
-    Automatically created task workspace for {ue_stream_client['Owner']}
-
-Root:   {root}
-Options:        noallwrite noclobber nocompress unlocked nomodtime normdir
-SubmitOptions:  submitunchanged
-LineEnd:        local
-Stream: {full_stream_name}"""
-        p4.input = client_spec
-        p4.run_client("-i")
-
-    #p4.client = task_client_name
-    secho(f"Switching current workspace {p4.client} to {full_stream_name}...")
-    p4.run_client("-s", "-S", full_stream_name)
-    ret = p4.run_client("-o")[0]
-    root_path = ret["Root"]
-
-#    if not task_client:
-#        secho("Force syncing your new workspace folder to latest")
-#        ret = p4.run_sync(f"{root}...#head")
-#    else:
-#        sync()
-
-
-    ret = p4.run_stream("-o")[0]
-    stream_name = ret["Stream"]
-    parent = ret["Parent"]
-
-    if ret["Type"] != "task":
-        abort(f"Something went wrong. Current stream {stream_name} is not a task stream")
-
-    # update the server without syncing
-    ret = p4.run_sync("-q", "-k", f"{path}...")
-
-    secho(f"You are now working in task stream {stream_name} from parent {parent}", bold=True, fg="green")
-
-@app.command()
-def switch():
-    """
-    Lists your current task streams and lets you switch between them
-    """
-    stream = get_current_stream()
-    client = p4.run_client("-o")[0]
-    client_owner = client["Owner"]
-    task_streams = get_task_streams(client_owner)
-    parent = None
-    if stream["Type"] == "task":
-        parent = stream["Parent"]
-    for i, t in enumerate(task_streams):
-        secho(f"{i+1} : {t['Stream']}")
-    if parent:
-        secho(f"0 : {parent}")
-    
-    if not task_streams:
-        abort("You have no task streams. You can create one with the 'create' command")
-    n = prompt("\nSelect a stream to work in")
-    if n is None:
-        abort("No stream selected")
-    try:
-        n = int(n)
-    except:
-        abort("Aborted.")
-    if n == 0:
-        new_stream = parent
-    else:
-        try:
-            new_stream = task_streams[n-1]["Stream"]
-        except:
-            abort("Aborted.")
-    
-    secho(f"\nSwitching to stream {new_stream}", bold=True)
-    try:
-        p4.run_client("-s", "-S", new_stream)
-    except P4Exception as e:
-        abort(e)
-
-    p4.run_sync("-q")
-
-
-@app.command()
-def mergedown():
-    """
-    Merge from parent into your current task branch
-    """
-    ret = p4.run_stream("-o")[0]
-    stream_name = ret["Stream"]
-    parent = ret["Parent"]
-    if ret["Type"] != "task":
-        abort(f"Current stream {stream_name} is not a task stream")
-
-    ret = p4.run_client("-o")[0]
-    root_path = ret["Root"]
-    client = ret["Client"]
-
-    ret = p4.run_opened()
-    for r in ret:
-        if r["change"] == "default":
-            abort("Your default changelist must be empty before merging down from main.")
-
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
-
-    try:
-        cmd = ["-Af", "-S", stream_name, "-r", f"{stream_name}/..."]
-        ret = p4.run_merge(*cmd)
-    except P4Exception as e:
-        if e.errors:
-            secho(e.errors[0], fg="red")
-        if e.warnings:
-            secho(e.warnings[0], fg="yellow")
-        if "already integrated" in str(e):
-            secho(f"Your task stream is already up to date with {UE_STREAM}", fg="green")
-        return
-    #ret = p4.run_opened()
-    #for f in ret:
-    try:
-        ret = p4.run_resolve("-f", "-am", "-as", f"{root_path}/...")
-    except P4Exception as e:
-        echo(str(e))
-    
-    try:
-        ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
-    except P4Exception as e:
-        echo(str(e))
-    if not ret:
-        abort("Your task stream is up to date.")
-
-    unresolved = []
-    for r in ret:
-        if "unresolved" in r:
-            unresolved.append(r)
-            secho(f"  {r['clientFile']}... conflict", fg="yellow")
-        else:
-            secho(f"  {r['clientFile']}... ok", fg="green")
-    
-    if unresolved:
-        secho(f"\nThere are conflicting files where you have changed files which have also been changed in {UE_STREAM}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v.")
-        overwrite_all = False
-        overwrite_none = False
-        num_skipped = 0
-        for i, r in enumerate(unresolved):
-            y = None
-            if not overwrite_all and not overwrite_none:
-                y = prompt(f"[{i+1}/{len(unresolved)}] Overwrite {r['clientFile']} [Yes/No/None/All] ").upper()
-            if y not in ("YES", "Y", "NO", "N", "NONE", "ALL"):
-                abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
-            if y in ("ALL"):
-                overwrite_none = False
-                overwrite_all = True
-            elif y in ("NONE"):
-                overwrite_none = True
-                overwrite_all = False
-
-            if y in ("Y", "YES") or overwrite_all:
-                ret = p4.run_resolve("-f", "-at", f"{r['clientFile']}")
-            if y in ("N", "NO") or overwrite_none:
-                secho(f"Skipping {r['clientFile']}...")
-                num_skipped += 1
-            
-        if num_skipped:
-            abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
-
-            
-        secho("All Unresolved files have been overwritten by parent stream")
-
-    try:
-        ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
-    except P4Exception as e:
-        echo(str(e))
-    filelist = ""
-    for r in ret:
-        if "unresolved" in r:
-            abort("There are still unresolved files in your pending changelist. Please resolve them in p4v")
-        filelist += f"    {r['depotFile']}\n"
-
-    mr = ""
-    if unresolved:
-        mr = f"{len(unresolved)} unresolvable files were overwritten."
-
-    txt = f"""
-Change: new
-Client:	{client}
-User:	{p4.user}
-
-Description:
-	Automatically merge {UE_STREAM} to {stream_name}. {mr}
-Files:
-{filelist}
-"""
-    p4.input = txt
-    p4.run_submit('-i')
-
-    try:
-        ret = p4.run_resolve("-f", "-am", "-as", f"{root_path}/...")
-    except P4Exception as e:
-        if "no file(s) to resolve" not in str(e):
-            raise
-    try:
-        ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
-    except P4Exception as e:
-        if 'not opened on this client.' in str(e) or "no such file(s)." in str(e):
-            secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
-            return
-        else:
-            echo(str(e))
-    if not ret:
-        secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
-    else:
-        abort("Something is amiss. Your task stream is not up to date after the merge. Take a look at p4v")
-
-@app.command()
-def copyup():
-    """
-    Finish the task and copy into the parent stream
-    """
-    ret = p4.run_opened()
-    if ret:
-        abort("There are unsubmitted files in your workspace")
-
-## p4 copy -Af -S //Project/jonb-2023-03-03-plugin_functional_tests //Project/SN2-Main/...
-    ret = get_current_stream()
-    stream_name = ret["Stream"]
-    parent = ret["Parent"]
-    if ret["Type"] != "task":
-        abort(f"Current stream {stream_name} is not a task stream")
-    
-    echo(f"Switching to parent stream {parent}...")
-    p4.run_client("-s", "-S", parent)
-
-    p4.run_sync("-q")
-    echo(f"Performing copy from {stream_name} to {ret['baseParent']}...")
-    try:
-        copy_ret = p4.run_copy("-Af", "-S", stream_name, ret["baseParent"] + "/...")
-    except P4Exception as e:
-        if "up-to-date" in str(e):
-            secho(f"Nothing to do. Parent {parent} is identical to task stream {stream_name}", fg="green")
-            return
-        else:
-            raise
-    else:
-        echo("Adding files...")
-        for r in copy_ret:
-            echo(f"  {r['fromFile']} -> {r['depotFile']}")
-
-    secho(f"You can now submit your changelist to {parent} in p4v", fg="green")
-
-@app.command()
-def delete(current: Optional[bool] = Option(False, help="Delete the current task stream")):
-    """
-    Permanently delete a named task stream or your current one"""
-
-    if current:
-        ret = p4.run_stream("-o")[0]
-        stream_name = ret["Stream"]
-        parent = ret["Parent"]
-        if ret["Type"] != "task":
-            abort(f"Current stream {stream_name} is not a task stream")
-
-        delete = confirm("Are you sure you want to delete the current task stream?")
-    else:
-        client = p4.run_client("-o")[0]
-        client_owner = client["Owner"]
-        task_streams = get_task_streams(client_owner)
-        parent = None
-        for i, t in enumerate(task_streams):
-            secho(f"{i+1} : {t['Stream']}")
-        
-        if not task_streams:
-            abort("You have no task streams.")
-        n = prompt("\nSelect a stream to delete")
-        try:
-            n = int(n)
-        except:
-            abort("Aborted.")
-        if n < 0 or n > len(task_streams):
-            abort("Aborted.")
-        stream_name = task_streams[n-1]["Stream"]
-        delete = confirm(f"Are you sure you want to delete the task stream {stream_name}?") 
-
-    if delete:
-        if current:
-            secho(f"Switching to {parent}...")
-            p4.run_client("-s", "-S", parent)
-            ret = p4.run_sync("-q", f"{path}...")
-
-        secho(f"Deleting task stream {stream_name}...")
-        try:
-            p4.run_stream("--obliterate", "-y", stream_name)
-        except P4Exception as e:
-            abort(str(e))
-    else:
-        abort("Aborted")
-    ret = p4.run_sync("-q", "-k", f"{path}...")
-    #sync()
-
+import random
+import datetime
+import json
+import time 
+import sys, os
+import requests
+import logging
+import socket
+from tabulate import tabulate
+from pathlib import Path
+from pprint import pprint
+from ..utils import dumps, abort, get_datafile
+from subprocess import check_call, call
+from P4 import P4, P4Exception
+import shutil
+from typing import Optional
+log = logging.getLogger(__name__)
+
+from typer import echo, secho, Option, Typer, confirm, prompt
+from rich.progress import track, Progress, SpinnerColumn, MofNCompleteColumn, TimeRemainingColumn, TimeElapsedColumn, BarColumn
+
+from multiprocessing import Pool, Manager
+import multiprocessing
+from concurrent.futures import ProcessPoolExecutor
+app = Typer()
+
+hostname = socket.gethostname().lower()
+SUBST_DRIVE = "S:"
+path = f"{SUBST_DRIVE}\\sn2-main\\"
+BASE_STREAM = "//Project/SN2-Main"
+UE_STREAM = "//project/sn2-main-ue"
+
+p4 = None
+
+def connect_p4():
+    p4_conn = P4()
+    try:
+        p4_conn.connect()
+    except Exception as e:
+        abort(f"Cannot establish connection with Perforce server: {e}...")
+    return p4_conn
+
+
+@app.callback()
+def main():
+    """
+    Manage task streams.
+    
+    This tool is highly opinionated and expects you to be using the //Project/SN2-Main-UE stream and be working in a workspace called <username>_<label>_sn2-main
+    """
+    global p4
+    p4 = connect_p4()
+    ret = get_current_stream()
+    ignore_file = (path + ".p4ignore.txt").lower()
+    if p4.ignore_file.lower() != ignore_file:
+        abort(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.\nPlease change the setting in your {p4.env('P4CONFIG')} file")
+    
+    if "Stream" not in ret:
+        abort("Invalid workspace. You must be working in Streams to use this tool")
+    stream_name = ret["Stream"]
+    parent = ret["Parent"]
+    secho(f"You are currently working in stream: {stream_name}", fg="blue")
+    if parent.lower() != UE_STREAM and stream_name.lower() != UE_STREAM:
+        abort(f"To use this tool you must be working in the {UE_STREAM} stream but your workspace is set on {stream_name}. Please change your workspace with 'p4 set'")
+
+def get_task_streams(owner):
+    lst = p4.run_streams("-F", f"Owner={owner} Type=task baseParent={BASE_STREAM}")
+    return lst
+
+def get_current_stream():
+    try:
+        ret = p4.run_stream("-o")[0]
+    except P4Exception as e:
+        client_name = "None"
+        try:
+            client = get_current_client()
+            client_name = client["Client"]
+        except:
+            pass
+        abort(f"Unable to get a stream from your current workspace, {client_name}. Make sure you are working in the {BASE_STREAM} stream. Error: {e}")
+    return ret
+
+def get_current_client():
+    ret = p4.run_client("-o")[0]
+    return ret
+
+def get_clients():
+    try:
+        specs = p4.run_clients("-u", p4.user)
+    except Exception as e:
+        abort(str(e))
+    ret = {}
+    for s in specs:
+        if "Stream" not in s:
+            continue
+        host = s["Host"].lower()
+        if host == hostname or not host:
+            ret[s["Stream"].lower()] = s
+    return ret
+
+def sync():
+    s = confirm("Sync latest?")
+
+    if not s:
+        return
+    
+    secho(f"Syncing latest...")
+    try:
+        ret = p4.run_sync("-q", f"{path}UE/Subnautica2/...")
+    except P4Exception as e:
+        print(e)
+
+@app.command()
+def create(label: str = Option(None, prompt="Task branch label")):
+    """
+    Create a new task branch
+    """
+    if not label:
+        abort("Aborted.")
+    clients = get_clients()
+    if get_current_stream()["Stream"].lower() != UE_STREAM:
+        abort(f"Please switch to the {UE_STREAM} before creating a new task stream")
+
+    ue_stream_client = None
+    for k, c in clients.items():
+        if k == UE_STREAM:
+            ue_stream_client = c
+    if not ue_stream_client:
+        abort(f"You have no workspace mapped to the {UE_STREAM} stream. Please set one up.")
+
+    ret = p4.run_opened()
+    if (len(ret)):
+        abort("You have opened files. Please revert or submit before creating new task stream.")
+
+
+    #print(ue_stream_client)
+    #task_client_name = ue_stream_client["client"] + "_task"
+    #task_client = None
+    #for k, c in clients.items():
+    #    if c["client"] == task_client_name:
+    #        echo(f"Reusing existin workspace {k}")
+    #        task_client = c
+    #        break
+    # sync latest from parent
+    echo("Syncing parent branch...")
+    try:
+        ret = p4.run_sync("-q", f"{path}...")
+    except P4Exception as e:
+        secho(str(e), fg="yellow")
+        abort("Please fix the issues above before continuing")
+
+    d = datetime.datetime.utcnow().isoformat().split("T")[0]
+    label = label.replace(" ", "_").lower()
+    stream_name = f"{p4.user}-{d}-{label}"
+    full_stream_name = f"//Project/{stream_name}"
+    secho(f"Creating task stream {stream_name} from {UE_STREAM}...")
+    args = f"""
+Stream: {full_stream_name}
+Owner:  {p4.user}
+Name:   {stream_name}
+Parent: {UE_STREAM}
+Type:   task
+Description:
+    Created by {p4.user}.
+Options:        allsubmit unlocked toparent fromparent mergedown
+ParentView:     inherit
+Paths:
+    share ...
+"""
+    p4.input = args
+    ret = p4.run_stream("-i", "-t", "task")
+    #print(ret[0])
+
+    secho(f"Populating stream {full_stream_name}...")
+    try:
+        ret = p4.run_populate("-o", "-S", full_stream_name, "-r", "-d", "Initial branch")
+    except P4Exception as e:
+        if e.errors:
+            secho(e.errors[0], fg="yellow")
+
+    secho(f"Switching current workspace {p4.client} to {full_stream_name}...")
+    p4.run_client("-s", "-S", full_stream_name)
+    ret = p4.run_client("-o")[0]
+    root_path = ret["Root"]
+
+    ret = p4.run_stream("-o")[0]
+    stream_name = ret["Stream"]
+    parent = ret["Parent"]
+
+    if ret["Type"] != "task":
+        abort(f"Something went wrong. Current stream {stream_name} is not a task stream")
+
+    # update the server without syncing
+    ret = p4.run_sync("-q", "-k", f"{path}...")
+
+    secho(f"You are now working in task stream {stream_name} from parent {parent}", bold=True, fg="green")
+
+@app.command()
+def switch():
+    """
+    Lists your current task streams and lets you switch between them
+    """
+    stream = get_current_stream()
+    old_stream_name = stream['Stream']
+    client = p4.run_client("-o")[0]
+    client_owner = client["Owner"]
+    task_streams = get_task_streams(client_owner)
+    parent = None
+    if stream["Type"] == "task":
+        parent = stream["Parent"]
+    for i, t in enumerate(task_streams):
+        secho(f"{i+1} : {t['Stream']}")
+    if parent:
+        secho(f"0 : {parent}")
+    
+    if not task_streams:
+        abort("You have no task streams. You can create one with the 'create' command")
+    n = prompt("\nSelect a stream to work in")
+    if n is None:
+        abort("No stream selected")
+    try:
+        n = int(n)
+    except:
+        abort("Aborted.")
+    if n == 0:
+        new_stream = parent
+    else:
+        try:
+            new_stream = task_streams[n-1]["Stream"]
+        except:
+            abort("Aborted.")
+    
+    secho(f"\nSwitching to stream {new_stream}", bold=True)
+    try:
+        p4.run_client("-s", "-S", new_stream)
+    except P4Exception as e:
+        abort(e)
+
+    secho(f"Running sync...")
+
+    try:
+        p4.run_sync("-q")
+    except P4Exception as e:
+        err = e.errors[0]
+        if "clobber" in err:
+            secho(err, fg="yellow")
+            if confirm("Would you like to overwrite writable files that are not open in your workspace?"):
+                p4.run_sync("-q", "-f")
+                return
+        secho(f"Switching back to {old_stream_name}", fg="yellow")
+        p4.run_client("-s", "-S", old_stream_name)
+        secho(f"Aborted. {err}", fg="red")
+
+
+def resolve(progress, task_id, files):
+    p4 = connect_p4()
+    len_of_task = len(files)
+    for n, filename in enumerate(files):
+        progress[task_id] = {"progress": n + 1, "total": len_of_task}
+        try:
+            ret = p4.run_resolve("-f", "-am", "-as", filename)
+        except P4Exception as e:
+            echo(str(e))
+
+
+@app.command()
+def mergedown(nosubmit: Optional[bool] = Option(False, help="Do not submit the changelist after resolving")):
+    """
+    Merge from parent into your current task branch
+    """
+    ret = p4.run_stream("-o")[0]
+    stream_name = ret["Stream"]
+    parent = ret["Parent"]
+    if ret["Type"] != "task":
+        abort(f"Current stream {stream_name} is not a task stream")
+
+    ret = p4.run_client("-o")[0]
+    root_path = ret["Root"]
+    client = ret["Client"]
+
+    ret = p4.run_opened()
+    for r in ret:
+        if r["change"] == "default":
+            abort("Your default changelist must be empty before merging down from main.")
+
+    secho(f"Integrating latest from parent {parent} to task stream {stream_name}...", bold=True)
+
+    p4.input = f"""
+Change: new
+Client:	{client}
+User:	{p4.user}
+
+Description:
+	Automatically merge {UE_STREAM} to {stream_name}
+
+"""
+    secho(f"Merging files from {UE_STREAM} to {stream_name}...", bold=True)
+
+    try:
+        cmd = ["-Af", "-S", stream_name, "-r", f"{stream_name}/..."]
+        merge_response = p4.run_merge(*cmd)
+    except P4Exception as e:
+        if e.errors:
+            secho(e.errors[0], fg="red")
+        if e.warnings:
+            secho(e.warnings[0], fg="yellow")
+        if "already integrated" in str(e):
+            secho(f"Your task stream is already up to date with {UE_STREAM}", fg="green")
+        return
+    num_files = len(merge_response)
+    resolves = []
+    with Progress(
+        "[green]Resolving files...",
+        BarColumn(),
+        "[progress.percentage]{task.percentage:>3.0f}%",
+        TimeRemainingColumn(),
+        MofNCompleteColumn(),
+        "{task.description}",
+        refresh_per_second=0.5,  # bit slower updates
+    ) as progress:
+        task = progress.add_task("", total=num_files)
+        for resp in merge_response:
+            depotFile = resp["depotFile"]
+            try:
+                ret = p4.run_resolve("-f", "-am", "-as", depotFile)
+                if ret:
+                    resolves.append(ret)
+            except P4Exception as e:
+                echo(str(e))
+            progress.update(task, advance=1, description="..."+depotFile[-50:])
+    try:
+        ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
+    except P4Exception as e:
+        echo(str(e))
+
+    if not ret:
+        abort("Your task stream is up to date.")
+
+    unresolved = []
+    for r in ret:
+        if "unresolved" in r:
+            unresolved.append(r)
+            secho(f"  {r['clientFile']}... conflict", fg="yellow")
+        else:
+            secho(f"  {r['clientFile']}... ok", fg="green")
+    
+    if unresolved:
+        secho(f"\nThere are conflicting files where you have changed files which have also been changed in {UE_STREAM}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v.")
+        overwrite_all = False
+        overwrite_none = False
+        num_skipped = 0
+        for i, r in enumerate(unresolved):
+            y = None
+            if not overwrite_all and not overwrite_none:
+                y = prompt(f"[{i+1}/{len(unresolved)}] Overwrite {r['clientFile']} [Yes/No/None/All] ").upper()
+            if y not in ("YES", "Y", "NO", "N", "NONE", "ALL"):
+                abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
+            if y in ("ALL"):
+                overwrite_none = False
+                overwrite_all = True
+            elif y in ("NONE"):
+                overwrite_none = True
+                overwrite_all = False
+
+            if y in ("Y", "YES") or overwrite_all:
+                ret = p4.run_resolve("-f", "-at", f"{r['clientFile']}")
+            if y in ("N", "NO") or overwrite_none:
+                secho(f"Skipping {r['clientFile']}...")
+                num_skipped += 1
+            
+        if num_skipped:
+            abort(f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}")
+            
+        secho("All Unresolved files have been overwritten by parent stream")
+
+    try:
+        ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
+    except P4Exception as e:
+        echo(str(e))
+    filelist = ""
+    for r in ret:
+        if "unresolved" in r:
+            abort("There are still unresolved files in your pending changelist. Please resolve them in p4v")
+        filelist += f"    {r['depotFile']}\n"
+
+    mr = ""
+    if unresolved:
+        mr = f"{len(unresolved)} unresolvable files were overwritten."
+
+
+    if not nosubmit:
+
+        txt = f"""
+    Change: new
+    Client:	{client}
+    User:	{p4.user}
+
+    Description:
+        Automatically merge {UE_STREAM} to {stream_name}. {mr}
+    Files:
+    {filelist}
+    """
+        p4.input = txt
+        p4.run_submit('-i')
+
+        try:
+            ret = p4.run_resolve("-f", "-am", "-as", f"{root_path}/...")
+        except P4Exception as e:
+            if "no file(s) to resolve" not in str(e):
+                raise
+        try:
+            ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
+        except P4Exception as e:
+            if 'not opened on this client.' in str(e) or "no such file(s)." in str(e):
+                secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
+                return
+            else:
+                echo(str(e))
+        if not ret:
+            secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
+        else:
+            abort("Something is amiss. Your task stream is not up to date after the merge. Take a look at p4v")
+    else:
+        echo(f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {UE_STREAM} to {stream_name}. {mr}")
+
+@app.command()
+def copyup():
+    """
+    Finish the task and copy into the parent stream
+    """
+    ret = p4.run_opened()
+    if ret:
+        abort("There are unsubmitted files in your workspace")
+
+## p4 copy -Af -S //Project/jonb-2023-03-03-plugin_functional_tests //Project/SN2-Main/...
+    ret = get_current_stream()
+    stream_name = ret["Stream"]
+    parent = ret["Parent"]
+    if ret["Type"] != "task":
+        abort(f"Current stream {stream_name} is not a task stream")
+    
+    echo(f"Switching to parent stream {parent}...")
+    p4.run_client("-s", "-S", parent)
+
+    p4.run_sync("-q")
+    echo(f"Performing copy from {stream_name} to {ret['baseParent']}...")
+    try:
+        copy_ret = p4.run_copy("-Af", "-S", stream_name, ret["baseParent"] + "/...")
+    except P4Exception as e:
+        if "up-to-date" in str(e):
+            secho(f"Nothing to do. Parent {parent} is identical to task stream {stream_name}", fg="green")
+            return
+        else:
+            raise
+    else:
+        echo("Adding files...")
+        for r in copy_ret:
+            echo(f"  {r['fromFile']} -> {r['depotFile']}")
+
+    secho(f"You can now submit your changelist to {parent} in p4v", fg="green")
+
+@app.command()
+def delete(current: Optional[bool] = Option(False, help="Delete the current task stream")):
+    """
+    Permanently delete a named task stream or your current one"""
+
+    if current:
+        ret = p4.run_stream("-o")[0]
+        stream_name = ret["Stream"]
+        parent = ret["Parent"]
+        if ret["Type"] != "task":
+            abort(f"Current stream {stream_name} is not a task stream")
+
+        delete = confirm("Are you sure you want to delete the current task stream?")
+    else:
+        client = p4.run_client("-o")[0]
+        client_owner = client["Owner"]
+        task_streams = get_task_streams(client_owner)
+        parent = None
+        for i, t in enumerate(task_streams):
+            secho(f"{i+1} : {t['Stream']}")
+        
+        if not task_streams:
+            abort("You have no task streams.")
+        n = prompt("\nSelect a stream to delete")
+        try:
+            n = int(n)
+        except:
+            abort("Aborted.")
+        if n < 0 or n > len(task_streams):
+            abort("Aborted.")
+        stream_name = task_streams[n-1]["Stream"]
+        delete = confirm(f"Are you sure you want to delete the task stream {stream_name}?") 
+
+    if delete:
+        if current:
+            secho(f"Switching to {parent}...")
+            p4.run_client("-s", "-S", parent)
+            ret = p4.run_sync("-q", f"{path}...")
+
+        secho(f"Deleting task stream {stream_name}...")
+        try:
+            p4.run_stream("--obliterate", "-y", stream_name)
+        except P4Exception as e:
+            abort(str(e))
+    else:
+        abort("Aborted")
+    ret = p4.run_sync("-q", "-k", f"{path}...")
+    #sync()
+
```

### Comparing `unknown-cli-0.5.5/unknowncli/data/.p4ignore.txt` & `unknown-cli-0.6.7/unknowncli/data/.p4ignore.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-# Here you can specify files to ignore when adding files to the depot.
-#
-# The syntax for P4IGNORE files is not the same as Perforce syntax.
-# Instead, it is similar to that used by other versioning systems:
-#
-# - Files are specified in local syntax
-# - a # character at the beginning of a line denotes a comment
-# - a ! character at the beginning of a line excludes the file specification
-# - a * wildcard matches substrings.
-#
-# http://stackoverflow.com/questions/18240084/how-does-perforce-ignore-file-syntax-differ-from-gitignore-syntax
-
-/*.sln
-/.p4sync.txt
-
-# Ignore all Visual Studio temp files.
-*.suo
-*.opensdf
-*.sdf
-.patch_*
-
-*/DerivedDataCache/
-**/DerivedDataCache/Boot.ddc
-**/DerivedDataCache/**/*.udd
-
-# Ignore all Intermediate and Saved directories
-*/Intermediate/*
-*/Saved/*
-
-# Ignore UBT's configuration.xml
-Engine/Programs/UnrealBuildTool/*
-*.uatbuildrecord
-*.tmp
-
-# Ignore built binaries and temporary build files
-*/obj/*
-*.csprojAssemblyReference.cache
-
-# Ignore UBT's log output files
-/Engine/Programs/UnrealBuildTool/*.txt
-
-# Ignore Python cached files
-*.pyc
-
-# Ignore JetBrain's IDE folders
-.idea/
-.gradle/
-
-# Ignore autogenerated files from HoloLens WMRInterop
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/packages/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/Generated Files/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/x64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/ARM64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/x64/*
-/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/ARM64/*
-
-Saved/
-LocalBuilds/
-*.csproj.*
-.vs/*
-.vsconfig
-*.pdb
-*.suo
-*.opensdf
-*.sdf
-*.tmp
-*.mdb
-obj/
-*.vcxproj
-*.sln
-*-Debug.*
-FileOpenOrder/
-*.xcworkspace
-*.xcodeproj
-./Makefile
-./CMakeLists.txt
-.ue4dependencies
-Samples/*
-FeaturePacks/*
-Templates/*
-Engine/Documentation/*
-
-# Engine intermediates
-Engine/Intermediate/*
-Intermediate/
-
-# Intermediate folders for programs should not be checked in
-Engine\Programs\*\Intermediate\*
-
-# Intermediate folders created for various C# programs
-Engine\Source\Programs\*\obj\*
-
-# Saved folders for programs should not be checked in
-Engine\Programs\*\Saved\*
-Engine\Programs\UnrealBuildTool\*
-
-# Derived data cache should never be checked in
-Engine/DerivedDataCache/*
-
-# Ignore any build receipts
-Engine/Build/Receipts/*
-
-# Ignore personal workspace vars
-p4config.txt
-
-# Ignore Unix backup files
-*~
-
-# Ignore Mac desktop services store files
-.DS_Store
-
-# Ignore crash reports
-crashinfo--*
-
-# Ignore linux project files
-*.user
-*.pro
-*.pri
-*.kdev4
-
-# Obj-C/Swift specific
-*.hmap
-*.ipa
-*.dSYM.zip
-*.dSYM
-
-# Ignore documentation generated for C# tools
-Engine/Binaries/DotNET/UnrealBuildTool.xml
-Engine/Binaries/DotNET/AutomationScripts/BuildGraph.Automation.xml
-
-# Ignore version files in the Engine/Binaries directory created by UBT
-/Engine/Binaries/**/*.version
-
-# Ignore exp files in the the Engine/Binaries directory as they aren't C/C++ source files
-/Engine/Binaries/**/*.exp
-
-# Ignore Swarm local save files
-Engine/Binaries/DotNET/SwarmAgent.DeveloperOptions.xml
-Engine/Binaries/DotNET/SwarmAgent.Options.xml
-
-# Intermediary Files
-*.target.xml
-*.exe.config
-*.exe.manifest
-
-# Ignore project-specific files
-*/Build/Receipts/*
-*/DerivedDataCache/*
-*/Binaries/*-Shipping.*
-*/Intermediate/*
-
-*/Logs/*
+# Here you can specify files to ignore when adding files to the depot.
+#
+# The syntax for P4IGNORE files is not the same as Perforce syntax.
+# Instead, it is similar to that used by other versioning systems:
+#
+# - Files are specified in local syntax
+# - a # character at the beginning of a line denotes a comment
+# - a ! character at the beginning of a line excludes the file specification
+# - a * wildcard matches substrings.
+#
+# http://stackoverflow.com/questions/18240084/how-does-perforce-ignore-file-syntax-differ-from-gitignore-syntax
+
+/*.sln
+/.p4sync.txt
+
+# Ignore all Visual Studio temp files.
+*.suo
+*.opensdf
+*.sdf
+.patch_*
+
+*/DerivedDataCache/
+**/DerivedDataCache/Boot.ddc
+**/DerivedDataCache/**/*.udd
+
+# Ignore all Intermediate and Saved directories
+*/Intermediate/*
+*/Saved/*
+
+# Ignore UBT's configuration.xml
+Engine/Programs/UnrealBuildTool/*
+*.uatbuildrecord
+*.tmp
+
+# Ignore built binaries and temporary build files
+*/obj/*
+*.csprojAssemblyReference.cache
+
+# Ignore UBT's log output files
+/Engine/Programs/UnrealBuildTool/*.txt
+
+# Ignore Python cached files
+*.pyc
+
+# Ignore JetBrain's IDE folders
+.idea/
+.gradle/
+
+# Ignore autogenerated files from HoloLens WMRInterop
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/packages/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/Generated Files/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/x64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInteropHoloLens/ARM64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/x64/*
+/Engine/Source/ThirdParty/WindowsMixedRealityInterop/MixedRealityInterop/ARM64/*
+
+Saved/
+LocalBuilds/
+*.csproj.*
+.vs/*
+.vsconfig
+*.pdb
+*.suo
+*.opensdf
+*.sdf
+*.tmp
+*.mdb
+obj/
+*.vcxproj
+*.sln
+*-Debug.*
+FileOpenOrder/
+*.xcworkspace
+*.xcodeproj
+./Makefile
+./CMakeLists.txt
+.ue4dependencies
+Samples/*
+FeaturePacks/*
+Templates/*
+Engine/Documentation/*
+
+# Engine intermediates
+Engine/Intermediate/*
+Intermediate/
+
+# Intermediate folders for programs should not be checked in
+Engine\Programs\*\Intermediate\*
+
+# Intermediate folders created for various C# programs
+Engine\Source\Programs\*\obj\*
+
+# Saved folders for programs should not be checked in
+Engine\Programs\*\Saved\*
+Engine\Programs\UnrealBuildTool\*
+
+# Derived data cache should never be checked in
+Engine/DerivedDataCache/*
+
+# Ignore any build receipts
+Engine/Build/Receipts/*
+
+# Ignore personal workspace vars
+p4config.txt
+
+# Ignore Unix backup files
+*~
+
+# Ignore Mac desktop services store files
+.DS_Store
+
+# Ignore crash reports
+crashinfo--*
+
+# Ignore linux project files
+*.user
+*.pro
+*.pri
+*.kdev4
+
+# Obj-C/Swift specific
+*.hmap
+*.ipa
+*.dSYM.zip
+*.dSYM
+
+# Ignore documentation generated for C# tools
+Engine/Binaries/DotNET/UnrealBuildTool.xml
+Engine/Binaries/DotNET/AutomationScripts/BuildGraph.Automation.xml
+
+# Ignore version files in the Engine/Binaries directory created by UBT
+/Engine/Binaries/**/*.version
+
+# Ignore exp files in the the Engine/Binaries directory as they aren't C/C++ source files
+/Engine/Binaries/**/*.exp
+
+# Ignore Swarm local save files
+Engine/Binaries/DotNET/SwarmAgent.DeveloperOptions.xml
+Engine/Binaries/DotNET/SwarmAgent.Options.xml
+
+# Intermediary Files
+*.target.xml
+*.exe.config
+*.exe.manifest
+
+# Ignore project-specific files
+*/Build/Receipts/*
+*/DerivedDataCache/*
+*/Binaries/*-Shipping.*
+*/Intermediate/*
+
+*/Logs/*
```

### Comparing `unknown-cli-0.5.5/unknowncli/utils.py` & `unknown-cli-0.6.7/unknowncli/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,291 +1,289 @@
-#!/usr/bin/env python
-
-import botocore.session
-from datetime import datetime, timedelta
-import requests
-import click
-import typer
-import configparser
-import logging
-import os
-import sys
-import json
-from jsonpath_rw import parse
-import yaml
-import dateutil
-from functools import wraps
-from urllib.parse import urlparse, urljoin
-import boto3
-from typer import secho, confirm
-from io import BytesIO
-import json
-import botocore
-from loguru import logger
-from pathlib import Path
-from P4 import P4, P4Exception
-from operator import attrgetter, itemgetter
-from . import read_version
-
-log_formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-
-console_handler = logging.StreamHandler()
-console_handler.setFormatter(log_formatter)
-console_handler.setLevel(logging.WARN)
-
-root_logger = logging.getLogger()
-root_logger.setLevel(logging.DEBUG)
-root_logger.addHandler(console_handler)
-
-log = logging.getLogger(__name__)
-
-
-def print_error(*txt):
-    color_print(*txt, color="red")
-
-
-def print_warn(*txt):
-    color_print(*txt, color="yellow")
-
-
-def print_success(*txt):
-    color_print(*txt, color="green")
-
-
-def color_print(*args, **kwargs):
-    color = kwargs.get("color", "reset")
-    for x in args:
-        typer.echo(typer.style(x, fg=color))
-
-
-def get_datafile(filename):
-    p = Path(__file__).parent / "data" / filename
-    with p.open("rt") as f:
-        return f.read()
-
-
-def print_tab(key, val):
-    val_txt = val
-    if isinstance(val, dict):
-        val_txt = ", ".join([f"{k}={v}" for k, v in val.items()])
-    val = typer.style(str(val_txt), bold=True)
-    typer.echo("{0:20}{1}".format(key, val))
-
-
-def print_table(obj):
-    try:
-        for k, v in obj.items():
-            print_tab(k, v)
-    except Exception:
-        typer.echo(obj)
-
-
-def dumps(obj):
-    try:
-        return json.dumps(obj, indent=4, sort_keys=True)
-    except Exception:
-        return repr(obj)
-
-
-def output_pretty_json(dct, keys):
-    ret = ""
-    for k in keys:
-        jsonpath_expr = parse(k)
-        ret = [match.value for match in jsonpath_expr.find(dct)]
-        lst = [""]
-        if ret:
-            if isinstance(ret[0], list) or isinstance(ret[0], dict):
-                lst = yaml.dump(ret[0]).split("\n")
-            else:
-                lst = [str(ret[0])]
-        print_tab(k.split(".")[-1], lst[0])
-        if len(lst) > 1:
-            for v in lst[1:]:
-                print_tab("", v)
-
-
-def find_aws_credentials(profile):
-    """
-    Returns the aws credentials for the specified profile.
-    If no profile is passed in, returns the credentials for the currently selected profile
-
-    Args:
-        profile name
-
-    Returns:
-        Dict containing at least aws_access_key_id, aws_secret_access_key
-
-    Raises:
-        RuntimeError is no default profile or the named profile was not found
-
-    """
-    if not profile:
-        access_key = None
-        secret_key = None
-        token = ""
-        credentials = botocore.session.get_session().get_credentials()
-        if credentials:
-            access_key = credentials.access_key
-            secret_key = credentials.secret_key
-            token = getattr(credentials, "token") or ""
-        if not access_key or not secret_key:
-            raise RuntimeError("No Default AWS profile set")
-
-        return {
-            "aws_access_key_id": access_key,
-            "aws_secret_access_key": secret_key,
-            "aws_session_token": token,
-        }
-
-    folder = os.path.join(os.path.expanduser("~"), ".aws")
-    filename = os.path.join(folder, "credentials")
-    cfg = configparser.ConfigParser()
-    with open(filename) as fp:
-        cfg.readfp(fp)
-        ret = {}
-        if profile not in cfg:
-            raise RuntimeError("No AWS profile '%s' found in %s" % (profile, filename))
-        for key in cfg[profile]:
-            ret[key] = cfg[profile][key]
-    return ret
-
-
-def abort(reason, code=1):
-    """
-    exit with non-zero exit code and write reason for error to stderr.
-    If we are outside a typer context and exception will be raised instead
-    """
-    ctx = click.get_current_context(silent=True)
-    if not ctx:
-        raise Exception(f"Abnormal Termination: {reason}")
-
-    if ctx.obj and ctx.obj.output == "json":
-        ret = {"success": False, "exit_code": code, "message": str(reason)}
-        typer.echo(json.dumps(ret))
-    else:
-        typer.echo(typer.style(str(reason), fg="red"), file=sys.stderr)
-    sys.exit(code)
-
-
-def out(txt, **kw):
-    ctx = click.get_current_context(silent=True)
-    if ctx and ctx.obj and ctx.obj.output == "json":
-        log.info(txt)
-    else:
-        typer.secho(txt, **kw)
-
-
-def success(reason, response=None, **kw):
-    ctx = click.get_current_context(silent=True)
-    if not ctx:
-        print(reason)
-
-    exit_code = 0
-    if ctx.obj and ctx.obj.output == "json":
-        ret = {
-            "success": True,
-            "exit_code": exit_code,
-            "message": str(reason),
-            "response": response,
-        }
-        typer.echo(json.dumps(ret))
-    else:
-        if not kw:
-            kw = {"fg": "white", "bold": True}
-        typer.secho(str(reason), **kw)
-    sys.exit(exit_code)
-
-
-def check_profile(ctx):
-    if not ctx.obj.client:
-        abort("You have no active profile or selected profile is invalid. Run 'unknown profile add [name]'")
-
-
-def fmt_date(dt: str):
-    try:
-        return dateutil.parser.parse(dt).strftime("%Y-%m-%d %H:%M")
-    except:
-        return dt
-
-def check_version():
-    """
-    Check for new version on pypi every 10 minutes
-    """
-    try:
-        version_check_file = Path("~/.unknown-cli-version").expanduser()
-        check_version = True
-        if version_check_file.exists():
-            with version_check_file.open() as f:
-                dt_txt = f.read().strip()
-                try:
-                    dt = dateutil.parser.parse(dt_txt)
-                    if dt >= datetime.utcnow() - timedelta(minutes=10):
-                        check_version = False
-                except:
-                    pass
-
-        if check_version:
-            contents = requests.get("https://pypi.org/pypi/unknown-cli/json").json()
-            v = contents["info"]["version"]
-            my_version = read_version()
-
-            if (v != my_version):
-                secho(f"Version {v} of this tool is available while you are on version {my_version}. Please upgrade using: pip install unknown-cli -U", fg="green", bold=True)
-            else:
-                with version_check_file.open("w") as f:
-                    f.write(f"{fmt_date(datetime.utcnow())}")
-    except:
-        raise
-
-def check_p4config():
-    try:
-        is_changes = False
-        p4 = P4()
-        ignore_file = "s:\\sn2-main\\.p4ignore.txt".lower()
-        p4_port = "ssl:perforce.reginald.cloud:1666"
-        cfg = Path(p4.env('P4CONFIG'))
-        if p4.ignore_file == "unset":
-            return
-        if p4.ignore_file.lower() != ignore_file:
-            secho(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.", fg="yellow")
-            y = confirm(f"Would you like to change the setting in your {cfg} file?")
-            if y:
-                _lines = []
-                lines = []
-                with cfg.open() as f:
-                    _lines = f.readlines()
-                for l in _lines:
-                    if not l.upper().startswith("P4IGNORE"):
-                        lines.append(l)
-                lines.append(f"P4IGNORE={ignore_file}\n")
-                with cfg.open("w") as f:
-                    f.writelines(lines)
-                is_changes = True
-
-        if p4.port.lower() != p4_port:
-            secho(f"Your p4 port should be set to '{p4_port}', not '{p4.port}'.", fg="yellow")
-            y = confirm(f"Would you like to change the setting in your {cfg} file?")
-            if y:
-                _lines = []
-                lines = []
-                with cfg.open() as f:
-                    _lines = f.readlines()
-                for l in _lines:
-                    if not l.upper().startswith("P4PORT"):
-                        lines.append(l)
-                lines.append(f"P4PORT={p4_port}\n")
-                with cfg.open("w") as f:
-                    f.writelines(lines)
-                is_changes = True
-
-        if is_changes:
-            secho("Your p4config file now contains the following:")
-            with cfg.open() as f:
-                lines = f.readlines()
-                for l in lines:
-                    secho(f"{l.strip()}")
-
-            secho("\nYou're all set!", fg="green")
-            exit(0)
-
-    except Exception as e:
+#!/usr/bin/env python
+
+import botocore.session
+from datetime import datetime, timedelta
+import requests
+import click
+import typer
+import configparser
+import logging
+import os
+import sys
+import json
+from jsonpath_rw import parse
+import yaml
+import dateutil
+from functools import wraps
+from urllib.parse import urlparse, urljoin
+import boto3
+from typer import secho, confirm
+from io import BytesIO
+import json
+import botocore
+from loguru import logger
+from pathlib import Path
+from P4 import P4, P4Exception
+from operator import attrgetter, itemgetter
+from . import read_version
+
+log_formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+
+console_handler = logging.StreamHandler()
+console_handler.setFormatter(log_formatter)
+console_handler.setLevel(logging.WARN)
+
+root_logger = logging.getLogger()
+root_logger.setLevel(logging.DEBUG)
+root_logger.addHandler(console_handler)
+
+log = logging.getLogger(__name__)
+
+
+def print_error(*txt):
+    color_print(*txt, color="red")
+
+
+def print_warn(*txt):
+    color_print(*txt, color="yellow")
+
+
+def print_success(*txt):
+    color_print(*txt, color="green")
+
+
+def color_print(*args, **kwargs):
+    color = kwargs.get("color", "reset")
+    for x in args:
+        typer.echo(typer.style(x, fg=color))
+
+
+def get_datafile(filename):
+    p = Path(__file__).parent / "data" / filename
+    with p.open("rt") as f:
+        return f.read()
+
+
+def print_tab(key, val):
+    val_txt = val
+    if isinstance(val, dict):
+        val_txt = ", ".join([f"{k}={v}" for k, v in val.items()])
+    val = typer.style(str(val_txt), bold=True)
+    typer.echo("{0:20}{1}".format(key, val))
+
+
+def print_table(obj):
+    try:
+        for k, v in obj.items():
+            print_tab(k, v)
+    except Exception:
+        typer.echo(obj)
+
+
+def dumps(obj):
+    try:
+        return json.dumps(obj, indent=4, sort_keys=True)
+    except Exception:
+        return repr(obj)
+
+
+def output_pretty_json(dct, keys):
+    ret = ""
+    for k in keys:
+        jsonpath_expr = parse(k)
+        ret = [match.value for match in jsonpath_expr.find(dct)]
+        lst = [""]
+        if ret:
+            if isinstance(ret[0], list) or isinstance(ret[0], dict):
+                lst = yaml.dump(ret[0]).split("\n")
+            else:
+                lst = [str(ret[0])]
+        print_tab(k.split(".")[-1], lst[0])
+        if len(lst) > 1:
+            for v in lst[1:]:
+                print_tab("", v)
+
+
+def find_aws_credentials(profile):
+    """
+    Returns the aws credentials for the specified profile.
+    If no profile is passed in, returns the credentials for the currently selected profile
+
+    Args:
+        profile name
+
+    Returns:
+        Dict containing at least aws_access_key_id, aws_secret_access_key
+
+    Raises:
+        RuntimeError is no default profile or the named profile was not found
+
+    """
+    if not profile:
+        access_key = None
+        secret_key = None
+        token = ""
+        credentials = botocore.session.get_session().get_credentials()
+        if credentials:
+            access_key = credentials.access_key
+            secret_key = credentials.secret_key
+            token = getattr(credentials, "token") or ""
+        if not access_key or not secret_key:
+            raise RuntimeError("No Default AWS profile set")
+
+        return {
+            "aws_access_key_id": access_key,
+            "aws_secret_access_key": secret_key,
+            "aws_session_token": token,
+        }
+
+    folder = os.path.join(os.path.expanduser("~"), ".aws")
+    filename = os.path.join(folder, "credentials")
+    cfg = configparser.ConfigParser()
+    with open(filename) as fp:
+        cfg.readfp(fp)
+        ret = {}
+        if profile not in cfg:
+            raise RuntimeError("No AWS profile '%s' found in %s" % (profile, filename))
+        for key in cfg[profile]:
+            ret[key] = cfg[profile][key]
+    return ret
+
+
+def abort(reason, code=1):
+    """
+    exit with non-zero exit code and write reason for error to stderr.
+    If we are outside a typer context and exception will be raised instead
+    """
+    ctx = click.get_current_context(silent=True)
+    if not ctx:
+        raise Exception(f"Abnormal Termination: {reason}")
+
+    if ctx.obj and ctx.obj.output == "json":
+        ret = {"success": False, "exit_code": code, "message": str(reason)}
+        typer.echo(json.dumps(ret))
+    else:
+        typer.echo(typer.style(str(reason), fg="red"), file=sys.stderr)
+    sys.exit(code)
+
+
+def out(txt, **kw):
+    ctx = click.get_current_context(silent=True)
+    if ctx and ctx.obj and ctx.obj.output == "json":
+        log.info(txt)
+    else:
+        typer.secho(txt, **kw)
+
+
+def success(reason, response=None, **kw):
+    ctx = click.get_current_context(silent=True)
+    if not ctx:
+        print(reason)
+
+    exit_code = 0
+    if ctx.obj and ctx.obj.output == "json":
+        ret = {
+            "success": True,
+            "exit_code": exit_code,
+            "message": str(reason),
+            "response": response,
+        }
+        typer.echo(json.dumps(ret))
+    else:
+        if not kw:
+            kw = {"fg": "white", "bold": True}
+        typer.secho(str(reason), **kw)
+    sys.exit(exit_code)
+
+
+def check_profile(ctx):
+    if not ctx.obj.client:
+        abort("You have no active profile or selected profile is invalid. Run 'unknown profile add [name]'")
+
+
+def fmt_date(dt: str):
+    try:
+        return dateutil.parser.parse(dt).strftime("%Y-%m-%d %H:%M")
+    except:
+        return dt
+
+def check_version():
+    """
+    Check for new version on pypi every 10 minutes
+    """
+    try:
+        version_check_file = Path("~/.unknown-cli-version").expanduser()
+        check_version = True
+        if version_check_file.exists():
+            with version_check_file.open() as f:
+                dt_txt = f.read().strip()
+                try:
+                    dt = dateutil.parser.parse(dt_txt)
+                    if dt >= datetime.utcnow() - timedelta(minutes=10):
+                        check_version = False
+                except:
+                    pass
+
+        if check_version:
+            contents = requests.get("https://pypi.org/pypi/unknown-cli/json").json()
+            v = contents["info"]["version"]
+            my_version = read_version()
+
+            if (v != my_version):
+                secho(f"Version {v} of this tool is available while you are on version {my_version}. Please upgrade using: pip install unknown-cli -U", fg="green", bold=True)
+            else:
+                with version_check_file.open("w") as f:
+                    f.write(f"{fmt_date(datetime.utcnow())}")
+    except:
+        raise
+
+def check_p4config():
+    try:
+        is_changes = False
+        p4 = P4()
+        ignore_file = "s:\\sn2-main\\.p4ignore.txt".lower()
+        p4_port = "ssl:perforce.reginald.cloud:1666"
+        cfg = Path(p4.env('P4CONFIG'))
+        if p4.ignore_file.lower() != ignore_file:
+            secho(f"Your p4ignore file should be set to '{ignore_file}', not '{p4.ignore_file}'.", fg="yellow")
+            y = confirm(f"Would you like to change the setting in your {cfg} file?")
+            if y:
+                _lines = []
+                lines = []
+                with cfg.open() as f:
+                    _lines = f.readlines()
+                for l in _lines:
+                    if not l.upper().startswith("P4IGNORE"):
+                        lines.append(l)
+                lines.append(f"P4IGNORE={ignore_file}\n")
+                with cfg.open("w") as f:
+                    f.writelines(lines)
+                is_changes = True
+
+        if p4.port.lower() != p4_port:
+            secho(f"Your p4 port should be set to '{p4_port}', not '{p4.port}'.", fg="yellow")
+            y = confirm(f"Would you like to change the setting in your {cfg} file?")
+            if y:
+                _lines = []
+                lines = []
+                with cfg.open() as f:
+                    _lines = f.readlines()
+                for l in _lines:
+                    if not l.upper().startswith("P4PORT"):
+                        lines.append(l)
+                lines.append(f"P4PORT={p4_port}\n")
+                with cfg.open("w") as f:
+                    f.writelines(lines)
+                is_changes = True
+
+        if is_changes:
+            secho("Your p4config file now contains the following:")
+            with cfg.open() as f:
+                lines = f.readlines()
+                for l in lines:
+                    secho(f"{l.strip()}")
+
+            secho("\nYou're all set!", fg="green")
+            exit(0)
+
+    except Exception as e:
         pass
```

