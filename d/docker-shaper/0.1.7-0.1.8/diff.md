# Comparing `tmp/docker_shaper-0.1.7.tar.gz` & `tmp/docker_shaper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.7.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.8.tar", max compression
```

## Comparing `docker_shaper-0.1.7.tar` & `docker_shaper-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,15 @@
--rw-r--r--   0        0        0     2481 2023-07-03 06:21:36.838441 docker_shaper-0.1.7/Readme.md
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/common.py
--rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0    27912 2023-07-04 15:49:46.449395 docker_shaper-0.1.7/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     6580 2023-07-04 15:23:50.424596 docker_shaper-0.1.7/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/static/bootstrap.css
--rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.7/docker_shaper/static/normalize.css
--rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.7/docker_shaper/static/pills.css
--rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.7/docker_shaper/static/style.css
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0     1170 2023-07-03 13:04:26.635859 docker_shaper-0.1.7/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.7/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0      956 2023-07-04 11:41:27.395858 docker_shaper-0.1.7/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.7/docker_shaper/templates/images.html
--rw-r--r--   0        0        0     5474 2023-07-04 15:11:26.966906 docker_shaper-0.1.7/docker_shaper/utils.py
--rw-r--r--   0        0        0     2259 2023-07-04 15:59:07.639134 docker_shaper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 docker_shaper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3006 2023-07-05 08:01:08.591249 docker_shaper-0.1.8/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/cli.py
+-rw-r--r--   0        0        0    31566 2023-07-07 15:54:26.006882 docker_shaper-0.1.8/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     8739 2023-07-07 15:54:25.814886 docker_shaper-0.1.8/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-07-05 08:01:08.599249 docker_shaper-0.1.8/docker_shaper/static/bootstrap.css
+-rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-07 06:45:33.419474 docker_shaper-0.1.8/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      321 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0      956 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      309 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0     5474 2023-07-06 14:45:56.181912 docker_shaper-0.1.8/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2259 2023-07-07 15:54:16.227094 docker_shaper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 docker_shaper-0.1.8/PKG-INFO
```

### Comparing `docker_shaper-0.1.7/docker_shaper/cli.py` & `docker_shaper-0.1.8/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.7/docker_shaper/dynamic.py` & `docker_shaper-0.1.8/docker_shaper/dynamic.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
 """Functionality that might change during runtime
 """
 import asyncio
 import logging
 import os
 import re
+import signal
+import sys
 import time
+import traceback
+from collections import Counter
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
+from pathlib import Path
 from subprocess import CalledProcessError
 from typing import MutableMapping, MutableSequence, Optional, Tuple, Union
 
 from aiodocker import Docker, DockerError
 from dateutil import tz
 from flask_table import Col, Table
 from quart import render_template, request, url_for
 
-from docker_shaper.utils import aimpatient, impatient, process_output, watchdog
+from docker_shaper.utils import impatient, process_output, watchdog
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.dynamic")
 
 
@@ -85,22 +90,22 @@
     )
     return f"{tds//86400:02d}d" f":{tds//3600%24:02d}h" f":{tds//60%60:02d}m"
 
 
 def date_str(date: datetime) -> str:
     if not date:
         return "--"
-    return (datetime.fromtimestamp(date) if isinstance(date, int) else date).strftime(
+    return (date if isinstance(date, datetime) else datetime.fromtimestamp(date)).strftime(
         "%Y.%m.%d-%H:%M:%S"
     )
 
 
-def date_from(timestamp: str) -> datetime:
+def date_from(timestamp: Union[int, float, str]) -> datetime:
     try:
-        if isinstance(timestamp, int):
+        if isinstance(timestamp, (int, float)):
             return datetime.fromtimestamp(timestamp)
 
         if timestamp[-1] == "Z":
             return (
                 datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
                 .replace(tzinfo=tz.tzutc())
                 .astimezone(tz.tzlocal())
@@ -184,14 +189,15 @@
         ("image", "push"),
         ("image", "tag"),
         ("image", "untag"),
         ("image", "save"),
         ("image", "delete"),
         ("image", "prune"),
         ("volume", "prune"),
+        ("volume", "create"),
         ("container", "prune"),
         ("network", "prune"),
         ("builder", "prune"),
     }, f"{len(uid)=} {(object_type, operator)}"
     return (
         int(
             datetime.strptime(
@@ -226,31 +232,31 @@
             uid,
         )
     elif object_type in {"network", "builder"}:
         return
     elif (object_type, operator) in {
         ("image", "untag"),
         ("image", "prune"),
+        ("image", "push"),
         ("image", "delete"),
-
         ("container", "exec_create:"),
         ("container", "exec_start:"),
         ("container", "exec_die"),
         ("container", "kill"),
         ("container", "start"),
         ("container", "attach"),
         ("container", "die"),
+        ("container", "top"),
         ("container", "destroy"),
         ("container", "prune"),
         ("container", "stop"),
         ("container", "archive-path"),
-
         ("network", "connect"),
         ("network", "disconnect"),
-
+        ("volume", "create"),
         ("volume", "mount"),
         ("volume", "unmount"),
         ("volume", "destroy"),
     }:
         return
     else:
         log().warning("unknown type/operator %s %s", object_type, operator)
@@ -283,34 +289,34 @@
         global_state.last_referenced[effective_ident] = [
             0,
             expiration_age_from_ident(effective_ident, global_state),
         ]
 
     # increase last reference date if applicable
     global_state.last_referenced[effective_ident][0] = max(
-        global_state.last_referenced[effective_ident][0], timestamp
+        global_state.last_referenced[effective_ident][0] or 0, timestamp
     )
 
 
 def expiration_age_from_ident(ident: str, global_state: GlobalState) -> int:
     if is_uid(ident):
-        return global_state.expiration_ages["tag_unknown"]
+        return global_state.expiration_ages["tag_default"]
 
     effective_ident = unique_ident(ident)
 
     matching_rules = tuple(
         (regex, age)
         for regex, age in global_state.tag_rules.items()
         if re.match(regex, effective_ident)
     )
 
     if len(matching_rules) == 1:
         return matching_rules[0][1]
     if not matching_rules:
-        log().warn("No rule found for %s", ident)
+        log().warn("No rule found for %r", ident)
     else:
         log().error("Multiple rules found for %s:", ident)
         for rule in matching_rules:
             log().error("  %s:", rule[0])
 
     return global_state.expiration_ages["tag_unknown"]
 
@@ -373,22 +379,24 @@
             "org.tribe29.cmk_version",
         )
         for w in l.split()
         if not (w.startswith("sha256") or len(w) == 64)
     )
 
 
-@aimpatient
 async def dump_global_state(global_state):
     global_state.counter += 1
-    print(global_state.intervals)
-    print(f"counter: {global_state.counter}")
-    print(f"images: {len(global_state.images)}")
-    print(f"containers: {len(global_state.containers)}")
-    print(f"tag_rules: {len(global_state.tag_rules)}")
+    print(f"STATE: {', '.join('='.join(map(str, i)) for i in global_state.intervals.items())}")
+    print(f"STATE: frame counter: {global_state.counter}")
+    print(f"STATE: images: {len(global_state.images)}")
+    print(f"STATE: containers: {len(global_state.containers)}")
+    print(f"STATE: tag_rules: {len(global_state.tag_rules)}")
+    print(
+        f"STATE: tasks: {', '.join('/'.join(map(str, i)) for i in Counter(t.get_coro().__name__ for t in asyncio.all_tasks()).items())}"
+    )
 
 
 class BaseTable(Table):
     allow_sort = True
     classes = ["table", "table-striped"]
 
     def __init__(self, endpoint, items):
@@ -425,23 +433,22 @@
             now_timestamp = now.timestamp()
             created_timestamp = date_from(image["created_at"]).timestamp()
 
             def coloured_ident(ident):
                 is_expired, last_referenced, expiration_age = expired(
                     ident, global_state, now_timestamp, created_timestamp
                 )
-                if is_expired:
-                    return (
-                        f"<div class='text-danger'>{ident} ({age_str(now, last_referenced)})</div>"
-                    )
-                return f"<div class='text-success'>{ident} ({age_str(now, last_referenced)})</div>"
+                return (
+                    f"<div class='text-{'danger' if is_expired else 'success'}'>"
+                    f"{ident} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)})</div>"
+                )
 
             return {
                 "short_id": coloured_ident(image["short_id"]),
-                "tags": "".join(map(coloured_ident, image["tags"])),
+                "tags": "".join(map(coloured_ident, image["tags"] or [])),
                 "created_at": date_str(image["created_at"]),
                 "age": age_str(now, date_from(image["created_at"])),
                 # "last_referenced": last_referenced_str(image["short_id"]),
                 # "class": "text-danger" if would_cleanup_image(image, now, global_state) else "text-success",
             }
 
         return ImageTable(
@@ -486,16 +493,16 @@
             endpoint,
             items=sorted(
                 (
                     {
                         "short_id": cnt["short_id"],
                         "name": cnt["name"],
                         "image": short_id(cnt["image"]) if is_uid(cnt["image"]) else cnt["image"],
-                        "mem_usage": mem_stats.get("usage", 0),
-                        "cpu": cpu_perc(cpu_stats, last_cpu_stats),
+                        "mem_usage": f"{(mem_stats.get('usage', 0)>>20)}MiB",
+                        "cpu": f"{int(cpu_perc(cpu_stats, last_cpu_stats) * 1000) / 10}%",
                         "cmd": " ".join(cnt["show"]["Config"]["Cmd"])[:100],
                         "job": jobname_from(
                             cnt["show"]["HostConfig"]["Binds"]
                             or list(cnt["show"]["Config"]["Volumes"] or [])
                         ),
                         "created_at": date_str(date_from(cnt["show"]["Created"])),
                         "started_at": date_str(
@@ -534,69 +541,73 @@
         "container_count": len(global_state.containers),
         "image_count": len(global_state.images),
         "extra_links": global_state.extra_links,
         "intervals": global_state.intervals,
         "hostname": global_state.hostname,
         "switches": global_state.switches,
         "expiration_ages": global_state.expiration_ages,
+        "self_pid": os.getpid(),
     }
 
 
-@aimpatient
 async def container_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_containers",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
-            reverse=request.args.get("sort_direction_containers", "asc") == "desc",
+            reverse=request.args.get("sort_direction_containers", "desc") == "desc",
         ),
     )
 
 
-@aimpatient
 async def image_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
-        "containers.html",
+        "images.html",
         meta=meta_info(global_state),
         images_html=ImageTable.html_from(
             "route_images",
             global_state,
             sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
     )
 
 
-@aimpatient
 async def dashboard(global_state):
     return await render_template(
         "dashboard.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_dashboard",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
-            reverse=request.args.get("sort_direction_containers", "asc") == "desc",
+            reverse=request.args.get("sort_direction_containers", "desc") == "desc",
         ),
         images_html=ImageTable.html_from(
             "route_dashboard",
             global_state,
             sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
-        messages=global_state.messages,
+        messages=[(date_str(m[0]), m[1], m[2]) for m in global_state.messages],
     )
 
 
-@aimpatient
+async def generic_html(generic, global_state):
+    if generic == "favicon.ico":
+        return ""
+
+    raise RuntimeError(f"not found: {generic}")
+
+
 async def print_container_stats(global_state):
     hostname = open("/etc/hostname").read().strip()
     stats = [
         {
             "short_id": cnt["short_id"],
             "name": cnt["name"],
             "usage": mem_stats.get("usage", 0),
@@ -683,15 +694,15 @@
     containers = global_state.containers
     try:
         container_info = containers[container.id]
         container_info["container"] = container
         container_info["short_id"] = (short_id_ := short_id(container.id))
         container_info["show"] = (show := await container.show())
         container_info["name"] = (name := show["Name"][1:])
-        container_info["image"] = (image := show["Config"]["Image"])
+        container_info["image"] = show["Config"]["Image"]
 
         # wrong - other things could have happened since..
         # register_reference(image, date_from(show["Created"]).timestamp(), global_state)
 
         log().info(">> new container: %s %s", short_id_, name)
 
         async for stats in container.stats():
@@ -702,35 +713,33 @@
     except DockerError as exc:
         log().error("DockerError: %s", exc)
     finally:
         log().info("<< container terminated: %s %s", short_id_, name)
         del containers[container.id]
 
 
-# @aimpatient
 async def watch_images(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl images..")
+    await asyncio.sleep(1)
+    # raise RuntimeError("XXX")
     for image in await docker_client.images.list(all=True):
         # log().debug("  found image %s", image["Id"])
         if True or image["Id"] not in global_state.images:
             global_state.images.setdefault(image["Id"], {}).update(
                 {
-                    # TODO: name (also for registration)
                     "short_id": short_id(image["Id"]),
-                    "name": image["Id"],
                     "created_at": image["Created"],
-                    "tags": image["RepoTags"],
+                    "tags": [tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"],
                     "size": image["Size"],
                     "parent": short_id(image["ParentId"]),
                 }
             )
 
 
-@aimpatient
 async def watch_containers(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl containers..")
     for container in await docker_client.containers.list(all=True):
         log().debug("  found container %s", container.id)
         if container.id not in global_state.containers:
             global_state.containers[container.id] = {}
@@ -758,79 +767,153 @@
             now - date_from(show["State"]["StartedAt"]).timestamp()
             > global_state.expiration_ages["container_running"]
         )
     return False
 
 
 def expired_idents(image, now, global_state: GlobalState):
+    log().debug("check expiration for image %s, tags=%s", image["short_id"], image["tags"])
     created_timestamp = int(date_from(image["created_at"]).timestamp())
-    for tag in image["tags"]:
+    for tag in image["tags"] or []:
         if expired(tag, global_state, now, created_timestamp)[0]:
             yield tag
     if expired(image["short_id"], global_state, now, created_timestamp)[0]:
         yield image["short_id"]
 
 
 async def image_from(docker_client: Docker, ident: str) -> bool:
     with suppress(DockerError):
         return await docker_client.images.get(ident)
     return None
 
 
-@aimpatient
 async def cleanup(docker_client: Docker, global_state):
     log().info("Cleanup!..")
-    now = int(datetime.now().timestamp())
 
-    # we could go through docker_client.containers, too, but to be more consistent, we work
-    # on one structure only
-    # also, we have to create a list we can operate on, in order to not modify the structure, we're
-    # iterating
-    for container_info in list(
-        filter(
-            lambda cnt: would_cleanup_container(cnt, now, global_state),
-            global_state.containers.values(),
-        )
-    ):
-        if not global_state.switches.get("remove_container"):
-            log().info(f"skip removal of container {container_info['short_id']}")
-            continue
-        report(
-            global_state,
-            "warn",
-            f"force removing container {container_info['short_id']}",
-            container_info["container"],
-        )
-        await container_info["container"].delete(force=True, v=True)
-
-    for image_info in global_state.images.values():
-        for ident in expired_idents(image_info, now, global_state):
-            if not global_state.switches.get("remove_images"):
-                log().info(f"skip removal of image/tag {ident}")
+    report(global_state, "info", f"start cleanup", None)
+    try:
+        now = int(datetime.now().timestamp())
+        # we could go through docker_client.containers, too, but to be more consistent, we work
+        # on one structure only
+        # also, we have to create a list we can operate on, in order to not modify the structure, we're
+        # iterating
+        for container_info in list(
+            filter(
+                lambda cnt: would_cleanup_container(cnt, now, global_state),
+                global_state.containers.values(),
+            )
+        ):
+            if not global_state.switches.get("remove_container"):
+                log().info(f"skip removal of container {container_info['short_id']}")
                 continue
-            report(global_state, "info", f"remove image/tag {ident}", None)
-            try:
-                await docker_client.images.delete(ident)
-            except DockerError as exc:
-                log().error("Could not delete image %s, error was %s", ident, exc)
-
-    for ident in [
-        ident for ident in global_state.images if not await image_from(docker_client, ident)
-    ]:
-        log().warning("reference to image %s has not been cleaned up, I'll do it now..", ident)
-        del global_state.images[ident]
+            report(
+                global_state,
+                "warn",
+                f"force removing container {container_info['short_id']}",
+                container_info["container"],
+            )
+            await container_info["container"].delete(force=True, v=True)
 
-    log().info("Cleanup done!")
+        for image_info in global_state.images.values():
+            for ident in expired_idents(image_info, now, global_state):
+                if not global_state.switches.get("remove_images"):
+                    log().info(f"skip removal of image/tag {ident}")
+                    continue
+                report(global_state, "info", f"remove image/tag {ident}", None)
+                try:
+                    await docker_client.images.delete(ident)
+                except DockerError as exc:
+                    log().error("Could not delete image %s, error was %s", ident, exc)
+
+        for ident in [
+            ident for ident in global_state.images if not await image_from(docker_client, ident)
+        ]:
+            log().warning("reference to image %s has not been cleaned up, I'll do it now..", ident)
+            del global_state.images[ident]
+    finally:
+        log().info("cleanup done!")
+        report(global_state, "info", f"cleanup done", None)
 
 
 @impatient
 def report(global_state, msg_type, message: str, extra):
     # TODO: cleanup
     # TODO: persist
     log().info(message)
     global_state.messages.insert(0, (datetime.now().timestamp(), msg_type, message, str(extra)))
+    global_state.messages = global_state.messages[
+        : global_state.additional_values.get("message_history_size", 100)
+    ]
 
 
 @impatient
 def reconfigure(global_state: GlobalState) -> None:
+    setup_introspection()
     for ident, reference in global_state.last_referenced.items():
         reference[1] = expiration_age_from_ident(ident, global_state)
+
+
+def increase_loglevel(*_):
+    """Become one level more verbose.
+    If level is already DEBUG we go back to WARNING.
+    """
+    try:
+        new_level = {
+            logging.WARNING: logging.INFO,
+            logging.INFO: logging.DEBUG,
+            logging.DEBUG: logging.WARNING,
+        }.get(log().level) or logging.INFO
+
+        log().setLevel(new_level)
+        logging.getLogger("docker-shaper.server").setLevel(new_level)
+        level = {
+            logging.CRITICAL: "CRITICAL",
+            logging.ERROR: "ERROR",
+            logging.WARNING: "WARNING",
+            logging.INFO: "INFO",
+            logging.DEBUG: "DEBUG",
+        }[new_level]
+        print(f"increase_loglevel to {level}", file=sys.stderr)
+    except Exception:
+        log().exception("Could not fully write application stack trace")
+
+
+def print_stacktrace_on_signal(sig, frame):
+    """interrupt running process, and provide a python prompt for
+    interactive debugging.
+    see http://stackoverflow.com/questions/132058
+       "showing-the-stack-trace-from-a-running-python-application"
+    """
+    try:
+        print(f"signal {sig} received - print stack trace", file=sys.stderr)
+
+        def print_stack_frame(stack_frame, file):
+            for _f in traceback.format_stack(stack_frame):
+                for _l in _f.splitlines():
+                    print(_l, file=file)
+
+        def print_stack_frames(file):
+            print("++++++ MAIN ++++++++", file=file)
+            print_stack_frame(frame, file)
+            for task in asyncio.all_tasks():
+                print(f"++++++ {task.get_coro().__name__} ++++++++", file=file)
+                for stack in task.get_stack(limit=1000):
+                    print_stack_frame(stack, file)
+
+        print_stack_frames(sys.stderr)
+        with open(Path("~/.docker_shaper/traceback.log").expanduser(), "w") as trace_file:
+            print_stack_frames(trace_file)
+    except Exception:
+        log().exception("Could not fully write application stack trace")
+
+
+def setup_introspection():
+    """Install signal handlers for some debug stuff"""
+
+    def setup_signal(sig, func, msg):
+        signal.signal(sig, func)
+        signal.siginterrupt(sig, False)
+        sig_str = {signal.SIGUSR1: "USR1", signal.SIGUSR2: "USR2"}.get(sig, sig)
+        print(f"Run `kill -{sig_str} {os.getpid()}` to {msg}", file=sys.stderr)
+
+    setup_signal(signal.SIGUSR1, increase_loglevel, "increase log level")
+    setup_signal(signal.SIGUSR2, print_stacktrace_on_signal, "print stacktrace")
```

### Comparing `docker_shaper-0.1.7/docker_shaper/server.py` & `docker_shaper-0.1.8/docker_shaper/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,162 +1,178 @@
 #!/usr/bin/env python3
 
 import asyncio
 import importlib
 import logging
-import time
 from contextlib import suppress
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_file_location
+from itertools import count
 from pathlib import Path
 
 from aiodocker import Docker
-from quart import Quart
+from quart import Quart, Response, redirect
 
 from docker_shaper import dynamic
 from docker_shaper.utils import fs_changes, read_process_output, watchdog
 
 CONFIG_FILE = Path("~/.docker_shaper/config.py").expanduser()
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.server")
 
 
-@watchdog
-async def print_container_stats(global_state):
+async def schedule_print_container_stats(global_state):
     while True:
         try:
-            await dynamic.print_container_stats(global_state)
-            await asyncio.sleep(global_state.intervals.get("container_stats"), 1)
-        except Exception:
+            await asyncio.ensure_future(dynamic.print_container_stats(global_state))
+            await asyncio.sleep(global_state.intervals.get("container_stats", 1))
+        except Exception as exc:
             log().exception("Unhandled exception caught!")
+            dynamic.report(
+                global_state, "error", f"exception in container_stats scheduler: {exc}", exc
+            )
             await asyncio.sleep(5)
 
 
-@watchdog
-async def print_state(global_state):
+async def schedule_print_state(global_state):
     while True:
         try:
-            await dynamic.dump_global_state(global_state)
+            await asyncio.ensure_future(dynamic.dump_global_state(global_state))
             await asyncio.sleep(global_state.intervals.get("state", 1))
-        except Exception:
+        except Exception as exc:
             log().exception("Unhandled exception caught!")
+            dynamic.report(global_state, "error", f"exception in state scheduler: {exc}", exc)
             await asyncio.sleep(5)
 
 
-@watchdog
-async def watch_containers(global_state):
+async def schedule_watch_containers(global_state):
     # TODO: also use events to register
     try:
         docker = Docker()
         while True:
             try:
-                await dynamic.watch_containers(docker, global_state)
+                await asyncio.ensure_future(dynamic.watch_containers(docker, global_state))
                 await asyncio.sleep(global_state.intervals.get("container_update", 1))
-            except Exception:
+            except Exception as exc:
                 log().exception("Unhandled exception caught!")
+                dynamic.report(
+                    global_state, "error", f"exception in container_update scheduler: {exc}", exc
+                )
                 await asyncio.sleep(5)
     finally:
         await docker.close()
 
 
-@watchdog
-async def watch_images(global_state):
+async def schedule_watch_images(global_state):
     # TODO: also use events to register
     try:
         docker = Docker()
         while True:
             try:
-                await dynamic.watch_images(docker, global_state)
+                await asyncio.ensure_future(dynamic.watch_images(docker, global_state))
                 await asyncio.sleep(global_state.intervals.get("image_update", 1))
-            except Exception:
+            except Exception as exc:
                 log().exception("Unhandled exception caught!")
+                dynamic.report(
+                    global_state, "error", f"exception in image_update scheduler: {exc}", exc
+                )
+                await asyncio.sleep(5)
+    finally:
+        await docker.close()
+
+
+async def schedule_cleanup(global_state):
+    try:
+        docker = Docker()
+        while True:
+            try:
+                for second in count():
+                    if (
+                        interval := global_state.intervals.get("cleanup", 3600)
+                    ) and second > interval:
+                        break
+                    if (interval - second) % 10 == 0:
+                        log().debug("cleanup: %s seconds to go.." % (interval - second))
+                    await asyncio.sleep(1)
+                await asyncio.ensure_future(dynamic.cleanup(docker, global_state))
+            except Exception as exc:
+                log().exception("Unhandled exception caught in cleanup()!")
+                dynamic.report(global_state, "error", f"exception in cleanup scheduler: {exc}", exc)
                 await asyncio.sleep(5)
     finally:
         await docker.close()
 
 
 def load_config(path, global_state):
     spec = spec_from_file_location("dynamic_config", path)
     if not (spec and spec.loader):
         raise RuntimeError("Could not load")
     module = module_from_spec(spec)
-    print(module)
-    # assert module
+    assert module
     # assert isinstance(spec.loader, SourceFileLoader)
     loader: SourceFileLoader = spec.loader
     loader.exec_module(module)
     try:
         module.modify(global_state)
         dynamic.reconfigure(global_state)
     except AttributeError:
         log().warning("File %s does not provide a `modify(global_state)` function")
 
 
-@watchdog
 async def watch_fs_changes(global_state):
     CONFIG_FILE.parent.mkdir(parents=True, exist_ok=True)
     async for changed_file in fs_changes(
         Path(dynamic.__file__).parent, CONFIG_FILE.parent, timeout=1
     ):
         log().info("file %s changed - reload module", changed_file)
         try:
             if changed_file == Path(dynamic.__file__):
                 importlib.reload(dynamic)
+                dynamic.setup_introspection()
             elif changed_file == CONFIG_FILE:
                 load_config(CONFIG_FILE, global_state)
-
-        except Exception:
+        except Exception as exc:
             log().exception("Reloading dynamic part failed!")
+            dynamic.report(global_state, "error", f"exception in module reload: {exc}", exc)
             await asyncio.sleep(5)
     assert False
 
 
-@watchdog
 async def handle_docker_events(global_state):
     try:
         docker = Docker()
         async for line in read_process_output("docker events"):
             try:
-                await dynamic.handle_docker_event_line(docker, global_state, line)
-            except Exception:
+                await asyncio.ensure_future(
+                    dynamic.handle_docker_event_line(docker, global_state, line)
+                )
+            except Exception as exc:
                 log().exception("Unhandled exception caught!")
-                await asyncio.sleep(5)
-    finally:
-        await docker.close()
-
-
-@watchdog
-async def cleanup(global_state):
-    try:
-        docker = Docker()
-        while True:
-            try:
-                await dynamic.cleanup(docker, global_state)
-                await asyncio.sleep(global_state.intervals.get("cleanup", 3600))
-            except Exception:
-                log().exception("Unhandled exception caught in cleanup()!")
+                dynamic.report(
+                    global_state, "error", f"exception in docker event watcher: {exc}", exc
+                )
                 await asyncio.sleep(5)
     finally:
         await docker.close()
 
 
 def no_serve():
     global_state = dynamic.GlobalState()
     load_config(CONFIG_FILE, global_state)
     with suppress(KeyboardInterrupt, BrokenPipeError):
         asyncio.ensure_future(watch_fs_changes(global_state))
-        asyncio.ensure_future(print_container_stats(global_state))
-        asyncio.ensure_future(print_state(global_state))
-        asyncio.ensure_future(watch_containers(global_state))
-        asyncio.ensure_future(watch_images(global_state))
+        asyncio.ensure_future(schedule_print_container_stats(global_state))
+        asyncio.ensure_future(schedule_print_state(global_state))
+        asyncio.ensure_future(schedule_watch_containers(global_state))
+        asyncio.ensure_future(schedule_watch_images(global_state))
         asyncio.ensure_future(handle_docker_events(global_state))
-        asyncio.ensure_future(cleanup(global_state))
+        asyncio.ensure_future(schedule_cleanup(global_state))
         asyncio.get_event_loop().run_forever()
 
 
 def serve():
     """"""
     app = Quart(__name__)
     app.config["TEMPLATES_AUTO_RELOAD"] = True
@@ -174,35 +190,51 @@
 
     @app.route("/shutdown")
     def route_shutdown():
         app.terminator.set()
         return "Server shutting down..."
 
     @app.route("/containers")
-    async def route_containers():
-        return await dynamic.container_table_html(global_state)
+    async def route_containers(site):
+        try:
+            return await dynamic.container_table_html(site, global_state)
+        except Exception as exc:
+            log().exception("Unhandled exception in containers")
+            dynamic.report(global_state, "error", f"exception in containers: {exc}", exc)
 
     @app.route("/images")
     async def route_images():
         return await dynamic.image_table_html(global_state)
 
-    @app.route("/", methods=["GET"])
+    @app.route("/dashboard")
     async def route_dashboard():
-        return await dynamic.dashboard(global_state)
+        try:
+            return await dynamic.dashboard(global_state)
+        except Exception as exc:
+            log().exception("Unhandled exception in dashboard")
+            dynamic.report(global_state, "error", f"exception in dashboard: {exc}", exc)
+
+    @app.route("/<generic>")
+    async def route_generic(generic):
+        return await dynamic.generic_html(generic, global_state)
+
+    @app.route("/")
+    async def root() -> Response:
+        return redirect("dashboard")
 
     @app.before_serving
     async def create_db_pool():
         asyncio.ensure_future(self_destroy())
         asyncio.ensure_future(watch_fs_changes(global_state))
         # asyncio.ensure_future(print_container_stats(global_state))
-        asyncio.ensure_future(print_state(global_state))
-        asyncio.ensure_future(watch_containers(global_state))
-        asyncio.ensure_future(watch_images(global_state))
+        asyncio.ensure_future(schedule_print_state(global_state))
+        asyncio.ensure_future(schedule_watch_containers(global_state))
+        asyncio.ensure_future(schedule_watch_images(global_state))
         asyncio.ensure_future(handle_docker_events(global_state))
-        asyncio.ensure_future(cleanup(global_state))
+        asyncio.ensure_future(schedule_cleanup(global_state))
 
     app.terminator = asyncio.Event()
     app.run(
         host="0.0.0.0",
         port=5432,
         debug=False,
         use_reloader=False,
```

### Comparing `docker_shaper-0.1.7/docker_shaper/static/bootstrap.css` & `docker_shaper-0.1.8/docker_shaper/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.7/docker_shaper/templates/base.html` & `docker_shaper-0.1.8/docker_shaper/templates/base.html`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,18 @@
      <table class="table table-striped"><tr>
       <td>Host: <b>{{meta.hostname}}</b></td>
       <td></td>
       {% for link in meta.extra_links %}
           <td><a href="{{ meta.extra_links[link] }}">{{link}}</a></td>
           <td></td>
       {% endfor %}
+    </tr><tr>
+
+      <td>configuration at <tt><b>~/.docker_shaper/config.py</b></tt></td>
+      <td>backtrace: <tt>`<b>kill -USR2 {{meta.self_pid}}</b>`</tt></td>
 
     </tr><tr>
       <td>intervals:</td>
 
       {% for interval in meta.intervals %}
           <td>{{interval}} = <b>{{meta.intervals[interval]}}s</b>  </td><td></td>
       {% endfor %}
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
 
 
-Host: {{meta.hostname}}                                 {{link}}
-intervals:              {{interval}} = {{meta.intervals
-                        [interval]}}s
-Dashboard                                               Containers  Images
+Host: {{meta.hostname}}                                    {{link}}
+configuration at           backtrace: `kill -USR2 {
+~/.docker_shaper/config.py {meta.self_pid}}`
+intervals:                 {{interval}} = {{meta.intervals
+                           [interval]}}s
+Dashboard                                                  Containers  Images
 {% block content %}{% endblock %}
```

### Comparing `docker_shaper-0.1.7/docker_shaper/templates/dashboard.html` & `docker_shaper-0.1.8/docker_shaper/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.7/docker_shaper/utils.py` & `docker_shaper-0.1.8/docker_shaper/utils.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.7/pyproject.toml` & `docker_shaper-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.7"
+version = "0.1.8"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
```

### Comparing `docker_shaper-0.1.7/PKG-INFO` & `docker_shaper-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.7
+Version: 0.1.8
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,20 +18,22 @@
 Project-URL: Repository, https://github.com/Checkmk/checkmk-dev-tools
 Description-Content-Type: text/markdown
 
 # Docker Shaper
 
 This repository includes scripts/tools for Checkmk developers.
 
+
 ## Installation
 
 ```sh
 [<PYTHON> -m] pip[3] install [--user] [--upgrade] docker-shaper
 ```
 
+
 ## Usage
 
 ```
 docker-shaper serve`
 ```
 Navigate to e.g. http://build-fra-003:5432/
 
@@ -41,23 +43,37 @@
 ### Todo
 
 - [x] pip package
 - [x] Quart interface
 - [x] bring in dockermon
 - [x] auto update
 - [x] outsource config
-- [ ] bring in dgcd
-- [ ] bring in list_volumes
-- [ ] increase/decrease logging
-- [ ] new: untag certain tags
-- [ ] new: container cleanup
+- [x] bring in dgcd
+- [x] new: untag certain tags
+- [x] new: container cleanup
+- [x] Fix `none` image lookup
+- [ ] Exceptions to messages
+- [ ] Clip / persist messages
+- [ ] Instructions to readme
+- [ ] List unmatched / overmatched tags
+- [ ] bring in `list_volumes` (volume monitoring)
+- [ ] Add volumes list (with recent owners)
+- [ ] Increase/decrease logging via web / signal
+- [ ] Links to `delete` / `remove`
+- [ ] Links to jobs
+- [ ] Skipable `wait`
+- [ ] Link: inspect
+- [ ] Link: cleanup (images/containers) now
+- [ ] Graph: cpu / containers (idle/up)
+- [ ] Authenticate (at least if we can modify behavior, like stopping/removing images/containers)
 
 
 ### Setup
 
+
 ### Prerequisites
 
 * Python 3.8.10
 * `poetry`
 * `pre-commit`
 
 
@@ -67,15 +83,17 @@
 cd checkmk_ci
 pre-commit install
 # if you need a specific version of Python inside your dev environment
 poetry env use ~/.pyenv/versions/3.8.10/bin/python3
 poetry install
 ```
 
+
 ### Workflow
+
 poetry config repositories.checkmk https://upload.pypi.org/legacy/
 poetry config pypi-token.checkmk pypi-
 
 pip3 install --user --upgrade docker-shaper
 ~/.local/bin/docker-shaper server
 
 poetry run mypy docker_shaper
```

