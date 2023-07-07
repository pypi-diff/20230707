# Comparing `tmp/key_switcheroo-0.0.4.tar.gz` & `tmp/key_switcheroo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.4.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.5.tar", max compression
```

## Comparing `key_switcheroo-0.0.4.tar` & `key_switcheroo-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.4/README.md
--rw-r--r--   0        0        0      540 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/__init__.py
--rw-r--r--   0        0        0     4590 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/custom_keygen.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     4162 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/server/__init__.py
--rw-r--r--   0        0        0     2987 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/data_stores.py
--rwxr-xr-x   0        0        0     1101 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/retrieve_public_keys.py
--rw-r--r--   0        0        0     5324 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/server.py
--rw-r--r--   0        0        0     1934 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/util.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.5/README.md
+-rw-r--r--   0        0        0      678 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/__init__.py
+-rw-r--r--   0        0        0     3164 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/custom_keygen.py
+-rw-r--r--   0        0        0       77 2023-07-07 03:40:51.516287 key_switcheroo-0.0.5/switcheroo/data_store/__init__.py
+-rw-r--r--   0        0        0     3211 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/data_store/data_stores.py
+-rw-r--r--   0        0        0     2939 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/data_store/s3.py
+-rw-r--r--   0        0        0      311 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/exceptions.py
+-rw-r--r--   0        0        0     1410 2023-07-07 03:40:51.516287 key_switcheroo-0.0.5/switcheroo/paths.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/publisher/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/publisher/__main__.py
+-rw-r--r--   0        0        0     1617 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/publisher/key_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/server/__init__.py
+-rwxr-xr-x   0        0        0     1915 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/server/__main__.py
+-rw-r--r--   0        0        0     5045 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/server/server.py
+-rw-r--r--   0        0        0     2658 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/util.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.5/PKG-INFO
```

### Comparing `key_switcheroo-0.0.4/switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.5/switcheroo/publisher/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from argparse import ArgumentParser
-from switcheroo.publisher.key_publisher import LocalPublisher, S3Publisher
+from switcheroo.publisher.key_publisher import Publisher, LocalPublisher, S3Publisher
 
 
 def create_argument_parser() -> ArgumentParser:
     argument_parser = ArgumentParser(
         prog="key_publisher",
         description="Creates public/private SSH keys and publishes "
         + "the public key either locally or to S3 (default is S3)",
@@ -25,19 +25,23 @@
         required=False,
         help="If s3 is selected, the bucket name to store the key in",
     )
 
     return argument_parser
 
 
-if __name__ == "__main__":
+def main():
     parser = create_argument_parser()
     args = parser.parse_args()
-
+    publisher: Publisher | None = None
     if args.datastore == "local":  # If the user chose to store the public key locally
         publisher = LocalPublisher(args.hostname, args.user)
-        publisher.publish_new_key()
     else:  # If the user chose to store the public key on S3 or chose to default to S3
         if args.bucket is None:
             parser.error("The s3 option requires a bucket name!")
         publisher = S3Publisher(args.bucket, args.hostname, args.user)
-        publisher.publish_new_key()
+    assert publisher is not None
+    publisher.publish_new_key()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `key_switcheroo-0.0.4/switcheroo/server/server.py` & `key_switcheroo-0.0.5/switcheroo/server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 "SSH Server"
 from typing import Callable
 import os
 import asyncio
 import pathlib
+from pathlib import Path
 import subprocess
 from asyncio.subprocess import Process
+from getpass import getuser
 from tempfile import NamedTemporaryFile
-from switcheroo.server.data_stores import DataStore
+from switcheroo.data_store import DataStore
 from switcheroo.util import get_open_port
-from switcheroo.util import get_user_path, get_username
 
 
 class Server:
     "Wrapper for SSH Server. Takes a DataStore to determine where to look for keys"
 
     def __init__(
         self,
         data_store: DataStore,
         port: int | Callable[[], int] = get_open_port,
-        authorized_key_command_executing_user: str = get_username(),
+        authorized_key_command_executing_user: str = getuser(),
     ):
         if callable(port):
             port = port()
         self.port = port
         self.data_store = data_store
         self.authorized_key_command_executing_user = (
             authorized_key_command_executing_user
         )
         self.process: Process | None = None
+        self.log_file = Path.home() / "ssh" / "sshd_log"
 
     async def start(self):
-        user_path = get_user_path()
+        user_path = Path.home()
+        self.log_file.parent.mkdir(parents=True, exist_ok=True)
+        self.log_file.touch(exist_ok=True)
         python_executable = f"{os.getcwd()}/.venv/bin/python"
-        target_script = "/ssh_key_switcheroo/retrieve_public_keys.py"
-        ky_cmnd = f"{python_executable} {target_script} %u {self.data_store.get_sshd_config_line()}"
-        python_executable = f"{os.getcwd()}/.venv/bin/python"
-        target_script = "/ssh_key_switcheroo/retrieve_public_keys.py"
+        target_script = "/ssh_key_switcheroo/__main__.py"
         ky_cmnd = f"{python_executable} {target_script} %u {self.data_store.get_sshd_config_line()}"
         config: list[str] = [
             "LogLevel DEBUG3",
             f"Port {self.port}",
-            f"HostKey {user_path}/etc/ssh/ssh_host_rsa_key",
-            f"PidFile {user_path}/var/run/sshd.pid",
+            f"HostKey {str(user_path)}/etc/ssh/ssh_host_rsa_key",
+            f"PidFile {str(user_path)}/var/run/sshd.pid",
             "UsePAM yes",
             "AuthorizedKeysFile none",
             f"AuthorizedKeysCommand {ky_cmnd}",
             f"AuthorizedKeysCommand {ky_cmnd}",
             f"AuthorizedKeysCommandUser {self.authorized_key_command_executing_user}",
             "PasswordAuthentication no",
             "KbdInteractiveAuthentication no",
@@ -54,19 +55,19 @@
         ]
         # Configuration is emitted as a temporary file to launch sshd
         with NamedTemporaryFile(mode="w+t") as temp_config:
             for option in config:
                 temp_config.write(f"{option}\n")
             temp_config.file.flush()
             command: str = (
-                f'/usr/sbin/sshd -f"{temp_config.name}" -E{user_path}/ssh/sshd_log'
+                f'/usr/sbin/sshd -f"{temp_config.name}" -E{str(self.log_file)}'
             )
             task: Process = await asyncio.create_subprocess_shell(
                 command,
-                user=get_username(),
+                user=getuser(),
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.PIPE,
             )
             self.process = task
             await self.process.wait()
 
     async def stop(self):
@@ -78,46 +79,43 @@
             await asyncio.sleep(1)
         kill_task = await asyncio.create_subprocess_shell(
             f"fuser -k {self.port}/tcp",
             stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.DEVNULL,
         )
         await kill_task.wait()
-        log_file = f"{get_user_path()}/ssh/sshd_log"
-        os.remove(log_file)
+        self.log_file.unlink()
 
     @property
     async def logs(self) -> list[str]:
         "Returns the sshd logs"
-        log_file = f"{get_user_path()}/ssh/sshd_log"
-        with open(log_file, mode="rt", encoding="utf-8") as logs:
+        with open(self.log_file, mode="rt", encoding="utf-8") as logs:
             return logs.readlines()
 
     @staticmethod
     def __setup_host_keys():
-        user_path = get_user_path()
-        ssh_dir = f"{user_path}/etc/ssh"
-        if not os.path.isdir(ssh_dir):
-            os.mkdir(ssh_dir)
-            subprocess.run("ssh-keygen -A -f ~", shell=True, check=True)
+        user_path = Path.home()
+        ssh_dir = user_path / "etc" / "ssh"
+        ssh_dir.mkdir(parents=True, exist_ok=True)
+        subprocess.run("ssh-keygen -A -f ~", shell=True, check=True)
 
     @staticmethod
     def __setup_pid_file():
-        user_path = get_user_path()
-        run_dir = f"{user_path}/var/run"
-        if not os.path.isdir(run_dir):
-            os.mkdir(run_dir)
+        user_path = Path.home()
+        run_dir = user_path / "var" / "run"
+        run_dir.mkdir(exist_ok=True, parents=True)
 
     def __setup_authorized_keys_script(self):
         parent_dir = pathlib.Path(__file__).parent.resolve()
         app_data_dir = "/ssh_key_switcheroo"
-        python_retrieval_script_path = f"{parent_dir}/retrieve_public_keys.py"
-        target_path = f"{app_data_dir}/retrieve_public_keys.py"
+        python_retrieval_script_path = f"{parent_dir}/__main__.py"
+        target_path = f"{app_data_dir}/__main__.py"
         if not os.path.exists(app_data_dir):
             subprocess.run(f"sudo mkdir {app_data_dir}", check=True, shell=True)
+        # Will change to rsync
         subprocess.run(
             f"sudo cp {python_retrieval_script_path} {target_path}",
             shell=True,
             check=True,
         )
         subprocess.run(
             f"sudo chgrp 0 {python_retrieval_script_path}", check=True, shell=True
@@ -126,15 +124,14 @@
             f"sudo chmod 755 {python_retrieval_script_path}", check=True, shell=True
         )
 
     async def __aenter__(self):
         self.__setup_host_keys()
         self.__setup_pid_file()
         self.__setup_authorized_keys_script()
-        self.__setup_authorized_keys_script()
         self.data_store.__enter__()
         await self.start()
         return self
 
     async def __aexit__(self, one, two, three):
         await self.stop()
         self.data_store.__exit__(None, None, None)
```

### Comparing `key_switcheroo-0.0.4/PKG-INFO` & `key_switcheroo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

