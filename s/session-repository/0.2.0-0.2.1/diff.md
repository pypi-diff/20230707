# Comparing `tmp/session-repository-0.2.0.tar.gz` & `tmp/session-repository-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.0.tar", last modified: Fri Jul  7 08:14:48 2023, max compression
+gzip compressed data, was "session-repository-0.2.1.tar", last modified: Fri Jul  7 14:13:19 2023, max compression
```

## Comparing `session-repository-0.2.0.tar` & `session-repository-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:48.541166 session-repository-0.2.0/
--rw-rw-rw-   0        0        0      599 2023-07-07 08:14:48.538926 session-repository-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:48.516433 session-repository-0.2.0/session_repository/
--rw-rw-rw-   0        0        0     9344 2023-07-07 07:59:50.000000 session-repository-0.2.0/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.2.0/session_repository/enum.py
--rw-rw-rw-   0        0        0     8007 2023-07-07 08:14:17.000000 session-repository-0.2.0/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:14:48.535614 session-repository-0.2.0/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-07 08:14:48.000000 session-repository-0.2.0/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-07 08:14:48.000000 session-repository-0.2.0/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:14:48.000000 session-repository-0.2.0/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 08:14:48.000000 session-repository-0.2.0/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 08:14:48.000000 session-repository-0.2.0/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 08:14:48.541546 session-repository-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-07 08:14:32.000000 session-repository-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.163034 session-repository-0.2.1/
+-rw-rw-rw-   0        0        0      599 2023-07-07 14:13:19.159901 session-repository-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.079191 session-repository-0.2.1/session_repository/
+-rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.1/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.2.1/session_repository/enum.py
+-rw-rw-rw-   0        0        0     8007 2023-07-07 08:14:17.000000 session-repository-0.2.1/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.146421 session-repository-0.2.1/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:13:19.164098 session-repository-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-07 14:12:50.000000 session-repository-0.2.1/setup.py
```

### Comparing `session-repository-0.2.0/PKG-INFO` & `session-repository-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.0
+Version: 0.2.1
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.0.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.0/session_repository/core.py` & `session-repository-0.2.1/session_repository/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,14 @@
     Dict,
     List,
     Optional,
     Tuple,
     Union,
 )
 
-# PYDANTIC
-from pydantic import BaseModel
-
 # SQLALCHEMY
 from sqlalchemy.orm import Session, InstrumentedAttribute
 
 # UTILS
 from session_repository.utils import (
     _FilterType,
     apply_no_load,
@@ -278,15 +275,15 @@
         model,
         filters: Optional[_FilterType] = None,
         flush: bool = True,
         commit: bool = False,
         current_session: Optional[Session] = None,
     ) -> bool:
         def _delete_from_session(session: Session):
-            rows: List[BaseModel] = self._select_all(
+            rows: List = self._select_all(
                 model=model,
                 filters=filters,
                 current_session=session,
             )
 
             if len(rows) == 0:
                 return False
```

### Comparing `session-repository-0.2.0/session_repository/utils.py` & `session-repository-0.2.1/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.0/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.1/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.0
+Version: 0.2.1
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.0.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.0/setup.py` & `session-repository-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.0"
+version = "0.2.1"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

