# Comparing `tmp/macrostrat_app_frame-1.0.4.tar.gz` & `tmp/macrostrat_app_frame-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_app_frame-1.0.4.tar", max compression
+gzip compressed data, was "macrostrat_app_frame-1.0.5.tar", max compression
```

## Comparing `macrostrat_app_frame-1.0.4.tar` & `macrostrat_app_frame-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0       59 2023-05-16 20:02:34.747827 macrostrat_app_frame-1.0.4/macrostrat/app_frame/__init__.py
--rw-r--r--   0        0        0      996 2023-05-17 18:01:29.460021 macrostrat_app_frame-1.0.4/macrostrat/app_frame/compose.py
--rw-r--r--   0        0        0     5365 2023-05-17 18:22:38.350306 macrostrat_app_frame-1.0.4/macrostrat/app_frame/control_command.py
--rw-r--r--   0        0        0     3780 2023-05-15 21:31:33.953594 macrostrat_app_frame-1.0.4/macrostrat/app_frame/core.py
--rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.4/macrostrat/app_frame/follow_logs.py
--rw-r--r--   0        0        0      481 2023-05-17 18:22:48.550034 macrostrat_app_frame-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-16 20:02:34.747827 macrostrat_app_frame-1.0.5/macrostrat/app_frame/__init__.py
+-rw-r--r--   0        0        0      996 2023-05-17 18:01:29.460021 macrostrat_app_frame-1.0.5/macrostrat/app_frame/compose.py
+-rw-r--r--   0        0        0     5519 2023-07-07 12:38:48.417842 macrostrat_app_frame-1.0.5/macrostrat/app_frame/control_command.py
+-rw-r--r--   0        0        0     3798 2023-07-07 12:38:48.418358 macrostrat_app_frame-1.0.5/macrostrat/app_frame/core.py
+-rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.5/macrostrat/app_frame/follow_logs.py
+-rw-r--r--   0        0        0      507 2023-07-07 12:38:48.419018 macrostrat_app_frame-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-07-07 12:38:48.419670 macrostrat_app_frame-1.0.5/test_app/Caddyfile
+-rw-r--r--   0        0        0      333 2023-07-07 12:38:48.420347 macrostrat_app_frame-1.0.5/test_app/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-07 12:38:48.421038 macrostrat_app_frame-1.0.5/test_app/docker-compose.yaml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.5/PKG-INFO
```

### Comparing `macrostrat_app_frame-1.0.4/macrostrat/app_frame/compose.py` & `macrostrat_app_frame-1.0.5/macrostrat/app_frame/compose.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.4/macrostrat/app_frame/control_command.py` & `macrostrat_app_frame-1.0.5/macrostrat/app_frame/control_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,61 +91,69 @@
     ctx: Context, container: str = typer.Argument(None), force_recreate: bool = False
 ):
     """Start the :app_name: server and follow logs."""
     app = ctx.find_object(Application)
     if app is None:
         raise ValueError("Could not find application config")
     if container is None:
-        container = ""
+        _container = ""
 
-    compose("build", container)
+    compose("build", _container)
 
     sleep(0.1)
 
     res = compose(
         "up",
         "--no-start",
         "--remove-orphans",
         "--force-recreate" if force_recreate else "",
-        container,
+        _container,
     )
     if res.returncode != 0:
         app.info(
             "One or more containers did not build successfully, aborting.",
             style="red bold",
         )
         sys.exit(res.returncode)
     else:
         app.info("All containers built successfully.", style="green bold")
+    print()
 
+    # Get list of currently running containers
     running_containers = check_status(app.name, app.command_name)
 
     app.info("Starting :app_name: server...", style="bold")
     compose("start")
+    print()
 
-    for _container, command in app.restart_commands.items():
-        if _container in running_containers:
-            app.info(f"Reloading {_container}...", style="bold")
-            compose("exec", _container, command)
+    run_restart_commands(app, running_containers)
 
-    res = follow_logs_with_reloader(app, container)
+    res = follow_logs_with_reloader(app, _container)
     if res == Result.RESTART:
         app.info("Restarting :app_name: server...", style="bold")
         ctx.invoke(up, ctx, container)
     elif res == Result.EXIT:
         app.info("Stopping :app_name: server...", style="bold")
         ctx.invoke(down, ctx)
     elif res == Result.CONTINUE:
         app.info(
             "[bold]Detaching from logs[/bold] [dim](:app_name: will continue to run)[/dim]",
             style="bold",
         )
         return
 
 
+def run_restart_commands(app, running_containers):
+    for c, command in app.restart_commands.items():
+        if c in running_containers:
+            app.info(f"Reloading {c}...", style="bold")
+            compose("exec", c, command)
+    print()
+
+
 def down(ctx: Context):
     """Stop all :app_name: services."""
     app = ctx.find_object(Application)
     if app is None:
         raise ValueError("Could not find application config")
     app.info("Stopping :app_name: server...", style="bold")
     compose("down", "--remove-orphans")
```

### Comparing `macrostrat_app_frame-1.0.4/macrostrat/app_frame/core.py` & `macrostrat_app_frame-1.0.5/macrostrat/app_frame/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         root_dir: Path | Callable[[Path], Path] = Path.cwd(),
         compose_files: ComposeFilesDependency = [],
         env: EnvironmentDependency = {},
         load_dotenv: bool | Path | list[Path] = False,
     ):
         self.name = name
         self.command_name = command_name or name.lower()
-        self.project_prefix = project_prefix or name.lower()
+        self.project_prefix = project_prefix or name.lower().replace(" ", "_")
         self.console = Console()
         self.restart_commands = restart_commands
         self.app_module = app_module
         self._dotenv_cfg = load_dotenv
 
         # Root dir and compose files can be specified using dependency injection.
         if callable(root_dir):
```

### Comparing `macrostrat_app_frame-1.0.4/macrostrat/app_frame/follow_logs.py` & `macrostrat_app_frame-1.0.5/macrostrat/app_frame/follow_logs.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.4/PKG-INFO` & `macrostrat_app_frame-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-app-frame
-Version: 1.0.4
+Version: 1.0.5
 Summary: A control script framework for containerized applications.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

