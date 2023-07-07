# Comparing `tmp/apidevtools-4.0.3.tar.gz` & `tmp/apidevtools-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-4.0.3.tar", last modified: Fri Jun 30 20:07:39 2023, max compression
+gzip compressed data, was "apidevtools-4.0.4.tar", last modified: Fri Jul  7 19:58:12 2023, max compression
```

## Comparing `apidevtools-4.0.3.tar` & `apidevtools-4.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.326477 apidevtools-4.0.3/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-06-30 20:07:39.325477 apidevtools-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.3/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-30 20:07:23.000000 apidevtools-4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 20:07:39.326477 apidevtools-4.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.164550 apidevtools-4.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.170476 apidevtools-4.0.3/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.3/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.3/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.193478 apidevtools-4.0.3/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.3/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.3/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.3/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.3/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.199476 apidevtools-4.0.3/src/apidevtools/orm/
--rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.3/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4930 2023-06-30 20:05:23.000000 apidevtools-4.0.3/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.3/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.3/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.204476 apidevtools-4.0.3/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.3/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2571 2023-06-30 19:57:03.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.213476 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2587 2023-06-30 20:00:49.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      974 2023-06-30 18:05:45.000000 apidevtools-4.0.3/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      522 2023-06-30 17:03:13.000000 apidevtools-4.0.3/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.217476 apidevtools-4.0.3/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.3/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.3/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.3/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.223480 apidevtools-4.0.3/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.232475 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.268475 apidevtools-4.0.3/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.3/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-06-30 14:42:33.000000 apidevtools-4.0.3/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:07:39.184479 apidevtools-4.0.3/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-06-30 20:07:39.000000 apidevtools-4.0.3/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-06-30 20:07:39.000000 apidevtools-4.0.3/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 20:07:39.000000 apidevtools-4.0.3/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-06-30 20:07:39.000000 apidevtools-4.0.3/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-30 20:07:39.000000 apidevtools-4.0.3/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.143501 apidevtools-4.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-07-07 19:58:12.143501 apidevtools-4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.4/README.md
+-rw-rw-rw-   0        0        0     2185 2023-07-07 19:57:48.000000 apidevtools-4.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 19:58:12.144502 apidevtools-4.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.100501 apidevtools-4.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.103501 apidevtools-4.0.4/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.4/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.4/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.112503 apidevtools-4.0.4/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.4/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.4/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.4/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.4/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.118502 apidevtools-4.0.4/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.4/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4930 2023-06-30 20:05:23.000000 apidevtools-4.0.4/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.4/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.4/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.121501 apidevtools-4.0.4/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.4/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2571 2023-06-30 19:57:03.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.128502 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2587 2023-06-30 20:00:49.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      974 2023-06-30 18:05:45.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      522 2023-06-30 17:03:13.000000 apidevtools-4.0.4/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.131501 apidevtools-4.0.4/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.4/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.4/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.4/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.134501 apidevtools-4.0.4/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.139501 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2074 2023-07-07 19:47:04.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.142501 apidevtools-4.0.4/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-06-30 14:42:33.000000 apidevtools-4.0.4/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.108501 apidevtools-4.0.4/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-4.0.3/LICENSE.txt` & `apidevtools-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/PKG-INFO` & `apidevtools-4.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.3
+Version: 4.0.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.3/README.md` & `apidevtools-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/pyproject.toml` & `apidevtools-4.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "4.0.3"
+version = "4.0.4"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-4.0.3/src/apidevtools/logman.py` & `apidevtools-4.0.4/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-4.0.4/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/media/imgproc.py` & `apidevtools-4.0.4/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/media/telegraph.py` & `apidevtools-4.0.4/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/mysql.py` & `apidevtools-4.0.4/src/apidevtools/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/postgresql.py` & `apidevtools-4.0.4/src/apidevtools/orm/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/sqlite.py` & `apidevtools-4.0.4/src/apidevtools/orm/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/types/_connector.py` & `apidevtools-4.0.4/src/apidevtools/orm/types/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/types/_operations/insert.py` & `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/insert.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/types/_operations/update.py` & `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/update.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/orm/types/types.py` & `apidevtools-4.0.4/src/apidevtools/orm/types/types.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/security/encryptor.py` & `apidevtools-4.0.4/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/security/hasher.py` & `apidevtools-4.0.4/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/orm.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/redis.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import aioredis as _aioredis
 from typing import Any
 
 from ..utils import evaluate as _evaluate
-from ..logman import LoggerManager, Logger
+from .. import logman
 
 
 class Redis:
     def __init__(self, database: int = 0,
                  host: str = 'localhost', port: int | str = 6379,
                  user: str | None = None, password: str | None = None,
-                 logger: Logger = LoggerManager.logger()):
+                 logger: logman.Logger = logman.logger):
         self.database: int = database
         self.host: str = host
         self.port: str | int = port
         self.user: str | None = user
         self.password: str | None = password
 
-        self.logger: Logger = logger
+        self.logger: logman.Logger = logger
         self.pool: _aioredis.Redis | None = None
 
     async def create_pool(self) -> bool:
         try:
             self.pool = _aioredis.Redis(
                 db=self.database, host=self.host, port=self.port, username=self.user, password=self.password
             )
```

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/types/records.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-4.0.4/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools/utils.py` & `apidevtools-4.0.4/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.3/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-4.0.4/src/apidevtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.3
+Version: 4.0.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.3/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-4.0.4/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

