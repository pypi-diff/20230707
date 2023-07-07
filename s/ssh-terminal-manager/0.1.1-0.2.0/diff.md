# Comparing `tmp/ssh_terminal_manager-0.1.1.tar.gz` & `tmp/ssh_terminal_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.1.1.tar", last modified: Sun Jul  2 02:35:25 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.2.0.tar", last modified: Fri Jul  7 08:15:04 2023, max compression
```

## Comparing `ssh_terminal_manager-0.1.1.tar` & `ssh_terminal_manager-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:35:25.599848 ssh_terminal_manager-0.1.1/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      841 2023-07-02 02:35:25.597845 ssh_terminal_manager-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.1.1/README.md
--rw-rw-rw-   0        0        0      859 2023-07-02 02:22:26.000000 ssh_terminal_manager-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 02:35:25.600848 ssh_terminal_manager-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 02:35:25.548850 ssh_terminal_manager-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 02:35:25.564845 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager/
--rw-rw-rw-   0        0        0    10344 2023-07-02 00:46:10.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager/__init__.py
--rw-rw-rw-   0        0        0      347 2023-07-02 00:46:10.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:35:25.595848 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      841 2023-07-02 02:35:25.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-02 02:35:25.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:35:25.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-02 02:35:25.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-02 02:35:25.000000 ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.632968 ssh_terminal_manager-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      841 2023-07-07 08:15:04.631968 ssh_terminal_manager-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.2.0/README.md
+-rw-rw-rw-   0        0        0      859 2023-07-07 08:02:41.000000 ssh_terminal_manager-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:15:04.632968 ssh_terminal_manager-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.565963 ssh_terminal_manager-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.590971 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/
+-rw-rw-rw-   0        0        0     9844 2023-07-07 07:51:11.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0      347 2023-07-07 07:51:11.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:15:04.629967 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      841 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-07 08:15:04.000000 ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.1.1/LICENSE` & `ssh_terminal_manager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.1.1/PKG-INFO` & `ssh_terminal_manager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.1.1
+Version: 0.2.0
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.1.1/pyproject.toml` & `ssh_terminal_manager-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with SSH terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,14 +21,14 @@
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "python-slugify >= 4.0.1",
-  "terminal-manager >= 0.1.0",
+  "terminal-manager >= 0.2.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.1.1/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.2.0/src/ssh_terminal_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,40 +25,40 @@
 )
 from terminal_manager.default_collections import ActionKey, SensorKey
 import wakeonlan
 
 from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
 
 _LOGGER = logging.getLogger(__name__)
-_TEST_COMMAND = Command("")
+_TEST_COMMAND = Command("echo ''")
 
 DEFAULT_PORT = 22
 DEFAULT_PING_TIMEOUT = 4
 DEFAULT_SSH_TIMEOUT = 4
 DEFAULT_ADD_HOST_KEYS = False
 DEFAULT_ALLOW_TURN_OFF = False
 
-IS_ONLINE = "is_online"
-IS_CONNECTED = "is_connected"
+ONLINE = "online"
+CONNECTED = "connected"
 
 
 class CustomRejectPolicy(paramiko.MissingHostKeyPolicy):
     """Custom reject policy for ssh client."""
 
     def missing_host_key(
         self, client: paramiko.SSHClient, hostname: str, key: paramiko.PKey
     ) -> None:
         raise SSHHostKeyUnknownError("Host key is unknown")
 
 
 class State:
     """The State class."""
 
-    is_online: bool = False
-    is_connected: bool = False
+    online: bool = False
+    connected: bool = False
 
     def __init__(self, manager: SSHManager) -> None:
         self._manager = manager
         self.on_change = Event()
 
     def update(self, name, value) -> None:
         """Update."""
@@ -154,52 +154,42 @@
     @property
     def machine_type(self) -> str | None:
         """Machine type."""
         if sensor := self.sensors_by_key.get(SensorKey.MACHINE_TYPE):
             return sensor.last_known_value
 
     def _execute_command_string(self, string: str, timeout: int) -> CommandOutput:
-        if not self.state.is_connected:
+        if not self.state.connected:
             raise CommandError("Not connected")
 
         try:
             stdin, stdout, stderr = self._client.exec_command(
                 string,
-                get_pty=True,  # required to be able to interrupt the command
-                timeout=float(timeout),  # channel timeout, used to be self.ssh_timeout
+                timeout=float(timeout),
             )
         except Exception as exc:
             self._disconnect()
             raise CommandError("Disconnected before execution") from exc
 
         try:
             return CommandOutput(
                 time(),
-                [line.strip() for line in stdout.readlines()],
-                [line.strip() for line in stderr.readlines()],
+                ["".join(line.splitlines()) for line in stdout],
+                ["".join(line.splitlines()) for line in stderr],
                 stdout.channel.recv_exit_status(),
             )
-        except TimeoutError:
-            pass
+        except TimeoutError as exc:
+            stdin.channel.close()
+            raise CommandError(f"Timeout ({timeout} s)") from exc
         except Exception as exc:
             self._disconnect()
             raise CommandError("Disconnected during execution") from exc
 
-        try:
-            # Interrupt the command if it takes longer then timeout
-            # https://github.com/fabric/fabric/blob/2.0/fabric/runners.py#L47-L59
-            stdin.channel.send("\x03")
-        except Exception as exc:
-            self._disconnect()
-            raise CommandError(f"Disconnected after timeout ({exc})") from exc
-
-        raise CommandError("Command interrupted after timeout")
-
     def _connect(self) -> None:
-        if self.state.is_connected:
+        if self.state.connected:
             return
 
         try:
             self._client.connect(
                 self.host,
                 self.port,
                 self.username,
@@ -214,22 +204,22 @@
         except paramiko.AuthenticationException as exc:
             self._disconnect()
             raise SSHAuthError("SSH authentication failed") from exc
         except Exception as exc:
             self._disconnect()
             raise SSHConnectError("SSH connection failed") from exc
 
-        self.state.update(IS_CONNECTED, True)
+        self.state.update(CONNECTED, True)
 
     def _disconnect(self) -> None:
-        if not self.state.is_connected:
+        if not self.state.connected:
             return
 
         self._client.close()
-        self.state.update(IS_CONNECTED, False)
+        self.state.update(CONNECTED, False)
 
         for command in self.sensor_commands:
             command.update_sensors(self, None)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
@@ -238,15 +228,15 @@
         return await loop.run_in_executor(
             None, self._execute_command_string, string, timeout
         )
 
     async def async_connect(self) -> None:
         """Connect the SSH client.
 
-        Set `state.is_connected` to `True` and update all
+        Set `state.connected` to `True` and update all
         sensor commands if successful, otherwise disconnect
         and raise an error.
 
         Raises:
             SSHHostKeyUnknownError
             SSHAuthError
             SSHConnectError
@@ -259,30 +249,30 @@
                 await self.async_execute_command(command)
             except CommandError:
                 pass
 
     async def async_disconnect(self) -> None:
         """Disconnect the SSH client.
 
-        Set `state.is_connected` to `False` and
+        Set `state.connected` to `False` and
         update all sensor commands with `None`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
     async def async_update_state(self, *, raise_errors: bool = False) -> None:
         """Update state.
 
         Raises:
             OfflineError (`raise_errors`)
             SSHHostKeyUnknownError
             SSHAuthError
             SSHConnectError (`raise_errors`)
         """
-        if self.state.is_connected:
+        if self.state.connected:
             try:
                 await self.async_execute_command(_TEST_COMMAND)
                 return
             except CommandError:
                 pass
 
         try:
@@ -290,32 +280,32 @@
                 self.host,
                 count=1,
                 timeout=self.ping_timeout,
                 privileged=False,
             )
         except Exception as exc:  # pylint: disable=broad-except
             self.logger.debug("%s: Ping request failed (%s)", self.name, exc)
-            self.state.update(IS_ONLINE, False)
+            self.state.update(ONLINE, False)
         else:
-            self.state.update(IS_ONLINE, host.is_alive)
+            self.state.update(ONLINE, host.is_alive)
 
-        if not self.state.is_online:
+        if not self.state.online:
             if raise_errors:
                 raise OfflineError("Host is offline")
             return
 
         try:
             await self.async_connect()
         except SSHConnectError:
             if raise_errors:
                 raise
 
     async def async_turn_on(self) -> None:
         """Turn the host on."""
-        if self.state.is_online:
+        if self.state.online:
             return
 
         wakeonlan.send_magic_packet(self.mac_address)
 
     async def async_turn_off(self) -> None:
         """Turn the host off.
```

### Comparing `ssh_terminal_manager-0.1.1/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.2.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.1.1
+Version: 0.2.0
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

