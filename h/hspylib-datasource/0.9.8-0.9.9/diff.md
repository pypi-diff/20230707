# Comparing `tmp/hspylib-datasource-0.9.8.tar.gz` & `tmp/hspylib-datasource-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-datasource-0.9.8.tar", last modified: Tue Dec  6 19:02:57 2022, max compression
+gzip compressed data, was "hspylib-datasource-0.9.9.tar", last modified: Tue Dec  6 19:22:48 2022, max compression
```

## Comparing `hspylib-datasource-0.9.8.tar` & `hspylib-datasource-0.9.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.568449 hspylib-datasource-0.9.8/
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2022-12-05 15:59:33.000000 hspylib-datasource-0.9.8/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1496 2022-12-06 19:02:57.567476 hspylib-datasource-0.9.8/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      676 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.511150 hspylib-datasource-0.9.8/datasource/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      348 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.522548 hspylib-datasource-0.9.8/datasource/cassandra/
--rw-r--r--   0 hjunior    (504) staff       (20)      215 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/cassandra/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1442 2022-12-05 15:39:38.000000 hspylib-datasource-0.9.8/datasource/cassandra/cassandra_configuration.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7605 2022-12-06 18:57:43.000000 hspylib-datasource-0.9.8/datasource/cassandra/cassandra_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2457 2022-12-05 18:57:31.000000 hspylib-datasource-0.9.8/datasource/crud_entity.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2511 2022-12-06 18:53:18.000000 hspylib-datasource-0.9.8/datasource/crud_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1358 2022-12-06 18:38:23.000000 hspylib-datasource-0.9.8/datasource/crud_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1354 2022-12-05 15:40:04.000000 hspylib-datasource-0.9.8/datasource/db_configuration.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2373 2022-12-06 18:58:15.000000 hspylib-datasource-0.9.8/datasource/db_repository.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.532040 hspylib-datasource-0.9.8/datasource/firebase/
--rw-r--r--   0 hjunior    (504) staff       (20)      212 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/firebase/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5307 2022-12-05 18:57:31.000000 hspylib-datasource-0.9.8/datasource/firebase/firebase_configuration.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7144 2022-12-06 18:56:11.000000 hspylib-datasource-0.9.8/datasource/firebase/firebase_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3068 2022-12-05 15:40:04.000000 hspylib-datasource-0.9.8/datasource/identity.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.537363 hspylib-datasource-0.9.8/datasource/mysql/
--rw-r--r--   0 hjunior    (504) staff       (20)      177 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/mysql/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6289 2022-12-06 18:56:34.000000 hspylib-datasource-0.9.8/datasource/mysql/mysql_repository.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.542843 hspylib-datasource-0.9.8/datasource/postgres/
--rw-r--r--   0 hjunior    (504) staff       (20)      183 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/postgres/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6381 2022-12-06 18:56:54.000000 hspylib-datasource-0.9.8/datasource/postgres/postgres_repository.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.550438 hspylib-datasource-0.9.8/datasource/redis/
--rw-r--r--   0 hjunior    (504) staff       (20)      203 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/redis/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1435 2022-12-05 15:39:38.000000 hspylib-datasource-0.9.8/datasource/redis/redis_configuration.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5811 2022-12-06 18:57:23.000000 hspylib-datasource-0.9.8/datasource/redis/redis_repository.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.557467 hspylib-datasource-0.9.8/datasource/sqlite/
--rw-r--r--   0 hjunior    (504) staff       (20)      179 2022-12-06 19:02:56.000000 hspylib-datasource-0.9.8/datasource/sqlite/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6188 2022-12-06 18:55:03.000000 hspylib-datasource-0.9.8/datasource/sqlite/sqlite_repository.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:02:57.566209 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1496 2022-12-06 19:02:57.000000 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)     1010 2022-12-06 19:02:57.000000 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-12-06 19:02:57.000000 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       88 2022-12-06 19:02:57.000000 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       11 2022-12-06 19:02:57.000000 hspylib-datasource-0.9.8/hspylib_datasource.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-12-06 19:02:57.568615 hspylib-datasource-0.9.8/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1858 2022-12-05 14:17:45.000000 hspylib-datasource-0.9.8/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.055906 hspylib-datasource-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2022-12-05 15:59:33.000000 hspylib-datasource-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1398 2022-12-06 19:22:48.054747 hspylib-datasource-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      678 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.012209 hspylib-datasource-0.9.9/datasource/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      348 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.017930 hspylib-datasource-0.9.9/datasource/cassandra/
+-rw-r--r--   0 hjunior    (504) staff       (20)      215 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/cassandra/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1442 2022-12-05 15:39:38.000000 hspylib-datasource-0.9.9/datasource/cassandra/cassandra_configuration.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7605 2022-12-06 18:57:43.000000 hspylib-datasource-0.9.9/datasource/cassandra/cassandra_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2457 2022-12-05 18:57:31.000000 hspylib-datasource-0.9.9/datasource/crud_entity.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2511 2022-12-06 18:53:18.000000 hspylib-datasource-0.9.9/datasource/crud_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1358 2022-12-06 18:38:23.000000 hspylib-datasource-0.9.9/datasource/crud_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1354 2022-12-05 15:40:04.000000 hspylib-datasource-0.9.9/datasource/db_configuration.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2373 2022-12-06 18:58:15.000000 hspylib-datasource-0.9.9/datasource/db_repository.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.024708 hspylib-datasource-0.9.9/datasource/firebase/
+-rw-r--r--   0 hjunior    (504) staff       (20)      212 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/firebase/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5307 2022-12-05 18:57:31.000000 hspylib-datasource-0.9.9/datasource/firebase/firebase_configuration.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7144 2022-12-06 18:56:11.000000 hspylib-datasource-0.9.9/datasource/firebase/firebase_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3068 2022-12-05 15:40:04.000000 hspylib-datasource-0.9.9/datasource/identity.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.028695 hspylib-datasource-0.9.9/datasource/mysql/
+-rw-r--r--   0 hjunior    (504) staff       (20)      177 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/mysql/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6289 2022-12-06 18:56:34.000000 hspylib-datasource-0.9.9/datasource/mysql/mysql_repository.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.032569 hspylib-datasource-0.9.9/datasource/postgres/
+-rw-r--r--   0 hjunior    (504) staff       (20)      183 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/postgres/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6381 2022-12-06 18:56:54.000000 hspylib-datasource-0.9.9/datasource/postgres/postgres_repository.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.039119 hspylib-datasource-0.9.9/datasource/redis/
+-rw-r--r--   0 hjunior    (504) staff       (20)      203 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/redis/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1435 2022-12-05 15:39:38.000000 hspylib-datasource-0.9.9/datasource/redis/redis_configuration.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5811 2022-12-06 18:57:23.000000 hspylib-datasource-0.9.9/datasource/redis/redis_repository.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.043524 hspylib-datasource-0.9.9/datasource/sqlite/
+-rw-r--r--   0 hjunior    (504) staff       (20)      179 2022-12-06 19:22:46.000000 hspylib-datasource-0.9.9/datasource/sqlite/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6188 2022-12-06 18:55:03.000000 hspylib-datasource-0.9.9/datasource/sqlite/sqlite_repository.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-12-06 19:22:48.053424 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1398 2022-12-06 19:22:47.000000 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)     1010 2022-12-06 19:22:47.000000 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-12-06 19:22:47.000000 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       88 2022-12-06 19:22:47.000000 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       11 2022-12-06 19:22:47.000000 hspylib-datasource-0.9.9/hspylib_datasource.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-12-06 19:22:48.056077 hspylib-datasource-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1760 2022-12-06 19:10:44.000000 hspylib-datasource-0.9.9/setup.py
```

### Comparing `hspylib-datasource-0.9.8/PKG-INFO` & `hspylib-datasource-0.9.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: hspylib-datasource
-Version: 0.9.8
-Summary: HomeSetup - Datasource integration
+Version: 0.9.9
+Summary: HSPyLib - Datasource integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-datasource/
 Keywords: datasource,database,sql,nosql,db
 Platform: Darwin
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # HomeSetup - Datasource integration
 
 ## Manage you datasource's
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
-[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
+[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-datasource)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-datasource-0.9.8/README.md` & `hspylib-datasource-0.9.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Datasource integration
 
 ## Manage you datasource's
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
-[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
+[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-datasource)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-datasource-0.9.8/datasource/cassandra/cassandra_configuration.py` & `hspylib-datasource-0.9.9/datasource/cassandra/cassandra_configuration.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/cassandra/cassandra_repository.py` & `hspylib-datasource-0.9.9/datasource/cassandra/cassandra_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/crud_entity.py` & `hspylib-datasource-0.9.9/datasource/crud_entity.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/crud_repository.py` & `hspylib-datasource-0.9.9/datasource/crud_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/crud_service.py` & `hspylib-datasource-0.9.9/datasource/crud_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/db_configuration.py` & `hspylib-datasource-0.9.9/datasource/db_configuration.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/db_repository.py` & `hspylib-datasource-0.9.9/datasource/db_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/firebase/firebase_configuration.py` & `hspylib-datasource-0.9.9/datasource/firebase/firebase_configuration.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/firebase/firebase_repository.py` & `hspylib-datasource-0.9.9/datasource/firebase/firebase_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/identity.py` & `hspylib-datasource-0.9.9/datasource/identity.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/mysql/mysql_repository.py` & `hspylib-datasource-0.9.9/datasource/mysql/mysql_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/postgres/postgres_repository.py` & `hspylib-datasource-0.9.9/datasource/postgres/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/redis/redis_configuration.py` & `hspylib-datasource-0.9.9/datasource/redis/redis_configuration.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/redis/redis_repository.py` & `hspylib-datasource-0.9.9/datasource/redis/redis_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/datasource/sqlite/sqlite_repository.py` & `hspylib-datasource-0.9.9/datasource/sqlite/sqlite_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/hspylib_datasource.egg-info/PKG-INFO` & `hspylib-datasource-0.9.9/hspylib_datasource.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: hspylib-datasource
-Version: 0.9.8
-Summary: HomeSetup - Datasource integration
+Version: 0.9.9
+Summary: HSPyLib - Datasource integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-datasource/
 Keywords: datasource,database,sql,nosql,db
 Platform: Darwin
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # HomeSetup - Datasource integration
 
 ## Manage you datasource's
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
-[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
+[![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-datasource)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-datasource-0.9.8/hspylib_datasource.egg-info/SOURCES.txt` & `hspylib-datasource-0.9.9/hspylib_datasource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-datasource-0.9.8/setup.py` & `hspylib-datasource-0.9.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name='hspylib-datasource',
     version=VERSION,
-    description='HomeSetup - Datasource integration',
+    description='HSPyLib - Datasource integration',
     author='Hugo Saporetti Junior',
     author_email='yorevs@hotmail.com',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yorevs/hspylib',
     project_urls={
         'GitHub': 'https://github.com/yorevs/hspylib',
@@ -44,20 +44,18 @@
     },
     license='MIT',
     license_files='LICENSE.md',
     packages=setuptools.find_namespace_packages(),
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Unix"
 
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.10',
     install_requires=REQUIREMENTS,
     keywords='datasource,database,sql,nosql,db',
     platforms='Darwin,Linux'
 )
```

