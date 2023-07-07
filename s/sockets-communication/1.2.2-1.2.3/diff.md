# Comparing `tmp/sockets-communication-1.2.2.tar.gz` & `tmp/sockets-communication-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.2.2.tar", last modified: Fri Jul  7 15:34:15 2023, max compression
+gzip compressed data, was "sockets-communication-1.2.3.tar", last modified: Fri Jul  7 15:38:52 2023, max compression
```

## Comparing `sockets-communication-1.2.2.tar` & `sockets-communication-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:34:15.098919 sockets-communication-1.2.2/
--rw-rw-rw-   0        0        0       98 2023-07-07 15:34:14.000000 sockets-communication-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-07 15:34:15.098919 sockets-communication-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.2.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.2.2/build.py
--rw-rw-rw-   0        0        0      708 2023-07-07 15:34:14.000000 sockets-communication-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.2.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 15:34:15.098919 sockets-communication-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-07 15:34:11.000000 sockets-communication-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:34:15.065965 sockets-communication-1.2.2/sockets_communication/
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.2.2/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.2.2/sockets_communication/process.py
--rw-rw-rw-   0        0        0     7830 2023-07-07 15:33:57.000000 sockets-communication-1.2.2/sockets_communication/service.py
--rw-rw-rw-   0        0        0    20597 2023-07-07 15:27:56.000000 sockets-communication-1.2.2/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:34:15.097918 sockets-communication-1.2.2/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-07 15:34:15.000000 sockets-communication-1.2.2/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-07 15:34:15.000000 sockets-communication-1.2.2/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:34:15.000000 sockets-communication-1.2.2/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-07 15:34:15.000000 sockets-communication-1.2.2/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 15:34:15.000000 sockets-communication-1.2.2/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.613258 sockets-communication-1.2.3/
+-rw-rw-rw-   0        0        0       98 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:38:52.613258 sockets-communication-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.2.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.2.3/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.2.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:38:52.614258 sockets-communication-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-07 15:38:31.000000 sockets-communication-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.602256 sockets-communication-1.2.3/sockets_communication/
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.2.3/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.2.3/sockets_communication/process.py
+-rw-rw-rw-   0        0        0     7898 2023-07-07 15:38:27.000000 sockets-communication-1.2.3/sockets_communication/service.py
+-rw-rw-rw-   0        0        0    20597 2023-07-07 15:27:56.000000 sockets-communication-1.2.3/sockets_communication/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:38:52.612256 sockets-communication-1.2.3/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-07 15:38:52.000000 sockets-communication-1.2.3/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.2.2/PKG-INFO` & `sockets-communication-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.2.2
+Version: 1.2.3
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.2.2/README.md` & `sockets-communication-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.2/build.py` & `sockets-communication-1.2.3/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.2/pyproject.toml` & `sockets-communication-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.2.2'
+version = '1.2.3'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.2.2/setup.py` & `sockets-communication-1.2.3/setup.py`

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
-        version='1.2.2',
+        version='1.2.3',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.2.2/sockets_communication/exceptions.py` & `sockets-communication-1.2.3/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.2/sockets_communication/process.py` & `sockets-communication-1.2.3/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.2/sockets_communication/service.py` & `sockets-communication-1.2.3/sockets_communication/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     "ServiceInterface"
 ]
 
 @represent
 class ServiceInterface:
     """The server object to control the communication ith multiple clients."""
 
+    SLEEP = 0.01
+
     def __init__(self) -> None:
         """Defines the server datasets for clients and client commands."""
 
         self._timeout_process: Optional[threading.Thread] = None
         self._updating_process: Optional[threading.Thread] = None
         self._refreshing_process: Optional[threading.Thread] = None
 
@@ -92,36 +94,38 @@
             current = time.time()
 
             if (current - start) >= refresh:
                 start = current
 
                 self.refresh()
             # end if
+
+            time.sleep(self.SLEEP)
         # end while
     # end update_loop
 
     def updating_loop(self) -> None:
         """Updates the options according to the screeners."""
 
         self._updating = True
 
         while self.updating:
             self.update()
 
-            time.sleep(0.001)
+            time.sleep(self.SLEEP)
         # end while
     # end updating_loop
 
     def blocking_loop(self) -> None:
         """Updates the options according to the screeners."""
 
         self._blocking = True
 
         while self.blocking:
-            time.sleep(0.001)
+            time.sleep(self.SLEEP)
         # end while
     # end blocking_loop
 
     def start_updating(self) -> None:
         """Starts the updating process."""
 
         if self.updating:
```

### Comparing `sockets-communication-1.2.2/sockets_communication/sockets.py` & `sockets-communication-1.2.3/sockets_communication/sockets.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.2.2/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.2.3/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.2.2
+Version: 1.2.3
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

