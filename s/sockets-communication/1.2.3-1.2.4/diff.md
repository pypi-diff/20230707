# Comparing `tmp/sockets-communication-1.2.3.tar.gz` & `tmp/sockets-communication-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.2.3.tar", last modified: Fri Jul  7 15:38:52 2023, max compression
+gzip compressed data, was "sockets-communication-1.2.4.tar", last modified: Fri Jul  7 15:48:15 2023, max compression
```

## Comparing `sockets-communication-1.2.3.tar` & `sockets-communication-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.613258 sockets-communication-1.2.3/
--rw-rw-rw-   0        0        0       98 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-07 15:38:52.613258 sockets-communication-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.2.3/build.py
--rw-rw-rw-   0        0        0      708 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 15:38:52.614258 sockets-communication-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-07 15:38:31.000000 sockets-communication-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.602256 sockets-communication-1.2.3/sockets_communication/
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.2.3/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.2.3/sockets_communication/process.py
--rw-rw-rw-   0        0        0     7898 2023-07-07 15:38:27.000000 sockets-communication-1.2.3/sockets_communication/service.py
--rw-rw-rw-   0        0        0    20597 2023-07-07 15:27:56.000000 sockets-communication-1.2.3/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.612256 sockets-communication-1.2.3/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 15:48:15.942886 sockets-communication-1.2.4/
+-rw-rw-rw-   0        0        0       98 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:48:15.942886 sockets-communication-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.2.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.2.4/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.2.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:48:15.942886 sockets-communication-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-07 15:48:09.000000 sockets-communication-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:48:15.928886 sockets-communication-1.2.4/sockets_communication/
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.2.4/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.2.4/sockets_communication/process.py
+-rw-rw-rw-   0        0        0     7899 2023-07-07 15:47:06.000000 sockets-communication-1.2.4/sockets_communication/service.py
+-rw-rw-rw-   0        0        0    20874 2023-07-07 15:48:03.000000 sockets-communication-1.2.4/sockets_communication/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:48:15.941887 sockets-communication-1.2.4/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-07 15:48:15.000000 sockets-communication-1.2.4/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.2.3/PKG-INFO` & `sockets-communication-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.2.3
+Version: 1.2.4
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.2.3/README.md` & `sockets-communication-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.3/build.py` & `sockets-communication-1.2.4/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.3/pyproject.toml` & `sockets-communication-1.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.2.3'
+version = '1.2.4'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.2.3/setup.py` & `sockets-communication-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.2.3',
+        version='1.2.4',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.2.3/sockets_communication/exceptions.py` & `sockets-communication-1.2.4/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.3/sockets_communication/process.py` & `sockets-communication-1.2.4/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.3/sockets_communication/service.py` & `sockets-communication-1.2.4/sockets_communication/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         if isinstance(wait, (int, float)):
             time.sleep(wait)
         # end if
     # end start_waiting
 
     def run(
             self,
-            update: Optional[bool] = True,
+            update: Optional[bool] = False,
             block: Optional[bool] = False,
             refresh: Optional[Union[Number, dt.timedelta]] = None,
             wait: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
     ) -> None:
         """
         Runs the api service.
```

### Comparing `sockets-communication-1.2.3/sockets_communication/sockets.py` & `sockets-communication-1.2.4/sockets_communication/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
     def run(
             self,
             connection: Optional[Socket] = None,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             listen: Optional[bool] = True,
             daemon: Optional[bool] = True,
-            update: Optional[bool] = True,
+            update: Optional[bool] = False,
             block: Optional[bool] = False,
             refresh: Optional[Union[Number, dt.timedelta]] = None,
             wait: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
         Runs the api service.
@@ -530,48 +530,53 @@
     def rerun(
             self,
             connection: Optional[Socket] = None,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             listen: Optional[bool] = True,
             daemon: Optional[bool] = True,
+            update: Optional[bool] = False,
             block: Optional[bool] = False,
+            refresh: Optional[Union[Number, dt.timedelta]] = None,
             wait: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
         Runs the api service.
 
         :param connection: The connection socket.
-        :param listen: The value to start serving_loop.
         :param host: The host of the server.
         :param port: The port of the server.
+        :param listen: The value to start serving_loop.
+        :param update: The value to update the service.
         :param daemon: The value to set the process as daemon.
         :param block: The value to block the execution and wain for the service.
         :param wait: The waiting time.
+        :param refresh: The value to refresh the service.
         :param timeout: The start_timeout for the process.
         """
 
         self.terminate()
 
         parameters = dict(
+            update=update, refresh=refresh,
             connection=connection, host=host,
             port=port, daemon=daemon, listen=listen,
             timeout=timeout, wait=wait, block=block
         )
 
         parameters = {
             key: value for key, value in parameters.items()
             if value is not None
         }
 
         self._run_parameters.update(parameters)
 
         self.run(**self._run_parameters)
-    # end run
+    # end rerun
 
     def stop_serving(self) -> None:
         """Stops the serving process."""
 
         if self.serving:
             self._serving = False
         # end if
```

### Comparing `sockets-communication-1.2.3/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.2.4/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.2.3
+Version: 1.2.4
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

