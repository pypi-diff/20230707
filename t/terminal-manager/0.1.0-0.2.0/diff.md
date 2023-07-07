# Comparing `tmp/terminal_manager-0.1.0.tar.gz` & `tmp/terminal_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.1.0.tar", last modified: Sun Jul  2 01:39:32 2023, max compression
+gzip compressed data, was "terminal_manager-0.2.0.tar", last modified: Fri Jul  7 07:58:48 2023, max compression
```

## Comparing `terminal_manager-0.1.0.tar` & `terminal_manager-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.986119 terminal_manager-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 terminal_manager-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      703 2023-07-02 01:39:31.981120 terminal_manager-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-01 07:31:05.000000 terminal_manager-0.1.0/README.md
--rw-rw-rw-   0        0        0      732 2023-07-02 01:35:25.000000 terminal_manager-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 01:39:31.986119 terminal_manager-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.732121 terminal_manager-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.831120 terminal_manager-0.1.0/src/terminal_manager/
--rw-rw-rw-   0        0        0     4306 2023-07-02 00:46:10.000000 terminal_manager-0.1.0/src/terminal_manager/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-07-02 00:46:10.000000 terminal_manager-0.1.0/src/terminal_manager/collection.py
--rw-rw-rw-   0        0        0     5192 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/command.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.980121 terminal_manager-0.1.0/src/terminal_manager/default_collections/
--rw-rw-rw-   0        0        0      161 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/const.py
--rw-rw-rw-   0        0        0     3825 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/linux.py
--rw-rw-rw-   0        0        0     3720 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3961 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0       56 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/errors.py
--rw-rw-rw-   0        0        0      645 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/event.py
--rw-rw-rw-   0        0        0      222 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/locker.py
--rw-rw-rw-   0        0        0     8599 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/sensor.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.952120 terminal_manager-0.1.0/src/terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      703 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.112207 terminal_manager-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 terminal_manager-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      703 2023-07-07 07:58:48.111214 terminal_manager-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-01 07:31:05.000000 terminal_manager-0.2.0/README.md
+-rw-rw-rw-   0        0        0      732 2023-07-07 07:55:18.000000 terminal_manager-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:58:48.113207 terminal_manager-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.014633 terminal_manager-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.056408 terminal_manager-0.2.0/src/terminal_manager/
+-rw-rw-rw-   0        0        0     4314 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/collection.py
+-rw-rw-rw-   0        0        0     5232 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/command.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.106224 terminal_manager-0.2.0/src/terminal_manager/default_collections/
+-rw-rw-rw-   0        0        0      161 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/const.py
+-rw-rw-rw-   0        0        0     3846 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/linux.py
+-rw-rw-rw-   0        0        0     4072 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-rw-rw-   0        0        0     3980 2023-07-07 07:51:12.000000 terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-rw-rw-   0        0        0       56 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/errors.py
+-rw-rw-rw-   0        0        0      645 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/event.py
+-rw-rw-rw-   0        0        0      222 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/helpers.py
+-rw-rw-rw-   0        0        0     1346 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/locker.py
+-rw-rw-rw-   0        0        0     8561 2023-07-07 07:51:11.000000 terminal_manager-0.2.0/src/terminal_manager/sensor.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:58:48.096214 terminal_manager-0.2.0/src/terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      703 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-07-07 07:58:48.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-07 07:58:47.000000 terminal_manager-0.2.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.1.0/LICENSE` & `terminal_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.1.0/PKG-INFO` & `terminal_manager-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Control and monitor devices with terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.1.0/pyproject.toml` & `terminal_manager-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/__init__.py` & `terminal_manager-0.2.0/src/terminal_manager/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,33 +57,33 @@
 
         Raises:
             CommandError
         """
         raise CommandError("Not implemented")
 
     async def async_execute_command(
-        self, command: Command, context: dict | None = None
+        self, command: Command, variables: dict | None = None
     ) -> CommandOutput:
         """Execute a command.
 
         Raises:
             CommandError
         """
-        await command.async_execute(self, context)
+        await command.async_execute(self, variables)
 
     async def async_run_action(
-        self, key: str, context: dict | None = None
+        self, key: str, variables: dict | None = None
     ) -> CommandOutput:
         """Run an action.
 
         Raises:
             CommandError
         """
         command = self.get_action_command(key)
-        return await self.async_execute_command(command, context)
+        return await self.async_execute_command(command, variables)
 
     async def async_poll_sensor(
         self, key: str, *, raise_errors: bool = False
     ) -> Sensor:
         """Poll a sensor.
 
         Raises:
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/collection.py` & `terminal_manager-0.2.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.1.0/src/terminal_manager/command.py` & `terminal_manager-0.2.0/src/terminal_manager/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,64 +31,66 @@
 
     def _render(self, string: str) -> str:
         if self.renderer:
             return self.renderer(string)
 
         return string
 
-    def get_context_keys(self, manager: Manager) -> set[str]:
-        """Get context keys."""
+    def get_variable_keys(self, manager: Manager) -> set[str]:
+        """Get variable keys."""
         return {key for key in self.field_keys if key not in manager.sensors_by_key}
 
     def get_sensor_keys(self, manager: Manager) -> set[str]:
         """Get sensor keys."""
         return {key for key in self.field_keys if key in manager.sensors_by_key}
 
-    async def async_format(self, manager: Manager, context: dict | None = None) -> str:
+    async def async_format(
+        self, manager: Manager, variables: dict | None = None
+    ) -> str:
         """Format the string.
 
         Raises:
             CommandError
         """
-        context = {**context} if context else {}
+        variables = {**variables} if variables else {}
         missing_sensor_keys = set()
 
-        for key in self.get_context_keys(manager):
-            if key not in context:
-                raise CommandError(f"Context key {key} is missing")
+        for key in self.get_variable_keys(manager):
+            if key not in variables:
+                raise CommandError(f"Variable {key} is missing")
 
         for key in self.get_sensor_keys(manager):
-            if key not in context:
+            if key not in variables:
                 sensor = manager.get_sensor(key)
                 if sensor.value is not None:
-                    context[sensor.key] = sensor.value
+                    variables[sensor.key] = sensor.value
                 else:
                     missing_sensor_keys.add(sensor.key)
 
         for sensor in await manager.async_poll_sensors(missing_sensor_keys):
             if sensor.value is not None:
-                context[sensor.key] = sensor.value
+                variables[sensor.key] = sensor.value
             else:
                 raise CommandError(f"Value of sensor {sensor.key} is None")
 
         try:
-            return self._render(self.string.format(**context))
+            return self._render(self.string.format(**variables))
         except Exception as exc:
             raise CommandError("Failed to generate string ({exc})") from exc
 
     async def async_execute(
-        self, manager: Manager, context: dict | None = None
+        self, manager: Manager, variables: dict | None = None
     ) -> CommandOutput:
         """Execute.
 
         Raises:
             CommandError
         """
         try:
-            string = await self.async_format(manager, context)
+            string = await self.async_format(manager, variables)
         except CommandError as exc:
             manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
             raise
 
         try:
             output = await manager.async_execute_command_string(string, self.timeout)
         except CommandError as exc:
@@ -120,17 +122,17 @@
         self.key = self.key or name_to_key(self.name)
 
 
 @dataclass
 class SensorCommand(Command):
     """The SensorCommand class."""
 
-    sensors: list[Sensor] = field(default_factory=list)
     _: KW_ONLY
     interval: int | None = None
+    sensors: list[Sensor] = field(default_factory=list)
 
     def __post_init__(self):
         self.last_update: float | None = None
 
     @property
     def sensors_by_key(self) -> dict[str, Sensor]:
         """Sensors by key."""
@@ -159,18 +161,18 @@
         for i, sensor in enumerate(self.sensors):
             if sensor.dynamic:
                 sensor.update(manager, data[i:] or None)
                 return
             sensor.update(manager, data[i] if len(data) > i else None)
 
     async def async_execute(
-        self, manager: Manager, context: dict | None = None
+        self, manager: Manager, variables: dict | None = None
     ) -> CommandOutput:
         try:
-            output = await super().async_execute(manager, context)
+            output = await super().async_execute(manager, variables)
         except CommandError:
             self.update_sensors(manager, None)
             raise
 
         self.update_sensors(manager, output)
 
         return output
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.2.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.1.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,134 @@
 from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..sensor import BinarySensor, NumberSensor, TextSensor
+from ..sensor import NumberSensor, TextSensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
-linux = Collection(
-    "Linux",
+windows_cmd = Collection(
+    "Windows",
     [
         ActionCommand(
-            "/sbin/shutdown -h now",
+            "shutdown -t 0",
             ActionName.TURN_OFF,
             ActionKey.TURN_OFF,
         ),
         ActionCommand(
-            "/sbin/shutdown -r now",
+            "shutdown -r -t 0",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
-        SensorCommand(
-            "cat /sys/class/net/{interface}/address",
-            [
+        # TODO: MAC_ADDRESS
+        # TODO: WOL_SUPPORT
+        # TODO: INTERFACE
+        SensorCommand(
+            "for /f \"skip=1 tokens=*\" %i in ('wmic ComputerSystem get SystemType') "
+            + "do @echo %i",
+            sensors=[
                 TextSensor(
-                    SensorName.MAC_ADDRESS,
-                    SensorKey.MAC_ADDRESS,
-                )
-            ],
-        ),
-        SensorCommand(
-            "cat /sys/class/net/{interface}/device/power/wakeup",
-            [
-                BinarySensor(
-                    SensorName.WOL_SUPPORT,
-                    SensorKey.WOL_SUPPORT,
-                    payload_on="enabled",
-                )
+                    SensorName.MACHINE_TYPE,
+                    SensorKey.MACHINE_TYPE,
+                ),
             ],
         ),
         SensorCommand(
-            "/sbin/route -n | awk '($1 == \"0.0.0.0\") {{print $NF; exit}}'",
-            [
+            "hostname",
+            sensors=[
                 TextSensor(
-                    SensorName.INTERFACE,
-                    SensorKey.INTERFACE,
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
                 )
             ],
         ),
         SensorCommand(
-            "uname -a | awk '{{print $1; print $3; print $2; print $(NF-1);}}'",
-            [
+            "for /f \"skip=1 tokens=*\" %i in ('wmic OS get Caption') do @echo %i",
+            sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
                 ),
+            ],
+        ),
+        SensorCommand(
+            "for /f \"skip=1\" %i in ('wmic OS get Version') do @echo %i",
+            sensors=[
                 TextSensor(
                     SensorName.OS_VERSION,
                     SensorKey.OS_VERSION,
                 ),
+            ],
+        ),
+        SensorCommand(
+            "for /f \"skip=1\" %i in ('wmic OS get OSArchitecture') do @echo %i",
+            sensors=[
                 TextSensor(
-                    SensorName.HOSTNAME,
-                    SensorKey.HOSTNAME,
-                ),
-                TextSensor(
-                    SensorName.MACHINE_TYPE,
-                    SensorKey.MACHINE_TYPE,
+                    SensorName.OS_ARCHITECTURE,
+                    SensorKey.OS_ARCHITECTURE,
                 ),
             ],
         ),
-        # TODO: OS_ARCHITECTURE
         SensorCommand(
-            "free -m | awk 'tolower($0)~/mem/ {{print $2}}'",
-            [
+            "for /f \"skip=1\" %i in ('wmic ComputerSystem get TotalPhysicalMemory') "
+            + "do @echo %i",
+            sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
-                    unit="MB",
-                )
+                    unit="B",
+                ),
             ],
         ),
         SensorCommand(
-            "free -m | awk 'tolower($0)~/mem/ {{print $4}}'",
-            [
+            "for /f \"skip=1\" %i in ('wmic OS get FreePhysicalMemory') do @echo %i",
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
-                    unit="MB",
-                )
+                    unit="kB",
+                ),
             ],
-            interval=30,
         ),
         SensorCommand(
-            "df -m | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
-            [
+            'for /f "tokens=1,2" %i in (\'wmic LogicalDisk get DeviceID^, FreeSpace ^| '
+            + 'findstr ":"\') '
+            + "do @echo %i^|%j",
+            interval=300,
+            sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
-                    unit="MB",
+                    unit="B",
                 )
             ],
-            interval=300,
         ),
         SensorCommand(
-            "top -bn1 | head -n3 | awk 'tolower($0)~/cpu/ "
-            + "{{for(i=1;i<NF;i++){{if(tolower($i)~/cpu/)"
-            + "{{idle=$(i+7); print 100-idle;}}}}}}'",
-            [
+            "for /f \"skip=1\" %i in ('wmic CPU get LoadPercentage') do @echo %i",
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
-                )
+                ),
             ],
-            interval=30,
         ),
         SensorCommand(
-            "echo $(($(cat /sys/class/thermal/thermal_zone0/temp) / 1000))",
-            [
+            "for /f %i in ('wmic /namespace:\\\\root\\wmi "
+            + "PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
+            + "do @set /a x=(%i - 2732) / 10",
+            interval=60,
+            sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
+                    float=True,
                 )
             ],
-            interval=60,
         ),
     ],
 )
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.2.0/src/terminal_manager/default_collections/linux.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,130 @@
 from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
 from ..sensor import BinarySensor, NumberSensor, TextSensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
-windows_cmd = Collection(
-    "Windows",
+linux = Collection(
+    "Linux",
     [
         ActionCommand(
-            "shutdown -t 0",
+            "/sbin/shutdown -h now",
             ActionName.TURN_OFF,
             ActionKey.TURN_OFF,
         ),
         ActionCommand(
-            "shutdown -r -t 0",
+            "/sbin/shutdown -r now",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
-        # TODO: MAC_ADDRESS
-        # TODO: WOL_SUPPORT
-        # TODO: INTERFACE
-        SensorCommand(
-            "for /f \"skip=1 delims=\" %i in ('wmic ComputerSystem get SystemType') "
-            + "do @echo %i",
-            [
+        SensorCommand(
+            "cat /sys/class/net/{interface}/address",
+            sensors=[
                 TextSensor(
-                    SensorName.MACHINE_TYPE,
-                    SensorKey.MACHINE_TYPE,
+                    SensorName.MAC_ADDRESS,
+                    SensorKey.MAC_ADDRESS,
                 )
             ],
         ),
         SensorCommand(
-            "hostname",
-            [
-                TextSensor(
-                    SensorName.HOSTNAME,
-                    SensorKey.HOSTNAME,
+            "file=/sys/class/net/{interface}/device/power/wakeup; "
+            + "[[ ! -f $file ]] || cat $file",
+            sensors=[
+                BinarySensor(
+                    SensorName.WOL_SUPPORT,
+                    SensorKey.WOL_SUPPORT,
+                    payload_on="enabled",
                 )
             ],
         ),
         SensorCommand(
-            "for /f \"skip=1 delims=\" %i in ('wmic OS get Caption') do @echo %i",
-            [
+            "/sbin/route -n | awk '/^0.0.0.0/ {{print $NF}}'",
+            sensors=[
                 TextSensor(
-                    SensorName.OS_NAME,
-                    SensorKey.OS_NAME,
+                    SensorName.INTERFACE,
+                    SensorKey.INTERFACE,
                 )
             ],
         ),
         SensorCommand(
-            "for /f \"skip=1 delims=\" %i in ('wmic OS get Version') do @echo %i",
-            [
+            "uname -a | awk '{{print $1; print $2; print $3; print $(NF-1)}}'",
+            sensors=[
+                TextSensor(
+                    SensorName.OS_NAME,
+                    SensorKey.OS_NAME,
+                ),
+                TextSensor(
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
+                ),
                 TextSensor(
                     SensorName.OS_VERSION,
                     SensorKey.OS_VERSION,
-                )
-            ],
-        ),
-        SensorCommand(
-            "for /f \"skip=1 delims=\" %i in ('wmic OS get OSArchitecture') do @echo %i",
-            [
+                ),
                 TextSensor(
-                    SensorName.OS_ARCHITECTURE,
-                    SensorKey.OS_ARCHITECTURE,
-                )
+                    SensorName.MACHINE_TYPE,
+                    SensorKey.MACHINE_TYPE,
+                ),
             ],
         ),
+        # TODO: OS_ARCHITECTURE
         SensorCommand(
-            # TODO: Should return MB but number is too long
-            "for /f  %i in ('wmic ComputerSystem get TotalPhysicalMemory ^| "
-            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-            + "do set /a mb=%i / 1024 / 1024",
-            [
+            "free -k | awk '/^Mem:/ {{print $2}}'",
+            sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
-                    unit="MB",
+                    unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "for /f  %i in ('wmic OS get FreePhysicalMemory ^| "
-            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-            + "do set /a mb=%i / 1024",
-            [
+            "free -k | awk '/^Mem:/ {{print $4}}'",
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
-                    unit="MB",
+                    unit="KiB",
+                )
+            ],
+        ),
+        SensorCommand(
+            "df -k | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
+            interval=300,
+            sensors=[
+                NumberSensor(
+                    SensorName.FREE_DISK_SPACE,
+                    SensorKey.FREE_DISK_SPACE,
+                    dynamic=True,
+                    separator="|",
+                    unit="KiB",
                 )
             ],
-            interval=30,
         ),
-        # TODO: FREE_DISK_SPACE
         SensorCommand(
-            "for /f \"skip=1\" %i in ('wmic CPU get LoadPercentage') do @echo %i",
-            [
+            "top -bn1 | awk 'NR<4 && tolower($0)~/cpu/ {{print 100-$8}}'",
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
                 )
             ],
-            interval=30,
         ),
         SensorCommand(
-            "for /f  %i in ('wmic /namespace:\\\\root\\wmi "
-            + "PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature ^| "
-            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-            + "do set /a mb=(%i - 2732) / 10",
-            [
+            "echo $(($(cat /sys/class/thermal/thermal_zone0/temp) / 1000))",
+            interval=60,
+            sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
+                    float=True,
                 )
             ],
-            interval=60,
         ),
     ],
 )
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.2.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..sensor import BinarySensor, NumberSensor, TextSensor
+from ..sensor import NumberSensor, TextSensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
 windows_ps = Collection(
     "Windows (Power Shell)",
     [
         ActionCommand(
             "Stop-Computer -Force",
@@ -22,15 +22,15 @@
         # TODO: WOL_SUPPORT
         # TODO: INTERFACE
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
             + "Select Name, SystemType;"
             + "$x.Name;"
             + "$x.SystemType;",
-            [
+            sensors=[
                 TextSensor(
                     SensorName.HOSTNAME,
                     SensorKey.HOSTNAME,
                 ),
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
@@ -39,15 +39,15 @@
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_OperatingSystem | "
             + "Select Caption, Version, OSArchitecture;"
             + "$x.Caption;"
             + "$x.Version;"
             + "$x.OSArchitecture;",
-            [
+            sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
                 ),
                 TextSensor(
                     SensorName.OS_VERSION,
                     SensorKey.OS_VERSION,
@@ -57,73 +57,74 @@
                     SensorKey.OS_ARCHITECTURE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
             + "Select TotalPhysicalMemory;"
-            + "[math]::Round($x.TotalPhysicalMemory/1MB);",
-            [
+            + "$x.TotalPhysicalMemory;",
+            sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
-                    unit="MB",
+                    unit="B",
                 )
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_OperatingSystem | "
             + "Select FreePhysicalMemory;"
-            + "[math]::Round($x.FreePhysicalMemory/1KB);",
-            [
+            + "$x.FreePhysicalMemory;",
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
-                    unit="MB",
+                    unit="kB",
                 )
             ],
-            interval=30,
         ),
         SensorCommand(
             "Get-CimInstance Win32_LogicalDisk | "
             + "Select DeviceID, FreeSpace | ForEach-Object "
-            + '{{$_.DeviceID+"|"+[math]::Round($_.FreeSpace/1MB)}}',
-            [
+            + '{{$_.DeviceID + "|" + $_.FreeSpace}}',
+            interval=300,
+            sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
-                    unit="MB",
+                    unit="B",
                 )
             ],
-            interval=300,
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_Processor | "
             + "Select LoadPercentage;"
             + "$x.LoadPercentage;",
-            [
+            interval=30,
+            sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
                 )
             ],
-            interval=30,
         ),
         SensorCommand(
             "$x = Get-CimInstance msacpi_thermalzonetemperature "
             + '-namespace "root/wmi" | '
             + "Select CurrentTemperature;"
             + "($x.CurrentTemperature - 2732) / 10;",
-            [
+            interval=60,
+            sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
+                    float=True,
                 )
             ],
-            interval=60,
         ),
     ],
 )
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager/event.py` & `terminal_manager-0.2.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.1.0/src/terminal_manager/locker.py` & `terminal_manager-0.2.0/src/terminal_manager/locker.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.1.0/src/terminal_manager/sensor.py` & `terminal_manager-0.2.0/src/terminal_manager/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-import re
 from collections.abc import Callable
 from copy import deepcopy
 from dataclasses import KW_ONLY, dataclass, field
+import re
 from typing import TYPE_CHECKING, Any
 
 from .event import Event
 from .helpers import name_to_key
 
 if TYPE_CHECKING:
     from . import Manager
@@ -58,19 +58,19 @@
         self.child_sensors.append(child)
         self.on_child_added.notify(self, child)
 
     def _remove_child(self, child: Sensor) -> None:
         self.child_sensors.remove(child)
         self.on_child_removed.notify(self, child)
 
-    def _render(self, value_string: str) -> str:
+    def _render(self, data: str) -> str:
         if self.renderer:
-            return self.renderer(value_string)
+            data = self.renderer(data)
 
-        return value_string
+        return data.strip()
 
     def _convert(self, value_string: str) -> Any:
         return value_string
 
     def _validate(self, value: Any) -> None:
         ...
 
@@ -81,31 +81,31 @@
             return
 
         try:
             value_string = self._render(data)
             value = self._convert(value_string)
             self._validate(value)
         except Exception as exc:  # pylint: disable=broad-except
-            manager.logger.warning("%s: %s => %s", manager.name, self.key, exc)
+            manager.logger.debug("%s: %s => %s", manager.name, self.key, exc)
             self.value = None
             return
 
         self.value = self.last_known_value = value
         manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
 
     def _update_child_sensors(self, manager: Manager, data: list[str] | None) -> None:
         if data is None:
             for child in self.child_sensors:
                 child.update(manager, None)
             return
 
         dynamic_data_list = [
-            DynamicData(self.name, self.key, *(field.strip() for field in row))
-            for row in (line.split(self.separator, 2) for line in data)
-            if len(row) >= 2
+            DynamicData(self.name, self.key, *fields)
+            for fields in (line.split(self.separator, 2) for line in data)
+            if len(fields) >= 2
         ]
 
         dynamic_data_by_key = {
             dynamic_data.key: dynamic_data for dynamic_data in dynamic_data_list
         }
 
         for key, dynamic_data in dynamic_data_by_key.items():
@@ -116,15 +116,15 @@
                 child.name = dynamic_data.name
                 child.dynamic = False
                 self._add_child(child)
 
         for child in self.child_sensors:
             if child.key in dynamic_data_by_key:
                 dynamic_data = dynamic_data_by_key[child.key]
-                child.update(manager, dynamic_data.value_string)
+                child.update(manager, dynamic_data.data)
             else:
                 self._remove_child(child)
 
     def update(self, manager: Manager, data: Any) -> None:
         """Update and notify `on_update` subscribers."""
         if self.dynamic:
             self.value = self.last_known_value = None
@@ -146,15 +146,15 @@
         self._validate(value)
         command = self._get_control_command(value)
 
         if command is None or value == self.value:
             return
 
         await manager.async_execute_command(
-            command, context={"id": self.id, "value": value}
+            command, variables={"id": self.id, "value": value}
         )
 
 
 @dataclass
 class TextSensor(Sensor):
     """The TextSensor class."""
 
@@ -182,31 +182,31 @@
 
 
 @dataclass
 class NumberSensor(Sensor):
     """The NumberSensor class."""
 
     _: KW_ONLY
-    integer: bool = False
+    float: bool = False
     minimum: int | float | None = None
     maximum: int | float | None = None
 
     def _convert(self, value_string: str) -> int | float:
-        if self.integer:
-            return int(float(value_string))
+        if self.float:
+            return float(value_string)
 
-        return float(value_string)
+        return int(float(value_string))
 
     def _validate(self, value: Any) -> None:
-        if self.integer and not isinstance(value, int):
-            raise TypeError(f"{value} is {type(value)} and not {int}")
-
-        if not self.integer and not isinstance(value, float):
+        if self.float and not isinstance(value, float):
             raise TypeError(f"{value} is {type(value)} and not {float}")
 
+        if not self.float and not isinstance(value, int):
+            raise TypeError(f"{value} is {type(value)} and not {int}")
+
         if self.minimum and value < self.minimum:
             raise ValueError(f"{value} is smaller then {self.minimum}")
 
         if self.maximum and value > self.maximum:
             raise ValueError(f"{value} is bigger then {self.maximum}")
 
 
@@ -265,16 +265,16 @@
 class DynamicData:
     """The DynamicData class."""
 
     def __init__(
         self,
         parent_name: str | None,
         parent_key: str,
-        data_id: str,
-        data_value_string: str,
-        data_name: str | None = None,
+        id_field: str,
+        data_field: str,
+        name_field: str | None = None,
     ) -> None:
-        name = data_name or data_id
-        self.id = data_id
+        self.id = id_field.strip()
+        name = name_field.strip() if name_field else self.id
         self.key = f"{parent_key}_{name_to_key(name)}"
         self.name = f"{parent_name} {name}" if parent_name else name
-        self.value_string = data_value_string
+        self.data = data_field
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.2.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Control and monitor devices with terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.1.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.2.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

