# Comparing `tmp/dynamic-service-1.1.1.tar.gz` & `tmp/dynamic-service-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.1.1.tar", last modified: Mon Jul  3 14:40:42 2023, max compression
+gzip compressed data, was "dynamic-service-1.2.0.tar", last modified: Fri Jul  7 15:22:22 2023, max compression
```

## Comparing `dynamic-service-1.1.1.tar` & `dynamic-service-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.437266 dynamic-service-1.1.1/
--rw-rw-rw-   0        0        0      236 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-03 14:40:42.437266 dynamic-service-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.395227 dynamic-service-1.1.1/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.426257 dynamic-service-1.1.1/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.1.1/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9234 2023-07-03 14:30:46.000000 dynamic-service-1.1.1/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.1.1/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.1.1/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.428226 dynamic-service-1.1.1/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    19671 2023-07-03 14:37:54.000000 dynamic-service-1.1.1/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3012 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.388000 dynamic-service-1.1.1/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.388000 dynamic-service-1.1.1/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.436254 dynamic-service-1.1.1/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-03 14:40:42.409256 dynamic-service-1.1.1/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-03 14:40:42.000000 dynamic-service-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       78 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:40:42.437266 dynamic-service-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-03 14:40:33.000000 dynamic-service-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.895662 dynamic-service-1.2.0/
+-rw-rw-rw-   0        0        0      236 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-07 15:22:22.895662 dynamic-service-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.837657 dynamic-service-1.2.0/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.882657 dynamic-service-1.2.0/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.2.0/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9234 2023-07-03 14:30:46.000000 dynamic-service-1.2.0/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.2.0/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.2.0/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.892657 dynamic-service-1.2.0/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20012 2023-07-07 15:21:17.000000 dynamic-service-1.2.0/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3012 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.826968 dynamic-service-1.2.0/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.826968 dynamic-service-1.2.0/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.893661 dynamic-service-1.2.0/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-07 15:22:22.852657 dynamic-service-1.2.0/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-07 15:22:22.000000 dynamic-service-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-03 14:45:22.000000 dynamic-service-1.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-07-01 09:47:05.000000 dynamic-service-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:22:22.895662 dynamic-service-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-07 15:22:19.000000 dynamic-service-1.2.0/setup.py
```

### Comparing `dynamic-service-1.1.1/PKG-INFO` & `dynamic-service-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.1.1
+Version: 1.2.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.1.1/README.md` & `dynamic-service-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/build.py` & `dynamic-service-1.2.0/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/base.py` & `dynamic-service-1.2.0/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/endpoints/data.py` & `dynamic-service-1.2.0/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/endpoints/engine.py` & `dynamic-service-1.2.0/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.2.0/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/endpoints/process.py` & `dynamic-service-1.2.0/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/service/rest.py` & `dynamic-service-1.2.0/dynamic_service/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,44 +590,52 @@
             self,
             serve: Optional[bool] = True,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             silent: Optional[bool] = None,
             daemon: Optional[bool] = True,
             block: Optional[bool] = False,
+            update: Optional[bool] = True,
+            refresh: Optional[Union[Number, dt.timedelta]] = True,
             wait: Union[Number, dt.timedelta, dt.datetime] = None,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
         Runs the api service.
 
         :param serve: The value to start serving.
         :param host: The host of the server.
         :param port: The port of the server.
         :param silent: The value to silent the output.
         :param daemon: The value to set the process as daemon.
         :param block: The value to block the execution and wain for the service.
+        :param refresh: The value to refresh the system.
+        :param update: The value to update the service.
         :param wait: The waiting time.
         :param timeout: The start_timeout for the process.
         """
 
         self._run_parameters = dict(
             host=host, port=port, serve=serve,
             silent=silent, daemon=daemon, wait=wait,
+            update=update, refresh=refresh,
             timeout=timeout, block=block
         )
 
         if serve:
             self.start_serving(
                 host=host, port=port,
                 silent=silent, daemon=daemon
             )
         # end if
 
-        super().run(block=block, wait=wait, timeout=timeout)
+        super().run(
+            update=update, refresh=refresh,
+            block=block, wait=wait, timeout=timeout
+        )
     # end run
 
     def rerun(
             self,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             silent: Optional[bool] = None,
```

### Comparing `dynamic-service-1.1.1/dynamic_service/service/sockets.py` & `dynamic-service-1.2.0/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.2.0/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.2.0/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.2.0/dynamic_service.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.1.1
+Version: 1.2.0
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.1.1/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.2.0/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.1.1/pyproject.toml` & `dynamic-service-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.1.1'
+version = '1.2.0'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.1.1/setup.py` & `dynamic-service-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.1.1',
+        version='1.2.0',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

