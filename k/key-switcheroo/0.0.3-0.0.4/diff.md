# Comparing `tmp/key_switcheroo-0.0.3.tar.gz` & `tmp/key_switcheroo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.3.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.4.tar", max compression
```

## Comparing `key_switcheroo-0.0.3.tar` & `key_switcheroo-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.3/README.md
--rw-r--r--   0        0        0      540 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/__init__.py
--rw-r--r--   0        0        0     1746 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/custom_keygen.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     2288 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/server/__init__.py
--rw-r--r--   0        0        0     2917 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/server/data_stores.py
--rwxr-xr-x   0        0        0     1093 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/server/retrieve_public_keys.py
--rw-r--r--   0        0        0     5324 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/server/server.py
--rw-r--r--   0        0        0     1934 2023-07-05 19:39:01.733785 key_switcheroo-0.0.3/switcheroo/util.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.4/README.md
+-rw-r--r--   0        0        0      540 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/__init__.py
+-rw-r--r--   0        0        0     4590 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/custom_keygen.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/publisher/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/publisher/__main__.py
+-rw-r--r--   0        0        0     4162 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/publisher/key_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.4/switcheroo/server/__init__.py
+-rw-r--r--   0        0        0     2987 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/data_stores.py
+-rwxr-xr-x   0        0        0     1101 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/retrieve_public_keys.py
+-rw-r--r--   0        0        0     5324 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/server/server.py
+-rw-r--r--   0        0        0     1934 2023-07-07 03:34:18.196449 key_switcheroo-0.0.4/switcheroo/util.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.4/PKG-INFO
```

### Comparing `key_switcheroo-0.0.3/pyproject.toml` & `key_switcheroo-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.3/switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.4/switcheroo/publisher/__main__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.3/switcheroo/server/data_stores.py` & `key_switcheroo-0.0.4/switcheroo/server/data_stores.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 "Data stores that specifies where a Server stores its keys"
 import os
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 import boto3
 from switcheroo.util import get_user_path
+from switcheroo.custom_keygen import KeyGen
 
 
 class DataStore(ABC):
     "A server uses a DataStore to get public keys from somewhere."
 
     @abstractmethod
     def get_sshd_config_line(self):
@@ -80,15 +81,15 @@
             return self._dir
         return self._dir.name
 
     def get_sshd_config_line(self) -> str:
         return f"local {self.dir}"
 
     def delete_key(self, host: str, user: str):
-        os.remove(f"{self.dir}/{host}/{user}")
+        os.remove(f"{self.dir}/{host}/{user}/{KeyGen.PRIVATE_KEY_NAME}")
 
     def __enter__(self):
         if isinstance(self._dir, str):
             if not os.path.isdir(self.dir):
                 os.mkdir(self.dir)
         else:
             self._dir.__enter__()
```

### Comparing `key_switcheroo-0.0.3/switcheroo/server/retrieve_public_keys.py` & `key_switcheroo-0.0.4/switcheroo/server/retrieve_public_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import socket
 import os
 import boto3
 
 
 def get_public_keys_local(connecting_user: str, ssh_home_dir: str) -> str:
     host_name = socket.getfqdn()
-    key_dir = f"{ssh_home_dir}/{host_name}"
-    key_path = f"{key_dir}/{connecting_user}-cert.pub"
+    key_dir = f"{ssh_home_dir}/{host_name}/{connecting_user}"
+    key_path = f"{key_dir}/key-cert.pub"
     if not os.path.isdir(key_dir):
         os.makedirs(key_dir)
     if not os.path.exists(key_path):
         return ""
     with open(key_path, mode="rt", encoding="utf-8") as key_file:
         return key_file.read()
 
 
 def get_public_keys_s3(connecting_user: str, bucket_name: str) -> str:
     host_name = socket.getfqdn()
     s3_client = boto3.client("s3")
     response = s3_client.get_object(
-        Bucket=bucket_name, Key=f"{host_name}/{connecting_user}-cert.pub"
+        Bucket=bucket_name, Key=f"{host_name}/{connecting_user}/key-cert.pub"
     )
     ssh_key = response["Body"].read().decode()
     return ssh_key
 
 
 if __name__ == "__main__":
     CONNECTING_USER = sys.argv[1]
```

### Comparing `key_switcheroo-0.0.3/switcheroo/server/server.py` & `key_switcheroo-0.0.4/switcheroo/server/server.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.3/switcheroo/util.py` & `key_switcheroo-0.0.4/switcheroo/util.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.3/PKG-INFO` & `key_switcheroo-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

